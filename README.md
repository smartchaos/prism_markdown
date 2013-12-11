prism_markdown
==============

It is a extension for python markdown parser and it can be used to hightlight code by prism.js directly.

I fork the code of fenced_code extension and alter it to meet the prism's need.
Now you can hightlight your code this way:
### Put the prism_code.py file to markdown extensions folder
Maybe `'your python folder'/Lib\site-packages\markdown\extensions`

### Write your code in markdown. better use \`\`\` notion
f.e. 
```
\`\`\`python  
\#Just print "hello world"  
print "hello world"  
\`\`\`
```
### Transfer the markdown file to html
`html = markdown.markdown(md, ['prism_code'])`  
the generated html maybe:
```html
<pre><code class="language-python">
#Just print "hello world"
print "hello world"
</code></pre>
```
Wonderfull!
### Import the prism.css file and prism.js(choose to include python) to your page
Now in the page that contains the python code can be beautifully hightlighted!

