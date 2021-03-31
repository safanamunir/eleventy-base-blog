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

<script>
// var books = [
//   {
//     title: "The Count of Monte Cristo",
//     author: "Alexandre Dumas",
//     alreadyRead: true
//   },
//   {
//     title: "Il Piacere",
//     author: "Gabriele D'Annunzio",
//     alreadyRead: true
//   },
//   {
//     title: "Hard Times",
//     author: "Charles Dickens",
//     alreadyRead: false
//   },
//   {
//     title: "Crime and Punishment",
//     author: "Fyodor Dostoevsky",
//     alreadyRead: false
//   },
//   {
//     title: "The Da Vinci Code",
//     author: "Dan Brown",
//     alreadyRead: true
//   }
// ];
// var recipes =[
//   {
//   title: "Biryani",
//   serving: 2, 
//   ingredients: ["rice", "chicken", "spices"] ,
//   direction: "Boil rice, add chicken and your biryani is ready."
//   },
//   {
//   title: "Qoorma",
//   serving: 5, 
//   ingredients: ["chicken", "spices", "onion"] ,
//   direction: "Boil rice, add chicken and your biryani is ready."
//   },{
//   title: "Qeema",
//   serving: 1, 
//   ingredients: ["qeema", "tomato", "spices"] ,
//   direction: "Boil rice, add chicken and your biryani is ready."
//   },{
//   title: "Pasta",
//   serving: 4, 
//   ingredients: ["pasta", "chicken", "spices"] ,
//   direction: "Boil rice, add chicken and your biryani is ready."
//   },
// ]
//console.log("RECIPES:",recipes);
//for(i = 0; i < recipes.length; i++ ){
  //console.log(recipes[i].ingredients);
//}
//for(counter = 0 ; counter < books.length ; counter ++){
 //var book = books[counter];
  //if (book.alreadyRead) {
    //console.log("You've already read " + book.title + " by " + book.author);
  //} else {
    //console.log("You still need to read " + book.title + " by " + book.author);
  //}
//}
// for(counter = 0 ; counter <= 100; counter ++){
//   let message = '';
//   if(counter % 3 == 0){
//     message += 'fizz'; 
//   }
//   if(counter % 5 == 0){
//       message += 'buzz'; 
//   }
//   if(!message){
//     message = counter;
//   }
//    console.log(message);
// }
// var number = 7;
// for(i = 1; i <= 12; i++)
// {
//   result = number * i;
//   console.log('7 x ' + i + ' = ' + result);
// }
</script>