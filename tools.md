---
layout: default
ref: tools
lang: en
---

## For Developers and Programmers

### Converters

Converters for converting Church Slavonic texts into Unicode from various legacy codepages.

* [HIP](http://orthlib.ru/hip/) to Unicode converter [Web interface](https://www.ponomar.net/cgi-bin/hip2utf.cgi) |
  [Standalone through Lingua::CU::Scripts](https://github.com/typiconman/Perl-Lingua-CU) module

* [Irmologion](http://irmologion.ru/) to Unicode converter [Web interface](https://www.ponomar.net/cgi-bin/ucs2utf.cgi) |
   [Standalone through Lingua::CU::Scripts](https://github.com/typiconman/Perl-Lingua-CU) module

* [Church Slavonic converter Extension for LibreOffice 3.0 and higher](https://extensions.libreoffice.org/extensions/church-slavonic-converter)


## Automatic translation from modern to Church Slavonic orthography
Translation tooling is published [in our GitHub repository](https://github.com/slavonic/translator).

Small texts can be conveniently translated [in our web application](/translate). Attention mobile internet users! This web-application will load 40+Mb of code and data.

## Automatic accenting of Church Slavonic text in modern orthography
Check out our web [our web application](/accent). Attention mobile internet users! This web-application will load 40+Mb of code and data.

## Automatic accenting of Russian text
Check out our web [our web application](/accentru). Attention mobile internet users! This web-application will load 30+Mb of code and data.

### APIs

APIs for developing Church Slavonic-aware applications provide a variety of tools,
such as collation (sorting), string comparison, conversion between Church Slavonic
and Russian (modern) orthography, automated generation of Slavonic numerals, and more.

* [Lingua::CU](https://github.com/typiconman/Perl-Lingua-CU) - a
  module for Church Slavonic support in Perl.

* [cslavonic](https://github.com/pgmmpk/cslavonic) - a
   module for Church Slavonic support in Python.

### Hyphenation

Church Slavic hyphenation patterns

* [For LibreOffice 5.0 and later](https://extensions.libreoffice.org/extensions/church-slavonic-dictionary)
* [For XeTeX, LuaTeX, and other TeX based systems](https://github.com/slavonic/cu-tex/tree/master/hyphenation)
* [For web pages using Hyphenator.js](https://mnater.github.io/Hyphenator/)

### Web Fonts

If you wish to display Church Slavonic text on your website or blog, you can simply
add a reference to our stylesheet in the `HEAD` section of your document:

```
<link rel="stylesheet" href="https://slavonic.github.io/css/fonts.css" type="text/css">
```

All of the necessary fonts will be loaded automatically. To use the fonts, just
declare the appropriate CSS classes, for example:

```
.slavonic {
  font-family: 'Ponomar Unicode';
}
```

If you do not wish to load the fonts from our server but would rather place
the embeddable web fonts on your own server, you can download the
[embeddable web font package](https://www.ponomar.net/files/sci-webfonts.zip)
and un-zip it to some directory on your server. 

The package provides all of the fonts in [WOFF2](https://www.w3.org/TR/WOFF2/),
[WOFF](https://www.w3.org/Fonts/WOFF-FAQ),
[EOT](https://www.w3.org/Submission/EOT/) (for Internet Explorer),
and TTF formats, which should work with all modern browsers, as well as a
working CSS stylesheet to get you started. 

The web fonts are distributed
under the same license as the installable fonts; see the [legal page](legal.html) for details.

### Miscellaneous Resources

* List of modern Church Slavonic words and their frequencies: [LibreOffice format](https://www.ponomar.net/files/wordlist.ods)
  | [Tab-separated values](https://www.ponomar.net/files/wordlist.tsv).
* Church Slavonic words and their definitions: [LibreOffice format](https://www.ponomar.net/files/dictout.ods)
  | [MS Excel format](https://www.ponomar.net/files/dictout.xls).
* Archive of all Church Slavonic books in the modern corpus: [Text-only in ZIP format](https://www.ponomar.net/files/cubooks.zip)
* _Church Slavonic Grammar_ (by Archbishop Alypy) [in Russian](https://www.ponomar.net/files/gama2/toc.html)


