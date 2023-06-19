# Clean-Architecture--Asp.Net-Core

Create a repo in git.
<br>Clone this repo.
<br>In this repo, create a src folder, create Services folder and run this command in src folder "dotnet new sln --name ShoppingMart-Services"
<br>
<br>push to git by commands:
<br>git add .
<br>git commit -m "Init"
<br>git push
<br>
<br>In services folder, add folder Ordering.
<br>
<br>in Ordering folder run commands : 
<br>dotnet new webapi --name Ordering.API (or) func init Ordering.Processors
<br>dotnet new classlib --name Ordering.Domain
<br>dotnet new classlib --name Ordering.Infrastructure
<br>dotnet new classlib --name Ordering.ApplicationCore
<br>
<br>in src folder run commands: 
<br>dotnet sln add Services\Ordering\Ordering.API --solution-folder src\Services\Ordering
<br>dotnet sln add Services\Ordering\Ordering.Domain --solution-folder src\Services\Ordering
<br>dotnet sln add Services\Ordering\Ordering.Infrastructure --solution-folder src\Services\Ordering
<br>dotnet sln add Services\Ordering\Ordering.ApplicationCore --solution-folder src\Services\Ordering
