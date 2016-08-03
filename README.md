# VS Code Redis
### Extension for Visual Studio Code 
[![Build Status](https://travis-ci.org/vitorsalgado/vscode-redis.svg?branch=master)](https://travis-ci.org/vitorsalgado/vscode-redis)

This extension allows execution of Redis commands directly from Command Palette

## Install
* Press `Ctrl + Shift + P`
* Pick  `Extensions: Install Extension`
* Search for **vscode-redis**

## Features

* Multiple Redis connections;
* Switch between server connections;
* Execute any Redis command with `Redis: Execute Command`
* "Command Palette" supported Redis commands:
    * `info`
    * `get`
    * `set`
    * `hget`
    * `hset`
    * `del`
    * `hdel`
    * `hgetall`

## Optional Extension Settings

You can configure multiple Redis connections on your workspace. 
First, place a file named "redis.json" in .vscode folder. Open "redis.json" and edit it following the sample below:
```
{
    "databases": [
        {
            "name": "local",
            "url": "http://localhost:6379"
        },
        {
            "name": "production",
            "addr": "http://production-address:9091"
        }
    ]
}
```

Execute the command `Redis: Reload Configuration` to load the servers listed in configuration file.

## Usage
![how use](https://github.com/vitorsalgado/vscode-redis/raw/master/how-to.gif)

## Release Notes

### 1.0.0
Initial release of **vscode-redis**

### 1.0.1
Fixed default server configuration url

## License
MIT © [vitorsalgado](https://github.com/vitorsalgado)
