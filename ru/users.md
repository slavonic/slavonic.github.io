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

  Затем следует перестроить форматы XeLaTeX и LuaLaTeX используя команду: 
  
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
  
* Если Вы не знаете, как начать, смотрите 
  [примерный TeX файл](http://www.ponomar.net/files/sample.tex) 
  и его [результат в PDF](http://www.ponomar.net/files/sample.pdf).

### Libre Office

Начина с версии 5.0, программа LibreOffice позволяет указать, что языком текста является церковнославянский 
(в программе он называется Church Slavic). Указав церковнославянский как язык документа, Вы можете нумеровать страницы 
кириллической цифирью, использовать автоматический перенос слов и сортировать в церковнославянском алфавитном порядке.

* Уставновите церковнославянские шрифты [отсюда](fonts.html)" Target="_blank"></A> и, если необходимо, клавиатурные 
  драйверы для Вашей системы [отсюда](http://www.ponomar.net/cu_support/keyboardru.html)

* Обновите LibreOffice до версии 5.0 или позже. Самую свежую версию можно скачать 
  [отсюда](http://www.libreoffice.org/download/libreoffice-fresh/). На платформе GNU / Linux, Вам возможно 
  придется удалить установленную через менеджер пакетов программу LibreOffice 4, например коммандой
  ```
  sudo apt-get remove libreoffice-core
  ```
  Хотя церковнославянский текст можно редактировать и в LibreOffice 4 и раньше, Вы не сможете указать, что язык 
  документа церковнославянский и не сможете использовать перенос слов и другие возможности.
  
* Установите словарь церковнославянских переносов. Для этого скачайте словарь 
  [отсюда](https://extensions.libreoffice.org/extensions/church-slavonic-dictionary). 
  Далее откройте LibreOffice, в меню `Tools` выберите `Extension Manager`. В окне `Extension Manager` щелкните 
  кнопку `Add...` и выберите файл `cu-lo.oxt`. Щелкните `Accept` чтобы принять лицензионное соглашение.
  ![install extension](http://www.ponomar.net/images/extension_install.png)

* Чтобы указать, что язык текста церковнославянский, выберите Options в меню `Tools`. В разделе `Language Settings`, 
  выберите `Languages`. На панели `Language Settings` в разделе `Default Languages for Documents` выберите `Church Slavic`.
  Если Вы хотите нумеровать страницы кириллической цифирью, Вам также придется указать церковнославянский как локаль 
  по умолчанию, что можно сделать выбрав `Church Slavic` в коробочке `Locale Setting`.
  ![language](http://www.ponomar.net/images/locale_libreoffice.png)
  
* Чтобы включить автоматизированный перенос слов, выберите Paragraph в меню Format. Перейдите на панель `Text Flow`. 
  В разделе Hyphenation щелкните `Automatically`.
  ![hyphenation](http://www.ponomar.net/images/hyphenation_writer.png)
  
* Чтобы нумеровать страницы кириллической цифирью, выберите `Page Number` в меню `Insert`. Дважды щелкните появившийся 
  номер страницы чтобы открыть окно `Edit Fields`. В разделе `Format` выберите `Native Numbering` и щелкните OK.    
  (**Внимание**: для этого нужно сначала указать, что локаль программы по умолчанию -- церковнославянская.)
  ![page numbering](http://www.ponomar.net/images/native_number.png)

* В программе LibreOffice Calc, Вы можете сортировать ячейки в церковнославянском алфавитном порядке. 
  Для этого выберите `Sort` в меню `Data`. Откройте панель `Options`. В коробочке `Language` выберите `Church Slavic`.
  ![sorting](http://www.ponomar.net/images/sort_calc.png)

* Инициативная группа славянской информатики также предоставляет 
  [надстройку `Church Slavonic Converter`](https://extensions.libreoffice.org/extensions/church-slavonic-converter),
  которая позволяет импортировать в Юникод документы из устаревших форматов UCS, HIP, и т.д. 
  Надстройка устанавливается в `Writer` и конвертирует выделенный текст, или, если текст не выделен, конвертирует 
  все содержимое документа. Исходный код надстройки доступен [здесь](https://github.com/slavonic/cuconverter-LO).
  
* Пока существуют некоторые баги: 
   - [85731](https://bugs.documentfoundation.org/show_bug.cgi?id=85731): Нельзя указать 
     подчеркивание (`_`) как символ переноса
   - [96343](https://bugs.documentfoundation.org/show_bug.cgi?id=96343): Нет конвертации из строчных букв в заглавные 
     для символов в блоке Cyrillic Extended-B

### Apache OpenOffice

К сожалению программа [Apache OpenOffice](http://www.openoffice.org) очень слабо поддерживается. 
Вы сможете набирать церковнославянские тексты, но не сможете указать церковнославянский как язык документа, 
и поэтому не сможете использовать цифирь, перенос слов и другие возможности. 
Мы советуем Вам перейти на [LibreOffice](https://www.libreoffice.org/download/libreoffice-fresh/), 
который также является свободным программным обеспечением.

### Microsoft Office

Корпорация Microsoft не признает церковнославянский как язык, не смотря на то, что он включен в 
[Общее хранилище данных о локалях](http://cldr.unicode.org), 
и поэтому Вы не сможете установить словари для переноса слов или проверки орфографии, 
даже разработанные другими разработчиками. В программе Microsoft Office нет поддержики церковнославянского языка. 
Мало того, старые версии Microsoft Windows (напр., XP, Vista, Windows 7) не поддерживают диакртические символы 
для кириллического текста. Каких-либо решений этой проблемы не существует, т.к. она прописана в системных файлах Windows. 
Ваши попытки работать с ЦСЯ в старых версиях Windows будут безрезультатными. Хотя **возможно**, 
что церковнославянский текст будет правильно отображаться в новых версиях Windows и Microsoft Office 
(используя шрифт Ponomar Unicode), мы не можем этого гарантировать.  
**Инициативная группа не занимается поддержкой программного обеспечения, разработанного корпорацией Microsoft**. Мы рекомендуем Вам экономить свое время и деньги и использовать свободную программу [LibreOffice](https://www.libreoffice.org/download/libreoffice-fresh)


### Adobe InDesign

Если Вы установили церковнославянские шрифты [с этой страницы](http://www.ponomar.net/cu_support/fonts.html),
то Вы сможете верстать церковнославянский текст в программе Adobe InDesign. Для поддержки переноса слов, 
скачайте [церковнославянские шаблоны переноса слов для LibreOffce](http://extensions.libreoffice.org/extension-center/church-slavonic-dictionary); 
затем следуйте инструкции [здесь](https://helpx.adobe.com/indesign/kb/add_cs_dictionaries.html)
чтобы установить их в InDesign. Нумерация страниц кириллической цифирью не поддерживается. 
Попытайтесь связаться с [Adobe](https://helpx.adobe.com/contact.html?step=IDSN) или перейдите на LibreOffice.

### Мне нужна помощь!

Полезную информацию Вы можете почерпнуть из этих источников:

* [Church Slavonic Typography in Unicode](http://www.unicode.org/notes/tn41/) 
  [Unicode Technical Note #41. Только по-английски.]

* [Ponomar Project Private Use Area (PUA) Allocation Policy](http://www.ponomar.net/files/pua_policy.pdf)
  (только по-английски)

### Список рассылки
Список рассылки [SCI-Users](http://ponomar.net/mailman/listinfo/sci-users_ponomar.net) (по-русски или поанглийски). 
Просьба НЕ задавать вопросы, связанные с продукцией корпорации Microsoft -- мы не сможем Вам помочь!
