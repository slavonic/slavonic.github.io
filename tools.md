---
layout: default
ref: tools
lang: en
---

## Church Slavonic Converters and other Utilities

This page provides various converters, utilities, and other tools for working with Slavonic text

### Converters

This section contains converters between Unicode and various legacy encoding formats.

* HIP to Unicode / Unicode to HIP converter [Web interface](http://www.ponomar.net/cgi-bin/hip2utf.cgi) |
  For standalone version, see Lingua::CU::Scripts module, below | 
  Read about the HIP format (in Russian) [here](http://orthlib.ru/hip/)

* Irmologion to Unicode / Unicode to Irmologion converter [Web interface](http://www.ponomar.net/cgi-bin/ucs2utf.cgi) |
  For standalone version, see Lingua::CU::Scripts | 
  Read about the &quot;Universal Church Slavonic&quot; (Irmologion) format (in Russian) 
  [here](http://irmologion.ru/ucsenc.html#atop)

* Irmologion to Unicode converter Extension for LibreOffice 3 (for converting DOC, DOCX and ODT files from 
  the &quot;Universal Church Slavonic&quot; format) [Download and install](http://www.ponomar.net/files/Ponomar-1.2.2.oxt)
  (**Updated**)
  
* Manuscript.ru to Unicode converter (for converting text from the [Manuscript project](http://manuscripts.ru/))
  Under development


### APIs

Software for researchers or software developers working with Slavonic text.

* Lingua::CU - a module for Church Slavic support in Perl (conversion between Church Slavic and Russian, 
  resolution of titlos, conversion of numerals, etc.). 
  Includes Lingua::CU::Collate (collation of Church Slavic text) and Lingua::CU::Scripts (standalone conversion scripts). 
  Get the code from [our github repository](https://github.com/typiconman/Perl-Lingua-CU).
  Get the Documentation from [here](http://www.ponomar.net/CU.html)
  
* _Developers wanted!_ We are also interested in developing similar APIs for other  scripting languages

### Hyphenation

Church Slavic hyphenation patterns

* [For LibreOffice 5.0 and later](http://extensions.libreoffice.org/extension-center/church-slavonic-dictionary)
* [For XeTeX, LuaTeX, and other TeX based systems](http://www.ctan.org/pkg/churchslavonic)

#### Research papers

* А. А. Андреев, М. П. Крутиков [Автоматизация слогоделения и переноса слов в церковнославянских текста](https://www.academia.edu/27011149/%D0%90%D0%B2%D1%82%D0%BE%D0%BC%D0%B0%D1%82%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F_%D1%81%D0%BB%D0%BE%D0%B3%D0%BE%D0%B4%D0%B5%D0%BB%D0%B5%D0%BD%D0%B8%D1%8F_%D0%B8_%D0%BF%D0%B5%D1%80%D0%B5%D0%BD%D0%BE%D1%81%D0%B0_%D1%81%D0%BB%D0%BE%D0%B2_%D0%B2_%D1%86%D0%B5%D1%80%D0%BA%D0%BE%D0%B2%D0%BD%D0%BE%D1%81%D0%BB%D0%B0%D0%B2%D1%8F%D0%BD%D1%81%D0%BA%D0%B8%D1%85_%D1%82%D0%B5%D0%BA%D1%81%D1%82%D0%B0%D1%85)
  [DRAFT PAPER]

### Church Slavonic OCR (Under development)

This is a project to develop Church Slavonic Optical Character Recognition for the free and open source package `Tesseract`
(read about Tesseract [here](https://code.google.com/p/tesseract-ocr/)). 
Volunteer to help with this project [on the sci-users mailing list](http://ponomar.net/mailman/listinfo/sci-users_ponomar.net).

Presently the only known way to do Slavonic OCR is via the proprietary ABBYY FineReader program and using the legacy 
HIP format (read about that [here](http://akafistnik.ru/tech/ocr/) in Russian).

### Church Slavonic Spell checking and Morphology analysis

This is a project to develop Church Slavonic morphology for Hunspell (read about Hunspell 
[here](http://hunspell.sourceforge.net/). Volunteer to help with this 
project [on the sci-users mailing list](http://ponomar.net/mailman/listinfo/sci-users_ponomar.net).
		
### Church Slavonic Collation

_TODO: Reorganize all of our Collation support and put it here. Add some documentation._

### Material for Computer-aided Church Slavonic Philology

* List of modern Church Slavonic words and their frequencies: [LibreOffice format](http://www.ponomar.net/files/wordlist.ods)
  | [Tab-separated values](http://www.ponomar.net/files/wordlist.tsv).
* Church Slavonic words and their definitions: [LibreOffice format](http://www.ponomar.net/files/dictout.ods)
  | [MS Excel format](http://www.ponomar.net/files/dictout.xls).
  (These data have been converted to Unicode on the basis of the data [here](http://www.orthodic.org/).)
* Archive of all Church Slavonic books in the modern corpus: [Text-only in ZIP format](http://www.ponomar.net/files/cubooks.zip)
* List of typographically challenging Church Slavonic words for testing fonts
  [download [in UTF-8 encoding]](http://www.ponomar.net//files/symcheck.txt)
  [this file is converted from the HIP file [here](http://irmologion.ru/tools.html#developer)]
