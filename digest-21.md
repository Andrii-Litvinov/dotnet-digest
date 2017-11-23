**.NET**

[Real-World ASP.NET Core Logging Configuration](https://mitchelsellers.com/blogs/2017/10/09/real-world-aspnet-core-logging-configuration)

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

