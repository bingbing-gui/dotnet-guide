# .NET 介绍
.NET是一个免费、开源 & 跨平台的开发框架。
+ 编程语言
  + C#
  + F# 以及另外一些编程语言
+ 工具
  + Visual Studio
  + Visual Studio Code
  + JetBrains Rider
# .NET和.NET Framework的区别
 |.NET|.NET Framework|
 |-----------------------------------------------------------------------------|------------------------------------------------------------------------------------|
 |运行在Linux、macOS & Windows|仅仅运行在Windows|
 |开源 & 接受社区贡献|代码可用但不接受新的贡献|
 |持续不断创建！支持更多应用程序类型和高性能交付|安全 & 可靠 仅仅修复bug|
 |不随操作系统一起提供|包含在Windows & 随着Windows而更新|
 |推荐使用开发新的应用程序||
# 为什么要选择.NET
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
# .NET 可以构建哪些类型应用程序
## Mindmap
![image](https://github.com/bingbing-gui/dotnet-guide/blob/main/.NETDevelopment.png)
## 服务器端应用程序
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
## 云原生应用程序
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
## Windows客户端应用程序
1. [WinForm](https://github.com/dotnet/winforms)
2. [WPF](https://github.com/dotnet/wpf)
3. [WinUI](https://github.com/microsoft/microsoft-ui-xaml)
## 跨平台应用程序
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
## 控制台应用程序
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
## IOT(Internet of Things)应用程序
1. [System.Device.Gpio](https://github.com/dotnet/iot)
2. [.NET nanoFramework](https://github.com/nanoframework)
3. [Meadow](https://github.com/WildernessLabs/Meadow.Foundation)
4. [IoTSharp](https://github.com/IoTSharp/IoTSharp)
5. [MQTTnet](https://github.com/dotnet/MQTTnet)
6. [Device.Net](https://github.com/MelbourneDeveloper/Device.Net)
## 数据库
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
## AI/机器学习
1. [ML.NET](https://github.com/dotnet/machinelearning)
2. [TensorFlow.NET](https://github.com/SciSharp/TensorFlow.NET)
3. [CNTK (Microsoft Cognitive Toolkit)](https://github.com/microsoft/CNTK)
4. [BotSharp](https://github.com/SciSharp/BotSharp)
5. [NumSharp](https://github.com/SciSharp/NumSharp)
## 游戏开发
1. [Unity](https://github.com/Unity-Technologies)
2. [Godot](https://github.com/godotengine/godot)
3. [CryEngine](https://github.com/CRYTEK)
4. [Flax Engine](https://github.com/FlaxEngine/FlaxEngine)
5. [Stride](https://github.com/stride3d/stride)
6. [MonoGame](https://github.com/MonoGame/MonoGame)
7. [evergine](https://github.com/everdevs)
8. [FlatRedBall](https://github.com/vchelaru/FlatRedBall)
9. [rbfx](https://github.com/rbfx/rbfx)

