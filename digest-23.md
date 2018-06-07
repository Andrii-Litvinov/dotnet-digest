**.NET**

[Allocation-free awaitable async operations with ValueTask&lt;T&gt; and ValueTask](https://github.com/dotnet/corefx/issues/27445)

[Migrating from aspnetcore docker repos to dotnet](https://github.com/aspnet/Announcements/issues/298)

[.NET Core Docker Samples](https://github.com/dotnet/dotnet-docker/blob/master/samples/README.md)

[System.IO in .NET Core 2.1 sneak peek](https://blogs.msdn.microsoft.com/jeremykuhne/2018/03/08/system-io-in-net-core-2-1-sneak-peek/)

[Custom directory enumeration in .NET Core 2.1](https://blogs.msdn.microsoft.com/jeremykuhne/2018/03/09/custom-directory-enumeration-in-net-core-2-1/)

[Go vs C#, part 1: Goroutines vs Async-Await](https://medium.com/@alexyakunin/go-vs-c-part-1-goroutines-vs-async-await-ac909c651c11)

[Develop ASP.NET Core Applications in a Container](https://github.com/dotnet/dotnet-docker/blob/master/samples/aspnetapp/aspnet-docker-dev-in-container.md)

[Performance traps of ref locals and ref returns in C#](https://blogs.msdn.microsoft.com/seteplia/2018/04/11/performance-traps-of-ref-locals-and-ref-returns-in-c/)

[Performance Improvements in .NET Core 2.1](https://blogs.msdn.microsoft.com/dotnet/2018/04/18/performance-improvements-in-net-core-2-1/)

Помимо прочего, значительные улучшения производительности и уменьшения аллокаций в асинхронных методах, и в работе с сетью (думаю, этому очень рад Dmitriy Onykyyenko)

[ASP.NET Core 2.1.0-preview2: Improvements to the Kestrel HTTP server](https://blogs.msdn.microsoft.com/webdev/2018/04/12/asp-net-core-2-1-0-preview2-improvements-to-the-kestrel-http-server/)

Kestrel перевели с libuv на собственною реализацют сокетов, что сделало его заметном более шустрым, особенно на Линуксе.

[Announcing .NET Core 2.1](https://blogs.msdn.microsoft.com/dotnet/2018/05/30/announcing-net-core-2-1/)

[.NET Core Hidden Gems](https://twitter.com/davidfowl/status/1004232622845804544)

David Fowler рассказывает про разные полезности в новом релизе.

[ObjectMethodExecutor](https://github.com/aspnet/Common/blob/ff87989d893b000aac1bfef0157c92be1f04f714/shared/Microsoft.Extensions.ObjectMethodExecutor.Sources/ObjectMethodExecutor.cs)

Оттуда же, метод, позволяющий эффективно вызывать методы объектов полученных через Reflection посредством построения Expression.

[Framework Benchmarks Round 16](https://www.techempower.com/blog/2018/06/06/framework-benchmarks-round-16/)

Производительность некоторых фреймворков, в том числе ASP.NET Core упирается в сетевой стек. И по остальным параметрам ASP.NET Core показывает невероятно крутые результаты. Ссылка в статье на результаты почему-то сломана, поэтому, [вот](https://www.techempower.com/benchmarks/#section=test&runid=aad43f39-48a2-460c-a363-99cd543a772a).

**Architecture**

[Event sourcing using Kafka](https://blog.softwaremill.com/event-sourcing-using-kafka-53dfd72ad45d)

Но есть нюансы, так как Kafka не поддерживат Optimistic Concurrency.

[Reactive DDD: Modeling Uncertainty](https://www.youtube.com/watch?v=MKLRXCiU5IE)

[Comparing AWS Lambda performance of Node.js, Python, Java, C# and Go](https://read.acloud.guru/comparing-aws-lambda-performance-of-node-js-python-java-c-and-go-29c1163c2581)

[Information Space-Time](https://thinkbeforecoding.com/post/2018/03/11/information-space-time)

[Time, Clocks, and the Ordering of Events in a Distributed System ](https://www.microsoft.com/en-us/research/uploads/prod/2016/12/Time-Clocks-and-the-Ordering-of-Events-in-a-Distributed-System.pdf)

Effective Aggregate Design [Part I](https://vaughnvernon.co/wordpress/wp-content/uploads/2014/10/DDD_COMMUNITY_ESSAY_AGGREGATES_PART_1.pdf), [Part II](https://vaughnvernon.co/wordpress/wp-content/uploads/2014/10/DDD_COMMUNITY_ESSAY_AGGREGATES_PART_2.pdf), [Part III](https://vaughnvernon.co/wordpress/wp-content/uploads/2014/10/DDD_COMMUNITY_ESSAY_AGGREGATES_PART_3.pdf)

Отличное эссе о принципах поектирования аггрегатов. Хотел бы чтобы оно попалось мне несколько лет назад. Очень рекомендую почитать.

[Vertical Slice Architecture](https://jimmybogard.com/vertical-slice-architecture/)

[Running Apache Kafka on Kubernetes](https://www.confluent.io/online-talks/stateful-stateless-and-serverless-running-apache-kafka-on-kubernetes)

**Tools**

[Introducing the JetBrains redistributable of MSBuild](https://blog.jetbrains.com/dotnet/2018/04/13/introducing-jetbrains-redistributable-msbuild/)

Кастомный билд для тех, у кого нет лицензии на VS.

[Learning best practices and language features using Rider code inspections](https://blog.jetbrains.com/dotnet/2018/05/23/learning-best-practices-language-features-using-rider-code-inspections/)

[Remediating the May 2018 Git Security Vulnerability](https://blogs.msdn.microsoft.com/devops/2018/05/29/announcing-the-may-2018-git-security-vulnerability/)

[Introducing the ReSharper performance series](https://blog.jetbrains.com/dotnet/2018/05/28/introducing-resharper-performance-series/)

Серия статей о планах и подходах для улучшения производительности R#.

[Version control improvements in Rider 2018.1](https://blog.jetbrains.com/dotnet/2018/06/05/version-control-improvements-rider-2018-1/)

**UI**

[Pixelpusher: Real-time peer-to-peer collaboration with React](https://medium.com/@pvh/pixelpusher-real-time-peer-to-peer-collaboration-with-react-7c7bc8ecbf74)

[dom-testing-library](https://github.com/kentcdodds/dom-testing-library)

**Books**

[Introducing GitHub, 2nd Edition](https://conferences.oreilly.com/oscon/oscon-or/public/content/introducing-github-2e)

[Designing Event-Driven Systems](https://www.confluent.io/designing-event-driven-systems)

**Разное**

[Developer Survey Results 2018](https://insights.stackoverflow.com/survey/2018/)

[What is “concurrent” access to mutable state?](https://proandroiddev.com/what-is-concurrent-access-to-mutable-state-f386e5cb8292)

[The Cost of Living Around the World 2018](https://www.movehub.com/blog/cost-of-living-worldwide-2018/)

Украина на третьем месте среди самых дешевых стран.

[People are not “Resources”](https://www.linkedin.com/pulse/people-resources-bogdan-vulcan/)

[Emoji code review](http://dawehner.github.io/github,/code/review/2017/09/08/emoji-code-review.html)

**Интересные твиты**

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">&quot;I don&#39;t ask permission to write a test or refactor any more than I ask permission to write an if statement or a for loop&quot; -<a href="https://twitter.com/RonJeffries?ref_src=twsrc%5Etfw">@RonJeffries</a> quoted at <a href="https://twitter.com/hashtag/sgcan?src=hash&amp;ref_src=twsrc%5Etfw">#sgcan</a></p>&mdash; Mishkin Berteig (@mberteig) <a href="https://twitter.com/mberteig/status/978266962810765312?ref_src=twsrc%5Etfw">March 26, 2018</a></blockquote>

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Do you know that you can use decostruction syntax to initialize more than one field/property in expression-body constructor?<br><br>And, BTW, the C# compiler is smart enough to eliminate a deconstruction code from the final assembly;) <a href="https://t.co/8cDCFx2JWD">pic.twitter.com/8cDCFx2JWD</a></p>&mdash; Sergey Teplyakov (@STeplyakov) <a href="https://twitter.com/STeplyakov/status/983206875582758912?ref_src=twsrc%5Etfw">April 9, 2018</a></blockquote>

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">know the difference between forward and back slash <a href="https://t.co/y0yxr1AmGX">pic.twitter.com/y0yxr1AmGX</a></p>&mdash; David Neal (@reverentgeek) <a href="https://twitter.com/reverentgeek/status/789135336437800960?ref_src=twsrc%5Etfw">October 20, 2016</a></blockquote>

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">&quot;Pipelined plaintext, that&#39;s fast, but the performance would be gone making a database call?&quot;<br><br>Non-pipelined, db query -&gt; html escape -&gt; utf-8 encode -&gt; format into html doc and table: 3.12Gb/s on a commodity server!<a href="https://twitter.com/hashtag/aspnetcore?src=hash&amp;ref_src=twsrc%5Etfw">#aspnetcore</a> is a 🚀 <br><br>/cc <a href="https://twitter.com/shayrojansky?ref_src=twsrc%5Etfw">@shayrojansky</a> <a href="https://t.co/vooxPgaMBO">pic.twitter.com/vooxPgaMBO</a></p>&mdash; Ben Adams (@ben_a_adams) <a href="https://twitter.com/ben_a_adams/status/1004641789653995520?ref_src=twsrc%5Etfw">June 7, 2018</a></blockquote>

<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>