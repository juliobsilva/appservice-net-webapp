# appservice-net-webapp

# Crie a solução
dotnet new sln -n MeuProjeto

# Crie o projeto ASP.NET Core MVC
dotnet new mvc -n MeuProjeto

# Adicione o projeto à solução
dotnet sln MeuProjeto.sln add MeuProjeto/MeuProjeto.csproj

# Crie o projeto de testes
dotnet new xunit -n MeuProjeto.Tests

# Adicione o projeto de testes à solução
dotnet sln MeuProjeto.sln add MeuProjeto.Tests/MeuProjeto.Tests.csproj

# Adicione a referência do projeto principal ao projeto de testes
dotnet add MeuProjeto.Tests/MeuProjeto.Tests.csproj reference MeuProjeto/MeuProjeto.csproj