# A-simple-jquery-code-to-search-a-text-inside-of-li-tag
A simple jquery code to search a text inside of li tag


```js

//searchText is a input type text

$('#searchText').bind('keyup', function() {
   
    var searchString = $(this).val();

    $("ul li").each(function(index, value) {
        
        currentName = $(value).text()
        if( currentName.toUpperCase().indexOf(searchString.toUpperCase()) > -1) {
           $(value).show();
        } else {
            $(value).hide();
        }
        
    });
    
});

```
