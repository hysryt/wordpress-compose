`docker-compose up`すると WordPressが8080、MailCatcherのWebサーバが1080で起動します。
複数起動する場合は適宜書き換えてください。

## Xdebug + VSCode
launch.json
```
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Listen for XDebug",
            "type": "php",
            "request": "launch",
            "port": 9000,
            "pathMappings": {
                "/var/www/html/wp-content/themes/twentyseventeen/": "${workspaceRoot}/"
            }
        }
    ]
}
```