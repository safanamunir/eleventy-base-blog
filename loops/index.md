---
layout: layouts/post.njk
title: Loops
templateClass: tmpl-post
eleventyNavigation:
  key: Loops
  order: 3
---
<script>
    var shoppingCart=[
        {name:"loaf of bread",type:"food",quantity:1,price:.85},{name:"multipack beans",type:"food",quantity:1,price:1},{name:"mushrooms",type:"food",quantity:10,price:.1},{name:"can of beer",type:"alcohol",quantity:4,price:1.1},{name:"prosecco",type:"alcohol",quantity:1,price:8.99},{name:"steak",type:"food",quantity:2,price:3.99},{name:"blue cheese",type:"food",quantity:1,price:2.99},{name:"candles",type:"home",quantity:3,price:1.99},{name:"cheesecake",type:"food",quantity:1,price:4.99},{name:"onions",type:"food",quantity:3,price:.4}
        ];

    //CREATE FUNCTION take arg shoppingCart
    function getTotalPrice(shoppingCart, discountAmount, type){
    //CREATE VAR totalPrice
    var totalPrice = 0;
    //LOOP items in shoppingCart
    for(var item of shoppingCart){
    //IF item.type === food
    if(item.type === type || type === 'any'){
        //SUB 20% from item.price
        var discountPrice = item.price - ((item.price * discountAmount) / 100);
       // console.log(discountPrice);
        //ADD discountPrice to totalPrice
        totalPrice += discountPrice * item.quantity; 
    }
    else{
         //ADD price to VAR totalPrice
    //Times by quantity
   totalPrice += item.price * item.quantity;
    }
   
    }
    //return VAR totalPrice
    return totalPrice;
    };
    console.log(getTotalPrice(shoppingCart, 30, 'any'));

    function lowHighPrice(cart, lowPrice, highPrice, quantity){
       var arrItems = [];
       var price = 0; 

       for(var item of cart){
           quantity ? price = item.price * item.quantity : price = item.price; //if else statement (if quantity = true then price = item.price * item.quantity else price = item.price ) 

        if(item.price >= lowPrice && item.price <= highPrice){
            arrItems.push(item);
           }
        }
               return arrItems;
       }
    
    console.log(lowHighPrice(shoppingCart, 0.2, 1, true));

 var numberArray = [3,6,1,68,23,15,3,9,56,10];
 function mean(numberArray){
     var totalSum = 0;
     for(var i = 0; i < numberArray.length ; i++) {
    totalSum += numberArray[i];
    //console.log(totalSum);
 }
     return totalSum / numberArray.length;

 }
console.log(mean(numberArray));

function median(numberArray){
    var sortedNumber = numberArray.sort(function(a,b){return a - b});
    var value = sortedNumber[sortedNumber.length/2 | 0];
    return value;
}
console.log(median(numberArray));

function mode (numberArray) {
  var modes , count = [], i, number, maxIndex = 0;

    for (i = 0; i < numberArray.length; i += 1) {
        number = numberArray[i];
        count[number] = (count[number] || 0) + 1;
        if (count[number] > maxIndex) {
            maxIndex = count[number];
        }
    }

    for (i in count)
        if (count.hasOwnProperty(i)) {
            if (count[i] === maxIndex) {
                modes = Number(i);
            }
        }

    return modes;
    }
console.log(mode(numberArray));

 function getNumberType(numberArray, type){
     switch (type){
        case 'mean':
             return mean(numberArray);  
            break;
        case 'median':
            return median(numberArray);
            break;
        case 'mode':
            return mode(numberArray);
            break;

        default:
            return numberArray;
     }
 }
 console.log(getNumberType(numberArray, 'mode'));
    </script>
    