# Friendship Day Jewellery Sale

This email template announces a Friendship Day Jewelry Sale for the retail jewelry industry, using marketing techniques to attract customers.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Retail, Jewelry
- **Message Type:** Marketing
- **Tags:** sale, discount, jewelry, friendshipday

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/friendship-day-jewellery-sale.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/friendship-day-jewellery-sale/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.friendship-day-jewellery-sale',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
