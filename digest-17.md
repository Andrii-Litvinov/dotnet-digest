**.NET**

[Валидация и авторизация JWT](https://blogs.msdn.microsoft.com/webdev/2017/04/06/jwt-validation-and-authorization-in-asp-net-core/) в ASP.NET Core.

Использование `Span<T>` и `ref` вместе [часть 1](http://blog.marcgravell.com/2017/04/spans-and-ref-part-1-ref.html), [часть 2](http://blog.marcgravell.com/2017/04/spans-and-ref-part-2-spans.html).

[Высокопроизводительный .NET](https://alexandrnikitin.github.io/blog/high-performance-dotnet-by-example/) на примере высоконагруженного прилрожения.

[Issue](https://github.com/aspnet/Home/issues/2022), которая сделала много шума в сообществе. Майкрософт решила убрать обратную совместимость .NET Core 2.0 c Full Framework. В итоге решили отложить это решение на потом.

Модет ли объек быть [собран GC](https://blogs.msdn.microsoft.com/seteplia/2017/05/09/garbage-collection-and-variable-lifetime-tracking/) до того, как метод закончит выполнение.

Анонс [ASP.NET Core 2.0.0-Preview1](https://blogs.msdn.microsoft.com/webdev/2017/05/10/aspnet-2-preview-1/).

Введение в [Razor Pages](https://docs.microsoft.com/en-us/aspnet/core/razor-pages/) в ASP.NET Core.

Обзор [.NET Standard - 2.0 Preview](https://www.youtube.com/watch?v=HyfDG4mjBPk).

Высокоуровневое планирование [ASP.NET Core 2.0.0-preview2](https://github.com/aspnet/Announcements/issues/243).

Пример проекта на [F#, ASP.NET Core and Docker](https://github.com/jakkaj/aspnetcore_fsharp_docker).

[Сравнение производительности](https://gist.github.com/mgravell/878e7fb19ad2378941f810820b9e90b5) `Task<T>` и `ValueTask<T>`.

Будущее Майкрософт [serverless](http://diginomica.com/2017/04/19/will-microsofts-serverless-future-turn-into-a-faas/).

МС открала исходный код [Service Fabric](https://blogs.msdn.microsoft.com/azureservicefabric/2017/03/24/service-fabric-net-sdk-goes-open-source/).

**#Build 2017**

Введение в [ASP.NET Core 2.0](https://channel9.msdn.com/events/Build/2017/B8048).

Обсуждение [.NET Standard 2.0 и .NET Core 2.0](https://channel9.msdn.com/Events/Build/2017/C9L18).

[.NET Standard](https://channel9.msdn.com/Events/Build/2017/B8001) для трех runtime в VS 2017.

[Aurelia и ASP.NET Core](https://channel9.msdn.com/events/Build/2017/T6032).

**Проектирование и все такое**

Решение [сложности в CQRS](https://dev.to/vladikk/tackling-complexity-in-cqrs).

Про распределенные системы и [альтернативу API](https://writings.quilt.org/2014/05/12/distributed-systems-and-the-end-of-the-api/).

[Валидация комманд](https://jimmybogard.com/domain-command-patterns-validation/).

Интеграция [MassTransit и EventStore](https://github.com/alexeyzimarev/MassTransit.EventStoreIntegration).

[Архитектура .NET приложений](https://www.microsoft.com/net/learn/architecture). В том числе упоминается Akka.NET а книге о микросервисах.

[Хороший дизайн - неидеальный дизайн](https://www.youtube.com/watch?v=lY54TmmEllY). Отличное выступление Эрика Эванса на DDD EU.

Девид Вест: [прошлое и будещее DDD](https://www.youtube.com/watch?v=XH_awPS6hK4).

[Самодостаточные системы](https://www.infoq.com/articles/scs-microservices-done-right) - миоросервисы приготовлненные правильно.

[Event-Driven архитектура](https://www.youtube.com/watch?v=STKCRSUsyP0) (Мартин Фаулер на goto;).

[Отладка](https://www.youtube.com/watch?v=30jNsCVLpAE), когда все горит.

**Инструменты**

[Rider](https://blog.jetbrains.com/dotnet/2017/05/08/rider-is-now-also-an-fsharp-ide-adding-fsharp-support/) будет поддерживать F#. И стали извенстны [цены](https://blog.jetbrains.com/dotnet/2017/05/03/rider-licensing-pricing/).

[Spource Tree 2.0](https://blog.sourcetreeapp.com/2017/01/27/sourcetree-for-windows-2-0-is-now-in-beta/) для Windows.

Расширение для [командной строки](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.OpenCommandLine) в VS.

[Апрельское обновление](https://code.visualstudio.com/updates/v1_12) VS Code.

[Исследование](https://thenewstack.io/tns-research-present-state-container-orchestration/) об оркестраторах контейнеров.

[Окружение для разработки](https://meta.discourse.org/t/how-my-dev-environment-is-configured/62444) Сэма Саффрона из Stack Overflow.

Обновление [IIS Express SSL](https://gist.github.com/blowdart/1cb907b68ed56bcf8498c16faff4221c) для хрома.

[Akka.NET](https://petabridge.com/blog/akkadotnet-2017-roadmap/) будет поддерживать .NET Standard 1.3 в следующем обновлении.

[NServiceBus](https://particular.net/blog/nservicebus-on-net-core-its-time) будет поддерживать .NET Core 2.0.

[Chrome 59](https://developers.google.com/web/updates/2017/04/headless-chrome) будет сожержать headless-browser (для Windows чуть позже).

[Развертывание](http://docs.servicestack.net/deploy-netcore-docker-aws-ecs) ASP.NET Core с Docker в AWS.

Оптимизированные [Docker образы](https://blogs.msdn.microsoft.com/stevelasker/2016/09/29/building-optimized-docker-images-with-asp-net-core/) с .NET Core.

**Интерфейсы**

[Управление сложностью в Redux](http://engineering.blogfoster.com/managing-complexity-in-redux-higher-order-reducers-and-async-state/): редьюсеры более высокого порядка и асинхронное состояние.

[Новый интерфейс YouTube](http://engineering.blogfoster.com/managing-complexity-in-redux-higher-order-reducers-and-async-state/) реализовали на Polymer.

Анонс [TypeScript 2.3](https://blogs.msdn.microsoft.com/typescript/2017/04/27/announcing-typescript-2-3/).

Анонс [Polymer 2.0](https://www.polymer-project.org/blog/2017-05-15-time-for-two).

[Прогрессивне веб-приложения](https://www.youtube.com/watch?v=aCMbSyngXB4) с JavaScript фреймворками.

[Polymer на Google I/O 2017](https://www.polymer-project.org/blog/2017-05-26-polymer-at-io-17): положение дел с веб-компонентами, работа на ошибками, инструменты.

[Шпаргалка](https://meowni.ca/posts/polymer-2-cheatsheet/) по Polymer 2.0.

Решение проблем с SEO с помощью [Headless Chrome](https://medium.com/@samdotli/solving-seo-with-headless-chrome-for-your-client-side-framework-288e66fdd2b7).

**События**

Работа с SQL в IDE на базе [IntelliJ](https://info.jetbrains.com/DataGrip-Webinar-Jun2017-Registration.html).

**Разное**
4 ошибки, которые не должен допускать [серьезный ревьюер кода](http://www.yegor256.com/2015/02/09/serious-code-reviewer.html).

[Практическое машинное обучение](https://monzo.com/blog/2017/05/03/practical-machine-learning-for-startups/) для стартапов.

Разница между HTTP 1.x и HTTP/2
<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">HTTP what? : I drew what HTTP is &amp; how HTTP1.x and HTTP2 are different✨<br><br>(tweetzine, drawsplainer, codedoodles…I don&#39;t know what to call it) <a href="https://t.co/NEhqlT9rdR">pic.twitter.com/NEhqlT9rdR</a></p>&mdash; Mariko Kosaka (@kosamari) <a href="https://twitter.com/kosamari/status/859958929484337152">May 4, 2017</a></blockquote>


[Stack Overflow](https://stackoverflow.blog/2017/05/09/introducing-stack-overflow-trends/) тренды.

[Новые дистрибутивы Linux](https://blogs.msdn.microsoft.com/commandline/2017/05/11/new-distros-coming-to-bashwsl-via-windows-store/) на Bash for Windows.

[Анализ WannCry](https://www.troyhunt.com/everything-you-need-to-know-about-the-wannacrypt-ransomware/) от Троя Ханта.

[Путешествие к фунуциональному программированию](http://hmemcpy.com/2017/05/from-net-to-scala-and-beyond-a-journey-to-functional-programming/) от .NET до Скала и далее.


**Книги**

Сжато про [Aurelia](https://www.syncfusion.com/resources/techportal/details/ebooks/aurelia_succinctly).

**Приколы**

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">When ransomware guys provide better customer support than most companies 😂<a href="https://twitter.com/hashtag/WannaCry?src=hash">#WannaCry</a> <a href="https://t.co/H7SIFV5WKl">pic.twitter.com/H7SIFV5WKl</a></p>&mdash; Faizal (@fztalks) <a href="https://twitter.com/fztalks/status/864852163230609408">May 17, 2017</a></blockquote>

Про [уязвимости AutoMapper](https://stackoverflow.com/questions/43648876/automapper-security-vulnerabilities-upgrade-from-3-2-1-0-to-5-1-1/).

<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>