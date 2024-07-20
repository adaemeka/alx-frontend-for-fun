Tasks

0. Start a script
Write a script markdown2html.py that takes an argument 2 strings:

First argument is the name of the Markdown file
Second argument is the output file name
Requirements:

If the number of arguments is less than 2: print in STDERR Usage: ./markdown2html.py README.md README.html and exit 1
If the Markdown file doesn’t exist: print in STDER Missing <filename> and exit 1
Otherwise, print nothing and exit 0

1. Headings
Improve markdown2html.py by parsing Headings Markdown syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown	HTML generated
# Heading level 1	<h1>Heading level 1</h1>
## Heading level 2	<h2>Heading level 1</h2>
### Heading level 3	<h3>Heading level 1</h3>
#### Heading level 4	<h4>Heading level 1</h4>
##### Heading level 5	<h5>Heading level 1</h5>
###### Heading level 6	<h6>Heading level 1</h6>

2. Unordered listing
Improve markdown2html.py by parsing Unordered listing syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown:
- Hello
- Bye

HTML generated:
<ul>
    <li>Hello</li>
    <li>Bye</li>
</ul>

3. Ordered listing
Improve markdown2html.py by parsing Ordered listing syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown:
* Hello
* Bye

HTML generated:
<ol>
    <li>Hello</li>
    <li>Bye</li>
</ol>


4. Simple text
Improve markdown2html.py by parsing paragraph syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown:

Hello
I'm a text
with 2 lines

HTML generated:
<p>
    Hello
</p>
<p>
    I'm a text
        <br />
    with 2 lines
</p>


5. Bold and emphasis text
Improve markdown2html.py by parsing bold syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown	HTML generated
**Hello**	<b>Hello</b>
__Hello__	<em>Hello</em>


6. ... but why??
Improve markdown2html.py by parsing bold syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown	HTML generated	description
[[Hello]]	8b1a9953c4611296a827abf8c47804d7	convert in MD5 (lowercase) the content
((Hello Chicago))	Hello hiago	remove all c (case insensitive) from the content

