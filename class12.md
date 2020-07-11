# Read 12 : EJS Partials

Partials come in handy when you want to reuse the same HTML across multiple views

 <img src="https://scotch-res.cloudinary.com/image/upload/w_auto,q_auto:good,f_auto/media/https://scotch.io/wp-content/uploads/2014/07/nodejs-templating-with-ejs.jpg">

 
* Fisrt of all,You must create Partials.
* Create a file. This file will contain only the HTML for the navigation bar at the top of the home and post pages
* Now that we have our partials defined, we can use them in our home.ejs and post.ejs templates! In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters (you could change these delimiters if you really wanted to).
* Including a partial in EJS is quite straightforward. You use <%- include( PARTIAL_FILE ) %> where the partial file is relative to the template you use it in.
* Note: The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc…

* Creating and including partials is very straightforward with EJS.

