**.NET**

[Performance Improvements in .NET Core 3.0](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-core-3-0/)

[Introducing Windows Terminal](https://devblogs.microsoft.com/commandline/introducing-windows-terminal/)

[Announcing WSL 2](https://devblogs.microsoft.com/commandline/announcing-wsl-2/)

[Introducing .NET 5](https://devblogs.microsoft.com/dotnet/introducing-net-5/)

[Announcing .NET Core 3.0 Preview 6](https://devblogs.microsoft.com/dotnet/announcing-net-core-3-0-preview-6/)

[ASP.NET Core A-Z](https://wakeupandcode.com/aspnetcore/#aspnetcore2019)

Любопытная подборка статей про ASP.NET Core. Не читал, но одобряю.

[ASP.NET  Core 3.0 now natively supports the w3c trace-context](https://twitter.com/davidfowl/status/1144127100997128197)

[VERSIONING LIMITATIONS IN .NET](https://codeblog.jonskeet.uk/2019/06/30/versioning-limitations-in-net/)

[Core dump of StackOverflowException](https://github.com/dotnet/coreclr/issues/24779)

Мы в компании стремительно движемся в сторону контейнеризации, много сервисов уже переехали в Docker и я задался вопросом как получить и анализировать crash dump (он же core dump) в случае возникновения StackOverflowException. Все оказалось совсем нетривиально и на данный момент хоть дамп получить и можно, явно выявить источник ошибки сходу не получится, придется проходится по каждому потоку, смотреть где огромный стек-трейс и мапить символы вручную. Обещают пофиксить это в релизу 3.0. Но то, что можно собрать дамп и хоть как-то его проанализировать уже большое дело. В issue я подробно описал шаги как это скофигурить.

**Architecture**

[Local-first software](https://www.inkandswitch.com/local-first.html)

[DDD and Messaging Architectures](http://verraes.net/2019/05/ddd-msg-arch/)

[Asynchronous Injection](https://blog.ploeh.dk/2019/02/11/asynchronous-injection/)

Замечательная статья о том, почему не нужно делать модель предметной области асинхронной. Ключевой момент:

>the method is close enough to be pure that it's testable. The interactions of TryAccept and any client code (including unit tests) is completely controllable and observable by the client.
>This means that there's no reason to Stub it out.

[Building a Distributed Log from Scratch](https://bravenewgeek.com/building-a-distributed-log-from-scratch-part-1-storage-mechanics/)

**Разное**

[HAProxy 2.0 Adds Kubernetes](https://thenewstack.io/haproxy-2-0-adds-kubernetes-pushes-polyglot-extensibility/)

[Little Things I Like to Do with Git](https://csswizardry.com/2017/05/little-things-i-like-to-do-with-git/)

[Эффективность не работает](https://www.youtube.com/watch?v=K6oZuB8_dU8)

О том как не доработаться до депрессии.

**События**

18-20 ноября в Киеве пройдет конференция [Build Stuff Ukraine](https://www.ukraine.buildstuff.events). Спешу поделиться промокодом на скидку в 10%: **BUILDUA10**, так как до 14-го июля действует Early Bird цена. Пользуйтесь возможностью. 
