# Microsoft SQL Sever on Mac - Apple Chip

## Configure Docker on Mac

> Download and Install: https://docs.docker.com/desktop/install/mac-install/

Create `.env` file and add `SA_PASSWORD` variable. You can see sample file `.env.example`.

> SA_PASSWORD is the password you will use to connect to SQL Server.

## Run SQL Server on Mac

```bash
docker-compose up -d
```

## Connect to SQL Server on VM

> Download and Install: https://www.parallels.com/

### Microsoft SQL Server Management Studio (SSMS)

> Download and Install: https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16&redirectedfrom=MSDN

- Server type: `Database Engine`
- Server name: `YOUR_MAC_IP`
- Authentication:
  - Login: `sa`
  - Password: `SA_PASSWORD` from `.env`

## Acknowledgments
- https://www.youtube.com/watch?v=co6TkSzc0s8
- https://learn.microsoft.com/en-us/dotnet/architecture/microservices/multi-container-microservice-net-applications/database-server-container
- https://docs.docker.com/compose/environment-variables/set-environment-variables/