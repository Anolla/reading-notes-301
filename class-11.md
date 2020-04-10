# EJS (Embedded JavaScript templating)

- To install it use this command : $ npm install ejs.

- To use it , we use render method with it to pass a template string and some data for example: 
  let ejs = require('ejs'),
    people = ['geddy', 'neil', 'alex'],
    html = ejs.render('<%= people.join(", "); %>', {people: people});.

- render method takes three parameters , the first one is a string of the file name you want to pass, the second one is an object of local variables , the third one is a callback function. It is important to note that res.render() will look in a views folder for the view. So we only have to define pages/index since the full path is views/pages/index.

### EJS tags :

- <% 'Scriptlet' tag, for control-flow, no output
- <%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
- <%= Outputs the value into the template (HTML escaped)
- <%- Outputs the unescaped value into the template
- <%# Comment tag, no execution, no output
- <%% Outputs a literal '<%'
- %> Plain ending tag
- -%> Trim-mode ('newline slurp') tag, trims following newline
- _%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it