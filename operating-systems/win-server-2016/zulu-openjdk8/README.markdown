# Windows Server 2016

## Prerequisites

- Local machine with Windows installed
- Windows 10 version 1709+ or Build 16299+
  - In order to run a Windows container, the host build must be greater than
    or equal to the container's build.
  - See [Windows Container Version Compatibility](https://docs.microsoft.com/en-us/virtualization/windowscontainers/deploy-containers/version-compatibility) for more information

## Environment Details

|Product|Version|
|:-----:|:-----:|
|Java|Azul Zulu OpenJDK JDK 8|
|Operating System| Windows Server Core 2016|
|Portal| master snapshot|

## Startup

```bash
docker build -t <tag> .

docker run -p 8080:8080 -d <tag>:latest
```

This will start up a Liferay instance on Tomcat using HSQLDB.