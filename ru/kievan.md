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


		<h5>Примеры партитур в киевской нотации</h5>
		<ul>
		<li>
		Дал еси знамение (самоподобен, глас 4, знаменный роспев): <a href="http://www.ponomar.net/files/dalesi.ly">исходный файл LilyPond</a> |
		<a href="http://www.ponomar.net/files/dalesi.pdf">PDF</a> | <a href="http://www.ponomar.net/files/dalesi.midi">MIDI</a></li>
		<li>Седален, глас 5, болгарский роспев: <a href="http://www.ponomar.net/files/sessional5.ly">исходный файл LilyPond</a> |
		<a href="http://www.ponomar.net/files/sessional5.pdf">PDF</a> | <a href="http://www.ponomar.net/files/sessional5.midi">MIDI</a>
		</li>
		</ul>

		<h4><a name="conv">Преобразователи</a></h4>
		<p>Утилита zf2ly преобразует материал с сайта <a href="http://www.znamen.ru/" Target="_new">Знаменного фонда</a> в формат LilyPond. Крюки пока не поддерживаются, преобразуется только подтекстовка и ноты, либо в круглую, либо в квадратную нотацию. Используйте на свой страх и риск. Скачать: <A Href="http://www.ponomar.net/cgi-bin/fetch_script.cgi?target=zf2ly">отсюда</A> (под Windows Вам потребуется <a href="http://strawberryperl.com/" target="_blank">Strawberry Perl</a>)
		</p>
		
		<h5>Примеры партитур с Знаменного фонда</h5>
		<p>
		Богородичен от малых, Глас 1. Круглая нотация: (<a href="http://www.ponomar.net/files/lesser_theotokion1.pdf">PDF</a> | <a href="http://www.ponomar.net/files/lesser_theotokion1.ly">Исходный код LilyPond</a>) | Квадратная нотация (<a href="http://www.ponomar.net/files/lesser_theotokion1_k.pdf">PDF</a> | <a href="http://www.ponomar.net/files/lesser_theotokion1_k.ly">Исходный код LilyPond</a>) | (<a href="http://www.ponomar.net/files/lesser_theotokion1.midi">MIDI</a>)<br>
		Богородичен от малых, Глас 2. Круглая нотация:  (<a href="http://www.ponomar.net/files/lesser_theotokion2.pdf">PDF</a> | <a href="http://www.ponomar.net/files/lesser_theotokion2.ly">Исходный код LilyPond</a>) | Квадратная нотация (<a href="http://www.-ponomar.net/files/lesser_theotokion2_k.pdf">PDF</a> | <a href="http://www.ponomar.net/files/lesser_theotokion2_k.ly">Исходный код LilyPond</a>) | (<a href="http://www.ponomar.net/files/lesser_theotokion2.mido">MIDI</a>)<br>
		</p>

		<p>Освободитесь наконец от рабства закрытым программам по набору музыкальных партитур! Эти утилиты помогут Вам сконвертировать партитуры в LilyPond:
		<ul>
			<li>Преобразователь из NoteWorthy Composer в LilyPond (<a href="http://nwc2ly.sourceforge.net/" target="_blank">здесь</a>)</li>
			<li>Преобразователь из формата MusicXML в LilyPond (<a href="http://www.nongnu.org/xml2ly/" target="_blank">здесь</a>) [этот преобразователь можно использовать для конвертирования из формата Finale]</li>
			<li>Преобразователь из Sibelius в LilyPond (<a href="http://sib2ly.sourceforge.net/" target="_blank">здесь</a>)</li>
		</ul>
		</p>
		
		<h4>Шрифты для киевской нотации</h4>
		<ul>
			<li>Если Вы набираете партитуры, мы советуем использовать программу <a href="http://www.lilypond.org/" target="_blank">LilyPond</a></li>
			<li>Если Вам нужны глифы киевских нот для набора текстов, мы рекомендуем шрифт Musica с сайта Георгия Дуроса: <a href="http://users.teilar.gr/~g1951d/" target="_blank">скачать</a>;</li>
			<li>Или шрифт Bravura, <a href="http://www.smufl.org/fonts/" target="_blank">доступный с сайта SMuFL</a></li>
		</ul>
		<p>Шрифт Metasuprasl изначально разработан авторами проекта для набора квадратной нотации. Глифы теперь включены в состав функциональных шрифтов Musica и Bravura. Однако шрифт может быть полезен для настройки программ набора нотации для работы с квадратной нотой</p>
		
		<table cellpadding=0 cellspacing=0 border=0 align="center">
		<tr>
			<td><b>Наименование</b></td>
			<td><b>Скачать</b><td>
		</tr>
		<tr>
			<td valign="top">Metasuprasl Regular</td>
			<td valign="top">
			Версия 1.3<br>
			<b>Шрифтовые файлы</b>:<br>
			Формат OpenType (<A Href="http://www.ponomar.net/files/Metasuprasl-Regular.otf">здесь</a>)<br>
			Формат TrueType, фичи OpenType и Graphite (<A Href="http://www.ponomar.net/files/Metasuprasl-SIL.ttf">отсюда</a>)<br>
			<br>
			<b>Исходный код</b>:<br>
			<A HREF="http://www.ponomar.net/files/Metasuprasl-Regular.sfd">FontForge</A><br>
			<A Href="http://www.ponomar.net/files/Metasuprasl-Regular.gdl">Файл Graphite Description Language (GDL)</A><BR>
			<br>
			</td>
		</tr>
		<tr>
			<td colspan="2">Шрифт Metasuprasl Regular можно использовать для набора квадратной ноты в текстовом редакторе. Вариант половинной ноты с длинным хвостом вверх доступен через фичу <I>salt</I></td>
		</tr>
		
		<tr>
			<td valign="top">Metasuprasl Notational</td>
			<td valign="top">
			Версия 1.1<br>
			<b>Исходный код</b>:<br>
			<A Href="http://www.ponomar.net/files/metasuprasl.mf">На языке METAFONT</A>
			<br>
			</td>
		</tr>
		<tr>
			<td colspan="2">Шрифт Metasuprasl Notational предназначен для загрузки в программы по набору нот. Измените метрику шрифта в файле METAFONT для вашей программы, скомпилируйте его в формат Type1 используя <A Href="http://www.ctan.org/pkg/mf2pt1" Target="_blank">mf2pt1</A>. <B>Лицензия</B>: Metasuprasl распространяется согласно с условиями лицензии GNU GPL (v. 3 или выше) с обычным исключением для шрифтов или, по вашему усмотрению, согласно с условиями лицензии SIL Open Font License.</td>
		</tr>
		</table>
		</p>
		
		<h4>Кодирование</h4>
		<p>
		<ul>
			<LI>A. Andreev, Y. Shardt, and N. Simmons. <A Href="http://www.ponomar.net/files/kievan.pdf">Proposal to Encode Medieval East-Slavic Music Notation in Unicode</A> [Accepted]</LI>
			<LI>Документация стандарта SMuFL (Standard Music Font Layout), который описывает кодирование дополнительных музыкальных символов в Зоне личного пользования (<A Href="http://www.smufl.org/download/" target="_blank">здесь</a>)</LI>
		</ul>
		</p>
		
		<h4>Музыковедение</h4>
		<p>
		Разная информация для работы с музыкальными источниками
		<ul>
			<li><A href="http://www.ponomar.net/files/automela.pdf">Standardization of Automela</A> [PONOMAR GREEN PAPER]</li>
		</ul>
		</p>

	</tr>
	<tr>
		<td colspan="5" class="copyright">
		Материалы проекта Пономарь &copy; 2005-2015 Александр Андреев  и другие
		<br>
		Вся информация на этом сайте предоставлена без каких бы то ни было гарантийных обязательств.
		<br>
		<center><a href="javascript:openWindow('http://www.ponomar.net/legal.html');">Юридическая справка</a>
		| <a href="javascript:openWindow('http://www.ponomar.net/mailme.html');">Обратная связь</a></center>
		</td>
	</tr>
</table>
</body>
</html> 

