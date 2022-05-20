Получение списка файлов и папок, содержащихся в папке

Get-ChildItem -Path C:\ -Force

Копирование файлов и папок

Copy-Item -Path C:\boot.ini -Destination C:\boot.bak

Создание файлов и папок

New-Item -Path 'C:\temp\New Folder' -ItemType Directory

New-Item -Path 'C:\temp\New Folder\file.txt' -ItemType File

Удаление всех файлов и папок, содержащихся в папке

Remove-Item -Path C:\temp\DeleteMe -Recurse

Подключение локальной папки как диска

New-PSDrive -Name P -Root $env:ProgramFiles -PSProvider FileSystem

