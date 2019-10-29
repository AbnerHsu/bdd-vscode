# bdd-vscode
Specflow on a .NET Core project using Visual Studio code

## Steps
1. Create a testing project from a dotnet core project template
```
dotnet new xunit
```
2. Creating a folder structure
``` 
- features 
- src
```
3. Add specflow dependencies
```
dotnet add package SpecFlow.xUnit
```
4. Clean and build project
```
dotnet clean
dotnet build
```
5. Create specflow.json
```
{
    "language":
    {
        "feature": "en-gb"
    }
 }
```
6. Auto generate feature.cs file by adding the following package
```
dotnet add package SpecFlow.Tools.MsBuild.Generation
```
7. Clean and build project to generate the feature.cs file automatically
```
dotnet clean
dotnet build
```
8. Create the step definition
Right click over the steps folder and select new “c# class”, we can name this class as “ExampleSteps.cs
### Extensions
- Snippets and Syntax Highlight for Gherkin (Cucumber)
- Gherkin step autocomplete
- C# Extensions

