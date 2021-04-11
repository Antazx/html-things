# My HTML things

## Web tools
- [Webp converter](https://www.online-convert.com/es/resultado#j=25134d36-5170-40a4-8bbc-a6c41a14f889)
- [W3 HTML Validator](https://validator.w3.org/)
- [What is my viewport](https://whatismyviewport.com/)
- [Markdown previewer & syntax](https://markdownlivepreview.com/)
- [Special entities: ASCII codes](https://ascii.cl/es/codigos-html.htm)

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

## [Line Tags](line-tags/index.html)
More line tags:
- `span`: line container, equals div, is used to enclose words or small texts and style them through CSS or localise them from JS, it has no semantic meaning.
- `q`: equivalent to blockquote, means quoute. To put quotations in line.
- `code`: to enclose code that we want to represent visually, it usually goes with the pre tag. It has semantic meaning.
- [Special entities: ASCII codes](https://ascii.cl/es/codigos-html.htm)

## [Forms](forms/index.html)
Basic form structure:
- `form`: wraps the form
    - `action=""`: where to send the data (server, other html ..)
    - `method=""`: method to execute GET/POST
- `label`: sets the field label
    - `for="fieldID"`: matches the label to the field
- `input`: field to allow users to enter data
    - `name`: **mandatory** 
- `button`: allow users perform an acction

**The default behaviour of forms reloads the current page**
Related form tags
- `fieldset`: used to group elements inside the form
- `legend`: label for the fieldset content
- `meter`: represents a value within a range
- `progress`: progress of a task
- `textarea`: multiline text input

Most frequent field attributes:
- `placeholder`: 
- `required`: mandatory field
- `readonly`: readonly field
- `min - max`: for number input
- `maxlenght - minlenght`: for text input
- `selected`: to set a default value
- `disabled`: disabled field
- `autofocus`: sets the focus on the field

## [Input types](forms/input-types.html)
- `button`: same as `<button></button>` but it doesn't reloads the page. Doesn't send the data.
- `color`: choose a color
- `date`: enter a date
- `datetime`: **Deprecated**
- `datetime-local`: date and time, doesn't works on firefox
- `email`: enter email
- `hidden`: hidden field, could have a value but it isn't shown
- `month`: enter a month
- `week`: enter a week number
- `number`: numeric values
- `password`: passwords ***
- `range`: set a range
    -`step="10"`: how much the bar moves
    -`min="0"`: min value
    -`max="30"`: max value
- `reset`: reset the forms
- `search`: search bars
- `submit`: sends the form
- `tel`: phone numbers
- `text`: **default value** plain texts
- `time`: hours
- `url`: URLs
- `file`: files

## [Selectable input types](forms/selectable-input-types.html)
- `radio`: select only one option
    - `name="category"`: sets the category to which the radio belongs and allows only one value per category
    - `value=""`: what is the value of the element 
    - `checked`: radio checked by default
- `checkbox`: select multiple options
    - Needs name and value as radio inputs
- `select`: select from a list
    - `name="category"`: sets the category
    - `multiple`: allow to select more than one option
    - `<option>`: each option goes in  tags, if there are lots of options, we can group them in `<optgroup>` and set a `label` atribute for each group. If has `selected` attribute, it's selected by default
- `list`: filter with the text in the related datalist `list="datalistID"` it also shows the value attribute of the tag, each element of the list is one `option` tag

## Embedded content
All the content that we retrive from outside our web. Usually these are the heaviest files on the web page (images, videos ..)
- Pictures: There are two images types:
    - Vectorial SVG (very ligth) icons logos .. 
    - Bit map: jpg, png (8/24), gif, webp (recommended)
- Audio
- Video
- Iframes
Usually placed on /assets

## [Images](embedded content/assets/index.html)
Inserted with `<img>` tag
- `src=""`: route to the image
- `alt=""`: description of the image
We can isert SVG images with the image tag or with the svg content on the html. The second option is only if we need to access the svg properties (i.e. to animate it from js)

## Device pixel ration DPR
Relation between the real amount of pixels of the devide and the available pixels to "draw" content
DPR = real pixels / avaliable pixels
On mobile devices, its usually 2.4 - 3
- Viewport: available space to draw (1920 x 1080) [What is my viewport](https://whatismyviewport.com/)
We shouldn't use the same image for mobile devices and for desktop, it's a big file that is not necessary on mobile devices. We can use one image or other depending on the device. We can do this with the `srcset` attribute, doesn't work on IE so we can also add `src` attribute.

When using the tags `<picture> - <source>` to display images, if the paths provided for the img tag is invalid the browser won't render any image. It works like a js switch, we set the sources for each case and its default fallback images, and the default picture is on img tag. 
 
## [Audio](embedded content/audio.html)
The audio tag allows to insert audio content on the web, it has:
- `src=""`: with the path to the audio file
- `controls`: to dysplay controls of the song
- `autoplay`: starts the audio on page load. If the content isn't muted the browser will stop autoplay
- `loop`: auto-replay

## [Video](embedded content/video.html)
The video tag allows to insert video content on the web, it has:
- `src=""`: with the path to the video file
- `controls`: to dysplay controls of the song
- `autoplay`: starts the video on page load. If the content isn't muted the browser will stop autoplay
- `loop`: auto-replay
- `poster`: sets the preview image

## [Iframes](embedded content/video.html)
We can insert pieces of web from other pages (twitter, instagram ...), the madatory attributes are:
- `width` and `heigth`
- `src`: uri to the content
**Performance is affected** 

## [Video](embedded content/figure.html)
The `figure` tag is used to add related content to the page but when it's opcional content
Used to break the flow of content with other content that is related but not necessary to understand the article.
The code snippets should be in a figure tag, data with kpi, tables... It can be accompanied by the `figcaption` tag to put details about the content both above and below the figure.