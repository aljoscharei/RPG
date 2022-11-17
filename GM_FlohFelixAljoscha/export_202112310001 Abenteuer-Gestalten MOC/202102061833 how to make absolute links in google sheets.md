# how to make absolute links in google sheets
 [[emacs]] [[how-to]] [[excel]] [[Computer]] [[202202111122 Bestiary MOC]] 
---



tabs in google Sheets sind definiert als gid
\=HYPERLINK(CONCAT("#gid=0range=",Stats!B2),Stats!C2)
das problem ist dass der gelbe und lila teil interpretiert werden und es nicht
also string bauen mit emacs:
formelzeile kopieren.
dann 1000 mal yanken/einfügen. Das geht nicht direkt sondern mit makro machen und 1000 mal ausführen.
zeilenumbruch mitmarkieren, dann killen mit cmd x
dann
C-x ( C-y C-u 100 C-x ).

dann rectangle killen c-x r k
dann u U mit text ersetzen bearbeiten C2 C ersetzen mit $C$
dann C-M-%  regexp replace

M-x delete-trailing-whitespace
Very easily, fortunately.

Use C-M-% (which runs the command query-replace-regexp), use the regexp (regular expression) $ (this matches exactly at the end of line) and replace it with your text. And that's it!
Another possibility involves Magnars Sveen's excellent multiple-cursors.el : select lines, use M-x mc/edit-lines then hit C-e (end-of-line) and start typing. Really magic.
damit kann man kommas klammern etc einsetzen.

[LinkName.txt](./resources/202102061833_how_to_make_absolute_links_in_google_sheets.resources/LinkName.txt)
[LinkJumpHere.txt](./resources/202102061833_how_to_make_absolute_links_in_google_sheets.resources/LinkJumpHere.txt)
[SheetMonsterLink.txt](./resources/202102061833_how_to_make_absolute_links_in_google_sheets.resources/SheetMonsterLink.txt)

---

_Created at 20210206._
_Last updated at 20210224._



