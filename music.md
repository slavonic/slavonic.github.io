---
layout: default
ref: music
lang: en
---

## Musical Notation

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
	+	PostScript outlines and OpenType features [OpenType-CFF format](http://www.ponomar.net/files/Metasuprasl-Regular.otf)
	+	TrueType outlines, OpenType and Graphite features [TrueType format](http://www.ponomar.net/files/Metasuprasl-SIL.ttf)

- **Source code**:
  + [FontForge source](http://www.ponomar.net/files/Metasuprasl-Regular.sfd)
  + [GDL Source code](http://www.ponomar.net/files/Metasuprasl-Regular.gdl)

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
  [LilyPond source](http://www.ponomar.net/files/dalesi.ly) |
  [PDF](http://www.ponomar.net/files/dalesi.pdf) |
  [MIDI](http://www.ponomar.net/files/dalesi.midi)
* Sessional hymn in Tone 5, Bulgarian chant: 
  [LilyPond source](http://www.ponomar.net/files/sessional5.ly) |
  [PDF](http://www.ponomar.net/files/sessional5.pdf) |
  [MIDI](http://www.ponomar.net/files/sessional5.midi)

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
  + [METAFONT source](http://www.ponomar.net/files/metasuprasl.mf)

#### Encoding

* A. Andreev, Y. Shardt, and N. Simmons.
[Proposal to Encode Medieval East-Slavic Music Notation in Unicode](http://www.ponomar.net/files/kievan.pdf) [Accepted]

* [Documentation for SMuFL](https://w3c.github.io/smufl/gitbook/)
Standard Music Font Layout), a standard for encoding additional musical glyphs
in the Private Use Area (PUA) of Unicode.

### Znamenny Notation

The repertoire of Znamenny, Demestvenny, and other notational systems has not yet been
added to Unicode and adequate support for working with these notations on the computer
is not yet available. We are working on a proposal to add the symbols for these notational
systems.

* A. Andreev and N. Simmons. [Proposal to Encode Paleoslavic Musical Notations in Unicode](http://www.ponomar.net/files/palaeoslavic.pdf)

While the proposal is being tested and approval is sought, the characters have been
temporarily encoded in the Private Use Area of Unicode. To test the proposed
methodology for working with Znamenny Notation, please see:

* [Private Use Area Policy](http://www.ponomar.net/files/pua_policy.pdf) (lists the codepoints)

* [Fonts for Znamenny Notation](https://github.com/slavonic/fonts-znam)
 (using the proposed encoding methodology)

* [Znamenny Notation Manual](http://www.ponomar.net/wiki/doku.php?id=znamenny_manual)
 (a sandbox for testing the font)

All of this material is ALPHA-PHASE SOFTWARE, comes with ABSOLUTELY NO WARRANTY,
and is intended for SOFTWARE TESTING PURPOSES ONLY.


