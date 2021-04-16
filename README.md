# BashScripts
Self notes

sudo apt -y update ; sudo apt -y upgrade ; sudo apt -y install git ; sudo apt -y install vim

# .NET
```
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb \
sudo dpkg -i packages-microsoft-prod.deb \
sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-5.0
  ```

# Lettuce Encrypt
dotnet new mvc  
dotnet add package LettuceEncrypt --version 1.0.1

Add to appsettings.json:

```{
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft": "Warning",
      "Microsoft.Hosting.Lifetime": "Information"
    }
  },
  "AllowedHosts": "*",
  "LettuceEncrypt": {
    "AcceptTermsOfService": true,
    "DomainNames": [ "example.com", "www.example.com" ],
    "EmailAddress": "it-admin@example.com"
  }
}
```
