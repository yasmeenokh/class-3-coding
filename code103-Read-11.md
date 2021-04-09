# Intro to EJS
**EJS** simply stands for Embedded Javascript. It is a simple templating language/engine that lets its user generate HTML with plain javascript.

- EJS is mostly useful whenever you have to output HTML with a lot of javascript.
- EJS is compatible with Express for back-end use as it hooks into the View engine architecture that Express provides and lets you render web pages to the client with res.render() in Express.

### Features
1. Complies with the Express view system
2. Unbuffered code for conditionals etc <% code %>
3. Escapes html by default with <%= code %>
4. Unescaped buffering with <%- code %>
5. Supports tag customization
6. Filter support for designer-friendly templates

- Get Started
to install it
        $ npm install ejs

        npm install --save express body-parser cors ejs

#### Tags
1. <% 'Scriptlet' tag, for control-flow, no output.
2. <%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it.
3. <%= Outputs the value into the template (HTML escaped).
4. <%- Outputs the unescaped value into the template.
5. <%# Comment tag, no execution, no output.
6. <%% Outputs a literal '<%'.
7. %> Plain ending tag.
8. -%> Trim-mode ('newline slurp') tag, trims following newline.
9. _%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it.

#### Includes
Includes are relative to the template with the include call. (This requires the 'filename' option.) For example if you have "./views/users.ejs" and "./views/user/show.ejs" you would use <%- include('user/show'); %>.

You'll likely want to use the raw output tag (<%-) with your include to avoid double-escaping the HTML output.

#### EJS Partials 
Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file and include it wherever you need it.

### Express EJS Layouts
Layout is some formatting that we insert into a separate file and specify, where we should insert body( <%-body -%>). In any other template we can indicate this. For example, in template/index.ejs. 

    $ npm install express-ejs-layouts

