# HTML Introduction
## Hypertext Markup Language
HTML provides foundational content structuture

## Elements and tags
HTML `elements` are represented with enclosing `tags` that may enclose other elements of text. 
* `p` -> paragraph element
* tags refer to a delimited textual name that we can use to designate the start and end of an HTML element
* tags are delmited with `<` and `>` symbols. closing tag also has a `/` before its name

'html` element represents top level page structure
`head` elment contains metadata bout the page and the page title
`body` represents the content structure
`main` represents main conent structure as opposed to things like headers, fotters, asides, navigation

'''
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <main>
      <p>Hello world</p>
    </main>
  </body>
</html>
'''

HTML is almost completely about structure. visual appearance of web page won't change until we start styling with CSS

# Attributes
every HTML element may have attributes
* describes specific details of element
* `id` gives unique ID to element
* `class` designates lement as being classified in a name group of lements
* are writeen inside the elment tag with a name followed by optional value

`<p id="hello" class="greeting">Hello world</p>`

## Hyperlinks
represented with anchor (`a`) element that has attribute containg adress of hyperlink ref (`href`)
`<a href="https://byu.edu">Go to the Y</a>`

## Complete example
HTML defines a header (`<!DOCTYPE html>`) that tells the browser the type and version of the document. You should always include this at the top of the HTML file. 

```
<!DOCTYPE html>
<html lang="en">
  <body>
    <main>
      <h1>Hello world</h1>
      <p class="introduction">
        HTML welcomes you to the amazing world of
        <span class="topic">web programming</span>.
      </p>
      <p class="question">What will this mean to you?</p>
      <p class="assignment">Learn more <a href="instruction.html">here</a>.</p>
    </main>
  </body>
</html>
```

HTML provides content and structure
Layout is left up to CSS (cascading stylesheets)

## Common elements
| element   | meaning                                                                |
| --------- | ---------------------------------------------------------------------- |
| `html`    | The page container                                                     |
| `head`    | Header information                                                     |
| `title`   | Title of the page                                                      |
| `meta`    | Metadata for the page such as character set or viewport settings       |
| `script`  | JavaScript reference. Either a external reference, or inline           |
| `include` | External content reference                                             |
| `body`    | The entire content body of the page                                    |
| `header`  | Header of the main content                                             |
| `footer`  | Footer of the main content                                             |
| `nav`     | Navigational inputs                                                    |
| `main`    | Main content of the page                                               |
| `section` | A section of the main content                                          |
| `aside`   | Aside content from the main content                                    |
| `div`     | A block division of content                                            |
| `span`    | An inline span of content                                              |
| `h<1-9>`  | Text heading. From h1, the highest level, down to h9, the lowest level |
| `p`       | A paragraph of text                                                    |
| `b`       | Bring attention                                                        |
| `table`   | Table                                                                  |
| `tr`      | Table row                                                              |
| `th`      | Table header                                                           |
| `td`      | Table data                                                             |
| `ol,ul`   | Ordered or unordered list                                              |
| `li`      | List item                                                              |
| `a`       | Anchor the text to a hyperlink                                         |
| `img`     | Graphical image reference                                              |
| `dialog`  | Interactive component such as a confirmation                           |
| `form`    | A collection of user input                                             |
| `input`   | User input field                                                       |
| `audio`   | Audio content                                                          |
| `video`   | Video content                                                          |
| `svg`     | Scalable vector graphic content                                        |
| `iframe`  | Inline frame of another HTML page                                      |

## Comments 
`<!-- commented text -->`

## HTML versions
 HTML is pretty stable, but it is still good to check a website like MDN or canIUse to make sure.

## index.html
by default a web server will display HTML file named `index.html` when browser makes request without asking for a specific HTML

## Rendering HTML
open file in browser, VS code with Live Server ext, CoePen sandbox


