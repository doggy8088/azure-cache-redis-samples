---
page_type: sample
languages:
- java
name: 'Quickstart: Use Azure Cache for Redis in Java'
description: Learn how to incorporate Azure Cache for Redis into a Java app using the Jedis Redis client.
products:
- azure
- azure-cache-redis
---
# Quickstart: Use Azure Cache for Redis in Java

This sample show you how to incorporate Azure Cache for Redis into a Java app using the [Jedis](https://github.com/xetorthio/jedis) Redis client. See the [accompanying article](https://docs.microsoft.com/azure/azure-cache-for-redis/cache-java-get-started) on the documentation site for details, including best practices and how to create the sample code from scratch.

## Prerequisites

- Azure subscription - [create one for free](https://azure.microsoft.com/free/)
- Azure Cache for Redis cache - [create one](https://docs.microsoft.com/azure/azure-cache-for-redis/quickstart-create-redis)
- [Apache Maven](https://maven.apache.org/download.cgi)

## Set up the working environment

Depending on your operating system, add environment variables for your cache's **Host name** and **Primary access key**. Open a command prompt, or a terminal window, and set up the following values:

```CMD
set REDISCACHEHOSTNAME=localhost
set REDISCACHEKEY=<YOUR_PRIMARY_ACCESS_KEY>
```

```bash
export REDISCACHEHOSTNAME=localhost
export REDISCACHEKEY=<YOUR_PRIMARY_ACCESS_KEY>
```

```powershell
$env:REDISCACHEHOSTNAME = 'localhost'
$env:REDISCACHEKEY = '<YOUR_PRIMARY_ACCESS_KEY>'
```

Replace the placeholders with the following values:

- `<YOUR_HOST_NAME>`: The DNS host name, obtained from the *Properties* section of your Azure Cache for Redis resource in the Azure portal.
- `<YOUR_PRIMARY_ACCESS_KEY>`: The primary access key, obtained from the *Access keys* section of your Azure Cache for Redis resource in the Azure portal.

## Run the sample

[Download the sample code to your development PC.](/README.md#get-the-samples)

Change directories to the folder containing this sample.

Execute the following Maven command to build and run the app:

```CMD
mvn compile
mvn exec:java -D exec.mainClass=example.demo.App
```

## References

* [Quickstart article on the documentation site](https://docs.microsoft.com/azure/azure-cache-for-redis/cache-java-get-started)
