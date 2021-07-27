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
- Bind Param to View:
```php
Route::get('/articles/{id}',function($id){
  return view("article",[
    'article_id'=>$id
    ]);
});

//then on resources/views/article.blade.php
<b> <?= $article_id; ?> </b>
//or
<b>{{ $article_id }}</b>
```
