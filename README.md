# data-eval
.Net Library for Evaluating Expressions at Runtime

Available on Nuget, [Data.Eval](https://www.nuget.org/packages/Data.Eval/).

    Install-Package Data.Eval


[![NuGet](https://img.shields.io/nuget/dt/Data.Eval.svg)](https://www.nuget.org/packages/Data.Eval/)

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

### Simple Addition

```csharp
Evaluator.Eval("return 1+1")
```

[.Net Fiddle](https://dotnetfiddle.net/DTLu6Z)

### Variable Addition

```csharp
var evaluator = new Evaluator("return x+y");
evaluator["x"] = 1;
evaluator["y"] = 2;
Console.WriteLine("Result: " + evaluator.Eval());
```

[.Net Fiddle](https://dotnetfiddle.net/DTLu6Z)
