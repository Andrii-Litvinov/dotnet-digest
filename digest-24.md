**.NET**

[Dissecting new generic constraints in C# 7.3](https://blogs.msdn.microsoft.com/seteplia/2018/06/12/dissecting-new-generics-constraints-in-c-7-3/)

[Staying up-to-date with .NET Container Images](https://blogs.msdn.microsoft.com/dotnet/2018/06/18/staying-up-to-date-with-net-container-images/)

[Hosting services in .NET Core console application](https://thinkrethink.net/2018/08/02/hostbuilder-ihost-ihostedserice-console-application/)

[System.IO.Pipelines: High performance IO in .NET](https://blogs.msdn.microsoft.com/dotnet/2018/07/09/system-io-pipelines-high-performance-io-in-net/)

[How to: Enable and Disable Automatic Binding Redirection](https://docs.microsoft.com/en-us/dotnet/framework/configure-apps/how-to-enable-and-disable-automatic-binding-redirection)

**Architecture**

[Is there any good open source C# sharding framework?](https://www.quora.com/Is-there-any-good-open-source-C-sharding-framework/answer/Greg-Young-8)

Интересный ответ почему шардинг - это не просто.

[Microservices, events, and upside-down databases](https://www.oreilly.com/ideas/microservices-events-and-upside-down-databases)

[The Proper Care and Feeding of Akka.NET Clusters: Understanding Reachability vs. Membership](https://petabridge.com/blog/proper-care-of-akkadotnet-clusters/)

[Greg Young - The art of destroying software](https://vimeo.com/108441214)

Относительно старое, но очень актуальное видео о том, что стоит разрабатывать сервисы так, чтобы их можно было легко удалить и переписать наново вместо того, чтобы тратить время и разбираться как там что работает внутри.

[From Secure Messaging to Secure Collaboration](http://martin.kleppmann.com/2018/03/20/security-protocols-workshop.html)

[REST vs. GraphQL: A Critical Review](https://blog.goodapi.co/rest-vs-graphql-a-critical-review-5f77392658e7)

Спорное мнение о том, что GraphQL - для тех, кто неумеет в REST.

[Event Sourcing in Action with eBay's Continuous Delivery Team](https://www.ebayinc.com/stories/blogs/tech/event-sourcing-in-action-with-ebays-continuous-delivery-team/)

Любопытный подход к реализации EventSourcing'а c MongoDB и Akka.

[7 best practices for building containers](https://cloudplatform.googleblog.com/2018/07/7-best-practices-for-building-containers.html)

[Goodbye Microservices: From 100s of problem children to 1 superstar](https://segment.com/blog/goodbye-microservices/)

[Consistency Models](https://jepsen.io/consistency)

[CRDTs and the Quest for Distributed Consistency](https://www.infoq.com/presentations/crdt-distributed-consistency)

**Tools**

[Unit test coverage and continuous testing. Now in Rider!](https://blog.jetbrains.com/dotnet/2018/07/20/unit-test-coverage-continuous-testing-now-rider/)

Пришло счатье к пользователям Райдера. Сильно уступает NCrunch, конечно, но уже что-то. Так как я переполз на Райдер уже польше полутора лет назад, для меня это просто потрясающая новость.

[An update on what's happening with protobuf-net](https://blog.marcgravell.com/2018/08/protobuf-net-august-2018-update.html)

Еще одна бімба. Теперь можно просто описать сообщение в .proto файле и C# класс будет сгенерен перед компиляцией в /obj папку. Не нужно больше захламлять проект сгенеренными файлами.

[Version control improvements in Rider 2018.1](https://blog.jetbrains.com/dotnet/2018/06/05/version-control-improvements-rider-2018-1/)

Крутая штука. Полностью перешел на работу с гитом их Райдера. Все невероятно шутро работает даже на больших проектах. До этого пользовался SorceTree и GitKraken.

**UI**

[React Native: A retrospective from the mobile-engineering team at Udacity](https://engineering.udacity.com/react-native-a-retrospective-from-the-mobile-engineering-team-at-udacity-89975d6a8102)

[Announcing TypeScript 3.0](https://blogs.msdn.microsoft.com/typescript/2018/07/30/announcing-typescript-3-0/)

**Разное**

[Backdoored images downloaded 5 million times finally removed from Docker Hub](https://arstechnica.com/information-technology/2018/06/backdoored-images-downloaded-5-million-times-finally-removed-from-docker-hub/)

[How Good Are Your Estimation Skills?](https://www.timecockpit.com/blog/2013/07/19/How-Good-Are-Your-Estimation-Skills)

[The State of Developer Ecosystem in 2018](https://www.jetbrains.com/research/devecosystem-2018/)

[Technical debt isn't technical - Einar W. Høst](https://www.youtube.com/watch?v=CXyNZYDO07Q)

Первые 15 минут обязательно стоит посмотреть чтобы понимать что нужно для хорошего рефакторинка. Дальше больше вода, но все равно можно глянуть.

**События**

26-27 октября в Киеве пройдет коференция [.NET Fest 2018](www.dotnetfest.com). Организаторы поделились 10%-й скидкой на билеты по промокоду **DOUDIGEST**.



В этом дайджесте материала меньше, чем обычно, лето, ведь. Поэтому, я решил поделиться радостью: мы с командой наконец-то решились перевести проект на PackageReference чтобы дальше мигрировать на .NET Standard/.NET Core. Проект довольно большой больше - ста проектов (простите за тавтологию). Миграция у меня заняла чуть больше дня. Были некоторые трудности с переводом Web API проектов, так как они не поддреживаюится из коробки, поэтому применялись некоторые хаки. И какое-то время заняла праильная настройка binding redirects. А вцелом все прошло довольно гладко. После этого мигрировал некоторые проекты на .NET Standard 2.0 - все замечательно вместе работает. Я делилтся впечатлениями в командном чате, вот несколько цитат:

> One of the benefits of package reference is that now we’ll predictably get the version of the package if multiple versions are present in the solution. Which makes it easier to deal with binding redirects. Previously assembly could have been overwritten by earlier version and break the redirect setting.

> Another cool feature of PackageReference is when you reference project that has a dependency on a package you don't need to add that other dependency to your project. E.g.: if Model project defines a reference to MongoDB.Driver we don't have to reference MongoDB.Driver in any other project in the entire solution to use it. Clean.

> With PackageReference it is possible to perform a regex find-and-replace to update/modify package version to update/consolidate packages which will perform incredibly fast comparing to doing it via UI. Still excited about it 😊.

Вот собственно статья, в которой описаны детали [How NuGet resolves package dependencies](https://docs.microsoft.com/en-us/nuget/consume-packages/dependency-resolution). Поэтому, очень рекомендую. Если есть вопросы - пишите в комментариях, попробую помочь.