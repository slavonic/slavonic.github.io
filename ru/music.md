---
layout: default
ref: music
lang: ru
---

## Музыкальная нотация

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
	+	[Формат OpenType](http://www.ponomar.net/files/Metasuprasl-Regular.otf)
	+	[Формат TrueType](http://www.ponomar.net/files/Metasuprasl-SIL.ttf)

- **Исходный код**:
  + [Для программы FontForge](http://www.ponomar.net/files/Metasuprasl-Regular.sfd)
  + [Для Graphite](http://www.ponomar.net/files/Metasuprasl-Regular.gdl)

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
  [Исходный код LilyPond](http://www.ponomar.net/files/dalesi.ly) |
  [PDF](http://www.ponomar.net/files/dalesi.pdf) |
  [MIDI](http://www.ponomar.net/files/dalesi.midi)
* Седален, глас 5, болгарский роспев: 
  [Исходный код LilyPond](http://www.ponomar.net/files/sessional5.ly) |
  [PDF](http://www.ponomar.net/files/sessional5.pdf) |
  [MIDI](http://www.ponomar.net/files/sessional5.midi)

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
  + [На языке METAFONT](http://www.ponomar.net/files/metasuprasl.mf)

#### Кодировка

* A. Andreev, Y. Shardt, и N. Simmons.
[Предложение по кодированию символов Киевской квадратной нотации
в Юникоде (на английском)](http://www.ponomar.net/files/kievan.pdf) [Предложение принято]

* [Документация формата SMuFL](https://w3c.github.io/smufl/gitbook/)
Standard Music Font Layout) -- стандарта кодирования дополнительных 
музыкальных символов в Зоне личного пользования Юникода.

### Знаменная (крюковая) нотация

К сожалению, репертуар знаменной, демественной и других невменных славянских
нотаций пока еще не доступен в Юникоде и полноценных способов работы с этими
нотациями на компьютере пока нет. Мы активно занимаемся разработкой стандарта
для поддержки этих нотаций.

* A. Andreev и N. Simmons. [Предложение по кодированию древнерусских невменных 
музыкальных нотаций в Юникоде (на английском)](http://www.ponomar.net/files/palaeoslavic.pdf)

Вы можете по-экспериментировать с предложенным нами стандартом в песочнице.
Однако на данном этапе, все шрифты и тексты предоставляются без каких-бы то ни было
гарантийных обязательств.

* [Песочница для работы с знаменной нотацией](http://www.ponomar.net/wiki/doku.php?id=znamenny_manual)

* [Mezenets Unicode](https://github.com/typiconman/fonts-cu/tree/master/Mezenets)
 (шрифт для набора знаменной нотации)

