---
layout: layouts/post.njk
title: Psuedocode
templateClass: tmpl-post
eleventyNavigation:
  key: Psuedocode
  order: 3
---


<code>
LOOP through numbers 0 - 100 <br>
    IF number is a multiple of 3 and 5 <br>
    THEN output 'fizzbuzz' <br>
    IF ELSE number is a multiple of 3 <br>
    THEN output 'fizz'<br>
    IF ELSE number is a multiple of 5<br>
    THEN output 'buzz'<br>
    ELSE <br>
    THEN output number<br>
FUNCTION readingList <br>
  CREATE an ARRAY of objects <br>
    include bookTitle(string), author(string), alreadyRead(boolean) <br>
  LOOP through each object in the array<br>
  THEN output 'book title' and 'book author'<br>
    IF already read <br>
    THEN output 'You already read'<br>
    ELSE<br>
    THEN output 'You still need to read'<br>
FUNCTION recipeList<br>
CREATE an ARRAY of objects <br>
    include recipeTitle(string), servings(number), ingredients(array), directions(string) <br>
    PRINT recipes<br>
    LOOP through ARRAY <br>
    THEN output 'all ingredients' <br>
</code>

