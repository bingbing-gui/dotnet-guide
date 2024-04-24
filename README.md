# dotnet-guide

# 目录
* [dotnet-guide](#dotnet-guide)
  * [.NET介绍](#NET介绍)
  * [.NET和.NET Framework的区别](#NET和NET-Framework的区别)
  * [为什么要选择.NET](#为什么要选择NET)
  * [.NET可以构建哪些类型应用程序](#NET可以构建哪些类型应用程序)
  * [C# 编程语言](#C\#编程语言)
  * [Windows客户端生态](#Windows客户端生态)
  * [通信框架](#通信框架)
  * [Excel和CSV处理库](#Excel和CSV处理库)
* [引用](#引用)

## .NET介绍
.NET是一个免费、开源 & 跨平台的开发框架。
+ 编程语言
  + C#
  + F# 以及另外一些编程语言
+ 工具
  + Visual Studio
  + Visual Studio Code
  + JetBrains Rider
## .NET和.NET Framework的区别
 |.NET|.NET Framework|
 |-----------------------------------------------------------------------------|------------------------------------------------------------------------------------|
 |运行在Linux、macOS & Windows|仅仅运行在Windows|
 |开源 & 接受社区贡献|代码可用但不接受新的贡献|
 |持续不断创建！支持更多应用程序类型和高性能交付|安全 & 可靠 仅仅修复bug|
 |不随操作系统一起提供|包含在Windows & 随着Windows而更新|
 |推荐使用开发新的应用程序||
## 为什么要选择.NET
1. 高效性
   >.NET 提供了像泛型、LINQ 和异步编程等先进的语言特性，以及丰富的类库和多语言支持，为开发者提供了强大的工具。Visual Studio 家族为开发者提供了强大的工具支持，实现了无缝的开发体验，而我们的免费开发者计划则提供了构建和部署应用程序所需的所有资源。
2. 通用性
   >.NET可以开发运行在任何平台上的任何的应用程序。开发人员可以重用自己的技能，而不用针对不同平台再单独学一门编程语言。这意味着开发人员可以更快地构建应用程序，并且成本更低。从iOS、Android移动客户端应用程序再到Windows PC客户端应用程序，
    再到Windows Server 和 Linux 上的服务器应用程序，或者在各大厂家提供的云(AWS，Azure, GCP, 阿里云，华为云，腾讯云等)上运行的高性能，可扩展的微服务应用程序，所有的这些.NET 都为您提供了解决方案。
3. 高性能
   >.NET性能方面用一词来形容就是快！这意味着应用程序提供更快的响应时间，并且需要更少的计算资源。TechEmpower Benchmarks测试比较了 Web 应用程序框架在 JSON 序列化、数据库访问和服务器端模板渲染等任务中的性能 - .NET 的性能比任何其他流行框架都要快。
4. 信赖和安全
   >.NET平台由微软官方支持，受到成千上万家公司和数百万开发者的信赖。微软在安全问题非常重视，一旦发现威胁，就会迅速发布更新。
5. 深受开发者喜欢
   >.NET 是一个现代化、创新性、开源的开发平台，深受开发者喜爱。在连续三年（2019年、2020年和2021年）的 Stack Overflow 开发者调查中，.NET 被评为排名第一的最受喜爱的框架。C# 荣获TIOBE 2023年度编程语言。
## .NET可以构建哪些类型应用程序
### 思维导图
![image](https://github.com/bingbing-gui/dotnet-guide/blob/main/.NETDevelopment.png)
### 服务器端应用程序
1. [ASP.NET Core](https://github.com/dotnet/aspnetcore)
   + MVC
   + Blazor
   + Web API
   + Minimal API
2. 通信 
   + REST
   + WebSockets
   + GraphQL
   + GRPC
### 云原生应用程序
1. 容器
   + [docker](https://github.com/docker)
   + [containerd](https://github.com/containerd/containerd)
   + [cri-o](https://github.com/cri-o/cri-o)
   + [firecracker](https://github.com/firecracker-microvm/firecracker)
   + [gvisor](https://github.com/google/gvisor)
   + [kata](https://github.com/kata-containers/kata-containers)
   + [lima](https://github.com/lima-vm/lima)
   + [lxd](https://github.com/canonical/lxd)
   + [runC](https://github.com/opencontainers/runc)
   + [podman](https://github.com/containers/podman)
2. 容器编排
   + [Kubernetes](https://github.com/kubernetes/kubernetes)
   + [OpenShift](https://github.com/openshift)
   + [Nomad](https://github.com/hashicorp/nomad)
   + [Docker Swarm](https://docs.docker.com/engine/swarm/)
   + [Docker Compose](https://github.com/docker/compose)
   + [Minikube](https://github.com/kubernetes/minikube)
   + [Marathon](https://github.com/mesosphere/marathon)
   + [Cloudify](https://github.com/cloudify-cosmo)
   + [rancher](https://github.com/rancher/rancher)
   + 阿里云ACK
   + 亚马逊云EKS
   + 谷歌云GKE
   + 微软云AKS
### Windows客户端应用程序
1. [WinForm](https://github.com/dotnet/winforms)
2. [WPF](https://github.com/dotnet/wpf)
3. [WinUI](https://github.com/microsoft/microsoft-ui-xaml)
### 跨平台应用程序
1. [.NET MAUI](https://github.com/dotnet/maui)
   + Windows
   + MacOS
   + iOS
   + Android
2. [UNO Platform](https://github.com/unoplatform/uno)
   + Windows
   + MacOS
   + iOS
   + Android
   + WebAssembly
   + Linux
   + Tizen
3. [Avalonia UI](https://github.com/AvaloniaUI/Avalonia)
   + Windows
   + MacOS
   + iOS
   + Android
   + WebAssembly
   + Linux 
### 控制台应用程序
   1. System.Console 
      >  Micrsoft内置的控制台应用程序的接口类
   2. [spectre.console](https://github.com/spectreconsole/spectre.console) 
   3. [CommandLineParser](https://github.com/commandlineparser/commandline)
   4. [Colorful.Console](https://github.com/tomakita/Colorful.Console)
   5. [PowerArgs](https://github.com/adamabdelhamed/PowerArgs)
   6. 下面是使用C#开发的控制台应用程序的一些例子
      > [PowerShell](https://github.com/PowerShell/PowerShell)     
      > [dnSpy](https://github.com/dnSpy/dnSpy)     
      > [NuGet](https://github.com/NuGet)
      > [FluentTerminal](https://github.com/felixse/FluentTerminal)     
      > [Chocolatey](https://github.com/chocolatey/choco)     
      > [GitVersion](https://github.com/GitTools/GitVersion)
      > [shellprogressbar](https://github.com/Mpdreamz/shellprogressbar)
### IOT(Internet of Things)应用程序
1. [System.Device.Gpio](https://github.com/dotnet/iot)
2. [.NET nanoFramework](https://github.com/nanoframework)
3. [Meadow](https://github.com/WildernessLabs/Meadow.Foundation)
4. [IoTSharp](https://github.com/IoTSharp/IoTSharp)
5. [MQTTnet](https://github.com/dotnet/MQTTnet)
6. [Device.Net](https://github.com/MelbourneDeveloper/Device.Net)
### 数据库
1. 关系型数据库
   + SQL Server
   + Postgresql
   + MySQL
   + SQLite
   + CosmosDB
2. 非关系型数据库
   + RevenDB
   + MongoDB
3. ORM 框架
   + [Entity Framework Core](https://github.com/dotnet/efcore)
   + [Dapper](https://github.com/DapperLib/Dapper)
   + [NHibernate](https://github.com/nhibernate/nhibernate-core)
   + [Fluent NHibernate](https://github.com/FluentNHibernate/fluent-nhibernate)
   + [PetaPoco](https://github.com/CollaboratingPlatypus/PetaPoco)
   + [Marten](https://github.com/JasperFx/marten)
   + [SqlSugar](https://github.com/sunkaixuan/SqlSugar)
   + [FreeSql](https://github.com/2881099/FreeSql)   
### AI/机器学习
1. [ML.NET](https://github.com/dotnet/machinelearning)
2. [TensorFlow.NET](https://github.com/SciSharp/TensorFlow.NET)
3. [CNTK (Microsoft Cognitive Toolkit)](https://github.com/microsoft/CNTK)
4. [BotSharp](https://github.com/SciSharp/BotSharp)
5. [NumSharp](https://github.com/SciSharp/NumSharp)
### 游戏开发
1. [Unity](https://github.com/Unity-Technologies)
2. [Godot](https://github.com/godotengine/godot)
3. [CryEngine](https://github.com/CRYTEK)
4. [Flax Engine](https://github.com/FlaxEngine/FlaxEngine)
5. [Stride](https://github.com/stride3d/stride)
6. [MonoGame](https://github.com/MonoGame/MonoGame)
7. [evergine](https://github.com/everdevs)
8. [FlatRedBall](https://github.com/vchelaru/FlatRedBall)
9. [rbfx](https://github.com/rbfx/rbfx)
## C\# 编程语言
### [C# 编程语言规范](https://github.com/dotnet/csharplang)
## Windows客户端生态
### 思维导图
![image](https://github.com/bingbing-gui/dotnet-guide/blob/main/WinClientDevelopment.png)
### UI控件库
1. 微软Visual Studio开发工具自带原生控件(免费)。
2. [DevExpress WPF 控件](https://www.devexpress.com/products/net/controls/wpf/) (付费，商业)DevExpress UI库提供超过130个UI控件和工具，可帮助您交付高性能的企业级应用程序，满足并超越您企业的需求。
3. [Telerik WPF 控件](https://www.telerik.com/products/wpf/overview.aspx) (付费，商业)Telerik UI 为您提供了构建美观且高性能的WPF应用程序的能力，同时支持最新的.NET版本。
4. [Actipro WPF 控件](https://www.actiprosoftware.com/products/controls/wpf) (商业，付费)提供丰富的UI控件，助力打造精美的WPF桌面应用程序。
5. [ComponentOne Studio WPF控件](https://developer.mescius.com/componentone/wpf-ui-controls) （商业，付费）拥有超过100个WPF UI控件。
6. [Syncfusion WPF 控件](https://www.syncfusion.com/wpf-controls) (商业，付费)提供超过100个现代化的WPF UI控件，助力打造漂亮、高性能的企业级WPF应用程序。
7. [Ultimate WPF 控件(付费，商业)](https://www.infragistics.com/products/wpf) (商业，付费)创建高性能、仿微软® Office的桌面和触摸设备应用程序。包含100多个WPF控件库，包括高速网格和图表，以及动态数据可视化。
8. [Adonis-UI](https://github.com/benruehl/adonis-ui) (免费、开源)提供给WPF应用程序的轻量级UI工具包，提供了经典但增强的Windows视觉效果。
9. [Extended WPF Toolkit](https://github.com/xceedsoftware/wpftoolkit) (非商用免费，开源)用于创建下一代Windows应用程序的WPF控件、组件和实用工具。
10. [ControlzEx](https://github.com/ControlzEx/ControlzEx) (免费、开源)WPF一套组件。
11. [HandyControl](https://github.com/handyOrg/HandyControl) (免费、开源)包含一些常用的简单WPF控件。
12. [Material Design In XAML Toolkit](https://github.com/MaterialDesignInXAML/MaterialDesignInXamlToolkit) (免费、开源)Material Design UI库和样式以及额外控件
13. [Material Design Extensions](https://github.com/spiegelp/MaterialDesignExtensions) (免费、开源)Material Design Extensions基于Material Design in XAML Toolkit扩展，为WPF应用程序提供额外的控件和功能。
14. [ModernWPF UI Library](https://github.com/Kinnara/ModernWpf) (免费、开源)一套WPF控件和样式库。
15. [Nevron UI for Win/Mac](https://www.nevron.com/products-open-vision-wpf-ui-controls-overview.aspx) (免费)Nevron WPF用户界面组件 | NOV .NET用户界面。
16. [Ookii Dialogs WPF](https://github.com/ookii-dialogs/ookii-dialogs-wpf) (免费、开源)包含了WPF应用程序常用的对话框的类。
17. [WPFSpark](https://github.com/ratishphilip/wpfspark) (免费、开源)一个丰富的UserControl库，用于增强WPF应用程序的外观和感觉。
18. [WPF UI](https://github.com/lepoco/wpfui) (免费、开源)基于现代微软Fluent Design系统的WPF应用程序的现代样式和控件。这是使您的WPF应用程序跟上现代设计趋势的简单方法。界面设计、颜色选择和控件外观受到了微软为Windows 11制作的项目的启发。

### 单个控件
1. [AvalonEdit](https://github.com/icsharpcode/AvalonEdit) (免费，开源)AvalonEdit是一款WPF的文本编辑器组件。
2. [CefSharp](https://github.com/cefsharp/cefsharp) (免费，开源)CefSharp可以将Chromium浏览器嵌入到WPF和Winform控件中。
3. [ffmediaelement](https://github.com/unosquare/ffmediaelement) (免费，开源)ffmediaelement是一款基于FFmpeg的媒体播放器。
4. [Fluent.Ribbon](https://github.com/fluentribbon/Fluent.Ribbon) (免费，开源)Fluent.Ribbon是一款类似于Office一个控件。
5. [LiveCharts2](https://github.com/beto-rodriguez/LiveCharts2) (开源、免费) LiveCharts2是.NET跨平台的一个图形控件。
6. [ScottPlot](https://github.com/scottplot/scottplot/) (开源、免费) ScottPlot是一个交互式的图形库。
### WPF 开发框架
1. [Prism](https://github.com/PrismLibrary/Prism) (开源、收费)Prism是一个框架，用于在WPF和Xamarin Forms中构建松散耦合、可维护和可测试的XAML应用程序。
2. [Caliburn.Micro](https://github.com/Caliburn-Micro/Caliburn.Micro) (免费，开源)Caliburn.Micro是一个小巧却功能强大的框架，专为跨所有XAML平台构建应用程序而设计。它对MV*模式提供了强大支持，使您能够快速构建解决方案，而不必牺牲代码质量或可测试性。
3. [FluentWPF](https://github.com/sourcechord/FluentWPF) (免费，开源)WPF的流畅设计系统
4. [MvvmCross](https://github.com/MvvmCross/MvvmCross) (免费，开源)MvvmCross是一个跨平台解决方案的.NET MVVM框架，包括Xamarin.iOS、Xamarin.Android、Windows和Mac。
5. [ReactiveUI](https://github.com/reactiveui/reactiveui)（免费，开源）ReactiveUI是一个先进的、模块化、函数式响应式MVVM框架，适用于所有.NET平台！
6. [Mahapps.Metro](https://github.com/MahApps/MahApps.Metro) (免费、开源)Mahapps.Metro是一个WPF框架，让开发者能够用更少的工作量为他们的WPF应用程序创建出更好的UI
7. [GongSolutions.WPF.DragDrop](https://github.com/punker76/gong-wpf-dragdrop) 提供了拖拽式开发解决方案

## 通信框架
### GraphQL
> GraphQL是一个开源的，面向API而创造出来的数据查询操作语言以及相应的运行环境。于2012年仍处于Facebook内部开发阶段，直到2015年才公开发布。2018年11月7日，Facebook将GraphQL项目转移到新成立的GraphQL基金会（隶属于非营利性的Linux基金会）。GraphQL相较于REST以及其他web service架构提供了一种更加高效、强大和灵活的开发web APIs的方式。它通过由客户端根据所需定义数据结构，同时由服务端负责返回相同数据结构的对应数据的方式避免了服务端大量冗余数据的返回，但与此同时也意味着这种方式不能有效利用查询结果的web缓存。GraphQL这种查询语言所带来的灵活性和丰富性的同时也增加了复杂性，导致简单的APIs有可能并不适合这种方式。
1. [Graphql DotNet](https://github.com/graphql-dotnet/graphql-dotnet)
2. [ChilliCream Graphql Platform](https://github.com/ChilliCream/graphql-platform)
### gRPC
> gRPC (gRPC Remote Procedure Calls) 是一个跨平台的开源高性能远程过程调用（RPC）框架。
gRPC最初由Google创建，它使用一个通用的RPC基础设施Stubby来连接其数据中心内外运行的大量微服务，始于2001年。2015年3月，Google决定构建下一个版本的Stubby并将其开源，于是就有了gRPC。现在除了Google之外，许多组织都在使用它来支持从微服务到计算的“最后一英里”（移动、Web和物联网）的用例。gRPC基于HTTP/2协议传输数据，使用Protocol Buffers作为接口描述语言，并提供认证（authentication）、双向流（bidirectional streaming）和流量控制、阻塞或非阻塞绑定以及取消和超时（Deadlines）等功能。它为许多语言生成跨平台的客户端和服务器绑定。最常见的使用场景包括在微服务风格的架构中连接服务，或将移动设备客户端连接到后端服务。
gRPC对HTTP/2的复杂使用使得在浏览器中无法实现gRPC客户端，而需要使用代理。
最常见的应用场景是：
微服务框架下，多种语言服务之间的高效交互。
将手机服务、浏览器连接至后台
产生高效的客户端库
1. [Grpc DotNet](https://github.com/grpc/grpc-dotnet/tree/master)
2. [MagicOnion](https://github.com/Cysharp/MagicOnion)
### Rest
> Representational State Transfer缩写：REST，是Roy Thomas Fielding博士于2000年在他的博士论文中提出来的一种万维网软件架构风格，目的是便于不同软件/程序在网络（例如互联网）中互相传递信息。表现层状态转换是根基于超文本传输协议（HTTP）之上而确定的一组约束和属性，是一种设计提供万维网络服务的软件构建风格。符合或兼容于这种架构风格（简称为 REST 或 RESTful）的网络服务，允许客户端发出以统一资源标识符访问和操作网络资源的请求，而与预先定义好的无状态操作集一致 
化。因此表现层状态转换提供了在互联网络的计算系统之间，彼此资源可交互使用的协作性质（interoperability）。相对于其它种类的网络服务，例如SOAP服务，则是以本身所定义的操作集，来访问网络上的资源。
目前在三种主流的Web服务实现方案中，因为REST模式与复杂的SOAP和XML-RPC相比更加简洁，越来越多的Web服务开始采用REST风格设计和实现。例如，Amazon.com提供接近REST风格的Web服务执行图书查询；雅虎提供的Web服务也是REST风格的。
1. [RestSharp](https://github.com/restsharp/RestSharp)
2. [Refit](https://github.com/reactiveui/refit)
3. [Flurl](https://github.com/tmenier/Flurl)
### WebSocket
> WebSocket是一种网络传输协议，可在单个TCP连接上进行全双工通信，位于OSI模型的应用层。WebSocket协议在2011年由IETF标准化为RFC 6455，后由RFC 7936补充规范。Web IDL中的WebSocket API由W3C标准化。
WebSocket使得客户端和服务器之间的数据交换变得更加简单，允许服务端主动向客户端推送数据。在WebSocket API中，浏览器和服务器只需要完成一次握手，两者之间就可以建立持久性的连接，并进行双向数据传输。
1. [ASP.NET SignalR](https://github.com/dotnet/aspnetcore/tree/main/src/SignalR)
2. [ASP.NET Core中支持WebSockets](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/websockets?view=aspnetcore-8.0)
## Excel和CSV处理库
1. [EPPlus](https://github.com/EPPlusSoftware/EPPlus)
2. [CSVHepler](https://github.com/JoshClose/CsvHelper)

# 引用
1. https://github.com/Carlos487/awesome-wpf 
2. https://github.com/tbolon/awesome-dotnet-winforms
3. https://zh.wikipedia.org/zh-cn/GraphQL
4. https://zh.wikipedia.org/zh-cn/GRPC
5. https://zh.wikipedia.org/zh-cn/%E8%A1%A8%E7%8E%B0%E5%B1%82%E7%8A%B6%E6%80%81%E8%BD%AC%E6%8D%A2
6. https://zh.wikipedia.org/zh-cn/WebSocket
