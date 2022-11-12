[[Python Statblock]]

re module
- match object methods
	- Match.group(0): returns the whole match
	- Match.group(1): returns the match of the first group
	- kann auch geschrieben werden als Match[0]
	- die eckigen klammern rufen die methode __getitem__ auf
- Regular Expressions können benannt werden mit
	- ```(?P<name>Regex)```
	- das macht vipin ajayakumar in seinem Script

Similar to regular parentheses, but the substring matched by the group is accessible via the symbolic group name _name_

- dicts
	- dict.keys() get list of the keys
	- dict.values() get a list of the values
	- dict.items() get a list containing a tuple for each key value pair
	- dict.get(key) get the value for the key
	- dict.update({1:'changed'}) besser dict[key] = value
- Wie kann ich den absoluten Pfad einer datei finden wenn ich deren Namen zwar weiß aber nicht, wo sie sich im Dateisystem befindet.
FileLocation = glob.glob(PathToParentFolderEndingWithSlash + '**/' + 'Filename.txt', recursive=TRUE)
[[Python Glob Filename Pattern Matching.pdf]]