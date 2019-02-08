**.NET**

[Practical samples for ASP.NET Core](https://github.com/dodyg/practical-aspnetcore/)

Очень классный репозиторий, в котором собрано множество примеров использования ASP.NET Core для разных задач. Большинство из низ в документации найти не получится. Очень рекомендую посмотреть.

[Building C# 8.0](https://blogs.msdn.microsoft.com/dotnet/2018/11/12/building-c-8-0/), [Take C# 8.0 for a spin](https://blogs.msdn.microsoft.com/dotnet/2018/12/05/take-c-8-0-for-a-spin/), [Do more with patterns in C# 8.0](https://blogs.msdn.microsoft.com/dotnet/2019/01/24/do-more-with-patterns-in-c-8-0/)

Обзор новых фич C# 8.0. Особенно интересно с pattern matching и using declarations.

[Performance Tuning for .NET Core](https://reubenbond.github.io/posts/dotnet-perf-tuning)

[Pattern matching in action using C# 6](http://tomasp.net/blog/2015/csharp-pattern-matching/)

Какая-то жесть с использованием исключений, но любопытно как народ изгаляется.

[ASP.NET Core: Saturating 10GbE at 7+ million request/s](https://www.ageofascent.com/2019/02/04/asp-net-core-saturating-10gbe-at-7-million-requests-per-second/)

Классная статья о текущем положении дел с производительностью в ASP.NET Core.

**Architecture**

[Apache Kafka is not for Event Sourcing](https://medium.com/serialized-io/apache-kafka-is-not-for-event-sourcing-81735c3cf5c)

Часто слышу, как люди заблуждаются на этот счет. Отличная статья с объяснениями на этот счет.

**Tools**

[.NET Diagnostics Tools](https://github.com/aspnet/AspLabs/tree/master/src/DotNetDiagnostics)

[Enable repeatable package restores using a lock file](https://blog.nuget.org/20181217/Enable-repeatable-package-restores-using-a-lock-file.html)

Интересный подход, думаю как-то попробовать.

**Разное**

[Freelancing in America 2018](https://www.upwork.com/i/freelancing-in-america/2018/)

Ежегодный отчет от Upwork

[GitHub Free users now get unlimited private repositories](https://techcrunch.com/2019/01/07/github-free-users-now-get-unlimited-private-repositories/)

[10 Personal Finance Lessons for Technology Professionals](https://www.troyhunt.com/10-personal-finance-lessons-for-technology-professionals/)

Очень занимательное чтиво. Полностью пока не осилил, но периодически к нему возвращаюсь.

[You're Wasting Your Time](https://news.gallup.com/businessjournal/928/youre-wasting-your-time.aspx)

**Tips & Tricks**

Несколько выпусков назад я рассказывал, что мы перевели проект на .NET Standard. И вот наконец-то мигрировали первый достаточно большой API на ASP.NET Core. Получилось очень круто и практически безболезненно. Я создал новый проект, вынес логику контроллеров в отдельные сервисы 1:1 (у нас тонкие контроллеры в основном), скопировал контроллеры в новый проект, немного поправил атрибуты и остальные вещи которые отличаются от WebAPI. Кроме этого, конечно, нужно было реализовать несколько интерфейсов сервисов, которые напрямую использовали System.Web, используя API .NET Core. При этом старый проект остался в .sln и при необходимости его можно задеплоить из Octopus в случае проблем .NET Core. Такой-себе backup plan. Через несколько недель удалим его полностью.

Еще один момент, который мне очень нравится в dotnet cli, это возможность запуска проектов из консоли, например `dotnet run Project.Directory.Name -- args`. Это позволяет удобно создавать разные утилитки и запускать их без явной компиляции как в dev окружении так и на CI. Например, у нас есть утилита, которая генерит триггеры для TeamCity и инструкции COPY для Dockerfile на основании зависимостей проекта. Повторюсь, очень удобно.

**XP Days 2018**

В прошлом выпуске я писал, что буду выступать на XP Days 2018. Конференция была отличная, много интересных докладов и общения. Своим выступлением [Event-Driven Systems With MongoDB](https://www.youtube.com/watch?v=4iTZUidlPJA) я доволен, хотя на видео и заметно, что я сильно нервничал. Это был мое первое выступление и лечится это только практикой. На lightning talk на DDD EU было уже проще. Если будете смотреть конструктивная критика очень приветствуются! Это поможет мне в будущем выступать лучше.

**Amazon Hiring Event Jan 21-25**

Как многие уже знают, в Киеве недавно прошел Amazon Hiring Event. [Vitaliy Bondarenko](https://dou.ua/users/VitaliyB/) организовал группу с Slack для подготовки к ивенту, проводил вебинары и mock-interview за что ему огромное спасибо! Весь процесс подготовки был очень увлекательными и продуктивным. Мы собирались с ребятами офлайн, решали задачи у доски и обсуждали разные вопросы с этим связанные, Решали алгоритмические задачки и задачи на System Design, созваниваясь в Skype, и с нетерпением ждали результатов каждого участника на каждом этапе - было очень весело. На митапе перед серией интервью мы познакомились с командами/интервьюерами из Амазона, пообщались, здорово провели время. Само интервью у меня прошло очень живо, много интересных дискуссий и интересных задач. В целом мне очень понравилось, много позитивных эмоций от общения и challange-а. Поэтому очень рекомендую поучаствовать в новых ивентах. Другие команды собираются приехать вот уже в марте, я думаю, скоро будет анонс, но не уверен. Так же собираются провести еще один инвент осенью.

Вот некоторые ссылки, которые мне помогли в подготовке.

[Interviewing at Amazon — Leadership Principles](hhttps://medium.com/@scarletinked/are-you-the-leader-were-looking-for-interviewing-at-amazon-8301d787815d)

[The System Design Primer](https://github.com/donnemartin/system-design-primer)

[Grokking the System Design Interview](https://www.educative.io/collection/5668639101419520/5649050225344512)

[InterviewBit Programming](https://www.interviewbit.com/courses/programming/)

[Cracking the Coding Interview](https://www.amazon.com/dp/0984782850/)

С удовольствием отвечу на вопросы.