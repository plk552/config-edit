# EDIT CONFIG
<img src = "aple.png" width = '100' hight = '100'  >

## Описание
данный код код создан для просмотра , а так же изменения параметров конфигурации файла config.json 

## Как запустить
1. загрузить файлы из репозиторий , затем закинуть из в папку созданную на рабочем столе 
2. открыть командную строку 
3. перейти в папку с фаайлами с помощью команды 

    ```cmd 
    cd  "C:\Users\ имя пользователя \Desktop\ наиминование папки "
    ```
4. ввести одну из команд команду 

    ```cmd 
    python main.py read json.cfg  
    ```
    ```cmd 
    python  main.py write --param server.port=100 
    ```
## Содержание
* aple.png 
* config.json
* main.py 
* README.md 

### Функции в файле main.py
* read_config
* write_config
* update_config
* main
## Примеры использования
   
```cmd 
python main.py read json.cfg
```
вывод:
 ```cmd
Содержимое конфига:
{
    "server": {
        "host": "1.1.11.1",
        "port": "100",
        "debug": "false"
    },
    "database": {
        "type": "postgresql",
        "host": "localhost",
        "port": 5432,
        "username": "db_user",
        "password": "db_password",
        "database_name": "my_database"
    },
    "logging": {
        "level": "INFO",
        "file": "/var/log/myapp.log"
    },
    "api": {
        "key": "my_api_key",
        "endpoint": "https://api.example.com/v1/"
    },
    "email": {
        "smtp_server": "smtp.example.com",
        "smtp_port": 587,
        "username": "email_user",
        "password": "email_password",
        "from_email": "no-reply@example.com",
        "to_email": "admin@example.com"
    },
    "features": {
        "enable_feature_x": true,
        "enable_feature_y": false
    }
}
 ```
## используемые модули
* argparse
* json
* indent from textwarp
## Автор
# https://github.com/plk552