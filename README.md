# SelectChildFromParentElement
Select Child from any element jQuery 

```JS

/**
* Define: This function can able to select any active child and do something on it
* for instance slider when any of the slide child has been clicked then can do something on it!
* 
* Or any div have child unpredictable to be selected but was selected the can do something!
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
    
    // Then if true any of child has class "red" remove the class red
    {  $( "li" ).removeClass('red'); } 

    // Then next after this child was fresh clicked must be add class name "red"
    let currentVal = $( this );

       // addClass red
       currentVal.addClass('red');
    
  });         
});


```
