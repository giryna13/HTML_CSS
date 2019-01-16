# Useful Links:
1. html5boilerplate.com - default version of HTML5 page
2. caniuse.com - supported/not supported features on different browsers
3. modernizr.com - feature detection
4. html5please.com

# Pseudo-classes:
1. :lang - is used to select an element based on its content language.

## :lang pseudo-class
The content of HTML documents can be in many different languages. To specify the primary language of a document, we use the lang attribute on the root element

`<html lang="en>`

We can also use the lang attribute within the page to demarcate specific elements or sections that are in a different language to the document’s primary language.

![screen shot 2019-01-16 at 3 22 26 pm](https://user-images.githubusercontent.com/17466723/51251719-9a8f7500-19a2-11e9-8bf3-cd63bd7eb19c.png)

If we wanted to style these sections of the page differently, we could use the [lang] attribute selector to select all elements, or children of elements, with the specific language attribute.
