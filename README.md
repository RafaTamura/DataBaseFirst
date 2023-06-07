# Entity Mini tutorial do DataBase First 
Este repositório foi utilizado para estudos com o entity framework O entity permite o mapeamento dos elementos do Banco de Dados para os elementos da aplicação, ela possui três linhas principais de utilização 

1 - Database First - Quando o BD já existe (Utilizado neste exemplo)

2 - Model First - É um modelo vazio 

3 - Code First - (Cria o banco de dados, e a manipulação de dados é realizada totalmente no Visual Studeo)

Este framework auxilia muito na produtividade

## Primeiro instale os pacotes NuGet

NuGet\Install-Package Microsoft.EntityFrameworkCore -Version 7.0.5
NuGet\Install-Package Microsoft.EntityFrameworkCore.Tools -Version 7.0.5
NuGet\Install-Package Microsoft.EntityFrameworkCore.SqlServer -Version 7.0.5
NuGet\Install-Package Microsoft.EntityFrameworkCore.Proxies -Version 7.0.5

## Code First
No terminal do NuGet foi utilizado os comandos Add-Migration Initial (Criação da pasta Migration) e o Update-Database (Case sensitive) este atualiza o BD no SQL. (Code First)

## DataBase First

Digitar no console: Scaffold-DbContect”” (entre as aspas colocar a string de conexão) por exemplo:
Scaffold-DbContext "Data Source=localhost;Initial Catalog=DBFirst;Integrated Security=True;Connect Timeout=30;Encrypt=False;TrustServerCertificate=False;ApplicationIntent=ReadWrite;MultiSubnetFailover=False"

Se tudo deu certo agora ele solicitará o provedor, pode inserir este:
Provider: Microsoft.EntityFrameworkCore.SqlServer
