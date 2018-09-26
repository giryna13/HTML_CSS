*The Pros And Cons Of Using Em*

When working on a responsive project it’s more flexible to use relative units like em for sizing text and 
spacing in and around elements rather than pixels. This is because this unit is relative to the font size of its parent element, 
allowing an element’s size, spacing and text content to grow proportionally as the font-size of parent elements change.
Using these relative units enables you to build a system of proportions where changing values of 
font-size on one element has a cascading effect on the child elements within. A system of proportions is a good thing, 
but this behavior of em does come with a downside.

Take the following snippet of HTML:

<ul>
  <li>lorem ipsum</li>
  <li>dolor sit 
    <ol>
      <li>lorem ipsum</li>
      <li>lorem ipsum</li>
      <li>lorem ipsum</li>
      <li>lorem ipsum</li>
    </ol>
  </li>
</ul>

This nested list isn’t the most common thing in the world but could likely appear in a page of terms and conditions or 
some other kind of formal document.

If we wanted to make the list items stand out, we could set their font-size to be 1.5 times the size of the base size of 16px.

li {
    font-size: 1.5em; /* 24px/16px */
}

But this will cause an issue with the nested li as they will be 1.5 times the size of their parent too. 
The nested items will be 1.5 times 24px rather than 1.5 times 16px. The result is that any nested list items 
will grow exponentially with each level of nesting. This is likely not what the designer intended!

A similar problem occurs with nested elements and em values of less than 1. In this case, any nested items 
would keep getting incrementally smaller with each level of nesting. What can we do instead?
