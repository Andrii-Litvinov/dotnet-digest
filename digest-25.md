**.NET**

[ASP.NET Core 2.2.0-preview1: HTTP/2 in Kestrel](https://blogs.msdn.microsoft.com/webdev/2018/08/22/asp-net-core-2-2-0-preview1-http-2-in-kestrel/)

Server Push, к сожалению, пока не поддерживается и команда все еще решает включать ли его в эту версию.

[.NET Standard 2.1](https://github.com/dotnet/standard/blob/master/docs/planning/netstandard-2.1/README.md)

Документ, объясняет почему были принято такое решение версионирования и какие API будут включены. Основная идея - включить `Span<T>` в стандарт.

[Announcing .NET Standard 2.1](https://blogs.msdn.microsoft.com/dotnet/2018/11/05/announcing-net-standard-2-1/)

[Diagnosing .NET Core ThreadPool Starvation with PerfView](https://blogs.msdn.microsoft.com/vancem/2018/10/16/diagnosing-net-core-threadpool-starvation-with-perfview-why-my-service-is-not-saturating-all-cores-or-seems-to-stall/)

**Architecture**

[Event Store scavenging and the hidden cost of link events](https://www.jefclaes.be/2018/08/ges-scavenging-and-hidden-cost-of-link.html)

[Modeling Uncertainty with Reactive DDD](https://www.infoq.com/articles/modeling-uncertainty-reactive-ddd)

Хорошая статья на о подходе к распределенным системам. Я как-то давал ссылку на запись доклада, тут это оформлено в виде статьи. Стоит ознакомиться тем, кто работает с распределенными системами.

[Distributed Data Management](https://docs.aws.amazon.com/aws-technical-content/latest/microservices-on-aws/distributed-data-management.html)

Amazon Kinesis Streams как вариант Single Source of Truth системы (подобие Event Sourcing).

[Microservices & Distributed Monoliths](https://www.youtube.com/watch?v=aE-p0cfwTVU)

[Managing data consistency in a microservice architecture using Sagas](https://www.youtube.com/watch?v=7dy5WPSv2DQ)

Хорошее обзорное видео о сагах и как они помогают решать проблему распределенных транзакций.

[Not Just Events: Developing Asynchronous Microservices](https://skillsmatter.com/skillscasts/12115-keynote-not-just-events-developing-asynchronous-microservices)

Отличный Keynote c конференции, которая проходила вот только в этот понедельник.

[Microservices, Bounded Contexts, and Everything in Between](https://skillsmatter.com/skillscasts/12765-microservices-bounded-contexts-and-everything-in-between)

Отличный доклад оттуда же о том, как выбирать границы микросервисов. Там еще были интересные выступления, так что рекомендую посмотреть, может что-то еще будет актуально.

**Practices**

[TDD, Where Did It All Go Wrong](https://www.youtube.com/watch?v=EZ05e7EMOLM)

Отличное видео о том, что на самом деле такое Unit-тесты и как писать тесты так, чтобы они не ломались при рефакторинге.

**Tools**

[RetireNet](https://github.com/RetireNet/dotnet-retire)

Расширение, позволяющее проверить содержат ли NuGet пакеты известные уязвимости.

[Building a .NET IDE with JetBrains Rider](https://www.codemag.com/Article/1811091/Building-a-.NET-IDE-with-JetBrains-Rider)

Интересная статья о внутренностях разработки Rider.

[A Detailed Look at RFC 8446 (a.k.a. TLS 1.3)](https://blog.cloudflare.com/rfc-8446-aka-tls-1-3/)

[The software engineer’s guide to asserting dominance in the workplace](https://medium.com/feature-creep/the-software-engineer-s-guide-to-asserting-office-dominance-ddea7b598df7)

Детальное расписание на неделю с инструкциями как занять доминантное положение в новой компании на уровне с "On your first day at the new job, squash every commit from the repo into a single commit with message "Legacy code" and force-push to master".

**P.S.:** Предыдущие несколько месяцев я замечаю, что у меня сместился фокус интересов и времени для подготовки качественного материала для дайджестов остается совсем немного. Поэтому, если кому-то было бы интересно перенять эстафету - дайте знать мне или администрации. Если нет, возможно, какое-то время дайджесты немного похудеют и буду содержать только то, что было очень полезным для меня или чем я очень хочу поделиться. Потому как информации приходится фильтровать много.

**P.P.S.:** Кстати, 7-го Декабря буду выступать с докладом на [XP Days](https://xpdays.com.ua/), приходите послушать про [Event-Driven Systems Backed By MongoDB](https://xpdays.com.ua/programs/event-driven-systems-with-mongodb/). Если хотите пойти, но нет возможности купить билет за полную стоимость - напишите мне, у меня, как у докладчика, есть возможность получить два промокода на хорошую скидку.