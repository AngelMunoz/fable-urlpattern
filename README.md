[urlpattern api]: https://developer.mozilla.org/en-US/docs/Web/API/URL_Pattern_API

# Fable.URLPattern

This are the bindings for the [URLPattern APi]

if you're using this package in the browser/bun you might need a polyfill

which can be installed via `npm install urlpattern-polyfill` after thad don't forget to define a compiler directive in your F# project to enable the polyfill usage. Example:

```xml
<Project Sdk="Microsoft.NET.Sdk">

  <PropertyGroup>
    <TargetFramework>net6.0</TargetFramework>
    <GenerateDocumentationFile>true</GenerateDocumentationFile>
    <Version>1.0.0-beta-001</Version>
    <!-- This line below -->
    <DefineConstants>$(DefineConstants);ENABLE_URLPATTERN_POLYFILL</DefineConstants>
  </PropertyGroup>
    <!-- the rest of the *.fsproj file -->
</Project>
```

if your environment (e.g. deno/chromium browsers) already provide URLPattern then there's no need to install the polyfill or enable the compiler directive
