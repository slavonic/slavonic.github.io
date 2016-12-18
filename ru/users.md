---
layout: default
ref: users
lang: ru
---

## Церковнославянская типографика : для пользователей

Эта страница описывает, как набирать церковнославянские тексты в разных популярных программах.

### XeTeX и LuaTeX

Для работы с церковнославянскими текстами в среде TeX, Вам потребуется программа верстки, поддерживающая Юникод, 
например XeTeX или LuaTeX. Обе распространяются в стандартном 
дистрибутиве [TeX Live](https://www.tug.org/texlive/).

Далее Вам следует сделать следующее:

* Установите шаблоны переноса слов для церковнославянского языка. Это можно сделать, запустив комманду: 
  ```
  tlmgr install hyphen-churchslavonic
  ```
  Затем следует перестроить форматы XeLaTeX и LuaLaTeX используя комманду: 
  ```
  fmtutil --byfmt xelatex
  fmtutil --byfmt lualatex
  ```
  
* Установите пакет `churchslavonic`. Этот пакет установит на Вашей системе набор церковнославянских ширфтов, 
  набор дополнительных макрокомманд и интерфейс для переключения языка в пакете `polyglossia`. 
  Пакет можно установить, запустив комманду 
  ```
  tlmgr install churchslavonic
  ```
  
* Если у Вас стоит старая версия TeX Live или другой дистрибутив TeX, Вам возможно придется установить шаблоны переноса и 
  пакеты вручную. Шаблоны переноса можно скачать [отсуда](https://github.com/slavonic/cu-tex/tree/master/hyphenation), 
  а пакет [с хранилища CTAN](https://www.ctan.org/tex-archive/language/churchslavonic).
  Следуйте инструкциям по установке, предоставленным в документации.

* Вы теперь готовы работать с церковнославянским текстом используя пакет `polyglossia`. Пакет `churchslavonic` включает
  ряд дополнительных макрокомманд для кириллической цифири, декоративных буквиц и других элементов набора. 
  Мы советуем посмотреть документацию [пакета Polyglossia](http://mirror.unl.edu/ctan/macros/latex/contrib/polyglossia/polyglossia.pdf)
  и [пакета `churchslavonic`](http://ctan.altspu.ru/language/churchslavonic/churchslavonic-ru.pdf).
  
* Если Вы не знаете, как начать, смотрите <A href="" Target="_blank">
  [примерный TeX файл](http://www.ponomar.net/files/sample.tex) и его [результат в PDF](http://www.ponomar.net/files/sample.pdf).

### Libre Office

Начина с версии 5.0, программа LibreOffice позволяет указать, что языком текста является церковнославянский 
(в программе он называется Church Slavic). Указав церковнославянский как язык документа, Вы можете нумеровать страницы 
кириллической цифирью, использовать автоматический перенос слов и сортировать в церковнославянском алфавитном порядке.

* Уставновите церковнославянские шрифты [отсюда](fonts.html)" Target="_blank"></A> и, если необходимо, клавиатурные драйверы для Вашей системы <a href="http://www.ponomar.net/cu_support/keyboardru.html" Target="_blank">отсюда</A>.</li>
			<li>Обновите LibreOffice до версии 5.0 или позже. Самую свежую версию можно скачать <a href="http://www.libreoffice.org/download/libreoffice-fresh/" Target="_blank">отсюда</A>. На платформе GNU / Linux, Вам возможно придется удалить установленную через менеджер пакетов программу LibreOffice 4, например коммандой <pre>sudo apt-get remove libreoffice-core</pre> Хотя церковнославянский текст можно редактировать и в LibreOffice 4 и раньше, Вы не сможете указать, что язык документа церковнославянский и не сможете использовать перенос слов и другие возможности.</li>
		<li>Установите словарь церковнославянских переносов. Для этого скачайте словарь <a href="http://extensions.libreoffice.org/extension-center/church-slavonic-dictionary" Target="_blank">отсюда</A>.  Далее откройте LibreOffice, в меню Tools выберите Extension Manager. В окне Extension Manager щелкните кнопку Add... и выберите файл cu-lo.oxt. Щелкните Accept чтобы принять лицензионное соглашение.
<br>
<img src="http://www.ponomar.net/images/extension_install.png" align="center" border="1" alt="install extension"></li>
	<li>Чтобы указать, что язык текста церковнославянский, выберите Options в меню Tools. В разделе Language Settings, выберите Languages. На панели Language Settings в разделе Default Languages for Documents выберите Church Slavic. Если Вы хотите нумеровать страницы кириллической цифирью, Вам также придется указать церковнославянский как локаль по умолчанию, что можно сделать выбрав Church Slavic в коробочке Locale Setting.<br>
<img src="http://www.ponomar.net/images/locale_libreoffice.png" align="center" border="1" alt="install extension"></li>
	<li>Чтобы включить автоматизированный перенос слов, выберите Paragraph в меню Format. Перейдите на панель Text Flow. В разделе Hyphenation щелкните Automatically.<br>
<img src="http://www.ponomar.net/images/hyphenation_writer.png" align="center" border="1" alt="install extension"></li>
	<li>Чтобы нумеровать страницы кириллической цифирью, выберите Page Number в меню Insert. Дважды щелкните появившийся номер страницы чтобы открыть окно Edit Fields. В разделе Format выберите Native Numbering и щелкните OK. (<B>Внимание</B>: для этого нужно сначала указать, что локаль программы по умолчанию -- церковнославянская.)<br>
<img src="http://www.ponomar.net/images/native_number.png" align="center" border="1" alt="install extension"></li>
	<li>В программе LibreOffice Calc, Вы можете сортировать ячейки в церковнославянском алфавитном порядке. Для этого выберите Sort в меню Data. Откройте панель Options. В коробочке Language выберите Church Slavic.<br>
<img src="http://www.ponomar.net/images/sort_calc.png" align="center" border="1" alt="install extension"></li>
	<li>Инициативная группа славянской информатики также представляет <A href="https://extensions.libreoffice.org/extensions/church-slavonic-converter" Target="_blank">надстройку Church Slavonic Converter</A>, которая позволяет конвертировать документы в Юникод из устаревших форматов UCS, HIP, и т.д. Надстройка устанавливается в Writer и конвертирует выделенный текст, или, если текст не выделен, конвертирует все содержимое документа. Исходный код надстройки доступен <A href="https://github.com/slavonic/cuconverter-LO" Target="_blank">здесь</A>.</li>
<li>Пока существуют некоторые баги: <A href="https://bugs.documentfoundation.org/show_bug.cgi?id=85731" Target="_blank">БАГ: Нельзя указать подчеркивание (_) как символ переноса</A>; <A href="https://bugs.documentfoundation.org/show_bug.cgi?id=96343" Target="_blank">БАГ: Нет конвертации из строчных букв в заглавные для символов в блоке Cyrillic Extended-B</A></li>
		</ul>

		<hr width="50%" style="color: black;">

		<h4 align="center">Apache OpenOffice</h4>
		<p>К сожалению программа <a href="http://www.openoffice.org/" target="_blank">Apache OpenOffice</A> очень слабо поддерживается. Вы сможете набирать церковнославянские тексты, но не сможете указать церковнославянский как язык документа, и поэтому не сможете использовать цифирь, перенос слов и другие возможности. Мы советуем Вам перейти на <a href="https://www.libreoffice.org/download/libreoffice-fresh/" target="_blank">LibreOffice</A>, который также является свободным программным обеспечением.</p>

		<hr width="50%" style="color: black;">

		<h4 align="center">Microsoft Office</h4>
		<p>Корпорация Microsoft не признает церковнославянский как язык, не смотря на то, что он включен в <a href="http://cldr.unicode.org/" target="_blank">Общее хранилище данных о локалях</a>, и поэтому Вы не сможете установить словари для переноса слов или проверки орфографии, даже разработанные другими разработчиками. В программе Microsoft Office нет поддержики церковнославянского языка. Мало того, старые версии Microsoft Windows (напр., XP, Vista, Windows 7) не поддерживают диакртические символы для кириллического текста. Каких-либо решений этой проблемы не существует, т.к. она прописана в системных файлах Windows. Ваши попытки работать с ЦСЯ в старых версиях Windows будут безрезультатными. Хотя <b>возможно</b>, что церковнославянский текст будет правильно отображаться в новых версиях Windows и Microsoft Office (используя шрифт Ponomar Unicode), мы не можем этого гарантировать.  <b>Инициативная группа не занимается поддержкой программного обеспечения, разработанного корпорацией Microsoft</b>. Мы рекомендуем Вам экономить свое время и деньги и использовать свободную программу <a href="https://www.libreoffice.org/download/libreoffice-fresh/" target="_blank">LibreOffice</A>.</p>

		<h4 align="center">Adobe InDesign</h4>
		<p>Если Вы установили церковнославянские шрифты <a href="http://www.ponomar.net/cu_support/fonts.html" Target="_blank">с этой страницы</A>, то Вы сможете верстать церковнославянский текст в программе Adobe InDesign. Для поддержки переноса слов, скачайте <a href="http://extensions.libreoffice.org/extension-center/church-slavonic-dictionary" Target="_blank">церковнославянские шаблоны переноса слов для LibreOffce</A>; затем следуйте инструкции <A href="https://helpx.adobe.com/indesign/kb/add_cs_dictionaries.html" Target="_blank">здесь</A> чтобы установить их в InDesign. Нумерация страниц кириллической цифирью не поддерживается. Попытайтесь связаться с <a href="https://helpx.adobe.com/contact.html?step=IDSN" target="_blank">Adobe</A> или перейдите на LibreOffice.</p>

		<h4 align="center">Мне нужна помощь!</h4>
		<p>Полезную информацию Вы можете почерпнуть из этих источников:</p>
		<ul>
		<li><A Href="http://www.unicode.org/notes/tn41/">Church Slavonic Typography in Unicode</A> [Unicode Technical Note #41. Только по-английски.]</li>
		<li><A Href="http://www.ponomar.net/files/pua_policy.pdf">Ponomar Project Private Use Area (PUA) Allocation Policy</A> (только по-английски) </li>
		</ul>
		<p>Список рассылки <a href="http://ponomar.net/mailman/listinfo/sci-users_ponomar.net" target="_blank">SCI-Users</A> (по-русски или по-английски). Просьба НЕ задавать вопросы, связанные с продукцией корпорации Microsoft -- мы не сможем Вам помочь!</p>
	</td>
	</tr>
	<tr>
		<td colspan="5" class="copyright">
		Ponomar Project is &copy; 2005-2016 Aleksandr Andreev and others.
		<br>
		All information on this website is provided with absolutely no warranty.
		<br>
		<center><a href="javascript:openWindow('http://www.ponomar.net/legal.html');">Legal information</a>
		| <a href="javascript:openWindow('http://www.ponomar.net/mailme.html');">Contact us</a></center>
		</td>
	</tr>
</table>
</body>
</html> 

