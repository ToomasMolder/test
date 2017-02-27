# My Test Document

## Table of Contents

[License](#license)  
[1 Paragraph A](#1-paragraph-a)  
[2 Paragraph B](#2-paragraph-b)  
[The End](#the-end)  

## Test Area

To be tested within Github and also with pandoc PDF

	>pandoc.exe --version
	pandoc.exe 1.19.2.1
	Compiled with pandoc-types 1.17.0.4, texmath 0.9, skylighting 0.1.1.4
	Default user data directory: <localdir>
	Copyright (C) 2006-2016 John MacFarlane
	Web:  http://pandoc.org
	This is free software; see the source for copying conditions.
	There is no warranty, not even for merchantability or fitness

Command 

	pandoc.exe -s test.md  -f markdown_github -t latex+auto_identifiers -o test.pdf

- Header 1. Paragraph A in form of `<div id = "1-paragraph-a" class = "anchor"></div>\n## 1. Paragraph A` (having prefix div id and prenumbered)
- Header 2. Paragraph B in form of `## 2. Paragraph B` (prenumbered)
- Header The End in form of `## The End` (no prenumbering)

Do these internal links/anchors work for [test.pdf](test.pdf)?

- Link \[[License (#license)](#license)\] Github: OK Pandoc: OK

- Link \[[1. Paragraph A (#paragraph-a)](#paragraph-a)\]  Github: NOK Pandoc: OK
- Link \[[1. Paragraph A (#-paragraph-a)](#-paragraph-a)\]  Github: NOK Pandoc: NOK
- Link \[[1. Paragraph A (#1-paragraph-a)](#1-paragraph-a)\]  Github: OK Pandoc: NOK

- Link \[[2. Paragraph B (#paragraph-b)](#paragraph-b)\] Github: NOK Pandoc: OK
- Link \[[2. Paragraph B (#-paragraph-b)](#-paragraph-b)\]  Github: NOK Pandoc: NOK
- Link \[[2. Paragraph B (#2-paragraph-b)](#2-paragraph-b)\]  Github: OK Pandoc: NOK

- Link \[[The End (##the-end)](#the-end)\]  Github: OK Pandoc: OK


## License

This work is licensed under the Creative Commons Attribution-ShareAlike 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/3.0/.

<div id="1-paragraph-a" class="anchor"></div>
## 1. Paragraph A

This is paragraph A

**The standard Lorem Ipsum passage, used since the 1500s**

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## 2. Paragraph B

**Section 1.10.33 of "de Finibus Bonorum et Malorum", written by Cicero in 45 BC**

At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio. Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere possimus, omnis voluptas assumenda est, omnis dolor repellendus. Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet ut et voluptates repudiandae sint et molestiae non recusandae. Itaque earum rerum hic tenetur a sapiente delectus, ut aut reiciendis voluptatibus maiores alias consequatur aut perferendis doloribus asperiores repellat.

**1914 translation by H. Rackham**

On the other hand, we denounce with righteous indignation and dislike men who are so beguiled and demoralized by the charms of pleasure of the moment, so blinded by desire, that they cannot foresee the pain and trouble that are bound to ensue; and equal blame belongs to those who fail in their duty through weakness of will, which is the same as saying through shrinking from toil and pain. These cases are perfectly simple and easy to distinguish. In a free hour, when our power of choice is untrammelled and when nothing prevents our being able to do what we like best, every pleasure is to be welcomed and every pain avoided. But in certain circumstances and owing to the claims of duty or the obligations of business it will frequently occur that pleasures have to be repudiated and annoyances accepted. The wise man therefore always holds in these matters to this principle of selection: he rejects pleasures to secure other greater pleasures, or else he endures pains to avoid worse pains.

## The End

End of story

End of story

End of story

End of story

End of story
