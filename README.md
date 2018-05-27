# hw9
1. Использовал регулярное выражение \n\r для поиска пустых строк. Попробовал заменить с использованием его же, но, почему-то удалились только некоторые строки, а некоторые отступы всё же сохранились. Для удаления оставшихся пустых строк использовал регулярное выражение \n.

2. Для поиска имён собственных, заканчивающихся на "слав" использовал регулярное выражение "[А-Я]\w+слав\wзвёздочка". Первый символ должен быть заглавным, затем могут идти несколько букв, потом "слав" и, возможно, окончание. Регулярное выражение было проверено в regexr, и слова, не являющиеся именами собственными, оно не учитывает. Всего упоминаний найдено - 592.

3. Для поиска упоминаний Новгорода использовал регулярное выражение Нов\w?г\w?р\w?д\w*. Оно позволило учесть все предложенные варианты написания. Я также проверил его в regexr, и упоминаний новгородцев (или любых других форм этого слова и его производных, пишушихся с маленькой буквы) оно не находит. Всего упоминаний найдено - 59.

Для расстановки знаков препинания использовал регулярные выражения "\.", "\,", "\:", "\[". Затем заменял их на соответствующие, только с пробелами в нужных позициях. Для того, чтобы исправить пробелы в многоточиях, нашел все последовательности ". . ." и заменил их на "...".
