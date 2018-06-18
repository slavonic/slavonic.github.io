---
layout: default
ref: users
lang: ru
---

## Церковнославянская типографика : для пользователей

Можно легко набирать, редактировать и оформлять церковнославянские тексты в разных популярных программах.

### XeTeX и LuaTeX

Для работы с церковнославянскими текстами в среде TeX, Вам потребуется программа верстки, поддерживающая Юникод, 
например XeTeX или LuaTeX. Обе распространяются в стандартном 
дистрибутиве [TeX Live](https://www.tug.org/texlive/).

Далее Вам следует сделать следующее:

* Установите шаблоны переноса слов для церковнославянского языка. Это можно сделать, запустив команду: 

  ```
  tlmgr install hyphen-churchslavonic
  ```

  Затем следует перестроить форматы XeLaTeX и LuaLaTeX используя команду: 
  
  ```
  fmtutil --byfmt xelatex
  fmtutil --byfmt lualatex
  ```
  
* Установите пакет `churchslavonic`. Этот пакет установит на Вашей системе набор церковнославянских шрифтов, 
  набор дополнительных макрокоманд и интерфейс для переключения языка в пакете `polyglossia`. 
  Пакет можно установить, запустив команду 
  
  ```
  tlmgr install churchslavonic
  ```
  
* Если у Вас стоит старая версия TeX Live или другой дистрибутив TeX, Вам возможно придется установить шаблоны переноса и 
  пакеты вручную. Шаблоны переноса можно скачать [с хранилища GitHub](https://github.com/slavonic/cu-tex/tree/master/hyphenation), 
  а пакет [с хранилища CTAN](https://www.ctan.org/tex-archive/language/churchslavonic).
  Следуйте инструкциям по установке, предоставленным в документации.

* Вы теперь готовы работать с церковнославянским текстом используя пакет `polyglossia`. Пакет `churchslavonic` включает
  ряд дополнительных макрокоманд для кириллической цифири, декоративных буквиц и других элементов набора. 
  Мы советуем посмотреть документацию [пакета Polyglossia](http://mirror.unl.edu/ctan/macros/latex/contrib/polyglossia/polyglossia.pdf)
  и [пакета `churchslavonic`](http://ctan.altspu.ru/language/churchslavonic/churchslavonic-ru.pdf).
  
* Если Вы не знаете, как начать, смотрите 
  [примерный TeX файл](https://www.ponomar.net/files/sample.tex) 
  и его [результат в PDF](https://www.ponomar.net/files/sample.pdf).

* Для проверки орфографии, установите программу Hunspell и пакет
  [церковнославянских словарей для Hunspell](https://github.com/slavonic/hunspell-cu/releases).
  Чтобы проверить орфографию документа TEX, написанного на ЦСЯ,
  запустите комманду `hunspell -d cu -t наименование-документа.tex`.

### LibreOffice

Начина с версии 5.0, программа LibreOffice позволяет указать, что языком текста является церковнославянский 
(в программе он называется `Church Slavic`). Указав церковнославянский как язык документа, Вы можете нумеровать страницы 
кириллической цифирью, использовать автоматический перенос слов и сортировать в церковнославянском алфавитном порядке.

* Установите церковнославянские шрифты [с нашего сайта](fonts.html) и, если необходимо,
 [клавиатурные драйверы для Вашей системы](https://www.ponomar.net/cu_support/keyboardru.html)

* Обновите LibreOffice до версии 5.0 или позже. Хотя церковнославянский текст можно редактировать и в LibreOffice 4 и раньше, Вы не сможете указать, что язык 
  документа церковнославянский и не сможете использовать перенос слов,
проверку орфографии и другие возможности.
  
* Установите словарь церковнославянских переносов и орфографии. Для этого [скачайте
  словарь](https://extensions.libreoffice.org/extensions/church-slavonic-dictionary). 
  Далее откройте LibreOffice, в меню `Tools` выберите `Extension Manager`. В окне `Extension Manager` щелкните 
  кнопку `Add...` и выберите файл `cu-lo.oxt`. Щелкните `Accept` чтобы принять лицензионное соглашение.
  
  ![install extension](https://www.ponomar.net/images/extension_install.png)

* Чтобы указать, что язык текста церковнославянский, выберите Options в меню `Tools`. В разделе `Language Settings`, 
  выберите `Languages`. На панели `Language Settings` в разделе `Default Languages for Documents` выберите `Church Slavic`.
  Если Вы хотите нумеровать страницы кириллической цифирью, Вам также придется указать церковнославянский как локаль 
  по умолчанию, что можно сделать, выбрав `Church Slavic` в коробочке `Locale Setting`.
  
  ![language](https://www.ponomar.net/images/locale_libreoffice.png)
  
* Чтобы включить автоматизированный перенос слов, выберите Paragraph в меню Format. Перейдите на панель `Text Flow`. 
  В разделе Hyphenation щелкните `Automatically`.
  
  ![hyphenation](https://www.ponomar.net/images/hyphenation_writer.png)
  
* Чтобы нумеровать страницы кириллической цифирью, выберите `Page Number` в меню `Insert`. Дважды щелкните появившийся 
  номер страницы чтобы открыть окно `Edit Fields`. В разделе `Format` выберите `Native Numbering` и щелкните OK.    
  (**Внимание**: для этого нужно сначала указать, что локаль программы по умолчанию -- церковнославянская.)
  
  ![page numbering](https://www.ponomar.net/images/native_number.png)

* В программе LibreOffice Calc, Вы можете сортировать ячейки в церковнославянском алфавитном порядке. 
  Для этого выберите `Sort` в меню `Data`. Откройте панель `Options`. В коробочке `Language` выберите `Church Slavic`.
  
  ![sorting](https://www.ponomar.net/images/sort_calc.png)

* Инициативная группа славянской информатики также предоставляет 
  [надстройку `Church Slavonic Converter`](https://extensions.libreoffice.org/extensions/church-slavonic-converter),
  которая позволяет импортировать в Юникод документы из устаревших форматов UCS, HIP, и т.д. 
  Надстройка устанавливается в `Writer` и конвертирует выделенный текст, или, если текст не выделен, конвертирует 
  все содержимое документа. Исходный код надстройки доступен [с хранилища GitHub](https://github.com/slavonic/cuconverter-LO).
  
* Пока существуют некоторые баги в LibreOffice: 
   - [85731](https://bugs.documentfoundation.org/show_bug.cgi?id=85731): Нельзя указать 
     подчеркивание (`_`) как символ переноса. Как решение этой проблемы, можно
    использовать OpenType фичу `ss01` (указав шрифт текста как `Ponomar Unicode:ss01`)
   или Graphite фичу `hyph` (указав шрифт текста как `Ponomar Unicode TT:hyph=1`).
   Дополнительную информацию о возможностях OpenType и Graphite смотрите в
  [документации для шрифтов](https://www.ponomar.net/files/fonts-churchslavonic.pdf).

   - [96343](https://bugs.documentfoundation.org/show_bug.cgi?id=96343): Нет конвертации из строчных букв в заглавные 
     для символов в блоке Cyrillic Extended-B

### Visual Studio Code

[Visual Studio Code](https://code.visualstudio.com/) — свободный, кроссплатформенный
редактор исходного кода. В нем удобно редактировать исходный код
церковнославянских богослужебных текстов, которые хранятся в форматах
[XML](https://github.com/slavonic/cu-books) и 
[Markdown](https://github.com/slavonic/cumd). 

  ![VS Code](https://www.ponomar.net/images/vscode.png)

Чтобы начать редактировать церковнославянский текст в Visual Studio Code:

* Установите расширение [Church Slavonic Markdown
Extensions](https://marketplace.visualstudio.com/items?itemName=pgmmpk.vscode-church-slavonic).

* Откройте панель предварительного просмотра Markdown
(надавите `Ctrl+Shift+P` чтобы открыть палитру и выбирите 
`Markdown: Open Preview to the Side`).

* Установите расширение [VS Code Church Slavonic
Keyboard](https://marketplace.visualstudio.com/items?itemName=pgmmpk.vscode-church-slavonic-keyboard).

* По умолчанию клавиатура отключена. Чтобы ее включить, надавите
`Ctrl+Alt+Space` (на системах GNU/Linux, `Meta+Space`) или
выбирите команду `Church Slavonic Keyboard: Toggle` из палитры.

* Помимо церковнославянских шрифтов [с нашего сайта](fonts.html),
Вам понадобится шрифт фиксированной ширины с поддержкой Unicode 10.0.
Похоже, на данный момент лучшим решением является шрифт
[GNU FreeFont](https://www.gnu.org/software/freefont/). Чтобы поменять шрифт редактора,
добавьте строку `"editor.fontFamily": "FreeMono"` в файл `User Settings`.

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
даже разработанные другими разработчиками. В программе Microsoft Office нет поддержки церковнославянского языка. 
Мало того, старые версии Microsoft Windows (напр., XP, Vista, Windows 7) не поддерживают диакритические символы 
для кириллического текста. Каких-либо решений этой проблемы не существует, т.к. она прописана в системных файлах Windows. 
Ваши попытки работать с ЦСЯ в старых версиях Windows будут безрезультатными. Хотя **возможно**, 
что церковнославянский текст будет правильно отображаться в новых версиях Windows и Microsoft Office 
(используя шрифт Ponomar Unicode), мы не можем этого гарантировать.  
**Инициативная группа не занимается поддержкой программного обеспечения, разработанного корпорацией Microsoft**. Мы рекомендуем Вам экономить свое время и деньги и использовать свободную программу [LibreOffice](https://www.libreoffice.org/download/libreoffice-fresh)


### Adobe InDesign

Если Вы установили церковнославянские шрифты [с нашего сайта](https://www.ponomar.net/cu_support/fonts.html),
то Вы сможете верстать церковнославянский текст в программе Adobe InDesign. Для поддержки переноса слов, 
скачайте [церковнославянские шаблоны переноса слов для LibreOffce](http://extensions.libreoffice.org/extensions/church-slavonic-dictionary); 
затем следуйте [инструкции](https://helpx.adobe.com/indesign/kb/add_cs_dictionaries.html)
чтобы установить их в InDesign. Нумерация страниц кириллической цифирью не поддерживается. 
Попытайтесь связаться с [Adobe](https://helpx.adobe.com/contact.html?step=IDSN) или перейдите на LibreOffice.

### Где находится нужный мне символ?

Таблицы церковнославянских букв и других символов представлены в документации:

* [Church Slavonic Typography in Unicode](http://www.unicode.org/notes/tn41/) 
  [Unicode Technical Note #41. Таблицы всех символов, включенных в Юникод.]

* [Политика использования Зоны личного пользования (PUA) Policy](https://www.ponomar.net/files/pua_policy.pdf)
  (Таблицы дополнительных символов, доступных в PUA)

### Мне нужна помощь!

Обратитесь в список рассылки [SCI-Users](https://ponomar.net/mailman/listinfo/sci-users_ponomar.net) (по-русски или по-английски).

Просьба НЕ задавать вопросы, связанные с продукцией корпорации Microsoft -- мы не сможем Вам помочь!
