## Test task for a Laravel Livewire developer position

## Context

There is a form for entering card data and processing it. It is outdated and requires improvement, since the service has learned to process not only card payments, but also other types of payments.

## Task

1. Modify the form so that you can choose a payment method based on the methods available to the merchant:
    - Bank Card
    - Qiwi
    - Yoomoney
    
    Implement data entry, masking and validation for each form.

2. Add an additional request for data before making the payment itself, but after entering the data. You can additionally request either E-mail or Phone.

## Start Project

For a start project, you need run these commands:

- `composer install`
- `npm run dev`
- `php artisan serve`

For `torann/currency` package you need to open `php artisan tinker` console and run this code:

``` 
currency()->create([
    'name' => 'U.S. Dollar',
    'code' => 'USD',
    'symbol' => '$',
    'format' => '$1,0.00',
    'exchange_rate' => 1.00000000,
    'active' => 1,
]);
```

By the way, for this task you don't need a DB