Добавил этот текст в мой printer.cfg.
Это отличный способ добавить свои собственные элементы меню без редактирования menu.cfg и других системных файлов.

[menu __main]
type: list
name: Main Menu
items:
    __tune
    __user
    __octoprint
    __sdcard
    __control
    __temp
    __filament
    __prepare
    __test

[menu __user]
type: list
name: USER
items:
    .__userfilchange
    .__userfilpurge
    .__userfilresume

[menu __user __userfilchange]
type:command
name: Change Filament
gcode:
    M600

[menu __user __userfilpurge]
type:command
name: Purge Filament
gcode:
    PURGE

[menu __user __userfilresume]
type:command
name: RESUME
gcode:
    RESUME_MACRO


