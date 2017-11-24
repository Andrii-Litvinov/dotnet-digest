**.NET**

[.NET Framework 4.7.1 Runtime and Compiler Features](https://blogs.msdn.microsoft.com/dotnet/2017/09/28/net-framework-4-7-1-runtime-and-compiler-features/)

Поддержки .NET Standard 2.0 на уровне BCL, улучшение производительности GC, `ValueTuple` теперь сериализуемые, Runtime Feature Detection.

[DotNetAnywhere: An Alternative .NET Runtime](http://mattwarren.org/2017/10/19/DotNetAnywhere-an-Alternative-.NET-Runtime/)

Осмотр древнего проекта, который используется в экспериментальном [Blazor](https://github.com/SteveSanderson/Blazor) для выполнения C# в браузере.

[.NET Core 2.0 and ASP.NET Core 2.0 are Here](https://weblog.west-wind.com/posts/2017/Oct/22/NET-Core-20-and-ASPNET-20-Core-are-finally-here)

Основатальный обзор нововведений, плюсов и минусов платформы.

[Welcome to C# 7.1](https://blogs.msdn.microsoft.com/dotnet/2017/10/31/welcome-to-c-7-1/)

Async Main, выведение имен элементов кортежа, default литералы.

[Detect blocking waits](https://github.com/dotnet/corefx/issues/8931#issuecomment-337354565)

Интересный метод как можно найти блокирующие ожиданя задач, такие как `Task.Result` или `Task.Wait`.

[C# 7.2: Understanding Span](https://channel9.msdn.com/Events/Connect/2017/T125)

Хорошее вводное видео о `Span<T>`, для чего нужен и как помогает минимизировать аллокации при работе с массиивами и строками.

[Introducing Nullable Reference Types in C#](https://blogs.msdn.microsoft.com/dotnet/2017/11/15/nullable-reference-types-in-csharp/)

[Plain Functional Programming by Martin Odersky](https://www.youtube.com/watch?v=YXDm3WHZT5g&feature=youtu.be&t=260)

Еще не успел посмотреть видео, но там интересный слайд, что синтаксис C# сильно больше, чем в С++, Java, Haskell и многих других.

[Announcing the Windows Compatibility Pack for .NET Core](https://blogs.msdn.microsoft.com/dotnet/2017/11/16/announcing-the-windows-compatibility-pack-for-net-core/)

Пакет, который добавляет много новых API, включая долгожданный System.Drawing Некоторые только под Win.

[HashCode based on xxHash32](https://github.com/dotnet/coreclr/pull/14863)

Генератор хороших хеш-кодов в corefx.

[Migrating from ASP.NET Identity to Service Stack Authentication](https://medium.com/@williams.jackj/migrating-from-asp-net-identity-to-service-stack-authentication-e9292495d218)

[In C# 7 is it possible to deconstruct tuples as method arguments
](https://stackoverflow.com/questions/41589540/in-c-sharp-7-is-it-possible-to-deconstruct-tuples-as-method-arguments/41590136)

Не сразу было очевидно как использовать деконсруктор в параметрах лямбда-выражения, поэтому решил поделиться: `((string s, int i) _) => ...`

**Архитектура**

[Using Akka.NET Actor Systems in Xamarin Apps](https://gregshackles.com/using-akka-net-in-xamarin-apps/)

[Why does Kafka scale better than other messaging systems like RabbitMQ?](https://www.quora.com/Why-does-Kafka-scale-better-than-other-messaging-systems-like-RabbitMQ/answer/Clemens-Vasters)

Основной поит в том, что MQ системы запопинают какие сообщения какой потребитель обрабатывает и это добавляет много накладных расходов. В Kafka (и EventStore) клиент сам запоминает позицию для чтения освобождая ресурсы системы и увеличиваю пропускную способность.

[The Dark Side of Event Sourcing: Managing Data Conversion](http://files.movereem.nl/2017saner-eventsourcing.pdf)

Пока не читал, но должно быть интетесно, добавил в закладки.

[Software architecture is failing](https://www.alexhudson.com/2017/10/14/software-architecture-failing/)

Статья, вызвавшая много споров в интернетах. Опять же, нужно понимать что делаешь и зачем. [Дисскусия](https://twitter.com/VaughnVernon/status/919712049323634688).

[Scaling Event-Sourcing at Jet](https://medium.com/@eulerfx/scaling-event-sourcing-at-jet-9c873cac33b8)

Крутая статья о архитектуре ES системы, в которой EventStore используется как single source of truth, а проекции строятся на основе Kafka. [Дисскусия](https://twitter.com/eulerfx/status/922881839857008642).

[Event Store Internals and SEDA](https://www.youtube.com/watch?v=jRmpYprh3aE)

Интересное видео о внутренностях Event Store от разработчика, к сожалению с плохим звуком и качеством картинки.

[The 7 Ways to Wash Dishes and the Case for Message-driven Reactive Systems](https://www.lightbend.com/blog/7-ways-washing-dishes-and-message-driven-reactive-systems)

Неблокирующая, асинхронная параллельная обработки сообщений на примере мытья посуды.

**Инструменты**

[Real-World ASP.NET Core Logging Configuration](https://mitchelsellers.com/blogs/2017/10/09/real-world-aspnet-core-logging-configuration)

[HashiCorp Consul 1.0](https://www.hashicorp.com/blog/hashicorp-consul-1-0)

[REST Client for VS Code, an elegant alternative to Postman](http://josephwoodward.co.uk/2017/10/rest-%20client-for-vs-code-an-elegant-alternative-postman)

[The Icon Journey](https://code.visualstudio.com/blogs/2017/10/24/theicon)

В VS Code вернули синюю иконку, немного детелей и размышлений на тему.

[Beta Docker for Mac and Windows with Kubernetes](https://blog.docker.com/2017/10/docker-for-mac-and-windows-with-kubernetes-beta/)

[Ben.Demystifier](https://github.com/benaadams/Ben.Demystifier)

Крутой инструмент для создания более читабФельных stack-traces. Уже можно найти расширения для фреймворков логгирования.

[Bundling .NET build tools in NuGet](http://www.natemcmaster.com/blog/2017/11/11/build-tools-in-nuget/)

В новой системе пакетов PackageReference добавили возможность добавлять команды MSBuild. Новые версии OctoPack уже умеют с этим работать.

[xUnit Roslyn Analyzers](http://davidpine.net/blog/xunit-powered-by-roslyn/)

[Introducing API Analyzer](https://blogs.msdn.microsoft.com/dotnet/2017/10/31/introducing-api-analyzer/)

[.NET debugger and assembly editor](https://github.com/0xd4d/dnSpy)

[dotnet xunit fails for .NET Core 2.0.3 with .NET Core SDK 2.0.3](https://github.com/xunit/xunit/issues/1573)

Задуманное поведение о котором стоит знать.

[.NET (Micro)ORM fetch benchmark results and the fine details](https://weblogs.asp.net/fbouma/net-micro-orm-fetch-benchmark-results-and-the-fine-details)

[Analyzing performance of asynchronous .NET code with dotTrace](https://blog.jetbrains.com/dotnet/2017/11/22/analyzing-performance-asynchronous-net-code-dottrace/)

Фича, которой очень нехватало и которую VS умела. Здорово, что они ее наконец добавили.

[Code formatting engine updates in ReSharper and Rider](https://blog.jetbrains.com/dotnet/2017/11/23/code-formatting-engine-updates-resharper-rider/)

**UI**

[Vue 2.5 released](https://medium.com/the-vue-point/vue-2-5-released-14bd65bf030b)

[Documenting the Web together](https://blogs.windows.com/msedgedev/2017/10/18/documenting-web-together-mdn-web-docs/)

MS решили использовать MDN как единый актуальный источник документации для веба.

[2018: 120fps and no jank](https://dassur.ma/things/120fps/)

Размышления о том, как можно добиться лушей производительность приложений в виду того, что новые девайсы подеерживают частоту обновления 120 Гц.

[The Cost Of JavaScript](https://medium.com/dev-channel/the-cost-of-javascript-84009f51e99e)

Очень интересная статья о производительности JS.

**Книги**

[Exploring .NET Core with Microservices, ASP.NET Core, and Entity Framework Core](https://www.manning.com/books/exploring-dot-net-core)

Бесплатная книга, сам пока не читал, но возможно, стоит полистать.

[Free Ebook: The Cloud Native Attitude](http://container-solutions.com/ebook-the-cloud-native-attitude)

**Разное**

[5 challenges in the developer to CEO transition](https://raygun.com/blog/top-5-challenges-in-the-developer-to-ceo-transition/)

[Life Is About to Get a Whole Lot Harder for Websites Without HTTPS](https://www.troyhunt.com/life-is-about-to-get-harder-for-websites-without-https/)

[Becoming Foolish](https://hmemcpy.com/2017/10/becoming-foolish/)

О том, почему стоит поинтересоваться фкнциональными языками программирования.

[The QUIC transport protocol: design and Internet-scale deployment](https://blog.acolyer.org/2017/10/26/the-quic-transport-protocol-design-and-internet-scale-deployment/)

Новый протокол от Гугла, который совершает шифрование и траспортировку за один запрос, т.е. экономит на запросах, но сильнее нагружает процессор.

[My First Day at Accenture – The Start of the 104-Hour Workweek](http://exposingevilempire.com/accenture/first-day-accenture-104-hour-workweek/)

О рабстве на работе.

[Promise Theory - Basic Concepts (part 1)](https://www.youtube.com/watch?v=2TPsB5WuZgk)

[Trunk Based Development](https://trunkbaseddevelopment.com/)

Сайт позвященные Trunk Based Development. Отличный ресурс чтобы понять почему, зачем и как.

[Architecting for Continuous Delivery](https://www.thoughtworks.com/insights/blog/architecting-continuous-delivery)

[How to choose (and contribute to) your first open source project](https://github.com/collections/choosing-projects)

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Generations of programmers have been confused because the wrong word is used...<br><br>Its &quot;offset&quot; from start, not &quot;index&quot; - and that&#39;s why it starts at zero! <a href="https://t.co/p1ecpscVY8">pic.twitter.com/p1ecpscVY8</a></p>&mdash; Ben Adams 🐝 (@ben_a_adams) <a href="https://twitter.com/ben_a_adams/status/929294843939098624?ref_src=twsrc%5Etfw">November 11, 2017</a></blockquote>

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Reminded of a past conversation ...<br>X: We&#39;re going to spend $1bn on this effort.<br>Me: I can deliver the same result for $20m.<br>X: How?<br>Me: pay me $20m to sit on a beach drinking and in five years I&#39;ll phone you up to say &quot;we failed&quot;. <br>... 5 years later<br>X: I wish we paid you $20m.</p>&mdash; swardley (@swardley) <a href="https://twitter.com/swardley/status/933069547271327744?ref_src=twsrc%5Etfw">November 21, 2017</a></blockquote>

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">&quot;Haskell is faster than C++, more concise than Perl, more regular than Python, more flexible than Ruby, more typeful than C#, more robust than Java, and has absolutely nothing in common with PHP.&quot; — Autrijus Tang</p>&mdash; Programming Wisdom (@CodeWisdom) <a href="https://twitter.com/CodeWisdom/status/933772527498874880?ref_src=twsrc%5Etfw">November 23, 2017</a></blockquote>

<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
