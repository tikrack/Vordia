<div align="center">
    <a href="https://github.com/Rayiumir/Vordia" target="_blank">
        <img src="./art/Vordia.png" alt="Vordia Logo">
    </a>
</div>
<br>
<div align="center">
    <img alt="Packagist Downloads" src="https://img.shields.io/packagist/dd/rayiumir/vordia">
    <img alt="Packagist Downloads" src="https://img.shields.io/packagist/dm/rayiumir/vordia">
    <img alt="Packagist Downloads" src="https://img.shields.io/packagist/dt/rayiumir/vordia">
    <img alt="Packagist License" src="https://img.shields.io/packagist/l/rayiumir/vordia">
    <img alt="GitHub Release" src="https://img.shields.io/github/v/release/rayiumir/vordia">
    <img alt="Packagist Dependency Version" src="https://img.shields.io/packagist/dependency-v/rayiumir/vordia/PHP">
</div>

# Vordia

A simple and lightweight mobile authentication package for Laravel And it has a default admin panel.

# How to use

Install Package :

```bash
composer require rayiumir/vordia
```

After Publish Config Files:

```bash
php artisan vendor:publish --provider="Rayiumir\\Vordia\\ServiceProvider\\VordiaServiceProvider"
```

And Migration Database:

```bash
php artisan migrate
```

Add Fields in Model user.php :

```php
protected $fillable = [
        'name',
        'email',
        'password',
        'mobile',
        'otp',
        'login_token'
    ];
```
# List of SMS Operator

<table>
    <thead>
        <tr>
            <th>SMS Operator</th>
            <th>Link</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>SMSIR</td>
            <td><a href="https://sms.ir">https://sms.ir/</a></td>
        </tr>
    </tbody>
</table>

# SMS API KEY

Add this code to `.env`

```bash
SMS_DRIVER=smsir
SMSIR_API_KEY= Add API KEY
SMSIR_OTP_TEMPLATE_ID= ADD OTP TEMPLATE ID
```

# Screenshots

<table class="table">
  <thead>
    <tr>
      <th scope="col" width="1000px">Login Mobile</th>
      <th scope="col" width="1000px">Check OTP Login Mobile</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <img src="./screenshots/login.png" width="100%" alt="Login Mobile">
      </td>
      <td>
        <img src="./screenshots/checkOTP.png" width="100%" alt="Check OTP Login Mobile">
      </td>
    </tr>
  </tbody>
</table>
