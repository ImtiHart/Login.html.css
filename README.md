# Post Submission Form (HTML/CSS + PHP)

A minimal web form that accepts a post title and content, submits it via HTTP POST,
and displays the submitted data back to the user. Includes both the frontend form
and a PHP handler with output escaping.

## 🎯 What It Demonstrates

- **HTML form handling** — labeled inputs, `required` attributes, POST method.
- **CSS layout** — centered card using flexbox, box-shadow, hover states on the button.
- **PHP request handling** — reads `$_POST`, checks the request method, and validates
  input server-side.
- **Output escaping (XSS prevention)** — all user input is passed through
  `htmlspecialchars(..., ENT_QUOTES, 'UTF-8')` before being written to HTML.

## 🗂️ Files

| File              | Purpose                                          |
|-------------------|--------------------------------------------------|
| `post-form.html`  | The submission form (renamed from `test.html`)   |
| `submit_post.php` | Receives the POST and displays the result safely |
| `style.css`       | Card layout and form styling                     |

## 🚀 How to Run

Requires PHP 7.4+.

```bash
# from the project folder
php -S localhost:8000
# open http://localhost:8000/post-form.html
