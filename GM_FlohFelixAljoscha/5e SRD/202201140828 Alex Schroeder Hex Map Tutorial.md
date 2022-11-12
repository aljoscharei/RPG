[[202112240523 inkscape]][[202201102142 Hexcrawl MOC]]

[Diary](https://alexschroeder.ch/wiki/Diary) [SiteMap](https://alexschroeder.ch/wiki/SiteMap) [Recent Changes](https://alexschroeder.ch/wiki/Recent_Changes) [About](https://alexschroeder.ch/wiki/About) [Contact](https://alexschroeder.ch/wiki/Contact)

Search:  Filter:   

# [Old School Hex Map Tutorial](https://alexschroeder.ch/wiki?search=%22Old+School+Hex+Map+Tutorial%22 "Click to search for references to this page")

This page explains how to create an old school hex map using [Inkscape](https://alexschroeder.ch/wiki?action=edit;id=Inkscape "Click to edit this page"). This will usually take you longer than a quick sketch that you can scan and post-process quickly. The benefit of this approach is this: As you keep playing in your campaign, you can extend the map piece by piece, adding elements as the players travel.

I think it is essential to _keep your initial map small_. Expand it as your players explore new areas, not for the sake of “completing” a map.

This tutorial was also [crossposted to the Art Tutorials Wiki](http://artwiki.wikidot.com/old-school-hex-maps-using-inkscape) and [crossposted to the Cartographers’ Guild](http://forum.cartographersguild.com/showthread.php?p=28121).

For a different approach, check out [Greg MacKenzie’s approach using icons and colors](http://www.busygamemaster.com/maps03.html). You could use [Text Mapper](https://alexschroeder.ch/wiki/Text_Mapper) to create a map based on Greg’s approach and then edit it using Inkscape.

## Hex

Start with a hex grid. There are several options:

1.  You can use online services like [Incompetech](http://incompetech.com/graphpaper/hexagonal/) to generate a hex PDF.
2.  Use the [Inkscape Hex Map Extension](https://github.com/lifelike/hexmapextension) by Pelle Nilsson. Find your extensions directory and copy both _hexmap.inx_ and _hexmap.py_ into it. I used `/usr/share/inkscape/extensions/`. Then choose Extensions → Boardgames → Generate Hex Map… from the menu. This will create four additinal layers. You can delete the layers Hex Centerdots and Hex Fill by switching to the layers dialog using **Ctrl-Shift-L**, selecting the layer to be deleted, and using the minus button.
3.  You can use the command-line utility [mkhexgrid](https://github.com/kensanata/mkhexgrid) to create your own.

For the particular map I wanted to do, I used the following mkhexgrid specfile:

output=svg
outfile=hex-layer.svg
hex-side=1in
rows=7
columns=6
grid-color=B3B3FF
coord-color=B3B3FF
coord-size=10pt
coord-distance=0.7in
coord-column-start=21
coord-row-start=11

In Inkscape, use **Ctrl-Shift-L** to show you the layer list. Rename Layer 1 to Hex and use **Ctrl-I** to insert the PDF or SVG hex image.

Result:

[![The Hex Layer](https://alexschroeder.ch/pics/2614850185_000f844b1c.jpg?v=0 "The Hex Layer")](https://alexschroeder.ch/pics/2614850185_000f844b1c.jpg?v=0)

If you used the Boardgames extensions, example values would be 6 columns, 7 rows, 1.0 hex size, 10.0 coordinate text size, 75.0 coordinate y offset %, zero-padded coordinates, coordinates every 1 row, 21 first col nr, 11 first row nr, 10% size of corners, force symmetrical hexes.

## Layers

Create a new layer and call it Known Map. Create a third layer and call it Unknown Map. If you want to produce different maps, you can now click on the eye symbol to show or hide that particular layer. And you can move things from one layer to the next using **Shift+PgUp** and **Shift+PgDown**.

As my game is an exploration game, I start with the first seven hexes on the Known Map and about twenty other hexes on the Unknown Map.

In another game I might put all the objects on the Known Map but keep the unknown towns and dungeons on the Labels layer.

As the players discover stuff, I keep moving elements to the Known Map. I usually Export this layer (**Ctrl+Shift+E**) every now and then to share with my players.

## Trees

Use the Create stars and polygons tool (**Shift+F9** or *****) to draw a little polygon with six corners, spoke ratio 0.8, and rounded 0.5. Call up the Fill & Stroke dialog (**Ctrl+Shift+F**) and make sure that there is no filling, black stroke paint, and that the stroke has width 0.677.

Pick Object to Path from the menu (**Ctrl+Shift+C**) and switch to the Edit path by nodes tool (**F2**). You should see 12 nodes in total. Change all the inner nodes to corners. This should change their symbol from a square to a diamond. For each inner node, drag the two handles such that it actuall forms a corner. Also consider dragging the handles of the outer nodes around to create a slightly asymmetric tree.

Now generate a number of trees by using paste & copy and rotating them a 1-3 times by 90°, and mirror them. You should get eight slightly different trees. Whenever I need some forest, I will use a lot of paste and copy. I’ll copy a handful of trees at a time to save time.

Result:

[![Trees](https://alexschroeder.ch/pics/2615697246_eb4915d92d.jpg?v=0 "Trees")](https://alexschroeder.ch/pics/2615697246_eb4915d92d.jpg?v=0)

## Hills

Draw a free-hand (**F6**) hill and simplify it several times (**Ctrl-L**). Call up the Fill & Stroke dialog (**Ctrl+Shift+F**) and make sure that there is no filling, black stroke paint, and that the stroke has width 1.000. Then switch to the Edit path by nodes tool (**F2**) and delete all but four nodes. We want really simple shapes.

Make sure that the nodes within the hill are smooth. Adjust the handles to make a really nice hill. Copy and paste it, make it smaller, reset the stroke width to 1.000. Now you have a big and a small hill. Do some paste and copy and arrange them nicely. Once you’re happy with an arrangement, group them: Shift-click them all and group them (**Ctrl+G**). Whenever I need some hills, I will use a lot of paste and copy. I’ll copy a handful of hills at a time to save time.

[![Hills](https://alexschroeder.ch/pics/2615710808_ac53fa7c89.jpg?v=0 "Hills")](https://alexschroeder.ch/pics/2615710808_ac53fa7c89.jpg?v=0)

## Rivers

Draw a free-hand (**F6**) line and simplify (**Ctrl-L**) if necessary. Call up the Fill & Stroke dialog (**Ctrl+Shift+F**) and make sure that there is no filling, black stroke paint, and that the stroke has width 3.000.

Easy. 🙂

[![River](https://alexschroeder.ch/pics/2614889649_06449da262.jpg?v=0 "River")](https://alexschroeder.ch/pics/2614889649_06449da262.jpg?v=0)

## Labels

Draw a circle (**F5**). If you get an arc insead, switch to the Edit path by nodes tool (**F2**) and Ctrl-drag one circle on top of the other until a circle is formed. If you get an ellipse, Ctrl-drag one of the two squares until you’re happy. Call up the Fill & Stroke dialog (**Ctrl+Shift+F**) and make sure that the circle has a black filling. Resize to taste.

Use the text tool (**F8**) to put a label next to it. Group the dot and the label (**Ctrl-G**) if you want.

Getting easier!

[![Labels](https://alexschroeder.ch/pics/2614905877_ec58a4371a.jpg?v=0 "Labels")](https://alexschroeder.ch/pics/2614905877_ec58a4371a.jpg?v=0)

## Roads

Like rivers, but on the Fill & Stroke dialog (**Ctrl+Shift+F**), pick dashed. Reduce stroke width to one or two.

## Result

This is what you might end up with for the start of an exploration campaign (since this is a Wilderlands of High Fantasy game, the names might ring a bell...).

[![Result](https://alexschroeder.ch/pics/2614914871_1f3af33480.jpg?v=0 "Result")](https://alexschroeder.ch/pics/2614914871_1f3af33480.jpg?v=0)

-   Check out the same map [a year later](https://alexschroeder.ch/wiki/2009-12-02_Hexcrawl)
-   And [two years later](https://alexschroeder.ch/wiki/2011-02-12_Map_Making_Using_Inkscape) I’m still working on the map! 🙂

Tags: [hex](https://alexschroeder.ch/wiki?action=tag;id=hex "Tag") [Maps](https://alexschroeder.ch/wiki?action=tag;id=Maps "Tag")

## Comments

GIMP oldschool hexmap brushes here: [http://inkwellideas.com/?page_id=9](http://inkwellideas.com/?page_id=9)

– [Haarald](http://www.abenteuerpunkt.ch) 2008-12-18 12:33 UTC

---

hey there, I tried this and hexmap chokes on the inches coordinates. any ideas?

– chris 2009-11-08 22:00 UTC

---

The Boardgames extension worked for me. I used the following: 6 columns, 7 rows, 1.0 hex size, 10.0 coordinate text size, 75.0 coordinate y offset %, zero-padded coordinates, coordinates every 1 row, 21 first col nr, 11 first row nr, 10% size of corners, force symmetrical hexes. I got _Latest Experimental Unstable Version 1.4.3_ of the extension and _Inkscape 0.47pre4_ r22446 (Oct 15 2009).

– [AlexSchroeder](https://alexschroeder.ch/wiki/AlexSchroeder) 2009-12-06 23:16 UTC

Add your comment here, send an email to [alex@alexschroeder.ch](mailto:alex@alexschroeder.ch), or contact me on [Octodon Social](https://octodon.social/@kensanata). Feel free to write a blog post and link to it!  

Please make sure you contribute only your own work, or work licensed under the [GNU Free Documentation License](http://www.emacswiki.org/FDL). Note: in order to facilitate peer review and fight vandalism, we will store your IP number for a number of days. See [Privacy Policy](https://alexschroeder.ch/wiki/Privacy_Policy) for more information. See [Info](https://alexschroeder.ch/wiki/Info) for text formatting rules. You can [edit the comment page](https://alexschroeder.ch/wiki?action=edit;id=Comments_on_Old_School_Hex_Map_Tutorial) if you need to **fix typos**. You can [subscribe](https://alexschroeder.ch/wiki?action=subscribe;pages=Comments_on_Old_School_Hex_Map_Tutorial) to **new comments by email** without leaving a comment.

To save this page you must answer this question:

> Just say HELLO

Your name:  Homepage URL:  Email:  [subscribe](https://alexschroeder.ch/wiki?action=subscribe;pages=Old_School_Hex_Map_Tutorial)

---

[Comments on Old School Hex Map Tutorial](https://alexschroeder.ch/wiki/Comments_on_Old_School_Hex_Map_Tutorial) [Edit this page](https://alexschroeder.ch/wiki?action=edit;id=Old_School_Hex_Map_Tutorial "Click to edit this page") [View other revisions](https://alexschroeder.ch/wiki?action=history;id=Old_School_Hex_Map_Tutorial) [Administration](https://alexschroeder.ch/wiki?action=admin;id=Old_School_Hex_Map_Tutorial)

Last edited 2015-07-29 12:38 UTC by [AlexSchroeder](https://alexschroeder.ch/wiki/AlexSchroeder) [(diff)](https://alexschroeder.ch/wiki?action=browse;diff=2;id=Old_School_Hex_Map_Tutorial)

Permission is granted to copy, distribute and/or modify this document under the terms of the [GNU Free Documentation License](https://www.emacswiki.org/FDL), Version 1.3 or any later version published by the [Free Software Foundation](http://www.fsf.org/).

Please note our [Privacy Policy](https://alexschroeder.ch/wiki/Privacy_Policy).