If you're using a Github wiki and are intending to use it with MkDocs you'll want to use [Commonmark](http://commonmark.org/help/) markdown. The reason for this is MkDocs has python parsers that handle markdown flavours differently and it will choke on certain aspects of github flavoured markdown which end up rendering the final HTML pages less than favourably. Commonmark will still render as intended in Github.

The following are some notes on proper syntax.

### Headings

The headings (defined by `#`) should follow a natural progression of the hierarchy of the page contents. You cannot have two title headings otherwise they won't show up on the table of contents on the right side of the page

E.G.
```
# Title
## Main heading one
### Sub Heading one
### Sub heading two
## Main heading two
```
etc.

### Links

Links should follow this syntax

```
[Link](path to link)
```
If it is a link to another wiki page it should be a relative path:
```
[Installation](Installation)
```
NOT
```
[Installation](https://github.com/username/repo/wiki/Installation)
```

### Code Blocks

Code blocks should be created with backticks: 1 set for inline code highlighting and 3 for code blocks

Inline code highlights:

`` `inline` ``

will render as:
`inline` 

Code blocks:


` ``` `

`code block`

` ``` ` 


will render as 
```
code block
```



### Bullets

If you are doing subnests on bullet points you need 4 spaces on the sub bullet, not two more explanation [HERE](https://pythonhosted.org/Markdown/#differences):

```
- Bullet one
    - Bullet sub
````
It should render like this:

- Bullet one
    - Bullet sub

### Numbering

Numbers will only order properly if in a listed sequence. If that sequence is broken by paragraphs then the numbering will restart.

Numbered lists are formatted as follows:
```
1. item 1
2. item 2
3. item 3
4. item 4
```
If they are not in a listed sequence then you can just label the numbers manually with:
```
Step 1.
Step 2.
Step 3.
```
etc. or you can just use bullet points if the numbers really aren't that important.

### Symbols/Emojis

Emojis are not supported with python markdown and should be avoided. Rather important text should be bolded or italicised

The following in github:
```
:exclamation:
```
renders to :exclamation:

but in the generated docs it will show
```
:exclamation:
```


This is a comment:

[I CAN WRITE WHATEVER I WANT HERE!]: #