# Guard Clause 设计模式
当业务增长导致代码变得臃肿且复杂时，函数作为最小的可执行单元，其易读性变得尤为重要。函数的清晰性可以通过良好的命名和结构来实现，而Guard Clauses设计模式则是简化复杂性的一种有效手段。通过使用Guard Clauses，我们可以在函数开始处进行预判并立即返回或抛出异常，以确保函数仅在有效条件下执行，避免深度嵌套的if和switch语句。进一步的优化是通过反转流程，即编写主逻辑而将错误情况作为else语句处理，使得代码更加简洁、清晰，减少了深层嵌套和沉长的可能性。
```
public void Subscribe(User user, Subscription subscription, Term term)
{
    if (user != null)
    {
        if (subscription != null)
        {
            if (term == Term.Annually)
            {
                // subscribe annually
            }
            else if (term == Term.Monthly)
            {
                // subscribe monthly
            }
            else
            {
                throw new InvalidEnumArgumentException(nameof(term));
            }
        }
        else
        {
            throw new ArgumentNullException(nameof(subscription));
        }
    }
    else
    {
        throw new ArgumentNullException(nameof(user));
    }
}
```
我们可以反转一下if语句中的逻辑并将抛出异常的语句放到if中，从而来消除else语句
```
public void Subscribe2(User user, Subscription subscription, Term term)
{
    if (user == null)
    {
        throw new ArgumentNullException(nameof(user));
    }
    if (subscription == null)
    {
        throw new ArgumentNullException(nameof(subscription));
    }
    if (term == Term.Annually)
    {
        // subscribe annually
    }
    else if (term == Term.Monthly)
    {
        // subscribe monthly
    }
    else
    {
        throw new InvalidEnumArgumentException(nameof(term));
    }
}
```
对null和抛出特定类型异常的常见行为的检查显然违反了DRY原则。可以将此代码提取到一个Helper方法中：
```
public static class Guard
{
    public static void AgainstNull(object argument, string argumentName)
    {
        if (argument == null)
        {
            throw new ArgumentNullException(argumentName);
        }
    }
    public static void AgainstInvalidTerms(Term term, string argumentName)
    {
        // note: currently there are only two enum options
        if (term != Term.Annually &&
            term != Term.Monthly)
        {
            throw new InvalidEnumArgumentException(argumentName);
        }
    }
}
```
现在可以调用这些帮助方法，设置不需要在函数中包含任何if语句，因为如果发生异常，它将从原始函数退出。现在你的代码将变成如下：
```
public void Subscribe3(User user, Subscription subscription, Term term)
{
    Guard.AgainstNull(user, nameof(user));
    Guard.AgainstNull(subscription, nameof(subscription));
    Guard.AgainstInvalidTerms(term, nameof(term));
    if (term == Term.Annually)
    {
        // subscribe annually
        return;
    }
    // subscribe monthly
}
```
随着项目的不断演进，您可以继续添加额外的辅助方法覆盖别的应用场景，例如空字符串、负数、无效枚举值等。

# 第三方 Ardalis.GuardClauses 包

## 引用
1. https://deviq.com/design-patterns/guard-clause
2. 
