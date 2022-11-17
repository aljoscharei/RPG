[[Programmieren MOC]]
[[Python MOC]]

- alle monster statblocks yaml kopieren und erneut als dataview frontmatter in Text.
- dscryb herunterladen mit selenium
	- https://www.scrapingbee.com/blog/selenium-python/
	- https://medium.com/@igorzabukovec/automate-web-crawling-with-selenium-python-part-1-85113660de96
	- [[Selenium A.pdf]]
	- [[Selenium B.pdf]]
	- [[Selenium 3.pdf]]
	- [[scrapingbee Web Scraping using Selenium and Python.pdf]]
	- Der zentrale Text in dscryp
 ```html
	<div class="page-content-text">
				                <div>
										<p>The crooked, gnarled broom ends in a wild cluster of twigs, bundled with loops of rough-spun twine. The haft is smooth and polished, not from craftsmanship, but from wear and use. Despite its mundane appearance, as you lift it, it seems to do so on its own momentarily, levitating almost.</p>

                </div>
				                </div>
	```

- Linklisten elemente haben eigenschaft: in diesen indexseiten gibt es keinen coretext
```html
<h3 class="elementor-post__title">
			<a href="https://dscryb.com/scene/skyship-brig/">
				Skyship Brig			</a>
		</h3>
```

- lego sorting machine:
	- [[Lego Sorter Python Tensorflow.pdf]]
- google keep api: https://developers.google.com/keep/api/reference/rest
- generall Cool. https://www.youtube.com/c/NeuralNine/videos
- youtube mp3 downloader: ![[youtube-downloader-converter-master.zip]]
- Google Keep to obsidian? https://developers.google.com/keep/api/reference/rest
	- https://gkeepapi.readthedocs.io/en/latest/
- PDFs:
	- extract:  https://www.youtube.com/watch?v=w2r2Bg42UPY
	-  merge https://www.youtube.com/watch?v=4gZgWXJpX-w
	- split: https://www.youtube.com/watch?v=Pe4UVIX7f-U 
	- password cracken pycrunch, pikepdf john the ripper
		- https://www.thepythoncode.com/article/crack-pdf-file-password-in-python
		- https://www.openwall.com/john/
		- https://github.com/x4nth055/ethical-hacking-tools-python/blob/main/chapter-3/cracking/pdf-cracker/pdf_cracker.py
	- ocr teseract google library
	- how to crack pdfs or azw3 files
- mit Obsidian interagieren:
	- https://github.com/mfarragher/obsidiantools
	- https://publish.obsidian.md/hub/04+-+Guides%2C+Workflows%2C+%26+Courses/for+Plugin+Developers
- [x] move linked files to folder
	- [[pynative.com-Move Files Or Directories in Python.pdf]]
	- https://www.youtube.com/watch?v=ve2pmm5JqmI
	- https://docs.python.org/3/library/shutil.html#module-shutil
	- [[batch rename python]]
- einarbeiten in API von Google Sheets
	- Haushaltsbuch: https://docs.google.com/spreadsheets/d/14jJq3pVrD8sLzJvGGwMSvjZmIFQkYOdePaXYHmWnMfc/edit#gid=2034836649
		- so automatisieren, dass man nachdem CSV eingelesen und getaggt ist, die erste seite automatisch geneiert wird
	- https://developers.google.com/sheets/api/quickstart/python 
	- https://console.cloud.google.com/iam-admin/serviceaccounts/details/116719771246576233917/keys?project=vivid-tuner-363411&supportedpurview=project
	- mit dieser Emailadresse müssen documente geteilt werden, damit du darauf zugreifen kannst.
		- aljoscha@vivid-tuner-363411.iam.gserviceaccount.com
	- das ist die key-datei für haushaltsbuch [[vivid-tuner-363411-68a1feaf49a6.json]]	
		- habe ich nach scripts kopiert
	- https://developers.google.com/sheets/api/quickstart/python
	- https://erikrood.com/Posts/py_gsheets.html
	- https://github.com/burnash/gspread
	- https://www.youtube.com/watch?v=bu5wXjz2KvU open with media extended
- Anki verstehen
- Web Scraping
	- https://www.youtube.com/watch?v=SPM1tm2ZdK4
	-  
- in Javascript einarbeiten um die plugins von Jeremy valentine zu verstehen.



[[Python Statblock]]

5 min python projects. jeden tag kurz
Video gucken, dann anwenden:
Funktionen
web scraping





202109090555 Programming Projects

- Aim: text Manipulation such as: use file name as headline,
- [[202109111730 sed awk.md]]
- Use Regular expressions to find links re package regex
	- Find note containing link text, find file name of that note
	- Insert new filename in link
Find the directory of text files
os module

Use flask or django as gui for simple projects electron is sth similar for javascript

- [ ] understand the Regex here

'''
https://stackoverflow.com/questions/63197371/detecting-all-links-in-markdown-files-in-python-and-replace-them-with-outputs-of
[[Library]] of Stuff to find markdown links
[[https://stackoverflow.com/questions/63197371/detecting-all-links-in-markdown-files-in-python-and-replace-them-with-outputs-of]]

def find_md_links(md):
    """Returns dict of links in markdown:
    'regular': [[201410251305.363 Neuropathie et al. - Unknown - Das diabetische Fußsyndrom Diabetic foot syndrome.md]]
    'footnotes': [foo][3]
    
    [3]: some.url
    """
    # https://stackoverflow.com/a/30738268/2755116

    INLINE_LINK_RE = re.compile(r'\[([^\]]+)\]\(([^)]+)\)')
    FOOTNOTE_LINK_TEXT_RE = re.compile(r'\[([^\]]+)\]\[(\d+)\]')
    FOOTNOTE_LINK_URL_RE = re.compile(r'\[(\d+)\]:\s+(\S+)')

    links = list(INLINE_LINK_RE.findall(md))
    footnote_links = dict(FOOTNOTE_LINK_TEXT_RE.findall(md))
    footnote_urls = dict(FOOTNOTE_LINK_URL_RE.findall(md))

    footnotes_linking = []
        
    for key in footnote_links.keys():
        footnotes_linking.append((footnote_links[key], footnote_urls[footnote_links[key]]))

    return {'regular': links, 'footnotes': footnotes_linking}


def replace_md_links(md, f):
    """Replace links url to f(url)"""
      links = find_md_links(md)
      newmd = md

    for r in links['regular']:
        newmd = newmd.replace(r[1], f(r[1]))

    for r in links['footnotes']:
        newmd = newmd.replace(r[1], f(r[1]))
    
    return newmd

def mychange(s, prefix="/static/entrades/", suffix=".md.html"):
    """Change links from tiddlywiki syntax [[201410251305.363 Neuropathie et al. - Unknown - Das diabetische Fußsyndrom Diabetic foot syndrome.md]] to [[201410251305.363 Neuropathie et al. - Unknown - Das diabetische Fußsyndrom Diabetic foot syndrome.md]]"""
    
    if s.startswith('#'):
        return prefix + slugify.slugify(urllib.parse.unquote( s.replace('#', '', 1) )) + suffix
    else:
        return s
'''

Backlinks
[[202109090554 Journal KW36.md]]