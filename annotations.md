## Comandos
 - dotnet add package Microsoft.EntityFrameworkCore.SqlServer --version=7.0.117
 - dotnet add package Microsoft.EntityFrameworkCore.Design --version=7.0.117

## Processos
Copiar o Data e Models do projeto anterior

## Detalhes de configuração
Quando for projeto no linux:
- adicionar <RuntimeIdentifier>ubuntu.22.04-x64</RuntimeIdentifier> no PropertyGroup do csproj depois do target framework
- adicionar ;Encrypt=False no final da connection string
Essas configurações evitam erro nos comandos abaixo.

## Comandos
    - dotnet ef migrations add CreateDatabase
    - dotnet ef database update
