# .net-scaffolding-my-sql

Document: 

https://learn.microsoft.com/en-us/ef/core/managing-schemas/scaffolding/?tabs=vs

https://learn.microsoft.com/en-us/ef/core/managing-schemas/scaffolding/?tabs=dotnet-core-cli

#1: Open command line: 

     D:\.net-scaffolding-my-sql\dotnet-scaffolding-my-sql

#2: Run docker compose to create new mysql: 

    docker compose up -d

#3: Create database: Run script.sql file

#4: Run cmd: 

    CD D:\.net-scaffolding-my-sql\dotnet-scaffolding-my-sql\dotnet-scaffolding-my-sql

#5: Run cmd to create DbContext and EntityModels: 

    dotnet ef dbcontext scaffold "Name=ConnectionString:DefaultConnection" Pomelo.EntityFrameworkCore.MySql -o EntityModels --data-annotations -c ScaffoldingMysqlDbContext

#Note:

	#2: If you alrealy have your database. You don't have need to this command "docker compose up -d". You just need to configure the your database parameters in the appsettings.json file
	
	
	#5: "Name=ConnectionString:DefaultConnection" in appsettings.json file
