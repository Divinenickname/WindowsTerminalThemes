# WindowsTerminalThemes
Темы для терминала Windows. Те, которые мне понравились и которыми пользуюсь.

Темы вносятся в файл ```profiles.json``` в который можно попасть через настройки терминала. Если файла нет - он создастся автоматически.


## Как добавить тему?
### Шаг 1 - добавить цветовую схему
Скопируйте понравившуюся тему и добавьте её атрибуты в "schemes"

Например:
```
"schemes": [
    {
        "background" : "#300A24",
        "black" : "#4E9A06",
        "blue" : "#3465A4",
        "brightBlack" : "#555753",
        "brightBlue" : "#729FCF",
        "brightCyan" : "#34E2E2",
        "brightGreen" : "#8AE234",
        "brightPurple" : "#AD7FA8",
        "brightRed" : "#979A9A",
        "brightWhite" : "#EEEEEE",
        "brightYellow" : "#ECF0F1",
        "cyan" : "#06989A",
        "foreground" : "#90FC36",
        "green" : "#300A24",
        "name" : "UbuntuLegit",
        "purple" : "#75507B",
        "red" : "#CC0000",
        "white" : "#D3D7CF",
        "yellow" : "#C4A000"
    }
```

### Шаг 2 - добавить тему в список для отображения
Во всех своих темах я добавляю пример в котором достаточно ввести лишь свой GUID. Для его получения откройте терминал и введите ```new-guid```. Скопируйте значение в соответсвующее поле

Например:

```
"list":
        [
            {
                "guid": "{ВАШ GUID}",
                "name": "Windows PowerShell",
                "commandline": "powershell.exe",
                "hidden": false
            },
```            

## Как сделать тему по-умолчанию
Достаточно перед ```"profiles"``` создать ``` "defaultProfile": "{GUID}",``` и тогда тема с данным ID будет запускаться сразу
