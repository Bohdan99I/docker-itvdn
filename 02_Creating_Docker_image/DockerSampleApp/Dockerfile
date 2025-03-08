FROM mcr.microsoft.com/dotnet/sdk:5.0-focal as build

EXPOSE 5000

ENV ASPNETCORE_URLS=http://*:5000

WORKDIR /src
COPY "DockerSampleApp.csproj" "./"
RUN dotnet restore "DockerSampleApp.csproj"

COPY . .

RUN dotnet build "DockerSampleApp.csproj" -c Release -o /app/build
RUN dotnet publish "DockerSampleApp.csproj" -c Release -o /app/publish

FROM mcr.microsoft.com/dotnet/aspnet:5.0-focal as runtime
COPY --from=build /app/publish .
ENTRYPOINT [ "dotnet", "DockerSampleApp.dll" ]