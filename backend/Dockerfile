FROM mcr.microsoft.com/dotnet/sdk:5.0
WORKDIR /app
COPY *.csproj .
RUN "dotnet" "restore"
COPY . .
EXPOSE 80
ENTRYPOINT [ "dotnet", "watch", "run", "--urls", "http://0.0.0.0:80" ]
