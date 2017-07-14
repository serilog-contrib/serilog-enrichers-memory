# Serilog.Enrichers.Memory

The memory usage enricher for Serilog.

[![Build status](https://ci.appveyor.com/api/projects/status/22t518uadi80n9ge?svg=true)](https://ci.appveyor.com/project/JoshSchreuder/serilog-enrichers-memory) [![NuGet Version](https://img.shields.io/nuget/v/Serilog.Enrichers.Memory.svg)](https://www.nuget.org/packages/Serilog.Enrichers.Memory/)


# Documentation

To use the enricher, first install the NuGet package:

```powershell
Install-Package Serilog.Enrichers.Memory
```

Then enrich your logging configuration:

```csharp
new LoggerConfiguration()
    .Enrich.WithMemoryUsage();
```

And finally utilise the token in your logging template:

```csharp
var template = "{MemoryUsage}";
```

Copyright &copy; 2017 Josh Schreuder - Provided under the [Apache License, Version 2.0](http://apache.org/licenses/LICENSE-2.0.html).
