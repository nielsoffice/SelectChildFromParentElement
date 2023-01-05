# SelectChildFromParentElement
Select Child from any element jQuery cooked by nielsoffice

```JS

/**
 * Cooked by nielsoffice
 * Define: This function can able to select any active child and do something on it
 * for instance slider when any of the slide child has been clicked then can do something on it!
 * 
 * Or any div have child unpredictable to be selected but was selected then can do something on it!
 * and remove last dom effect from recent child was clicked.
 * 
 */
$(() => {
            
  // Select the parent element  
  let findSpan = $('#parentElem');

  // Any of the child of parent has clicked!
  findSpan.find( "li" ).on('click', function () {
               
    // *Before anything else this must be implemented once I clicked any of child!
    // find the child element who has "class" named "red"
    if( findSpan.find( "li" ).hasClass('red') == true ) 
    
    // Then if true any of child has class "red" remove the class red or remove last effects like animation for this because this is recent
    {  $( "li" ).removeClass('red'); } 

    // Then next after this child was fresh clicked must be add class name "red" // or run the animation for this child has been clicked
    let currentVal = $( this );

       // addClass red or in otherhand do something on it
       currentVal.addClass('red');
    
  });         
});


```

```JS

// jQuery Defining function 
// invoke function by itself
jQuery(() => {

  const performSlides = jQuery.fn.sliderDynamicPost = function() {  // do something };

  setInterval(performSlides, 1000);

});

 // Ready function 
 jQuery(function() {  // do something });
 
 // inner function
 jQuery.fn.sliderDynamicPost = function() { // do something };
 
 // invoking for inner or simply function set function itself
 jQuery(this).sliderDynamicPost();

 // ex.
 jQuery(function() {  
    
    // inner function
    jQuery.fn.sliderDynamicPost = function() { // do something };
 
    // invoking for inner or simply function set function itself
    jQuery(this).sliderDynamicPost();

  }

```
