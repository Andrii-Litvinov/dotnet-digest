**.NET**

[ASP.NET Core 2.0 Authentication and Authorization System Demystified](https://digitalmccullough.com/posts/aspnetcore-auth-system-demystified.html)

Общее представление о том, как устроена аутентификация и авторизация в ASP.NET 2.0.

[Zero Garbage Collector for .NET Core](http://tooslowexception.com/zero-garbage-collector-for-net-core/)

Пример реализации GC, который не собирает мусор. Может быть полезно для небольших утилит, чтобы выжать максимус производительности.

[ASP.NET Core 2.0 Features](https://blogs.msdn.microsoft.com/webdev/2017/08/25/asp-net-core-2-0-features-1/)

Новооведения в ASP.NET Core, такие, как WebHost builder APIs, Configuration основной сервис, изменения в [HTTP.sys](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/httpsys) и особонно приятный, на мой взгляд, IHostedServices интерфейс, котоый позволяет регистрировать дополнительные background процессы перед стартом ASP.NET Core, как то подписки на очереди сообщений, старт системы акторов, другие сервисы и все это используя теже зарегестрированние в контейнере сервисы. Джва года ждал этой фичи.

[F# and .NET Core Roadmap Update](https://blogs.msdn.microsoft.com/dotnet/2017/08/14/f-and-net-core-roadmap-update/)

[Runtime package store](https://docs.microsoft.com/en-us/dotnet/core/deploying/runtime-store)

Позволяет указать приложению, что на машине, на которую будет осуществлятся развертывание, предустановлены некоторые пакеты, и они не будут включены при релизе, что может значитально уменьшить колличество и размер библиотек, которые нужно копировать при релизе.

[The layout](https://blogs.msdn.microsoft.com/seteplia/2017/05/26/managed-object-internals-part-1-layout/)

[Object header layout and the cost of locking](https://blogs.msdn.microsoft.com/seteplia/2017/09/06/managed-object-internals-part-2-object-header-layout-and-the-cost-of-locking/)

[The layout of a managed array](https://blogs.msdn.microsoft.com/seteplia/2017/09/12/managed-object-internals-part-3-the-layout-of-a-managed-array-3/)

[Fields layout](https://blogs.msdn.microsoft.com/seteplia/2017/09/21/managed-object-internals-part-4-fields-layout/)

Отличная серия статей о внутренностях managed объектов.

[Configuring ASPNET Core Apps with WebHostBuilder](https://ardalis.com/configuring-aspnet-core-apps-with-webhostbuilder)

В статье показаны простые примеры как сконфигурировать сервисы и логирование перед запуском `Starup` класса.

[Could not load file or assembly 'netfx.force.conflicts'](https://github.com/dotnet/corefx/issues/23229)

Неприятная проблема, с котороый пришлось столкнуться при поэтапной миграции проекта на .NET Standard 2.0/.NET Core 2.0 и пути ее решения.

**Архитектура**

[Hewitt, Meijer and Szyperski: The Actor Model (everything you wanted to know...)](https://www.youtube.com/watch?v=7erJ1DV_Tlo)

[Avoiding all DI antipatterns for types requiring asynchronous initialization](https://stackoverflow.com/questions/45924027/avoiding-all-di-antipatterns-for-types-requiring-asynchronous-initialization/46027058)

Актульный вопрос о том, как конфигурировать объекты DI контейрерах, для которых нужна асинхронная инициализация. Рекомендуют делать инициализацию перед конфигурацие контейнера.

[Reactive Mistakes: Distributed Transactions](http://www.cakesolutions.net/teamblogs/reactive-mistakes-distributed-transactions)

Статья, о негативном влиянии распределенных транзакций на производительность системы.

[GraphQL vs REST: Overview](https://philsturgeon.uk/api/2017/01/24/graphql-vs-rest-overview/)

GraphQL и REST - это не конкуренты, а интсрументы для разных задач и могут сосуществовать.

**Инструменты**

[Bogus](https://github.com/bchavez/Bogus)

Генератор фейковых данный с осмысленными значаниями.

[Refit](https://paulcbetts.github.io/refit/)

Библиотека для автоматической генерации типизированных колиентов для REST API.

[Call and value tracking come to Rider](https://blog.jetbrains.com/dotnet/2017/09/27/call-value-tracking-come-rider/)

Удобный функционал для отслеживания откуда могло прийти значение переменной или где вызывается данный метод. Похоже, эта функция уже была в R#, но я как-то ее пропустил.

**CI/CD**

[Trunk-Based Development instead of GitFlow](https://twitter.com/IndritSelimi/status/902878608598986752)

Интересная дискуссия на счет организации работы с системами контроля версий.

[The Death of Continuous Integration](https://www.infoq.com/presentations/death-continuous-integration)

О том, как правильно организовать процесс CD.