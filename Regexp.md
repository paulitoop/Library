1. **Базовые символы**:
   - `.` — любой символ, кроме новой строки.
   - `^` — начало строки.
   - `$` — конец строки.

2. **Квантификаторы**:
   - `*` — ноль или более вхождений.
   - `+` — одно или более вхождений.
   - `?` — ноль или одно вхождение.
   - `{n}` — ровно n вхождений.
   - `{n,}` — n или более.
   - `{n,m}` — от n до m вхождений.

3. **Группировка**:
   - `(...)` — группировка символов.
   - `(?:...)` — группировка без запоминания.

4. **Выбор**:
   - `|` — логическое "или". Например, `a|b` соответствует "a" или "b".

5. **Специальные символы**:
   - `\d` — любая цифра (эквивалентно `[0-9]`).
   - `\D` — любой нецифровой символ.
   - `\w` — любой алфавитно-цифровой символ (буквы, цифры и `_`, эквивалентно `[a-zA-Z0-9_]`).
   - `\W` — любой неалфавитно-цифровой символ.
   - `\s` — пробельный символ (пробел, табуляция и т.д.).
   - `\S` — непроходной символ.

6. **Экранирование**:
   - Если нужно искать специальные символы (например, `.`, `*`, `?`), используем обратный слеш `\` для их экранирования.

7. **Работа с классами символов**:
   - `[abc]` — любой из символов a, b или c.
   - `[a-z]` — любой символ из диапазона a до z.
   - `[^abc]` — любой символ, кроме a, b или c.

8. **Жадные и нежадные квантификаторы**:
   - По умолчанию квантификаторы жадные (например, `.*` захватит максимально возможное количество). Чтобы сделать их нежадными, добавляем `?` (например, `.*?` захватит минимально возможное количество).
