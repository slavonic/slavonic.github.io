---
layout: default
ref: kievan
lang: ru
---

## Квадратная (синодальная) нотация

Этот раздел сайта посвящен работе с квадратной (синодальной) певческой нотацией (т.н. топорики). Эта нотация используется 
в певческих книгах, изданных Святейшим Синодом, а также в карпато-русских певческих сборниках.

* Никита Симмонс написал хорошее введение в чтение квадратной нотации ([здесь](http://www.synaxis.info/psalom/research/simmons/Kievan_notation.pdf))

* Корпус певческих книг, изданных в Русской Православной Церкви, с певческим материалом в квадратной нотации раньше был 
  доступен [здесь](http://seminaria.ru/raritet/quadsborn.htm)
  (сейчас видимо в работе сервера произошел сбой, мы надеемся выложить эти материалы у нас)

### Поддержка квадратной нотации в программе LilyPond

[LilyPond](http://www.lilypond.org/) &mdash; свободная программа для набора музыкальной нотации, причем качество партитур, 
набранных в LilyPond &ndash; очень высокое. Нотация набирается на текстовом языке разметки, что делает программу удобной 
для музыковедческой работы. Примеры партитур, набранных в  LilyPond см. [здесь](http://lilypond.org/examples.html).

* Скачать свежую версию программы можно [здесь](http://www.lilypond.org/download.html)
* К сожалению, у программы нет документации на русском языке. 
  На английском можно почитать [введение](http://www.lilypond.org/text-input.html) 
  и [документацию](http://lilypond.org/manuals.html).
* Конкретно о наборе квадратной ноты 
  [по-английски](http://lilypond.org/doc/v2.18/Documentation/notation/typesetting-kievan-square-notation),
  [по-немецки](http://lilypond.org/doc/v2.18/Documentation/notation/typesetting-kievan-square-notation.de.html)
  или [по-французски](http://lilypond.org/doc/v2.18/Documentation/notation/typesetting-kievan-square-notation.fr.html)

Примеры партитур в киевской нотации

* Дал еси знамение (самоподобен, глас 4, знаменный роспев): 
  [Исходный код LilyPond](http://www.ponomar.net/files/dalesi.ly) |
  [PDF](http://www.ponomar.net/files/dalesi.pdf) |
  [MIDI](http://www.ponomar.net/files/dalesi.midi)
* Седален, глас 5, болгарский роспев: 
  [Исходный код LilyPond](http://www.ponomar.net/files/sessional5.ly) |
  [PDF](http://www.ponomar.net/files/sessional5.pdf) |
  [MIDI](http://www.ponomar.net/files/sessional5.midi)


### Преобразователи

Утилита `zf2ly` преобразует материал с сайта [Знаменного фонда](http://www.znamen.ru/) в формат LilyPond. 
Крюки пока не поддерживаются, преобразуется только подтекстовка и ноты, либо в круглую, либо в квадратную нотацию. 
Используйте на свой страх и риск. Скачать: [отсюда](http://www.ponomar.net/cgi-bin/fetch_script.cgi?target=zf2ly)
(под Windows Вам потребуется [Strawberry Perl](http://strawberryperl.com/))
		
Примеры партитур с Знаменного фонда

* Богородичен от малых, Глас 1. 
  [MIDI](http://www.ponomar.net/files/lesser_theotokion1.midi)
  + Круглая нотация: 
    [Исходный код LilyPond](http://www.ponomar.net/files/lesser_theotokion1.ly) |
    [PDF](http://www.ponomar.net/files/lesser_theotokion1.pdf)
  + Квадратная нотация:
    [Исходный код LilyPond](http://www.ponomar.net/files/lesser_theotokion1_k.ly) |
    [PDF](http://www.ponomar.net/files/lesser_theotokion1_k.pdf)
* Богородичен от малых, Глас 2. 
  [MIDI](http://www.ponomar.net/files/lesser_theotokion2.midi)
  + Круглая нотация:
    [Исходный код LilyPond](http://www.ponomar.net/files/lesser_theotokion2.ly) |
    [PDF](http://www.ponomar.net/files/lesser_theotokion2.pdf)
  + Квадратная нотация:
    [Исходный код LilyPond](http://www.ponomar.net/files/lesser_theotokion2_k.ly) |
    [PDF](http://www.ponomar.net/files/lesser_theotokion2_k.pdf)


Освободитесь наконец от рабства закрытым программам по набору музыкальных партитур! 
Эти утилиты помогут Вам сконвертировать партитуры в LilyPond:

* Преобразователь из NoteWorthy Composer в LilyPond ([здесь](http://nwc2ly.sourceforge.net/)
* Преобразователь из формата MusicXML в LilyPond ([здесь](http://www.nongnu.org/xml2ly/)) 
  [этот преобразователь можно использовать для конвертирования из формата Finale]
* Преобразователь из Sibelius в LilyPond ([здесь](http://sib2ly.sourceforge.net/))

### Шрифты для киевской нотации

*  Если Вы набираете партитуры, мы советуем использовать программу [LilyPond](http://www.lilypond.org/)
* Если Вам нужны глифы киевских нот для набора текстов, мы рекомендуем шрифт Musica с сайта Георгия Дуроса: 
  [скачать](http://users.teilar.gr/~g1951d/);
* Или шрифт Bravura, [доступный с сайта SMuFL](http://www.smufl.org/fonts/)

Шрифт Metasuprasl изначально разработан авторами проекта для набора квадратной нотации. 
Глифы теперь включены в состав функциональных шрифтов Musica и Bravura. 
Однако шрифт может быть полезен для настройки программ набора нотации для работы с квадратной нотой

#### Metasuprasl Regular, Версия 1.3

* **Шрифтовые файлы**:
  + Формат OpenType ([здесь](http://www.ponomar.net/files/Metasuprasl-Regular.otf)
  + Формат TrueType, возможности OpenType и Graphite ([отсюда](http://www.ponomar.net/files/Metasuprasl-SIL.ttf))
* **Исходный код**:
  + [FontForge](http://www.ponomar.net/files/Metasuprasl-Regular.sfd)
  + [Файл Graphite Description Language (GDL)](http://www.ponomar.net/files/Metasuprasl-Regular.gdl)
  
Шрифт Metasuprasl Regular можно использовать для набора квадратной ноты в текстовом редакторе. 
Вариант половинной ноты с длинным хвостом вверх доступен через фичу _salt_

#### Metasuprasl Notational, Версия 1.1

* **Исходный код**:
  + [На языке METAFONT](http://www.ponomar.net/files/metasuprasl.mf)

Шрифт Metasuprasl Notational предназначен для загрузки в программы по набору нот. 
Измените метрику шрифта в файле METAFONT для вашей программы, скомпилируйте его в формат Type1 используя 
[`mf2pt1`](http://www.ctan.org/pkg/mf2pt1).

**Лицензия**: Metasuprasl распространяется согласно с условиями лицензии GNU GPL (v. 3 или выше) с 
обычным исключением для шрифтов или, по вашему усмотрению, согласно с условиями лицензии SIL Open Font License.

### Кодирование

* A. Andreev, Y. Shardt, and N. Simmons. [Proposal to Encode Medieval East-Slavic Music Notation in Unicode](http://www.ponomar.net/files/kievan.pdf) [Accepted]

* Документация стандарта SMuFL (Standard Music Font Layout), который описывает кодирование дополнительных 
  музыкальных символов в Зоне личного пользования ([здесь](https://w3c.github.io/smufl/gitbook/))

### Музыковедение

Разная информация для работы с музыкальными источниками

* [Standardization of Automela](http://www.ponomar.net/files/automela.pdf) [PONOMAR GREEN PAPER]
