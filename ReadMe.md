The monolith has become the ugly sweater. It has plenty of utility, but none of the fashion of trendy microservices. The project will document builing an ugly sweater monolith and then transforming it into
a microservices application.



## Building the Monolith

Using the command line, create the backend as a web api project, the frontend as a Blazor WASM project, and a shared class library for models and repitive logic.


```dotnet new webapi -n backend```
```dotnet new blazorwasm -n frontend```
```dotnet new classlib -n shared```

```
dotnet new sln
dotnet sln add frontend backend shared
```

* Set the solution to have multiple start-up projects.


Run it in Visual Studio and both the Blazor app and the Web Api backend should come up

## Transform the Monolith into a Microservices Application