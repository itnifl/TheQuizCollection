# C# and ASP.NET Core Web API

[← All courses](../readme.md)

> **Link types:** 📝 starts a quiz · 📖 opens reading material (lecture notes, course pages, external sites)

[![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)](https://en.wikipedia.org/wiki/C_Sharp_(programming_language))
[![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)](https://en.wikipedia.org/wiki/ASP.NET_Core)
[![LINQ](https://img.shields.io/badge/LINQ-68217A?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/Language_Integrated_Query)
[![Async / Await](https://img.shields.io/badge/Async%20%2F%20Await-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)](https://en.wikipedia.org/wiki/Async/await)
[![REST API](https://img.shields.io/badge/REST%20API-25A162?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/REST)

General-purpose quizzes on core C# language features and ASP.NET Core Web API development. Most questions show a short code snippet that you must read carefully before choosing an answer.

## Contents

- [Part 1 – C# fundamentals and Web API essentials](#part-1--c-fundamentals-and-web-api-essentials)
- [Part 2 – ValueTask and records](#part-2--valuetask-and-records)
- [Part 3 – Language fundamentals, records and strings](#part-3--language-fundamentals-records-and-strings)
- [Part 4 – Async, LINQ and ASP.NET Core services](#part-4--async-linq-and-aspnet-core-services)
- [Part 5 – Web APIs, HTTP and REST](#part-5--web-apis-http-and-rest)

### Part 1 – C# fundamentals and Web API essentials

*C# language fundamentals (value vs reference types, `const` vs `readonly`, records, `using`, nullable types, pattern matching, `yield`, LINQ, `IEnumerable` vs `IQueryable`, equality and `GetHashCode`, generic constraints, extension methods, `ConfigureAwait`) and ASP.NET Core Web API essentials (controllers, routing, `[From*]` model binding, headers, `[ApiController]` validation, `[Authorize]` / `[AllowAnonymous]`, DI lifetimes, middleware ordering, CORS, `IOptions`, `ILogger`, `IHttpClientFactory`, `CancellationToken`, `System.Text.Json` defaults, idempotent verbs and REST conventions).*

📝 **Quiz:** [C# and Web API – Part 1](https://dev-quizmachine.itautomasjon.no/Quiz/Take/CSharp-Quiz-1)

**Topics:** Value vs reference types · Nullable types & `default(T)` · `const` vs `static readonly` · DLL hot-swap inlining considerations · Records & immutability · Pattern matching & switch expressions · `using` / `IDisposable` · `yield` & deferred execution · LINQ operators · `IEnumerable<T>` vs `IQueryable<T>` · `Equals` & `GetHashCode` · Generic constraints · Extension methods · `ConfigureAwait(false)` in libraries · `[ApiController]` & routing · `[FromRoute]` / `[FromQuery]` / `[FromHeader]` / `[FromBody]` · Reading request headers · Model validation & ProblemDetails · `[Authorize]` / roles · DI lifetimes (Scoped/Transient/Singleton) · Middleware ordering · CORS configuration · `IOptions` / `IOptionsSnapshot` · `ILogger` structured templates · `IHttpClientFactory` · `CancellationToken` & `RequestAborted` · `System.Text.Json` defaults · REST conventions & idempotent verbs · HTTP status codes · `IActionResult` / `ActionResult<T>`

[↑ Back to top](#c-and-aspnet-core-web-api)

### Part 2 – ValueTask and records

*`ValueTask<T>` allocation semantics and correct consumption patterns, plus an in-depth look at C# records: positional records, `record struct`, `readonly record struct`, `with` expressions, compiler-generated members and equality.*

📝 **Quiz:** [C# and Web API – Part 2](https://dev-quizmachine.itautomasjon.no/Quiz/Take/CSharp-Quiz-2)

**Topics:** `ValueTask<T>` vs `Task<T>` · Appropriate uses of `ValueTask<T>` · Consuming `ValueTask` correctly · Awaiting twice / `.AsTask()` pitfalls · `ValueTask<T>` allocation behavior · Sync hot path vs async fallback · Positional record class · Compiler-generated members for records · Record value equality (`==` / `Equals`) · `ReferenceEquals` & `GetHashCode` on records · `record struct` (mutable) · `readonly record struct` (init-only) · `with`-expressions on records · `with` on `record struct` vs `record class` · `record class` vs `record struct` · Inheritance & extending positional records

[↑ Back to top](#c-and-aspnet-core-web-api)

### Part 3 – Language fundamentals, records and strings

*12 randomly selected questions, four each from C# language fundamentals, records and strings: core type behaviour, modern record types, equality, immutability, interpolation and efficient string building.*

📝 **Quiz:** [C# and Web API – Part 3](https://dev-quizmachine.itautomasjon.no/Quiz/Take/csharp-quiz-3)

**Topics:** Reference types and value types · Default values and nullable value types · `const` vs `readonly` · Null-conditional operators · `try` / `finally` execution · Switch expressions · Positional record classes · Compiler-generated record members · Record value equality · `record class` vs `record struct` · Mutable and `readonly record struct` · `with`-expressions and nondestructive mutation · `System.String` behavior · String immutability · `StringBuilder` for repeated concatenation · String interpolation and extension methods

[↑ Back to top](#c-and-aspnet-core-web-api)

### Part 4 – Async, LINQ and ASP.NET Core services

*12 randomly selected questions, four each from asynchronous programming, LINQ and data access, and ASP.NET Core services: correct async behaviour, efficient query execution, dependency injection, configuration, logging and HTTP client management.*

📝 **Quiz:** [C# and Web API – Part 4](https://dev-quizmachine.itautomasjon.no/Quiz/Take/csharp-quiz-4)

**Topics:** `Task<T>` and `ValueTask<T>` · Synchronous completion and allocation behavior · Consuming `ValueTask<T>` correctly · Multiple-await and `.AsTask()` pitfalls · `.Result` / `.Wait()` risks · `ConfigureAwait(false)` in reusable libraries · LINQ deferred execution · Iterator methods and `yield return` · `IEnumerable<T>` vs `IQueryable<T>` · Server-side EF Core query composition · ASP.NET Core dependency-injection lifetimes · Options pattern and configuration binding · Structured logging · Message templates vs string interpolation · `IHttpClientFactory` · Managing outgoing HTTP connections correctly

[↑ Back to top](#c-and-aspnet-core-web-api)

### Part 5 – Web APIs, HTTP and REST

*12 randomly selected questions, four each from ASP.NET Core Web APIs, HTTP and REST, and ASP.NET Core services: controller behaviour, routing, validation, authentication, REST semantics, CORS, dependency injection, configuration, logging and outgoing HTTP calls.*

📝 **Quiz:** [C# and Web API – Part 5](https://dev-quizmachine.itautomasjon.no/Quiz/Take/csharp-quiz-5)

**Topics:** `[ApiController]` behavior · Model binding and automatic validation · Controller routing and route constraints · Route, query, body, and header values · `ControllerBase` and action return types · Middleware ordering · Authorization and `[AllowAnonymous]` · HTTP `401` vs `403` · HTTP methods and idempotency · REST-style resource design · JSON content types and serialization · CORS for browser clients · Dependency-injection lifetimes · Options pattern and configuration binding · Structured logging and `IHttpClientFactory` · Request cancellation and service reliability

[↑ Back to top](#c-and-aspnet-core-web-api)
