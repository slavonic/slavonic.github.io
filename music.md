---
layout: default
ref: music
lang: en
css: 
  - znamenny
---

## Musical Notation

### Znamenny Notation

The Slavonic Computing Initiative provides Unicode-compliant fonts for typesetting
music in Znamenny and Put / Demestvenny (Kazan) Notations.
**Warning**: the characters required for these notational systems have been 
[accepted for encoding](http://www.unicode.org/alloc/Pipeline.html)
into a future version of the Unicode standard, but the codepoints
may still be subject to change.

* [Znamenny Font documentation](https://www.ponomar.net/files/fonts-znam.pdf)

* Znamenny Priznaki documentation [ODT format](https://www.ponomar.net/files/priznaki_documentation.odt) [PDF format](https://www.ponomar.net/files/priznaki_documentation.pdf)

* [Proposal to Encode Znamenny Notation in Unicode](https://www.ponomar.net/files/palaeoslavic.pdf) [Updates from March 2021](https://www.ponomar.net/files/update0321.pdf)

* [Fork the fonts on GitHub](https://github.com/slavonic/fonts-znam/)

#### Fonts for Znamenny Notation

* Mezenets Unicode is a font for typesetting Znamenny Notation with or without priznaki
 (Type A and Type B notations according to the classification of J. Gardner). [Download the font](https://www.ponomar.net/files/MezenetsUnicode.zip)

<div class="sample" contenteditable="true">
	<table align="center">
	<tr><td class="neume">𜽰𜽂𜼅</td>
	<td class="neume">𜽐𜼱𜼆</td>
	<td class="neume">&nbsp;&nbsp;</td>
	<td class="neume">𜽐𜽂𜼰𜼅</td>
	<td class="neume">𜽝𜽂𜼄</td>
	<td class="neume">𜽐𜽂𜼰𜼅</td>
	<td class="neume">𜽖𜽂𜼢</td>
	<td class="neume">𜽗𜽂𜼢</td>
	<td class="neume">𜽲𜼆</td>
	<td class="text">&nbsp;&nbsp;</td>
	<td class="neume">𜽯𜼅</td>
	<td class="neume">𜽟</td><td class="neume">𜾆𜽂𜼰𜼅</td>
	</tr>
	<tr><td class="text">Тво</td>
	<td class="text">ѧ</td>
	<td class="text">&nbsp;&nbsp;</td>
	<td class="text">по</td>
	<td class="text">бѣ</td>
	<td class="text">ди</td>
	<td class="text">тел</td>
	<td class="text">на</td>
	<td class="text">ѧ</td>
	<td class="text">&nbsp;&nbsp;</td>
	<td class="text">де</td>
	<td class="text">сни</td>
	<td class="text">ца</td></tr>
	</table>
</div>

* Smolensky Regular is a font for typesetting archaic Znamenny Notation as found
  in manuscripts from the 12th--15th centuries.
  [Download the font](https://www.ponomar.net/files/Smolensky-Regular.zip)

<div class="sample" contenteditable="true">
	<table align="center">
	<tr><td class="neumeB">𜽒</td>
	<td class="neumeB">𜽐</td>
	<td class="neumeB">&nbsp;&nbsp;</td>
	<td class="neumeB">𜽖</td>
	<td class="textB">&nbsp;&nbsp;</td>
	<td class="neumeB">𜽖</td>
	<td class="neumeB">𜽐𜼱</td>
	<td class="neumeB">𜽖</td>
	<td class="neumeB">𜽖</td>
	<td class="neumeB">𜽖</td>
	<td class="text">&nbsp;&nbsp;</td>
	<td class="neumeB">𜽖</td>
	<td class="neumeB">𜽐</td>
	<td class="neumeB">𜽞</td>
	</tr>
	<tr><td class="textB">Ко</td>
	<td class="textB">нѧ</td>
	<td class="textB">&nbsp;&nbsp;</td>
	<td class="textB">и</td>
	<td class="textB">&nbsp;&nbsp;</td>
	<td class="textB">въ</td>
	<td class="textB">са</td>
	<td class="textB">дь</td>
	<td class="textB">ни</td>
	<td class="textB">ки·</td>
	<td class="textB">&nbsp;&nbsp;</td>
	<td class="textB">въ</td>
	<td class="textB">мо</td>
	<td class="textB">ре</td></tr>
	</table>
</div>

#### Input and Editing

* In LaTeX, Znamenny Notation may be typeset using the `churchslavonic` package 
[View details&nbsp;»](/users.html) 

* For other software, you may use the [HTML-based Neumatic Notation
Editor](https://www.ponomar.net/znamenny/hookup2.html)

### Kievan Square Notation

Kievan (Square or Synodal) notation is a type of five-line musical notation
used in the chantbooks of the Russian Orthodox Church. Variants of Kievan
notation are also used in Prostopinje chantbooks of the Carpatho-Russians.

* [A primer in Kievan notation](http://www.synaxis.info/psalom/research/simmons/Kievan_notation.pdf)
by Nikita Simmons

* [The corpus of chantbooks in Kievan notation](http://seminaria.ru/raritet/quadsborn.htm)

#### Entering Kievan notation symbols

Kievan Notation symbols have been encoded in Unicode (beginning with version 8.0)
in the Musical Symbols block at `U+1D1DE` and following. To enter Kievan Notation
symbols in a text, you will need a font that supports these codepoints. We suggest:

* [The free Musica font by George Douros](http://users.teilar.gr/~g1951d/);
* [The free Bravura font](http://www.smufl.org/fonts/), part of the SMuFL standard; or
* The Metasuprasl font, provided by the Slavonic Computining Initiative.

- **Binaries**:
	+	PostScript outlines and OpenType features [OpenType-CFF format](https://www.ponomar.net/files/Metasuprasl-Regular.otf)
	+	TrueType outlines, OpenType and Graphite features [TrueType format](https://www.ponomar.net/files/Metasuprasl-SIL.ttf)

- **Source code**:
  + [FontForge source](https://www.ponomar.net/files/Metasuprasl-Regular.sfd)
  + [GDL Source code](https://www.ponomar.net/files/Metasuprasl-Regular.gdl)

Metasuprasl Regular is a font for typesetting Kievan notation inline.
In the SIL Graphite version, the half note with the 
long stem up and short stem down may be accessed by setting the _salt_ feature to 1 (true).
In the OpenType version, the same variant is available as stylistic alternative (salt) 1.

#### Typesetting Scores in LilyPond

Kievan Square Notation is fully supported in [LilyPond](http://www.lilypond.org/),
which is a free music engraving program, devoted to producing the highest-quality sheet music 
possible. To familiarize yourself with LilyPond, please see:

* [Some examples of LilyPond at work](http://www.lilypond.org/examples.html)

* [The introduction to LilyPond](http://www.lilypond.org/text-input.html)

* [The LilyPond manual](http://www.lilypond.org/manuals.html)

* [How to typeset scores in square notation](http://www.lilypond.org/doc/v2.18/Documentation/notation/typesetting-kievan-square-notation)

* [Download the latest version of LilyPond](http://www.lilypond.org/download.html) to get started.

Some examples of scores in square notation produced using LilyPond:

* Дал еси знамение (automelon in Tone 4, Znamenny chant): 
  [LilyPond source](https://www.ponomar.net/files/dalesi.ly) |
  [PDF](https://www.ponomar.net/files/dalesi.pdf) |
  [MIDI](https://www.ponomar.net/files/dalesi.midi)
* Sessional hymn in Tone 5, Bulgarian chant: 
  [LilyPond source](https://www.ponomar.net/files/sessional5.ly) |
  [PDF](https://www.ponomar.net/files/sessional5.pdf) |
  [MIDI](https://www.ponomar.net/files/sessional5.midi)

Here are some utilities offered on other websites to help convert 
your scores to LilyPond:

* [NoteWorthy Composer to LilyPond converter](http://nwc2ly.sourceforge.net/)
* [MusicXML to LilyPond converter](http://www.nongnu.org/xml2ly/)
* [Sibelius to LilyPond converter](http://sib2ly.sourceforge.net/)

#### Typesetting Scores in other Software

You can typeset Kievan Square Notation in other software products, such as
NoteWorthy Composer and Finale, by overriding the default font for musical symbols.
We offer for this purpose the Metasuprasl Notational font. You will need to
modify the font metrics in the METAFONT file to suit your notational program.
Then compile into a Type1 font using [mf2pt1](http://www.ctan.org/pkg/mf2pt1).

- **Source**:
  + [METAFONT source](https://www.ponomar.net/files/metasuprasl.mf)

#### Encoding

* A. Andreev, Y. Shardt, and N. Simmons.
[Proposal to Encode Medieval East-Slavic Music Notation in Unicode](https://www.ponomar.net/files/kievan.pdf) [Accepted]

* [Documentation for SMuFL](https://w3c.github.io/smufl/gitbook/)
Standard Music Font Layout), a standard for encoding additional musical glyphs
in the Private Use Area (PUA) of Unicode.

