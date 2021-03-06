**.NET**

[ASP.NET Core 2.0 Authentication and Authorization System Demystified](https://digitalmccullough.com/posts/aspnetcore-auth-system-demystified.html)

Общее представление о том, как устроена аутентификация и авторизация в ASP.NET 2.0.

[Zero Garbage Collector for .NET Core](http://tooslowexception.com/zero-garbage-collector-for-net-core/)

Пример реализации GC, который не собирает мусор. Может быть полезно для небольших утилит, чтобы выжать максимум производительности.

[ASP.NET Core 2.0 Features](https://blogs.msdn.microsoft.com/webdev/2017/08/25/asp-net-core-2-0-features-1/)

Нововведения в ASP.NET Core, такие, как WebHost builder APIs, Configuration основной сервис, изменения в [HTTP.sys](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/httpsys) и особенно приятный, на мой взгляд, IHostedServices интерфейс, который позволяет регистрировать дополнительные background процессы перед стартом ASP.NET Core, как то подписки на очереди сообщений, старт системы акторов, другие сервисы и все это используя те же зарегистрированные в контейнере сервисы. Джва года ждал этой фичи.

[F# and .NET Core Roadmap Update](https://blogs.msdn.microsoft.com/dotnet/2017/08/14/f-and-net-core-roadmap-update/)

[Runtime package store](https://docs.microsoft.com/en-us/dotnet/core/deploying/runtime-store)

Позволяет указать приложению, что на машине, на которую будет осуществляться развертывание, предустановлены некоторые пакеты, и они не будут включены при релизе, что может значитально уменьшить количество и размер библиотек, которые нужно копировать при релизе.

[The layout](https://blogs.msdn.microsoft.com/seteplia/2017/05/26/managed-object-internals-part-1-layout/), [Object header layout and the cost of locking](https://blogs.msdn.microsoft.com/seteplia/2017/09/06/managed-object-internals-part-2-object-header-layout-and-the-cost-of-locking/), [The layout of a managed array](https://blogs.msdn.microsoft.com/seteplia/2017/09/12/managed-object-internals-part-3-the-layout-of-a-managed-array-3/), [Fields layout](https://blogs.msdn.microsoft.com/seteplia/2017/09/21/managed-object-internals-part-4-fields-layout/)

Отличная серия статей о внутренностях managed объектов.

[Configuring ASPNET Core Apps with WebHostBuilder](https://ardalis.com/configuring-aspnet-core-apps-with-webhostbuilder)

В статье показаны простые примеры как сконфигурировать сервисы и логирование перед запуском `Starup` класса.

[Could not load file or assembly 'netfx.force.conflicts'](https://github.com/dotnet/corefx/issues/23229)

Неприятная проблема, с которой пришлось столкнуться при поэтапной миграции проекта на .NET Standard 2.0/.NET Core 2.0 и пути ее решения.

**Архитектура**

[Hewitt, Meijer and Szyperski: The Actor Model (everything you wanted to know...)](https://www.youtube.com/watch?v=7erJ1DV_Tlo)

[Avoiding all DI antipatterns for types requiring asynchronous initialization](https://stackoverflow.com/questions/45924027/avoiding-all-di-antipatterns-for-types-requiring-asynchronous-initialization/46027058)

Актульный вопрос о том, как конфигурировать объекты в DI контейрерах, для которых нужна асинхронная инициализация. Рекомендуют делать инициализацию перед конфигурацией контейнера.

[Reactive Mistakes: Distributed Transactions](http://www.cakesolutions.net/teamblogs/reactive-mistakes-distributed-transactions)

Статья, о негативном влиянии распределенных транзакций на производительность системы.

[GraphQL vs REST: Overview](https://philsturgeon.uk/api/2017/01/24/graphql-vs-rest-overview/)

GraphQL и REST - это не конкуренты, а интсрументы для разных задач и могут сосуществовать.

**Инструменты**

[Bogus](https://github.com/bchavez/Bogus)

Генератор фейковых данных с осмысленными значениями.

[Refit](https://paulcbetts.github.io/refit/)

Библиотека для автоматической генерации типизированных клиентов для REST API.

[Call and value tracking come to Rider](https://blog.jetbrains.com/dotnet/2017/09/27/call-value-tracking-come-rider/)

Удобный функционал для отслеживания откуда могло прийти значение переменной или где вызывается данный метод. Похоже, эта функция уже была в R#, но я как-то ее пропустил.

[AutoFixture: Test name strategies for NUnit3](https://github.com/AutoFixture/AutoFixture/wiki/Known-Issues#test-name-strategies-for-nunit3)

Релиз 3.51 решает проблему именования тестов с динамическими параметрами для VS и NCrunch с помощью атрибутов `AutoDataFixedName` и `InlineAutoDataFixedName`.

[Respawn vs SQL Server Snapshots](https://jimmybogard.com/respawn-vs-sql-server-snapshots/)

Respawn подготавливает состояние БД перед тестом на порядки быстрее, чем восстановление из слепка. Тем не менее, как говорит автор, оптимальнее всего огранизовывать тесты таким образом, чтобы они не зависили от состояния таблиц. Это увеличит скорость тестов и позволит выполнять их параллельно.

**CI/CD**

[Trunk-Based Development instead of GitFlow](https://twitter.com/IndritSelimi/status/902878608598986752)

Интересная дискуссия на счет организации работы с системами контроля версий.

[The Death of Continuous Integration](https://www.infoq.com/presentations/death-continuous-integration)

О том, как правильно организовать процесс CD.

**UI**

[Polymer 3.0 preview: npm and ES6 Modules](https://www.polymer-project.org/blog/2017-08-22-npm-modules)

Polymer переезжает на ES6 модули, что позволит намного проще использовать компоненты в других фреймворках.

[Custom Elements Everywhere](https://custom-elements-everywhere.com/)

Сайт, который показывает насколько хорошо Custom Elements поддерживаются разными фреймворками.

[Use TypeScript to Develop Vue.js Web Applications](https://egghead.io/courses/use-typescript-to-develop-vue-js-web-applications)

[Polymer 3.0 Preview — Building a mini card game](https://medium.com/@jecelynyeen/polymer-3-0-preview-building-a-mini-card-game-ce8948265fd6)

Мини-игра построенная на Polymer 3.0 с TypeScript, WebPack и вынесенной в отдельный файл разметкой для компонента.

[Announcing TypeScript 2.5](https://blogs.msdn.microsoft.com/typescript/2017/08/31/announcing-typescript-2-5/)

**Книги**

[Understand The Actor Model From The Ground Up (In < 1 Hour)](https://www.lightbend.com/blog/designing-reactive-systems-with-the-actor-model-free-oreilly-book-by-hugh-mckee)

Довольно интересная небольшая бесплатная книга для понимания модели акторов.

**Видео**

[Progressive .NET London 2017](https://skillsmatter.com/conferences/8268-progressive-dot-net-2017#skillscasts)

[NDC Sydney 2017](https://www.youtube.com/watch?v=63k0Zc3yWb4&list=PL03Lrmd9CiGdch9Ul3PynPDZcZ18sz9KV)

**События**

[Microsoft Connect();](https://www.microsoft.com/en-us/connectevent) November 15-17, 2017

**Разное**

[How image recognition and AI recruit new employees](https://twitter.com/ValaAfshar/status/904097878049779712)

[Deploying Docker Compose to production](https://twitter.com/yogthos/status/910530558832336901)