---
layout: default
ref: music
lang: ru
css: 
  - znamenny
---

## Музыкальная нотация

### Знаменная (крюковая) нотация

Инициативная группа предоставляет шрифты для работы с символами знаменной
и путевой / демественной (казанской) нотаций в рамках стандарта Юникод.
**Внимание**: символы этих нотаций были недавно
[приняты для включения](http://www.unicode.org/alloc/Pipeline.html)
в будущую версию стандарта Юникод, но кодовые точки все еще могут измениться.

* [Документация к знаменным шрифтам](https://www.ponomar.net/files/fonts-znam.pdf) (по-английски)

* Документация системы признаков [формат ODT](https://www.ponomar.net/files/priznaki-documentation.odt) [формат PDF](https://www.ponomar.net/files/priznaki-documentation.pdf)

* [Предложение по кодированию нотации](https://www.ponomar.net/files/palaeoslavic.pdf) (по-английски)

* [Исходный код шрифтов на GitHub](https://github.com/slavonic/fonts-znam/)

#### Шрифты для набора знаменной нотации

* Mezenets Unicode разработан для набора символов призначной и беспризначной
знаменной нотации, а также символов демественной нотации.
[Скачать шрифт](https://www.ponomar.net/files/MezenetsUnicode.zip)

<div class="sample" contenteditable="true">
	<table align="center">
	<tr><td class="neume">𜽰𜽂𜼅</td>
	<td class="neume">𜽐𜼱𜼆</td>
	<td class="neume">&nbsp;&nbsp;</td>
	<td class="neume">𜽐𜽂𜼰𜼅</td>
	<td class="neume">𜽝𜽂𜼄</td>
	<td class="neume">𜽐𜽂𜼰𜼅</td>
	<td class="neume">𜽖𜽂𜼢</td>
	<td class="neume">𜽗𜽂𜼢</td>
	<td class="neume">𜽲𜼆</td>
	<td class="text">&nbsp;&nbsp;</td>
	<td class="neume">𜽯𜼅</td>
	<td class="neume">𜽟</td><td class="neume">𜾆𜽂𜼰𜼅</td>
	</tr>
	<tr><td class="text">Тво</td>
	<td class="text">ѧ</td>
	<td class="text">&nbsp;&nbsp;</td>
	<td class="text">по</td>
	<td class="text">бѣ</td>
	<td class="text">ди</td>
	<td class="text">тел</td>
	<td class="text">на</td>
	<td class="text">ѧ</td>
	<td class="text">&nbsp;&nbsp;</td>
	<td class="text">де</td>
	<td class="text">сни</td>
	<td class="text">ца</td></tr>
	</table>
</div>

* Smolensky Regular разработан для набора символов архаической знаменной нотации,
как она встречается в певческих рукописях XII-XV веков.
[Скачать шрифт](https://www.ponomar.net/files/Smolensky-Regular.zip)

<div class="sample" contenteditable="true">
	<table align="center">
	<tr><td class="neumeB">𜽒</td>
	<td class="neumeB">𜽐</td>
	<td class="neumeB">&nbsp;&nbsp;</td>
	<td class="neumeB">𜽖</td>
	<td class="textB">&nbsp;&nbsp;</td>
	<td class="neumeB">𜽖</td>
	<td class="neumeB">𜽐𜼱</td>
	<td class="neumeB">𜽖</td>
	<td class="neumeB">𜽖</td>
	<td class="neumeB">𜽖</td>
	<td class="text">&nbsp;&nbsp;</td>
	<td class="neumeB">𜽖</td>
	<td class="neumeB">𜽐</td>
	<td class="neumeB">𜽞</td>
	</tr>
	<tr><td class="textB">Ко</td>
	<td class="textB">нѧ</td>
	<td class="textB">&nbsp;&nbsp;</td>
	<td class="textB">и</td>
	<td class="textB">&nbsp;&nbsp;</td>
	<td class="textB">въ</td>
	<td class="textB">са</td>
	<td class="textB">дь</td>
	<td class="textB">ни</td>
	<td class="textB">ки·</td>
	<td class="textB">&nbsp;&nbsp;</td>
	<td class="textB">въ</td>
	<td class="textB">мо</td>
	<td class="textB">ре</td></tr>
	</table>
</div>

#### Ввод и редактирование нотации

* В системе верстки текста LaTeX, знаменную нотацию можно набирать,
используя пакет `churchslavonic` 
[См. подробнее&nbsp;»](/ru/users.html) 

* Для удобного набора, воспользуйтесь программой
[набора крюков в HTML](https://www.ponomar.net/znamenny/hookup2.html)

### Киевская квадратная (синодальная) нотация

Пятилинейная Киевская квадратная нотация используется в певческих
книгах Русской православной церкви, изданных, начиная с 1772 г.,
Святейшим Правительствующим Синодом. Аналогичная форма нотации
(с несколько отличным начертанием) используется в карпато-русских
певческих книгах.

* [Краткое руководство по квадратной нотации](http://seminaria.ru/raritet/solov_rukovod.htm)

* [Корпус квадратнонотных певческих книг](http://seminaria.ru/raritet/quadsborn.htm)

#### Компьютерный набор Киевской квадратной нотации

Символы Киевской квадратной нотации доступны в Юникоде (начиная с версии 8.0)
в разделе Musical Symbols (кодовая точка `U+1D1DE` и далее). Для набора
Киевской квадратной нотации, Вам потребуется шрифт, который поддерживает эти
символы. Мы советуем следующие шрифты:

* [Свободный шрифт Musica Г. Дуроса](http://users.teilar.gr/~g1951d/);
* [Свободный шрифт Bravura](http://www.smufl.org/fonts/), часть стандарта SMuFL; или
* Свободный шрифт Metasuprasl, разработанный Инициативной группой славянской информатики.

- **Шрифтовые файлы**:
	+	[Формат OpenType](https://www.ponomar.net/files/Metasuprasl-Regular.otf)
	+	[Формат TrueType](https://www.ponomar.net/files/Metasuprasl-SIL.ttf)

- **Исходный код**:
  + [Для программы FontForge](https://www.ponomar.net/files/Metasuprasl-Regular.sfd)
  + [Для Graphite](https://www.ponomar.net/files/Metasuprasl-Regular.gdl)

Шрифт Metasuprasl Regular можно использовать для набора квадратной ноты в текстовом редакторе. 
Версия шрифта в формате TrueType содержит возможности SIL Graphite. 
Вариант половинной ноты с длинным хвостом вверх доступен через фичу _salt_.
Версия шрифта в формате OpenType использует возможности OpenType; этот
же вариант доступен как стилистическая альтернатива (salt) 1.

#### Набор партитур в LilyPond

Для набора партитур в Киевской квадратной нотации мы советуем пользоваться программой
[LilyPond](http://www.lilypond.org/). Это -- свободная программа для набора
музыкальных партитур, причем она производит партитуры
очень высокого качества оформления и типографики.

* [Примеры партитур, набранных в LilyPond](http://www.lilypond.org/examples.html)

* К сожалению, у программы нет документации на русском языке. 
  Есть [введение](http://www.lilypond.org/text-input.html) 
  и [документация](http://www.lilypond.org/manuals.html) на английском, а также
  на [французском](http://lilypond.org/manuals.fr.html) и
  [немецком](http://lilypond.org/manuals.de.html).

* Глава, посвященная набору Квадратной нотации доступна
 [по-английски](http://www.lilypond.org/doc/v2.18/Documentation/notation/typesetting-kievan-square-notation),
  [по-немецки](http://www.lilypond.org/doc/v2.18/Documentation/notation/typesetting-kievan-square-notation.de.html)
  или [по-французски](http://www.lilypond.org/doc/v2.18/Documentation/notation/typesetting-kievan-square-notation.fr.html)

* Чтобы начать работать с квадратной нотацией, 
[скачайте самую свежую версию LilyPond](http://www.lilypond.org/download.html).

Несколько примеров партитур в квадратной нотации, набранных в LilyPond:

* Дал еси знамение (самоподобен, глас 4, знаменный роспев): 
  [Исходный код LilyPond](https://www.ponomar.net/files/dalesi.ly) |
  [PDF](https://www.ponomar.net/files/dalesi.pdf) |
  [MIDI](https://www.ponomar.net/files/dalesi.midi)
* Седален, глас 5, болгарский роспев: 
  [Исходный код LilyPond](https://www.ponomar.net/files/sessional5.ly) |
  [PDF](https://www.ponomar.net/files/sessional5.pdf) |
  [MIDI](https://www.ponomar.net/files/sessional5.midi)

Если Вы уже работаете в другой программе набора нотации, Вам
могут быть интересны преобразователи из форматов других программ в формат LilyPond:

* [Преобразователь из NoteWorthy Composer в LilyPond](http://nwc2ly.sourceforge.net/)
* [Преобразователь из MusicXML в LilyPond](http://www.nongnu.org/xml2ly/)
* [Преобразователь из Sibelius в LilyPond](http://sib2ly.sourceforge.net/)

#### Набор партитур в других программах

Набор квадратной нотации в других программах также возможен, но
Вам будет необходимо заменить шрифт, используемый для символов нотации.
В этих целях мы предоставляем шрифт Metasuprasl Notational. Вы можете
поменять метрику шрифта в исходном файле METAFONT на метрику
Вашей программы и затем скомпилировать шрифт формата Type1 используя
утилиту [mf2pt1](http://www.ctan.org/pkg/mf2pt1).

- **Исходный код**:
  + [На языке METAFONT](https://www.ponomar.net/files/metasuprasl.mf)

#### Кодировка

* A. Andreev, Y. Shardt, и N. Simmons.
[Предложение по кодированию символов Киевской квадратной нотации
в Юникоде (на английском)](https://www.ponomar.net/files/kievan.pdf) [Предложение принято]

* [Документация формата SMuFL](https://w3c.github.io/smufl/gitbook/)
Standard Music Font Layout) -- стандарта кодирования дополнительных 
музыкальных символов в Зоне личного пользования Юникода.

