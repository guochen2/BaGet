FROM mcr.microsoft.com/dotnet/core/aspnet:3.1-buster-slim AS base
WORKDIR /app
ENV ASPNETCORE_URLS=http://+:80
ENV Storage__Path=/var/baget/packages
ENV Database__ConnectionString="Data Source=/var/baget/baget.db"
ENV ApiKey=
RUN mkdir /var/baget
COPY . .
ENTRYPOINT ["dotnet", "BaGet.dll"]
