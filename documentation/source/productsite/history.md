
### 9 Feb 2022 (SIL WSTech Team) Doulos SIL version 6.101

This is a maintenance release primarily focused on making the v6 font available on *TypeTuner Web*.

#### New

- The font now supports SIL *TypeTuner*. Customized fonts can be created at *TypeTuner Web* (https://scripts.sil.org/ttw/fonts2go.cgi)

- New `locl` OpenType feature that supports Macedonian (MKD/mk) Cyrillic alternates

- Serbian and Macedonian alternates are also available through a new OpenType feature (cv84) for applications that do not support language-specific `locl` features

- Characters have been added to support Unicode versions up to 14.0.0 (more to be added in future releases):
    - U+A7C4 LATIN CAPITAL LETTER C WITH PALATAL HOOK
    - U+A7C5 LATIN CAPITAL LETTER S WITH HOOK
    - U+1DF00 LATIN SMALL LETTER FENG DIGRAPH WITH TRILL
    - U+1DF01 LATIN SMALL LETTER REVERSED SCRIPT G
    - U+1DF02 LATIN LETTER SMALL CAPITAL TURNED G
    - U+1DF03 LATIN SMALL LETTER REVERSED K
    - U+1DF05 LATIN SMALL LETTER LEZH WITH RETROFLEX HOOK
    - U+1DF07 LATIN SMALL LETTER REVERSED ENG
    - U+1DF09 LATIN SMALL LETTER T WITH HOOK AND RETROFLEX HOOK
    - U+1DF0A LATIN LETTER RETROFLEX CLICK WITH RETROFLEX HOOK
    - U+1DF0B LATIN SMALL LETTER ESH WITH DOUBLE BAR
    - U+1DF0C LATIN SMALL LETTER ESH WITH DOUBLE BAR AND CURL
    - U+1DF0D LATIN SMALL LETTER TURNED T WITH CURL
    - U+1DF0E LATIN LETTER INVERTED GLOTTAL STOP WITH CURL
    - U+1DF0F LATIN LETTER STRETCHED C WITH CURL
    - U+1DF10 LATIN LETTER SMALL CAPITAL TURNED K
    - U+1DF11 LATIN SMALL LETTER L WITH FISHHOOK
    - U+1DF12 LATIN SMALL LETTER DEZH DIGRAPH WITH PALATAL HOOK
    - U+1DF13 LATIN SMALL LETTER L WITH BELT AND PALATAL HOOK
    - U+1DF14 LATIN SMALL LETTER ENG WITH PALATAL HOOK
    - U+1DF15 LATIN SMALL LETTER TURNED R WITH PALATAL HOOK
    - U+1DF16 LATIN SMALL LETTER R WITH FISHHOOK AND PALATAL HOOK
    - U+1DF17 LATIN SMALL LETTER TESH DIGRAPH WITH PALATAL HOOK
    - U+1DF19 LATIN SMALL LETTER DEZH DIGRAPH WITH RETROFLEX HOOK
    - U+1DF1A LATIN SMALL LETTER I WITH STROKE AND RETROFLEX HOOK
    - U+1DF1B LATIN SMALL LETTER O WITH RETROFLEX HOOK
    - U+1DF1C LATIN SMALL LETTER TESH DIGRAPH WITH RETROFLEX HOOK
    - U+1DF1D LATIN SMALL LETTER C WITH RETROFLEX HOOK
    - U+1DF1E LATIN SMALL LETTER S WITH CURL
    
#### Improved

- The special-purpose modified fonts have been updated to be based on the current version. These are available at https://software.sil.org/lcgfonts/download/ and include *Literacy* and *Compact* versions.

- U+02DE MODIFIER LETTER RHOTIC HOOK position improved with modifier vowels: 
    - U+02B8 MODIFIER LETTER SMALL Y
    - U+1D53 MODIFIER LETTER SMALL OPEN O
    - U+1D5A MODIFIER LETTER SMALL TURNED M
    - U+1DBA MODIFIER LETTER SMALL TURNED V

- Design improved for these characters:
    - U+0184 LATIN CAPITAL LETTER TONE SIX
    - U+0185 LATIN SMALL LETTER TONE SIX

- The small caps feature (smcp) now supports more characters

#### Changed encoding

- The following characters were in the SIL PUA but have now been given Unicode assignments. The SIL PUA characters are now deprecated:
    - U+A7C6 LATIN CAPITAL LETTER Z WITH PALATAL HOOK (was U+F234)
    - U+10783 MODIFIER LETTER SMALL AE (was U+F1A1)
    - U+1078F MODIFIER LETTER SMALL CLOSED REVERSED OPEN E (was U+F1A4)
    - U+10791 MODIFIER LETTER SMALL RAMS HORN (was U+F1B5)
    - U+10795 MODIFIER LETTER SMALL H WITH STROKE (was U+F1BC)
    - U+107A0 MODIFIER LETTER SMALL TURNED Y (was U+F1CE)
    - U+107A2 MODIFIER LETTER SMALL O WITH STROKE (was U+F1AB)
    - U+107A3 MODIFIER LETTER SMALL CAPITAL OE (was U+F1AE)
    - U+107B2 MODIFIER LETTER SMALL CAPITAL Y (was U+F1B4)
    - U+1088E NABATAEAN LETTER FINAL KAPH (was U+F1A3)
    - U+1DF04 LATIN LETTER SMALL CAPITAL L WITH BELT (was U+F268)
    - U+1DF06 LATIN SMALL LETTER TURNED Y WITH BELT (was U+F267)
    - U+1DF08 LATIN SMALL LETTER TURNED R WITH LONG LEG AND RETROFLEX HOOK (was U+F269)
    - U+1DF18 LATIN SMALL LETTER EZH WITH PALATAL HOOK (was U+F235)

### 2 July 2021 (SIL WSTech Team) Doulos SIL version 6.001

- Reverted font Postscript name to that used in v5 and earlier to avoid problems with unrecognized fonts when opening older documents.

### 29 Jun 2021 (SIL WSTech Team) Doulos SIL version 6.000

***Note that this is a major upgrade that may cause document reflow as some glyphs widths have changed and some features have been removed.***

#### Removed

- **Removed DSIGs added in version 5.000.** These have now been removed to reflect current best practice font development guidance. Adobe InDesign will complain that fonts cannot be found if a document last saved with version 5.000 is opened with version 5.960 or later installed. It will be necessary to find/replace the fonts in the document using the command in the Type menu. Please also look over the document carefully to note any places where changes in the fonts have affected letterforms or spacing.

- **Graphite has been removed.** Application and OS support for OpenType has greatly improved, so the need for Graphite in this font is greatly reduced. *If this affects you, and you find that OpenType does not provide sufficient support for your needs, please contact us right away.*  

- Removed the "Show Invisibles" feature.

- Removed support for nine-level pitch contours. These will be replaced by a standalone pitch contours font in the future.

#### Added

Characters added to support Unicode versions 7.0-13.0, including feature support (e.g. small caps) where appropriate:

- U+03D1 GREEK THETA SYMBOL
- U+03F4 GREEK CAPITAL THETA SYMBOL
- U+1AB0 COMBINING DOUBLED CIRCUMFLEX ACCENT
- U+1AB1 COMBINING DIAERESIS-RING
- U+1AB2 COMBINING INFINITY
- U+1AB3 COMBINING DOWNWARDS ARROW
- U+1AB4 COMBINING TRIPLE DOT
- U+1AB5 COMBINING X-X BELOW
- U+1AB6 COMBINING WIGGLY LINE BELOW
- U+1AB7 COMBINING OPEN MARK BELOW
- U+1AB8 COMBINING DOUBLE OPEN MARK BELOW
- U+1AB9 COMBINING LIGHT CENTRALIZATION STROKE BELOW
- U+1ABA COMBINING STRONG CENTRALIZATION STROKE BELOW
- U+1DF5 COMBINING UP TACK ABOVE
- U+203B REFERENCE MARK
- U+20BE LARI SIGN
- U+20BF BITCOIN SIGN
- U+27E8 MATHEMATICAL LEFT ANGLE BRACKET
- U+27E9 MATHEMATICAL RIGHT ANGLE BRACKET
- U+2E13 DOTTED OBELOS
- U+2E14 DOWNWARDS ANCORA
- U+2E17 DOUBLE OBLIQUE HYPHEN
- U+2E22 TOP LEFT HALF BRACKET
- U+2E23 TOP RIGHT HALF BRACKET
- U+2E24 BOTTOM LEFT HALF BRACKET
- U+2E25 BOTTOM RIGHT HALF BRACKET
- U+A78F LATIN LETTER SINOLOGICAL DOT
- U+A7AE LATIN CAPITAL LETTER SMALL CAPITAL I
- U+A7AF LATIN LETTER SMALL CAPITAL Q
- U+A7B3 LATIN CAPITAL LETTER CHI
- U+A7B4 LATIN CAPITAL LETTER BETA
- U+A7B5 LATIN SMALL LETTER BETA
- U+A7B6 LATIN CAPITAL LETTER OMEGA
- U+A7B7 LATIN SMALL LETTER OMEGA
- U+A7B8 LATIN CAPITAL LETTER U WITH STROKE
- U+A7B9 LATIN SMALL LETTER U WITH STROKE
- U+AB30 LATIN SMALL LETTER BARRED ALPHA
- U+AB53 LATIN SMALL LETTER CHI
- U+AB5C MODIFIER LETTER SMALL HENG
- U+AB5E MODIFIER LETTER SMALL L WITH MIDDLE TILDE
- U+F26E CAPITAL RAMS HORN (in SIL PUA)

#### New

- First release that uses a UFO-based design and production workflow
    - All sources are in open formats
    - Build toolkit and workflow is completely open-source
    - See https://silnrsi.github.io/silfontdev/en-US/Introduction.html

- Web fonts are provided in both WOFF and WOFF2 formats

- Applied new hinting techniques to try to improve screen rendering on Windows

- All-new documentation in HTML and PDF formats

- Features for controlling literacy forms of a and g separately
    - Literacy a alternates (ss02)
    - Literacy g alternates (ss03)

- Feature to support side-by-side rendering of U+0300 plus U+0301
    - Kayan diacritics (cv79)

- Tone letter features (cv91 & cv92) now supported through OpenType

#### Fixes

- Width of typographic spaces have been made more consistent to reflect
common publishing industry usage. Note that this may affect line and page
lengths. Affected spaces:

    - U+2008 PUNCTUATION SPACE (made width consistent)
    - U+202F NARROW NO-BREAK SPACE (made narrower)

- Fixed some small capital correspondences, including added support for clicks

- Fixed problems with spacing of tone letters

- Improved miscellaneous anchor positions, including the position of diacritics 
below glyphs with macrons below (e.g. U+1E0F LATIN SMALL LETTER D WITH LINE BELOW)

- Improved position of diacritics for superscripts and modifier letters
(including cedilla, ogonek, rhotic hook)

- Fixes and improvements to various glyphs:
    - U+01E5 LATIN SMALL LETTER G WITH STROKE (bar position on single-story variant)
    - U+02D6 MODIFIER LETTER PLUS SIGN (size)
    - U+02DF MODIFIER LETTER CROSS ACCENT (size)
    - U+02E4 MODIFIER LETTER SMALL REVERSED GLOTTAL STOP (form)
    - U+031F COMBINING PLUS SIGN BELOW (design)
    - U+033B COMBINING SQUARE BELOW (more rectangular)
    - U+1AB3 COMBINING DOWNWARDS ARROW (position fixes since beta 1)
    - U+1D15 LATIN LETTER SMALL CAPITAL OU (form)
    - U+1D77 LATIN SMALL LETTER TURNED G (position)
    - U+1D78 MODIFIER LETTER CYRILLIC EN (form)
    - U+A76A LATIN CAPITAL LETTER ET
    - U+A76B LATIN SMALL LETTER ET
    - U+A76C LATIN CAPITAL LETTER IS
    - U+A76D LATIN SMALL LETTER IS
    - U+A77F LATIN SMALL LETTER TURNED INSULAR G (position)
    - U+A7F8 MODIFIER LETTER CAPITAL H WITH STROKE (form)

#### Known issues

- There is no support for TypeTuner or TypeTuner Web. We hope to add that support soon.

- There are no regional subsets. Please contact us if these are a priority for you and describe how you use them. We are reassessing whether to provide these subsets. With current web technology and WOFF2 compression most uses can be met equally well with the full fonts.

### 27 Oct 2014 (SIL NRSI team) Doulos SIL version 5.000
- Added Stylistic Sets to the font for OpenType support 
	of previously Graphite-only features
- Added Character Variants to the font for OpenType support 
	of previously Graphite-only features
- Added Serbian feature when Serbian language is turned on
- Added hook D variant feature (for U+018A/U+0257)
- Removed "Show deprecated PUA" feature
- Removed "Romanian-style diacritics" feature 
  (because glyphs are now encoded)
- Removed "Diacritic selection" feature
- Added U+039E, U+03BC, U+03C6 and U+03C9 in the Greek and Coptic block
- Added U+0528..U+052F in the Cyrillic Supplement block
- Added U+2041 in the General Punctuation block
- Added U+2095..U+209C in the Superscripts and Subscripts block
- Added U+20B6..U+20BD in the Currency Symbols block
- Added U+210C, U+2113, U+2117, U+212D, U+2135, U+214F in the 
  Letterlike Symbols block
- Added U+2150..U+2152 and U+2189 in the Number Forms block
- Added U+2226, U+2234..U+2235, U+2262, U+2282..U+2287 in the 
  Mathematical Operators block
- Added U+2640, U+2642, U+266D, U+266F in the Miscellaneous Symbols block
- Added U+27E8..U+27E9 in the Miscellaneous Mathematical Symbols-A block
- Added U+2C7E..U+2C7F in the Latin Extended-C block
- Added U+2C88 in the Coptic block
- Added U+2E00..U+2E0D, U+2E3A..U+2E3B in the Supplemental 
  Punctuation block
- Added U+A736..U+A73F, U+A742..U+A74D, U+A750..U+A787, U+A790..U+A7AD, 
  U+A7B0..U+A7B1, U+A7F7..U+A7FA in the Latin Extended-D block. 
  These were also added to relevant features.
- Added U+A92E in the Kayah Li block (to support the Kayah Li language 
  when using the Roman script)
- Added U+AB64..U+AB65 in the Latin Extended-E block
- Added U+1D40C, U+1D504..U+1D505, U+1D50A, U+1D50E..U+1D50F, U+1D514, 
  U+1D516..U+1D517, U+1D519 in the Mathematical Alphanumeric Symbols block
- Added PUA characters U+F26C (curl J) and U+F26D (left-hook b)
- Characters in our PUA that were added to Unicode have had their 
  codepoints updated:
  F1AD>A7F9, F266>A78E, F26B>A78D, F32C>0526, F32D>0527, F17B>1DFD, F209>2C70
- These PUA characters were deprecated (now white on black glyphs): 
  U+F17B, U+F1AD, U+F209, U+F247, U+F248, U+F266, U+F26B, U+F32C, U+F32D
- Deleted U+0149 as it is officially deprecated in Unicode
- Added support for shorter macrons under narrow letters (i,l,r,t).
  (This only works for Graphite or using precomposed characters in OpenType.)
- Made it possible for saltillo characters (U+A78B and U+A78C) to "carry" 
  diacritics
- Improved design of U+A722..U+A725 and U+A78D
- Refactored all cedilla positioning
- Removal of unneeded duplicate glyphs (because of improvements in smart 
  font code)
- Bug fix in Graphite code to allow for simultaneous selection of Vietnamese 
  alternates and Small Caps
- Bug fix in Graphite code to allow for simultaneous selection of Ogonek 
  alternates and Small Caps
- Subscript and Superscript parentheses, minus, plus and equals were raised.
	Metrics were not changed.
- Adjusted tails on U+2C6B, U+2C6C
- Arrowhead design of U+21A8 modified to match the other arrows
- Placement of Ogonek revisited
- Changed the strongly curved hooks on Cyrillic U+04C3..U+04C4, U+04C7..U+04C8, 
  U+04FC..U+04FD, U+0512..U+0513 to be more consistent with other hooks
- Modified design of U+A78D to be more curved and less squared
- Changed postscript names for U+0218 and U+0219
- Changed postscript names for U+2203, U+232A and U+2329
- "Hide tone contour staves" feature now works with single tonebar
- Allowed combining marks to render properly with U+02D0

### 1 Aug 2012 (SIL NRSI team) Doulos SIL version 4.112
- Changed Graphite feature identifiers from integers to 4-character 
  alphanumeric tags (no other changes)

### 12 Sep 2011 (SIL NRSI team) Doulos SIL version 4.110
- Removed the VDMX table
- Changed version number (using ttfsetver)

### 25 Aug 2011 (SIL NRSI team) Doulos SIL version 4.108
- Double-encoded the SIL PUA characters which were added to Unicode 5.2 and 6.0
  (using ttfremap)
- Encoded 1D29 (using ttfremap)
- Corrected problem with coverage tables (using ttfsortcover)
- Changed version number (using ttfsetver)
- Added device metric tables
- Added an empty dsig table

### 05 May 2009 (Alan Ward) Doulos SIL version 4.106
- TypeTuner (Silt) table changed so that line metrics from legacy fonts
  can be imported

### 20 Mar 2009 (SIL NRSI team) Doulos SIL version 4.106
- Added support for Unicode 5.1 Latin and Cyrillic additions
- Other characters added: 0462, 0463, 0474, 0475, 0524, 0525, 20E5, 2203, 2204,
  231C..U+231F, 2329, 232A, 239B..23AD, A722..U+A725 
- Added PUA characters F26B, F32C, F32D 
- Design changes: 002F, 02D0, 02ED, 02FF, 034B, 04A8, 04A9, 04BC, 
  04BD, 04BE, 04BF, 04E0, 04E1, 045F, 04AA, 04AB, F208, F209, 0358
- Fixed attachment points on 04FA, 04FB, fi and fl ligatures 
- Fixed advance of t-caron
- Feature modifications:
    * new alternates added to feature ID 1033 and renamed from Small v-hook
      alternate to V-hook alternates
    * new alternate U+2C65 LATIN SMALL LETTER A WITH STROKE added to 
      Literacy alternates feature
    * default for Diacritic selection was changed from "on" to "off" 
     (by request of FieldWorks team) 
- Added new features:
    * Small Caps
    * Non-European caron alternates
    * Capital B-hook alternate
    * Show deprecated PUA 
- Slant italic bug fixed (dot on i was not disappearing with combining marks) 
- Removal of about 700 unused glyphs (including precomposed chao tone letters 
  which were no longer needed since these are now dynamically created)
- Fixed issues: kern table error, usMaxContext and yMax errors
- Several OpenType issues fixed
- Graphite reordering bug fixed
- Automated AAT build process
- Changed OFL license to version 1.1 

### 9 May 2008 (SIL NRSI team) Doulos SIL version 4.104
- Double-encoded the SIL PUA characters which were added to Unicode 5.1 (using
  ttfremap)
- Changed version number (using ttfsetver)

### 16 Aug 2007 (SIL NRSI team) Doulos SIL version 4.102
- Modified the OpenType features so that InDesign's built-in small caps work

### 31 Jan 2007 (SIL NRSI team) Doulos SIL version 4.100
- Added PUA character F26A
- Added 2308, 2309
- Removed Cyrillic italic alternates feature and added those 3 characters to the
  slant italic specials feature
- Fixed bug in nine-level tones (in PUA) feature
- Made Chinantec tones larger, added 02C9 to this feature
- Fixed bug in GSUB table to work in Pango

### 15 Dec 2006 (SIL NRSI team)  Doulos SIL version 4.0.16 beta 1 (Version 4.016)
- Beta release (should not be distributed!)
- Added support for Unicode 5 Latin and Cyrillic additions
- Other new chars: 2053, 211F, 2123, 2423, FE20..FE23
- Numerous new PUA characters
- Deprecated some existing PUA chars now added to Unicode
- New features:
	- Open O alternate
	- Chinantec tones
	- Pitch contour tramlines
- Tone bars no longer limited to 3 sequences (OpenType)
- Added glyphs for nine-level tones (in PUA)
- Design changes to some Greek, Cyrillic, ogonek and modifier glyphs,
particularly in italic faces

### 31 Jan 2006 (SIL NRSI team)  Doulos SIL version 4.0.14 (Version 4.014)
- First version released under the SIL Open Font License
