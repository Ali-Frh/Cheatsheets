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

## Views:
- MasterPage:
```php
//in file: resources/view/layouts/master.blade.php
<head>
  <h4>This is Fucking Header</h4>
</head>
<body>
  @yield("content")
</body>
<footer>
  <h4> Fucking Footer </h4>


//in file: resources/view/aboutus.blade.php
@extends('layouts.master')

@section('content')
  <h4> This is the Content </h4>
@endsection
```
## Blade Commands:
- @if - @endif

- Sections:
```php
//in masterpage (layout.master)
<title>@yield("title")</title>

//for example in about file:
@section("title","about us") //one linear

@section("title")
About Us
@endsection

//or even
@section("title")
About Us
@show

If You Use third one, it can be Replicable Later.
```

- @include("penis") //Absolute Path Only

## Database
- DB::Table("sometable")->get();

