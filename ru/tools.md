---
layout: default
ref: tools
lang: ru
---

## Для разработчиков и программистов

### Преобразователи

Преобразователи из различных исторических кодовых таблиы в Юникод:

* Преобразователь [HIP](http://orthlib.ru/hip/) -> Юникод
  [веб интерфейс](http://www.ponomar.net/cgi-bin/hip2utf.cgi) | 
 [или как самостоятельная программа в пакете Lingua::CU::Scripts]
(https://github.com/typiconman/Perl-Lingua-CU) module

* Преобразователь [Ирмологий](http://irmologion.ru/ucsenc.html#atop) -> Юникод
  [веб интерфейс](http://www.ponomar.net/cgi-bin/ucs2utf.cgi) |
 [или как самостоятельная программа в пакете Lingua::CU::Scripts]

* Расширение преобразователей для LibreOffice 3 и старше
  (для конвертирования документов RTF, DOC, DOCX и ODT) 
  [Скачать и установить]
(https://extensions.libreoffice.org/extensions/church-slavonic-converter)

### Интерфейсы программирования приложений

Церковнославянские ИПП позволяют внедрять поддержику церковнославянского
языка в авоторские программы и предоставляют ряд возомжностей, например,
сортировку, сравнение строковых переменных, конвертацию между славянской
орфографией и современной, генерирование кириллических цифр.

* [Lingua::CU](https://github.com/typiconman/Perl-Lingua-CU) - для
  поддержки церковнославянских текстов на языке Перл.
  
* [cslavonic](https://github.com/pgmmpk/cslavonic) - для
   поддержки церковнославянских текстов на языке Питон.

### Перенос слов

Словари слогоделения для автоматизированного переноса слов

* [Для LibreOffice 5.0 и новее](https://extensions.libreoffice.org/extensions/church-slavonic-dictionary)
* [Для XeTeX, LuaTeX, и других систем, основанных на TeX](https://github.com/slavonic/cu-tex/tree/master/hyphenation)

Информация о слогоделении

* А. А. Андреев, М. П. Крутиков
[Автоматизация слогоделения и переноса слов в церковнославянских текстах](https://www.academia.edu/27011149/%D0%90%D0%B2%D1%82%D0%BE%D0%BC%D0%B0%D1%82%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F_%D1%81%D0%BB%D0%BE%D0%B3%D0%BE%D0%B4%D0%B5%D0%BB%D0%B5%D0%BD%D0%B8%D1%8F_%D0%B8_%D0%BF%D0%B5%D1%80%D0%B5%D0%BD%D0%BE%D1%81%D0%B0_%D1%81%D0%BB%D0%BE%D0%B2_%D0%B2_%D1%86%D0%B5%D1%80%D0%BA%D0%BE%D0%B2%D0%BD%D0%BE%D1%81%D0%BB%D0%B0%D0%B2%D1%8F%D0%BD%D1%81%D0%BA%D0%B8%D1%85_%D1%82%D0%B5%D0%BA%D1%81%D1%82%D0%B0%D1%85)

### Внедрение шрифтов в веб-страницы

Если вы хотите отображать церковнославянский текст на вашем веб-сайте или
блоге, то вы можете внедрить шрифты непосредственно с нашего сайта, просто
указав ссылку на наш стиль в разделе `HEAD` вашей веб-страницы:

```
<link rel="stylesheet" href="https://slavonic.github.io/css/fonts.css" type="text/css">
```

Эта команда автоматически загрузит все необходимые шрифты. Текст можно
отобразить церковнославянским шрифтом, объявив его в стиле CSS, например:

```
.slavonic {
  font-family: 'Ponomar Unicode';
}
```

Если вы не хотите загружать шрифты с нашего сервера, но хотите расположить
их непосредственно на вашем сервере, то вы можете скачать 
[архив с веб шрифтами](http://www.ponomar.net/files/sci-webfonts.zip)
и раскрыть его в какой-либо директории на вашем сервере.

Этот архив содержит шрифты в форматах [WOFF2](https://www.w3.org/TR/WOFF2/),
[WOFF](https://www.w3.org/Fonts/WOFF-FAQ),
[EOT](https://www.w3.org/Submission/EOT/) (для Internet Explorer),
и TTF, и, таким образом, шрифты должны поддерживаться во всех
современных браузерах. В пакете также есть работающий файл CSS
для объявления стилей. 

Лицензия веб шрифтов такая же, что и для устанавливаемых шрифтов;
см. [страницу о лицензиях и отказе от ответственности](legal.html).

### Разное

* Список современных церковнославянских словоформ и их частоты использования в корпусе 
  текстов: [в формате LibreOffice](http://www.ponomar.net/files/wordlist.ods) |
  [в формате Tab-separated values](http://www.ponomar.net/files/wordlist.tsv).
* Современные церковнославянские слова и их значения (словарь): 
  [в формате LibreOffice](http://www.ponomar.net/files/dictout.ods) |
  [в формате MS Excel](http://www.ponomar.net/files/dictout.xls).
* Современные церковнославянские богослужебные книги одним архивом: 
  [в формате ZIP](http://www.ponomar.net/files/cubooks.zip)
* _Грамматика церковнославянского языка_ (архиеп. Алипия Гамановича)(http://www.ponomar.net/files/gama2/toc.html)

