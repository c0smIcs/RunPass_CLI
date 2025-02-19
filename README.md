# Password Generator CLI

**Password Generator CLI** - это простое CLI-приложение для генерации случайных паролей с настраиваемыми параметрами. Приложение создано с использованием библиотеки [Cobra](https://github.com/spf13/cobra)

---

## 📋 Описание

Приложение позволяет генерировать случайные пароли со следующими параметрами:
- **Длина пароля**
- **Включение букв** (строчные и заглавные)
- **Включение цифр**
- **Включение специальных символов**

Также есть возможность сохранять пароль в файл.

---

## 💡 Использование

### Генерация пароля

Чтобы сгенерировать пароль, используйте команду `generate` с необходимыми флагами.

Например:
```bash
./RunPass generate --length 16 --letters --numbers
```
Это создаст пароль длиной 16 символов, состоящий из букв и цифр.


### Сохранение пароля в файл

Вы можете сохранить сгенерированный пароль в файл, используя флаг `--output`:

```bash 
./RunPass generate --length 12 --letters --numbers --output password.txt
```
Пароль будет записан в файл `password.txt`

### Получение справки

Чтобы получить подробную информацию о командах и флагах, используйте флаг `--help`:
```bash
./RunPass generate --help
```

## 🛠️ Флаги

| ФЛАГ | ОПИСАНИЕ | ЗНАЧЕНИЕ ПО УМОЛЧАНИЮ |
-------------------
| -l, --length  | Указывает длину пароля | 12 |
| -a, --letters | Включает буквы (строчные и заглавные) в пароль | false
| -n, --numbers | Включает цифры в пароль | false |
| -s, --symbols | Включает специальные символы (например,!@#$%^*) в пароль. | false |
| -o, --output  | Сохраняет сгенерированный пароль в указанный файл. Если флаг не указан, пароль выводится в консоль | нет |

---

🌟 Примеры использования

1. Генерация пароля длинной 16 символов с буквами и цифрами:
\```
./RunPass generate --length 16 --letters --numbers
\```

2. Генерация пароля длиной 20 символов с буквами, цифрами и специальными символами :
\```
./RunPass generate --length 20 --letters --numbers --symbols
\```

3. Сохранение пароля в файл:
\```
./RunPass generate --length 12 --letters --numbers --output password.txt
\```

4. Получение справки:
\```
./RunPass generate --help
\```
