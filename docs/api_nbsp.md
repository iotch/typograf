# Неразрывные пробелы
По умолчанию типограф не заменяет неразрывные пробелы на обычные, чтобы не удалить ранее проставленные неразрывные пробелы. Если в тексте неправильно расставлены неразрывные пробелы, включите правило `common/nbsp/replaceNbsp`.
```js
var tp = new Typograf({locale: ['ru', 'en-US']});
tp.enableRule('common/nbsp/replaceNbsp');
```

Перед типографированием в live-режиме неразрывные пробелы заменяются на обычные, т. к. один и тот же текст типографируется многократно при каждом вводе символа.
