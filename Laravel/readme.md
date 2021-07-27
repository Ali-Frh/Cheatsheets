# Laravel

## Routes:
GET:
- Simple:
```php
Route::get('/articles',function(){
  return "Articles List" ;
});
```
- with Parameter:
```php
Route::get('/articles/{id}',function($id){
  return "Article #".$id;
});
```

  
