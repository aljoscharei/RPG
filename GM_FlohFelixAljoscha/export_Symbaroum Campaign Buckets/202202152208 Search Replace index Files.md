
[[Programmieren MOC]]

```python
import re

import os

from collections import OrderedDict

from xxlimited import new

  

# Define the path and filenames

BASEPATH = r"/Users/aljoschabeyer/Scripting_temp/"

output_path = "/Users/aljoschabeyer/Scripting_temp/output/"

path_of_indexed_files = "/Users/aljoschabeyer/Scripting_temp/spells/"

name_of_index_file = "Wizard Spell File list.txt"

suffix = ".md"

  

new_index_file = ""

  
  

#read in index file

with open(BASEPATH + name_of_index_file) as file:

lines = [line.rstrip() for line in file]

  

# open the indexed_file. Line1 to separate from line in string statement above

for line1 in lines:

print(line1)

with open(path_of_indexed_files + line1 + suffix) as indexed_file:

#read in file as string

text_of_indexed_file = indexed_file.read()

#now search and replace

text_of_indexed_file = text_of_indexed_file.replace("wizard", "[[wizard_spells]]")

text_of_indexed_file = text_of_indexed_file.replace("warlock", "[[warlock_spells]]")

text_of_indexed_file = text_of_indexed_file.replace("sorcerer", "[[sorcerer_spells]]")

text_of_indexed_file = text_of_indexed_file.replace("ranger", "[[ranger_spells]]")

text_of_indexed_file = text_of_indexed_file.replace("paladin", "[[paladin_spells]]")

text_of_indexed_file = text_of_indexed_file.replace("druid", "[[druid_spells]]")

text_of_indexed_file = text_of_indexed_file.replace("cleric", "[[clerid_spells]]")

text_of_indexed_file = text_of_indexed_file.replace("bard", "[[bard_spells]]")

  

text_of_indexed_file = text_of_indexed_file.replace("abjuration", "[[abjuration spells]]")

text_of_indexed_file = text_of_indexed_file.replace("conjuration", "[[conjuration spells]]")

text_of_indexed_file = text_of_indexed_file.replace("divination", "[[divination spells]]")

text_of_indexed_file = text_of_indexed_file.replace("enchantment", "[[enchantment spells]]")

text_of_indexed_file = text_of_indexed_file.replace("evocation", "[[evocation spells]]")

text_of_indexed_file = text_of_indexed_file.replace("illusion", "[[illusion spells]]")

text_of_indexed_file = text_of_indexed_file.replace("necromancy", "[[necromancy spells]]")

text_of_indexed_file = text_of_indexed_file.replace("transmutation", "[[transmutation spells]]")

  
  
  
  
  

# here you can change filename, eg append a w, then you need to update index File

writefile = open(

output_path + line1 + " w" + suffix, "w"

# output_path + line1 + suffix, "w"

)

writefile.write(text_of_indexed_file)

writefile.close()

#append new filename to new index file

new_index_file += "[[" + line1 + " w" + "]]" +"\n"

#write new index file

writefile = open(

output_path + "new_index_file" + suffix, "w"

)

writefile.write(new_index_file)

writefile.close()

pass
```

Problem ist, dass index nicht geordnet ist