# DotNetCoreBackend

setup environment. If you not install .NET, then folow [this script](https://docs.microsoft.com/en-us/dotnet/core/install/linux-ubuntu)

```script
wget https://packages.microsoft.com/config/ubuntu/21.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-5.0
sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y aspnetcore-runtime-5.0
```

Create service:

```script
dotnet new worker -o <service name>
dotnet restore
```

```script
dotnet new console
dotnet restore
```

```script
dotnet new mvc -au NONE
dotnet restore
```
