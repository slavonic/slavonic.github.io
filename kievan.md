---
layout: default
ref: kievan
lang: en
---
## Liturgical Music in Kievan Notation

Kievan (Square or Synodal) notation is a type of five-line musical notation used in the chantbooks of the Russian 
Orthodox Church. Variants of Kievan notation are also used in Prostopinje chantbooks of the Carpatho-Russians.

* A primer in Kievan notation by Nikita Simmons is 
  available [here](http://www.synaxis.info/psalom/research/simmons/Kievan_notation.pdf)

* The corpus of chantbooks published by the Russian Orthodox Church in Kievan notation is available 
  [here](http://seminaria.ru/raritet/quadsborn.htm)
  (this website has recently been having problems; we plan on making these materials available through the Ponomar Project)

### Support for Kievan notation in LilyPond

[LilyPond](http://www.lilypond.org/) is a music engraving program, devoted to producing the highest-quality sheet music 
possible. LilyPond is free software, has a text-based input format that makes it fully integrable with the Ponomar API, 
and is easily extendable with the Scheme language, which makes it ideal for musicological work. And it produces beatiful 
musical scores. See examples of LilyPond at work [here](http://lilypond.org/examples.html)

* To download the latest version [click here](http://www.lilypond.org/download.html)

* Follow these links to read the [introduction](http://www.lilypond.org/text-input.html)
  and the [Manual](http://lilypond.org/manuals.html)

* Read about typesetting scores in square notation 
  [here](http://lilypond.org/doc/v2.18/Documentation/notation/typesetting-kievan-square-notation)


Some examples of scores in square notation:

* Дал еси знамение (automelon in Tone 4, Znamenny chant): 
  [LilyPond source](http://www.ponomar.net/files/dalesi.ly) |
	[PDF](http://www.ponomar.net/files/dalesi.pdf) |
  [MIDI](http://www.ponomar.net/files/dalesi.midi
* Sessional hymn in Tone 5, Bulgarian chant: 
  [LilyPond source](http://www.ponomar.net/files/sessional5.ly) |
  [PDF](http://www.ponomar.net/files/sessional5.pdf) |
  [MIDI](http://www.ponomar.net/files/sessional5.midi)


### Converters

`zf2ly` is a Perl script used to convert materials from the [Znamenny Fund website](http://www.znamen.ru/)
into LilyPond. Znamenny neumes are not yet supported. The script presently ONLY converts the lyrics from ZF's format 
to Unicode and the notes to either Common (round) or Kievan (square) notation. 
*Warning*: this script is BETA-stage software! 
To download: [click here](http://www.ponomar.net/cgi-bin/fetch_script.cgi?target=zf2ly)
(supported natively in Linux; on Windows, install [Strawberry Perl](http://strawberryperl.com/))


Examples of converted scores:

* Lesser Theotokion, Tone 1. 
  [MIDI](http://www.ponomar.net/files/lesser_theotokion1.midi)
  - Round Notation: 
    [LilyPond source](http://www.ponomar.net/files/lesser_theotokion1.ly) |
    [PDF](http://www.ponomar.net/files/lesser_theotokion1.pdf)
  - Square Notation:
    [LilyPond source](http://www.ponomar.net/files/lesser_theotokion1_k.ly) |
    [PDF](http://www.ponomar.net/files/lesser_theotokion1_k.pdf)

* Lesser Theotokion, Tone 2. [MIDI](http://www.ponomar.net/files/lesser_theotokion2.midi)
  - Round Notation: 
    [LilyPond source](http://www.ponomar.net/files/lesser_theotokion2.ly) |
    [PDF](http://www.ponomar.net/files/lesser_theotokion2.pdf)
  - Square Notation:
    [LilyPond source](http://www.ponomar.net/files/lesser_theotokion2_k.ly) |
    [PDF](http://www.ponomar.net/files/lesser_theotokion2_k.pdf)

Get out of the proprietary software jail. Here are some utilities offered on other websites to help convert 
your scores to LilyPond:

* NoteWorthy Composer to LilyPond converter ([here](http://nwc2ly.sourceforge.net/))
* MusicXML to LilyPond converter ([here](http://www.nongnu.org/xml2ly/))
  [this can be used to export from Finale into LilyPond]
* Sibelius to LilyPond converter ([here](http://sib2ly.sourceforge.net/))

### Kievan notation fonts

* If you are typesetting Kievan notation scores, we suggest using [LilyPond](http://www.lilypond.org/)
* If you need to type Kievan symbols in a text, we suggest the free Musica font by George Douros, which 
  is [available from here](http://users.teilar.gr/~g1951d/);
* Or the free Bravura font [available from here](http://www.smufl.org/fonts/) as part of the SMuFL standard

Metasuprasl was originally developed by the authors for typesetting Kievan notation. Its glyphs have now been subsumed 
into Musica and Bravura. It may still be useful for getting music notation software to support Kievan notation.

#### Metasuprasl Regular, Version 1.3

- **Binaries**:
	+	PostScript outlines and OpenType features [OpenType-CFF format](http://www.ponomar.net/files/Metasuprasl-Regular.otf)
	+	TrueType outlines, OpenType and Graphite features [TrueType format](http://www.ponomar.net/files/Metasuprasl-SIL.ttf)

- **Source code**:
  + [FontForge source](http://www.ponomar.net/files/Metasuprasl-Regular.sfd)
  + [GDL Source code](http://www.ponomar.net/files/Metasuprasl-Regular.gdl)

Metasuprasl Regular is a font for typesetting Kievan notation inline. In the SIL Graphite version, the half note with the 
long stem up and short stem down may be accessed by setting the _salt_ feature to 1 (true). In the OpenType version, 
the same variant is available as stylistic alternative (salt) 1.

#### Metasuprasl Notational, Version 1.1

- **Source**:
  + [METAFONT source](http://www.ponomar.net/files/metasuprasl.mf)

Metasuprasl Notational is a font for music notation software. Instructions: modify the font metrics in the METAFONT file to 
suit your notational program. Then compile into a Type1 font using [mf2pt1](http://www.ctan.org/pkg/mf2pt1). 

**License**: Metasuprasl is licensed under the GNU GPL (v. 2 or higher) with Font Exception or, at your choosing, 
the SIL Open Font License.

### Encoding

* A. Andreev, Y. Shardt, and N. Simmons. [Proposal to Encode Medieval East-Slavic Music Notation in Unicode](http://www.ponomar.net/files/kievan.pdf) [Accepted]

* Documentation for SMuFL (Standard Music Font Layout), a standard for encoding additional musical glyphs in the Private 
  Use Area (PUA) of Unicode ([click here](http://www.smufl.org/download/))

### Musicological work

This section contains various helpful information for working with chant.

* [Standardization of Automela](http://www.ponomar.net/files/automela.pdf) [PONOMAR GREEN PAPER]
