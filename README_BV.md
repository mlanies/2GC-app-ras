# Server Manager

Server Manager - это приложение с графическим интерфейсом для управления списком серверов через системный трей. Вы можете включать и выключать сервера, а также просматривать их статус.

## Установка

Для работы с приложением необходимо установить следующие зависимости:

- PyQt5
- (дополнительно) Cloudflared (для функции доступа к удаленным рабочим столам)

Установите зависимости с помощью следующей команды:

```bash
pip install -r requirements.txt
```
## Использование
Запустите приложение с помощью следующей команды:
bash
```bash
python beta_version.py
```
Приложение запуститься в трее.
По умолчанию в ней есть всего 2 кнопки: 
>Добавить приложение
> 
>Выключить

При добавлении приложение он попадает в список серверов.

Для каждого сервера доступны две кнопки - "Включить" и "Удалить из списка". Нажмите на "Включить", чтобы активировать сервер, Кнопка заменится на "Выключить". При нажатии на "Выключить", деактивируется сервер. Состояние сервера будет отображаться на кнопке.

Дополнительно, если у вас установлен Cloudflared, при включении сервера также будет доступен доступ к удаленным рабочим столам.

## Конвертация в .exe

Для того, что бы превратить пайтон фаил в полноценное приложение, введите в терминале :
```bash
pyinstaller --onefile --icon="/images/icon.ico" --noconsole beta_version.py
```

## Замечания
Убедитесь, что у вас установлены все необходимые зависимости, указанные в разделе "Установка".

Убедитесь, что на вашей системе установлен Cloudflared, если вы хотите использовать функцию доступа к удаленным рабочим столам.
## Автор

>SlaverPy
