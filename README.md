# Laravel Sanctum Rest api basic

<br>
<a href="https://www.youtube.com/watch?v=GAB_BqFZNOA" target="_blank">Video From</a> <br>
<a href="https://techtoolindia.com/how-to-use-laravel-sanctum-for-api-authentication" target="_blank">Article</a> <br>


## Steps

<p>
    php artisan make:controller Api\\AuthController
<br>

    In routes\api.php file update the API
</p>


<p>

    Route::post('/auth/register', [AuthController::class, 'store']);
    Route::post('/auth/login', [AuthController::class, 'login']);   
</p>

 Protected Route

 <p>

    Route::post('/auth/register', [AuthController::class, 'store']);
    Route::post('/auth/login', [AuthController::class, 'login']);   
</p>

<p>

Route::post('/posts', [TheNameoffController::class, 'login'])->middleware('auth:sanctum');


</p>
