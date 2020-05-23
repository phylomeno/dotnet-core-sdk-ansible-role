# Ansible Role for .NET Core SDK installation
Tested on:
- Raspbian Buster Lite

## Role Variables

| Variable                | Required | Default                   | Choices  | Comments                                 |
|-------------------------|----------|---------------------------|----------|------------------------------------------|
| archive_url             | no       | https://download.visualstudio.microsoft.com/download/pr/349f13f0-400e-476c-ba10-fe284b35b932/44a5863469051c5cf103129f1423ddb8/dotnet-sdk-3.1.102-linux-arm.tar.gz   |  | URL of the install archive to use  |
| archive_path            | no       | /opt/dotnet/sdk-install   |          | Path where install archive is stored to  |
| sdk_path                | no       | /opt/dotnet/sdk           |          | Path where SDK is installed to           |

## Example Playbook
```
- hosts: all
  roles:
    - dotnet-core-sdk
```

## License
MIT
