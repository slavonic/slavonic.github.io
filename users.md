---
layout: default
ref: users
lang: en
---

## Church Slavonic : For Users

You can easily enter, edit, and publish Church Slavonic texts in standard, popular software.

### XeTeX and LuaTeX

To work with Church Slavonic texts in TeX, you will need to use a modern Unicode-compatible TeX engine such as XeTeX or LuaTeX.
Both are part of the [TeX Live distribution](https://www.tug.org/texlive/). The following will be helpful:

* Install the hyphenation patterns for Church Slavonic. To do this, run the following command: 

  ```
  tlmgr install hyphen-churchslavonic
  ```
  
  Then rebuild the XeLaTeX and LuaLaTeX formats with this command: 
  
  ```
  fmtutil --byfmt xelatex 
  fmtutil --byfmt lualatex
  ```
  
* Install the `churchslavonic` package. This will install a set of Church Slavonic OpenType fonts, additional macros, 
  and handlers for polyglossia. You can install the package by running the command 
  
  ```
  tlmgr install churchslavonic
  ```
  
* If you have an older version of TeX Live or another distribution of TeX, you may need to install the hyphenation patterns 
  and additional packages manually. You can get the hyphenation patterns 
  [from GitHub](https://github.com/slavonic/cu-tex/tree/master/hyphenation)
  and [Church Slavonic package on CTAN](https://www.ctan.org/tex-archive/language/churchslavonic).
  Follow the instructions in the documentation.

* You can now type Church Slavonic texts using the standard commands of Polyglossia. The `churchslavonic` package 
  offers additional macros for Cyrillic numerals, drop caps and other features. See the documentation for 
  [Polyglossia](http://mirror.unl.edu/ctan/macros/latex/contrib/polyglossia/polyglossia.pdf)
  and [churchslavonic](http://ctan.altspu.ru/language/churchslavonic/churchslavonic-en.pdf) for details.

* Here is a [sample TeX file](https://www.ponomar.net/files/sample.tex)
  and its [resulting PDF output](https://www.ponomar.net/files/sample.pdf) to get you started.

* For spell-checking of documents in Church Slavonic, install Hunspell and the
  [Hunspell Church Slavonic dictionary](https://github.com/slavonic/hunspell-cu/releases).
  You can spell-check a Church Slavonic TEX file by running `hunspell -d cu -t your-file-name.tex`.

### LibreOffice

Beginning with version 5.0, LibreOffice allows you to specify Church Slavonic (which it calls Church Slavic) as a 
document language. You can then take advantage of a number of features such as Cyrillic numerals (for page numbering, etc.), 
hyphenation and sorting.

* Install the Church Slavonic fonts from [our site](fonts.html) and, if needed, the 
  Church Slavonic [keyboard drivers for your operating system](keyboard.html).

* If you have not already, upgrade LibreOffice to version 5.0 or later. You can download the 
  [latest version from the Document Foundation](http://www.libreoffice.org/download/libreoffice-fresh/). While you can view and edit Church Slavonic text in LibreOffice 4 and earlier, you will not be able to take advantage 
  of spell-checking, hyphenation and other features.

* Install the Church Slavonic Spelling and Hyphenation dictionaries. To do this, download 
  [the extension](https://extensions.libreoffice.org/extensions/church-slavonic-dictionary).
  To install, open LibreOffice, from the Tools menu select Extension Manager. The Extension Manager window will open. 
  Click the Add... button, and select the cu-lo.oxt file. When the License Agreement window opens, scroll to the end of 
  the license agreement text and click Accept.

  ![install extension](https://www.ponomar.net/images/extension_install.png)

* To set the document text to Church Slavonic, select Options from the Tools menu. Under Language Settings, select Languages. 
  The Language Settings panel will appear. Under Default Languages for Documents, select Church Slavic. 
  If you need to number the pages of a document in Cyrillic numerals, you will also need to select Church Slavic under 
  Locale Setting.

  ![locate setting](https://www.ponomar.net/images/locale_libreoffice.png)

* To turn on hyphenation, select Paragraph from the Format menu. Click on the Text Flow tab. Under Hyphenation, 
  click Automatically.

  ![enable hyphenation](https://www.ponomar.net/images/hyphenation_writer.png)
  
* To number your pages in Cyrillic numerals, click Page Number from the Insert menu. Then double-click the resulting 
  page number. The Edit Fields dialog will open. Under Format select Native Numbering and click OK. 
  (*Note*: the default locale must be set to Church Slavic for this to work.)

  ![cyrillic page numbers](https://www.ponomar.net/images/native_number.png)
  
* In LibreOffice Calc, you can sort data according to the Church Slavonic alphabetical order. To do this, select 
  Sort from the Data menu. Go to the Options tab. Under Language select Church Slavic.

  ![sorting](https://www.ponomar.net/images/sort_calc.png)
  
* The Slavonic Computing Initiative also provides the 
  [Church Slavonic Converter Extension](https://extensions.libreoffice.org/extensions/church-slavonic-converter).
  It allows you to convert Church Slavonic documents into Unicode from UCS, HIP and other legacy codepages. 
  It converts a selection, or if no selection is made, the entire document. The source code is available 
  [on GitHub](https://github.com/slavonic/cuconverter-LO).
  
* There are still a number of bugs: 
   - [85731](https://bugs.documentfoundation.org/show_bug.cgi?id=85731): Cannot specify `_` as hyphenation symbol. As a workaround to this bug, you can enable the `ss01` OpenType feature
(by setting the font name to, e.g., `Ponomar Unicode:ss01`) or the `hyph` Graphite feature
(by setting the font name to, e.g., `Ponomar Unicode TT:hyph=1`). Please take a look at
[the font documentation](https://www.ponomar.net/files/fonts-churchslavonic.pdf) for more information.

   - [96343](https://bugs.documentfoundation.org/show_bug.cgi?id=96343): Cannot convert Cyrillic Extended-B symbols to uppercase

### Visual Studio Code

[Visual Studio Code](https://code.visualstudio.com/) is a free, portable source code editor.
It is useful for editing the raw Church Slavonic liturgical texts stored in 
[XML](https://github.com/slavonic/cu-books) and 
[Markdown](https://github.com/slavonic/cumd) formats. 

  ![VS Code](https://www.ponomar.net/images/vscode.png)

To set up editing Church Slavonic texts in Visual Studio Code:

* Install [Church Slavonic Markdown
Extensions](https://marketplace.visualstudio.com/items?itemName=pgmmpk.vscode-church-slavonic).

* Open the Markdown preview pane (press `Ctrl+Shift+P` to open the palette and select 
`Markdown: Open Preview to the Side`).

* Install the [VS Code Church Slavonic
Keyboard](https://marketplace.visualstudio.com/items?itemName=pgmmpk.vscode-church-slavonic-keyboard).

* Initially the keyboard is off. To toggle, press `Ctrl+Alt+Space` (on GNU/Linux, `Meta+Space`)
or select the command `Church Slavonic Keyboard: Toggle` from the palette.

* It is best to edit text using a monospaced font supporting Unicode 10.0 or newer.
See our [FiraSlav font](fonts.html). To change the font for the editor,
place the line `"editor.fontFamily": "Fira Slav"` in the `User Settings` file.

### Apache OpenOffice

[Apache Office](http://www.openoffice.org/) is not well maintained. While you can view and edit Church Slavonic texts, 
the software will not allow declaring Church Slavonic as a language. Hence, you will not be able to use hyphenation or 
spell checking and you will not have access to Cyrillic numerals and other features. 

We suggest [using LibreOffice](https://www.libreoffice.org/download/libreoffice-fresh/) instead.

### Microsoft Office

Microsoft Corporation does not recognize Church Slavonic as a language, and so hyphenation and spell checking are 
not available, even in third-party extensions.
Church Slavonic texts **may** display correctly in Microsoft Office using the Ponomar Unicode font. 
However, your results may vary, and you may see incorrectly positioned diacritical marks,
missing characters and other problems. There are no workarounds for these issues. 

*We do not provide any support for Microsoft products*.

We suggest [using LibreOffice](https://www.libreoffice.org/download/libreoffice-fresh/) instead.

### Adobe InDesign

Once you have installed the Church Slavonic fonts from [this page](fonts.html), you should be able to work with Church 
Slavonic texts in Adobe InDesign. To get support for Church Slavonic hyphenation and spell-checking, 
download the 
[Church Slavonic Dictionary Extension for LibreOffce](http://extensions.libreoffice.org/extensions/church-slavonic-dictionary);
then follow [the instructions](https://helpx.adobe.com/indesign/kb/add_cs_dictionaries.html) to install it into InDesign.
Page numbering using Cyrillic numerals is not available. If you need it, [ask Adobe](https://helpx.adobe.com/contact.html?step=IDSN)
to add this feature or switch to LibreOffice.

### Where is the letter / symbol that I need?

Tables of Church Slavonic letters and other symbols are available in the documentation:

* [Church Slavonic Typography in Unicode](http://www.unicode.org/notes/tn41/) - Unicode Technical Note #41. Provides tables of all relevant characters encoded in Unicode.
* [Ponomar Project Private Use Area (PUA) Allocation Policy](https://www.ponomar.net/files/pua_policy.pdf)
  Provides tables of other characters available in fonts.

### I need help!

If you are having difficulties, all questions (except for those related to Microsoft products) may be addressed to 
the [SCI-Users mailing list](https://ponomar.net/mailman/listinfo/sci-users_ponomar.net).

