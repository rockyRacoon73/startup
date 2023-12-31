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

## Special characters

HTML uses several reserved characters for defining its file format. If you want to use those characters in your content then you need to escape them using the `entity` syntax. For example, to display a less than symbol (`<`) you would instead use the less than entity (`&lt;`). You can also use the entity syntax to represent any unicode character.

| Character | Entity      |
| --------- | ----------- |
| &amp;     | `&amp;`     |
| <         | `&lt;`      |
| >         | `&gt;`      |
| "         | `&quot;`    |
| '         | `&apos;`    |
| &#128512; | `&#128512;` |

## HTML versions
 HTML is pretty stable, but it is still good to check a website like MDN or canIUse to make sure.

## index.html
by default a web server will display HTML file named `index.html` when browser makes request without asking for a specific HTML

## Rendering HTML
open file in browser, VS code with Live Server ext, CoePen sandbox


# HTML input elements

| Element    | Meaning                          | Example                                        |
| ---------- | -------------------------------- | ---------------------------------------------- |
| `form`     | Input container and submission   | `<form action="form.html" method="post">`      |
| `fieldset` | Labeled input grouping           | `<fieldset> ... </fieldset>`                   |
| `input`    | Multiple types of user input     | `<input type="" />`                            |
| `select`   | Selection dropdown               | `<select><option>1</option></select>`          |
| `optgroup` | Grouped selection dropdown       | `<optgroup><option>1</option></optgroup>`      |
| `option`   | Selection option                 | `<option selected>option2</option>`            |
| `textarea` | Multiline text input             | `<textarea></textarea>`                        |
| `label`    | Individual input label           | `<label for="range">Range: </label>`           |
| `output`   | Output of input                  | `<output for="range">0</output>`               |
| `meter`    | Display value with a known range | `<meter min="0" max="100" value="50"></meter>` |


## Form element
hte main purpose of `form` element is to submit values of inputs it contains

(form element is often simply used as a container, but it is not required to use input element)

```
<form action="submission.html" method="post">
  <label for="ta">TextArea: </label>
  <textarea id="ta" name="ta-id">
Some text
  </textarea>
  <button type="submit">Submit</button>
</form>
```

browser generates data by combining textarea's `name` with current value of textarea
-> `ta-id=Some+text`

## Input element
input element represents many dif types of inputs
you can set `type` attribute

| Type           | Meaning                           |
| -------------- | --------------------------------- |
| text           | Single line textual value         |
| password       | Obscured password                 |
| email          | Email address                     |
| tel            | Telephone number                  |
| url            | URL address                       |
| number         | Numerical value                   |
| checkbox       | Inclusive selection               |
| radio          | Exclusive selection               |
| range          | Range limited number              |
| date           | Year, month, day                  |
| datetime-local | Date and time                     |
| month          | Year, month                       |
| week           | Week of year                      |
| color          | Color                             |
| file           | Local file                        |
| submit         | button to trigger form submission |

in order to create an input you specify the desired type along with any other att assiciated with the specific input

`<label for="checkbox1">Check me</label> <input type="checkbox" name="varCheckbox" value="checkbox1" checked />`

| Attribute |	Meaning |
| --------- | -------------------|
| name	| The name of the input. This is submitted as the name of the|
| input if | used in a form |
| disabled | Disables the ability for the user to interact with the input |
| value | The initial value of the input |
| required | Signifies that a value is required in order to be valid |

![image](https://github.com/rockyRacoon73/startup/assets/90075184/3676f6f5-37a7-4a27-8e31-0189ccfaea25)

## Validating input
several input elements have validation built into them
(such as url number, email)
* you can also specify the `required` att on an input element to mark it to requiring a vaule before being submitted

* `pattern` att exists on  exists on text, search, url, tel, email, and password inputs. provides reg exp

* you should have validation built into JavaScript that checks input data to ensure everything is valid before it is submitted
* use CSS for visualizing validity of input
* give good user feed back as, before the user begins to input

# HTML media elements
The `img`, `audio`, and `video` elements are all simple references to an external file, but `svg` and `canvas` both contain the code to render a visual image that can even be animated.

## external media
media tags that ref ext media all take a URL as an att
full or relative path
Full path: protocol, domain name, and path to file
`https://images.pexels.com/photos/164170/pexels-photo-164170.jpeg`
relative path: references a file served from same location of HTML page rendering the element

`images/photo.jpg`

## image 
`<img alt="mountain landscape" src="https://images.pexels.com/photos/164170/pexels-photo-164170.jpeg" />`

## audio
to include an audio file in your content use `audio` element and specify `src` att with url to audio
* can add `controls` att to let user control playback (no controls no vis rep of audio )
* `autoplay` plays audio as soon as audio file is loaded
* `loop` att keeps it playing over and over
* `<audio controls src="testAudio.mp3"></audio>`
* (strongly discouraged automatically playing audio unless give user a way to opt-in)

## video
`video` element specify `src` att with URL to source video
can include `controls` and `autoplay` att

(may need to include `crossorigin="anonymous"` att if you are requesting files from a diff domain that the one serving your content)

```
<video controls width="300" crossorigin="anonymous">
  <source src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4" />
</video>
```

## internal media
`svg` and `canvas` create images within HTML

### scalable vector graphics (SVG)
combined with JavaScript and CSS can produce some amazing visualizations
ex:
```
<svg viewBox="0 0 300 200" xmlns="http://www.w3.org/2000/svg" stroke="red" fill="red" style="border: 1px solid #000000">
  <circle cx="150" cy="100" r="50" />
</svg>
```

### canvas
`canvas` element is fairly simple but drawing on canvas requires javascript support

<canvas id="canvasDemo" width="300" height="200" style="border: 1px solid #000000"></canvas>
<script>
  const ctx = document.getElementById('canvasDemo').getContext('2d');
  ctx.beginPath();
  ctx.arc(150, 100, 50, 0, 2 * Math.PI);
  ctx.fillStyle = 'red';
  ctx.strokeStyle = 'red';
  ctx.fill();
  ctx.stroke();
</script>


# Deploy to production
Use the deployFiles.sh script found in the example code to deploy Simon to your production environment. Take some time to understand how the script works. The script does three things. Deletes any previous deployment for simon, copies up all of the files found in the project directory, and makes sure Caddy is hosting the files under the simon subdomain of your domain (e.g. simon.yourdomain.click).

`./deployFiles.sh -k <yourpemkey> -h <yourdomain> -s simon`
For example,

`./deployFiles.sh -k ~/keys/production.pem -h yourdomain.click -s simon`
⚠ Make sure you run deployFiles.sh from the console in your project directory.




