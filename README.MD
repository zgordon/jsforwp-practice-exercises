# Practice Exercises for the JavaScript for WordPress Bootcamp

**Bold exercise** - Denotes a fundamental exercise one should be able to complete.

## Week 1 - JS Basics

1. Create a variable with your name
2. Create a function that logs your name with console.log()
3. Create an object called "me" that includes properties for your first and last names as well as other properties for your website and social media
4. Create a boolean variable called loggedIn (set to either true or false)
5. Write a conditional statement that logs "Logged In" when loggedIn is true and "Please login" when loggedIn is false
6. Create an array called ids filled with numbers that could represent post ids
7. Loop over the ids and log them all out
8. **Create an array of post objects.  Include an id, title and content property on each object**
9. **Loop over the array of posts and log out the title of each one**
10. **Create a function that will take an array of posts and log out the title and content of each post.**

## Week 2 - The DOM and Events

1. Select the following elements from the page and log them to the console: All the links on the page, the element with an id of "main," all elements with a class of "featured," the first element with a class of "featured."
2. Select the element with an id of "start-here." Then select the syblings of the element, the parent of the element, the parent of the parent of the element, and the children of the element and save them as variables. Then log them all to the console.
3. Set the text for the h2 to "Newsletter Signup," set the value for the name input field to your name, set the value for the email input field to your email.
4. **Create the following markup using createElement() and createTextNode() and then append it to the page inside of the element with id of "posts."**
```html
<article class="post">
  <h2 class="entry-title"><a href="#">Title</a></h2>
  <div class="entry-excerpt">
    <p>Excerpt here...</p>
  </div>
</article>
```
5. Create a clone of the list item and append it to the end of the list.
6. **Create an event handler on all links with a class of "special" that prevents the event default and logs the text of the link and the url of the link to the console.**
7. Add an event handler to the form that prevents the default event, removes the form from the page and displays a thank you message with the person's name and email.
8. Add a button to the page that adds a new list item with an input field inside it
9. Create a simple lightbox that pops up with a full size image when any image inside of a container with a class of "lightbox" is clicked on.
10. Create a form with an input and textarea that let's you add a post title and content. Create a live preview of the form that let's you see what the title and content would look like on the page.

## Week 3

1. Create a JSON string of 3 post objects.
2. **Create a JSON string of 3 post objects then render them to the page with the following markup**
```html
<article class="post">
  <h2 class="entry-title"><a href="#">Title</a></h2>
  <div class="entry-excerpt">
    <p>Excerpt here...</p>
  </div>
</article>
```
3. Create a JSON string of 3 post objects and save them in local storage
4. **Create a JSON string of 3 post objects and save them in local storage then get them from local storage and render them to the page**
5. Create an API call to a working WordPress site and render 3 posts to the page
6. Create an API call to a working WordPress site and get 3 images and render them to the page
7. Create an interface that let's you enter a URL for a WordPress site in a form and when you click submit it displays the latest 10 posts from that site
8. Extend the previous example to make a blog reader that let's you click on a post and read the content of it. Also display the featured image if one exists.
9. Build a simple de-coupled WordPress site that lists pages and posts and let's you view them without leaving or refreshing the page.
10. Look over this list of [Open APIs](https://github.com/toddmotto/public-apis) and choose one to make an API call to and display information from

## Week 4

1. Write a two helper functions getLocalStore() and updateLocalStore() that can take an array or object, stringify it and save to local storage as well as pull content out of local storage and parse it.
2. Write a helper function that renders posts to the page using the following markup:
```html
<article class="post">
  <h2 class="entry-title"><a href="#slug">Title</a></h2>
  <div class="entry-content">
    <p>Content here...</p>
  </div>
</article>
```
3. Write an init() function that gets posts from JSON and saves them to local store.  Then it should get content from local store and render to the page.  Use the functions created in #1 and #2.
4. **Create a JSON string of 3 page objects that include an id, slug, title and content. Grab the collection of pages from JSON and create a function that returns an unordered list of the pages.**
5. Modify the list of pages to include a slug like the following that logs out the link when it is clicked
```html
<li><a href="#1">Post #1</a></li>
<li><a href="#2">Post #2</a></li>
```
6. When you click on the link in the navigation list from #5, find the corresponding post from the list of posts from the JSON list and log it to the screen.
7. Modify the navigation menu so that when you click on a link the entire post is displayed.

## Week 6

1. Create variables with `var` `let` and `const` and test their scope and ability to be re-assigned or changed.
2. Create an object using const and make it immutable with freeze.
3. Convert the following function to an arrow function.
```js
function getPost(postIndex) {
  return posts[postIndex];
}
```
4. Simplify the arrow function from exercise #3 as much as possible.
5. Use `.filter` to find all posts with a title longer that 10 characters.
6. Use `.map()` to iterate over all the posts and log their title.
7. Use a template literal (template string) to use multiple variables inside a string.
8. Loop through 3 JSON posts and render them to the page (like Week 3 exercise 4) but using `.map()`
9. Add event listeners to posts to exercise #8 and on click render the full post (with a back button). Use `this` in event handler instead of event.target


## Week 7 - Enqueuing JavaScript & Admin AJAX

1. Create a WordPress theme that loads JavaScript on the frontend
2. Make the theme from exercise #1 dependent on jQuery and load your JavaScript using the jQuery no conflict wrapper.
3. Add another JavaScript file to your theme from exercise #3.  Make it dependent on your first JS file, but also makes sure it only conditionally loads on one page (of your choice).
4. Modify your theme so that on the single page where your JS loads it pulls in three posts from the REST API and loads them to the page in the following format:
```
<h2><a href="${slug}>${title}</a></h2>
<p>{excerpt}<p>
```
5. Create a WordPress plugin that loads a JavaScript file on the frontend.
6. Add the ability for your plugin from exercise #4 to load a different JavaScript file just in the admin area.
7. Create a settings page for your plugin and conditionally load your admin JavaScript file only on that page.
8. Use `wp_localize_script` to load the name of the site and the path to the REST API route (https://site.com/wp-json) into your JavaScript.
9. Create an interface with JavaScript that let's you edit a setting in WP Options using AJAX on your plugin settings page.

## Week 8 - REST API
1. Setup a WordPress site and visit the REST API Root in the browser?
2. Make a fetch request to the  WordPress REST API Root and `console.log()` the site `name` and `description`
3. Make a fetch request to get the posts and `console.log()` them out
4. Get a specific post based on the post id and `console.log()` the post titles and excerpts
5. Get 3 posts and `console.log()` the post titles
6. Get 3 posts in alphabetic order by title and `console.log()` the post titles
7. Make a request to get all the users.  Then another request to get the latest 3 posts for each user.  Build a simple user page with the author name then their posts listed below.
8. Rebuild #7 using async and await.
9. Build a custom endpoint that gives only the id, title, slug, and excerpt for posts.
10. Create a custom endpoint that let's you get and save data to the WP Options table.

## Week 9 - React
1. Create a paragraph with createElement() with a class of special and content of "Hello React". [in repo]
2. Repeat #1 using JSX
3. Setup a React App using Create React App (README.md with instructions?)
4. Create a component named Header that has an h1 and a site description in it
5. Modify #3 so the title and description are based on props
6. Create a counter example based on state (example in repo) 
7. Have state save to local storage
8. Make an API request to a WordPress site in a componentDidMount and render the posts to the page
9. Create a page in WordPress called "API Posts" and have #8 display the posts in the main content area
10. Create a WordPress plugin with a settings page.  Have #8 display on the settings page.

BONUS - Some more [React practice examples](https://fabiankaegy.github.io/react-exercises/) from Fabian
