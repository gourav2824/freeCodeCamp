---
title: Create a dummy file with a specific size
localeTitle: Создайте фиктивный файл с определенным размером
---
## Как создать фиктивные файлы с определенным размером с помощью команды «dd»:

Команда «dd» может использоваться для создания файла определенного размера. Это полезно, если вы хотите проверить скорость загрузки или любые другие тесты и нуждаться в файле определенного размера.
```
dd if=/dev/zero of=file_name.txt bs=1024k count=10 
```

Это создаст файл 1MB с именем file\_name.txt.

bs - ваш размер байта, а количество - количество блоков. Простой способ посмотреть - 1024K X 10.

Вот еще более простой способ создать 1 МБ-файл:
```
dd if=/dev/zero of=file_name.txt bs=1MB count=1 

```