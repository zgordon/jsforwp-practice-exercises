# Practice Exercises for the JavaScript for WordPress Bootcamp

## Week 1 - JS Basics

1. Create a variable with your name
2. Create a function that logs your name with console.log()
3. Create an object called "me" that includes properties for your first and last names as well as other properties for your website and social media
4. Create a boolean variable called loggedIn (set to either true or false)
5. Write a conditional statement that logs "Logged In" when loggedIn is true and "Please login" when loggedIn is false
6. Create an array called ids filled with numbers that could represent post ids
7. Loop over the ids and log them all out
8. Create an array of post objects.  Include an id, title and content property on each object
9. Loop over the array of posts and log out the title of each one
10. Create a function that will take an array of posts and log out the title and content of each post.

## Week 2 - The DOM and Events

1. Select the following elements from the page and log them to the console: All the links on the page, the element with an id of "main," all elements with a class of "featured,"  the first element with a class of "featured."
2. Select the element with an id of "start-here."  Then select the syblings of the element, the parent of the element, the parent of the parent of the element, and the children of the element and save them as variables.  Then log them all to the console.
3. Set the text for the h2 to "Newsletter Signup," set the value for the name input field to your name, set the value for the email input field to your email.
4. Create the following markup using createElement() and createTextNode() and then append it to the page inside of the element with id of "posts."
```
<article class="post">
  <h2 class="entry-title"><a href="#">Title</a></h2>
  <div class="entry-excerpt">
    <p>Excerpt here...</p>
  </div>
</article>
```
5. Create a clone of the list item and append it to the end of the list.
6. Create an event handler on all links with a class of "special" that prevents the event default and logs the text of the link and the url of the link to the console.
7. Add an event handler to the form that prevents the default event, removes the form from the page and displays a thank you message with the person's name and email.
8. Add a button to the page that adds a new list item with an input field inside it
9. Create a simple lightbox that pops up with a full size image when any image inside of a container with a class of "lightbox" is clicked on.
10. Create a form with an input and textarea that let's you add a post title and content.  Create a live preview of the form that let's you see what the title and content would look like on the page.


## Week 3

1. Create a JSON string of 3 post objects.
2. Create a JSON string of 3 post objects then render them to the page with the following markup
```
<article class="post">
  <h2 class="entry-title"><a href="#">Title</a></h2>
  <div class="entry-excerpt">
    <p>Excerpt here...</p>
  </div>
</article>
```
3. Create a JSON string of 3 post objects and save them in local storage
4. Create a JSON string of 3 post objects and save them in local storage then get them from local storage and render them to the page
5. Create an API call to a working WordPress site and render 3 posts to the page
6. Create an API call to a working WordPress site and get 3 images and render them to the page
7. Create an interface that let's you enter a URL for a WordPress site in a form and when you click submit it displays the latest 10 posts from that site
8. Extend the previous example to make a blog reader that let's you click on a post and read the content of it.  Also display the featured image if one exists.
9. Build a simple de-coupled WordPress site that lists pages and posts and let's you view them without leaving or refreshing the page.
10. Look over this list of [Open APIs](https://github.com/toddmotto/public-apis) and choose one to make an API call to and display information from
