# Мои настройки Visual Studio Code

## Расширения

### Запись списка расширений
Команда для записи установленных расширений в файл `extensions_list.txt`.

```shell
code --list-extensions > extensions_list.txt
```

### Установка расширений

#### Установка в PowerShell (Windows)
Для установки расширений из файла `extensions_list.txt` используйте следующую команду в PowerShell на Windows.

```powershell
Get-Content extensions_list.txt | ForEach-Object { code --install-extension $_ }
```

#### Установка в Bash (macOS и Linux)
Для установки расширений из файла `extensions_list.txt` используйте следующую команду в терминале Bash на macOS и Linux.

```bash
cat extensions_list.txt | xargs -L 1 code --install-extension
```
