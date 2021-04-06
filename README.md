# My HTML things

## [W3 HTML Validator](https://validator.w3.org/)

## [Headings and paragraphs](./titles-and-paragraphs/index.html) 
Headings tags are not only  to control the size of the text, they also have their own meaning. We shouldn't write `h2` headings without writting `h1` heading before and so on.

## [Header Main and Footer](./header-main-footer/index.html)
It's important to structure the HTML code with this 3 tags, 
- `header` must contain navigation menus, logos, social media links...
- `footer` should contain usefull information, contact links, FAQs, creator name, the small print of the contracts... 
- `main` has all the relevant content of the page.

## [Section Article and Aside](./section-article-aside/index.html)
Content section labels, section can contain articles and articles can contain sections
- `section`: generic container used to group related content. When we are creating blocks wich content is related to an upper block we will use sections.
- `article`: container that represents independent content, i.e. when we can read that fragment elsewhere and it would make sense on its own. 
- `aside`: used to display content that is related but not part of the main content. It can be placed inside or outside the main tag.

Nesting: section can contain articles, i.e. if we have some articles about HTML tags, they should be placed inside one section, due to they have related content, and articles would be independent because we could read one whitout reading the others and it would still have its own sense. Article is defined as component of the page with independent content, this tag could have a header and a footer.

## [Block and Line elements](./block-and-line-elements/index.html)
Block elements will occupy the full available width even if their content does not, so the elements below will go to the following line. Line elements will take only the width they need, so it's possible to display more than one element in the same line.
Each element has semantic value strong > em > normal > small. With these labels we can set the relevance of each part of the text.
- Line elements:
    - `em`: emphas
    - `strong`: more emphasis
    - `small`: less emphasis
    - `br`: line break
    - `wbr`: We can select where the line breaks when needed. Same as '-' 
    - `time`: dates and times
    - `i`: italic (only style tag, no semantic value). Also icon tag
    - `u`: underline (only style tag, no semantic value) 
    - `b`: bold (only style tag, no semantic value) 
    - `sup`: adds supper indexes 
    - `sub`: adds sub indexes

## [Attribute](./tag-atributes/index.html)
Aditional values to modify the HTML tags or it's behaviour
- Common: `attribute="value"`
- Boolean: `attribute`

## [Global attributes](./tag-atributes/index.html)
These attributes can be used in almost every HTML tag:
- `class`: to add a CSS class
- `id`: to add identifiers
- `title`: accesibility tag to show element descriptions
- `data-*` : allows to save values in the HTML tag

## [Links](links/index.html)
Links are very important, they allow us to navigate through the web or to other webs. It has one mandatory attribute `href` with the route, it also has the `target` attribute to modify how the resource will be displayed:
- `href`: absolute paths (with http:// or https://) for external webs: https://www.google.com, relative paths for internal pages
- `target`: with absolute paths for external webs `_blank`
- `download`: download the file in the path, the file must be in our server. Best practices are to save the files under assets/files, images, icons ...
We can navigate in the page to tags with id by using, `href=#id-name`, this can be used to navigate to specific points in other pages like /other/other.html#someid

## [Lists](lists/index.html)
Used to list content, there are 3 types of lists:
- `ul`: unordered list: Order does not matters (used to create menus). It can has list type,to style the item marks (type="value"):
    - disc (default value)
    - circle
    - square
- `ol`: ordered list: Order does matter. It can has list type,to style the item marks (type="value"), it also has the start="value" attribute to star on a default value:
    - 1: (1, 2, 3 ...) (default value)
    - A: (A, B, C ...)
    - a: (a, b, c ...)
    - I: (I, II, III ...)
    - i: (i, ii, iii ...)
- `dl`: definition list: List of definitions (dictionary)
Browsers differentiate between the type of site.
Elements of the list are represented by `li` tag `ul` and `ol` lists.
For `dt`: list each element is represented with 2 tags:
    - `dt`: definition term: term to define
    - `dd`: definition description: term description

## [Tables](tables/index.html)
Tables are used to display tabbed content, this is the basic structure of one table:
- `table`: represents the table
- `tr`: table row
- `td`: table data, one cell
The number of cells inside a row sets the number of columns of the table.
The title of the table can be setted with the optional `caption` tag.
We can set the header of the table with the `thead` tag and the `th` tag for each header. When we set a `thead` tag, we must place all the table content inside the `tbody` tag. Tables can also have a footer `tfoot`.
We can modify the space of each cell, we have the following attributes:
- `rowspan` the cell will take more than one row. (default value 1). It will take the space of the next rows. Common error
- `colspan` the cell will take more than one col. (default value 1)
We can group cols with the `colgroup` tag.

## [Block Tags](block-tags/index.html)
More block tags:
- `address`: adds contact information to the nearest artible or the body
- `blockquote`: used to mark citations to other authors or documents. It can has the attribute `cite=""` to reference the source of the content
- `pre`: used to maintain the format of the text (tabs, end of lines ..) i.e. to print some formated code.
- `div`: used to split the document, no semantic meaning, generic container normally used for styling from css
- `hr`: horizontal rule, the browser understands that there is a change of subject. Don't use it to draw lines