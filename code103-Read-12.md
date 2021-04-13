# EJS Partials
Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file and include it wherever you need it.

**NOTE**
- EJS Partials help us avoid repetition of the same code on several web pages.

- EJS partials work like EJS layouts too in creating a single fix content on a web page.

- The <% %> tags allow you to output the unescaped content onto the page (mind the -). It is important when using the include() statement since you won’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc.

- creating and including partials is very straightforward with EJS, you just have to create the partial files for HTML pieces that you want to reuse, and then just include them in other pages using the syntax. 

- perfect candidates for partials are headers and footers because they remain the same from page to another: 

#### creating partials :
1. inside the “views/partials/ folder
2. create a “navbar.ejs”
3. only contain the HTML for the nav bar on each page
5. create the same thing for the footer
6. now that they are created we can use them in our other .ejs files

7.      <%-include(PARTIAL_FILE) %> 
put this where you want the included content to be.

8. don't forget the  (-) .