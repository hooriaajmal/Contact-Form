## Contact Form

A modern, responsive, and accessible contact form built with semantic HTML, CSS, and vanilla JavaScript. It includes client-side validation, inline error messaging, loading states, and a success notification. No external dependencies.

### Features
- **Responsive layout**: Optimized for desktop, tablet, and mobile (breakpoints at 768px and 480px)
- **Client-side validation**: Real-time and on-blur checks with friendly error messages
- **Inline errors and focus**: First invalid field is focused automatically
- **Loading state**: Submit button shows spinner and disables during submission
- **Success feedback**: Dismissible success banner auto-hides after 5 seconds
- **Zero dependencies**: Pure HTML/CSS/JS

![alt text](https://github.com/hooriaajmal/Contact-Form/blob/main/form.png?raw=true)

### Get the code (clone)
- Using HTTPS :

```bash
git clone https://github.com/hooriaajmal/Contact-Form
cd contact
```

- Using SSH:

```bash
git clone git@github.com:hooriaajmal/contact.git
cd contact
```

### Run locally
- Open directly in a browser:

```bash
# Linux
xdg-open Contact-Form.html
# macOS
open Contact-Form.html
# Windows (PowerShell)
start Contact-Form.html
```

- Serve via a local web server (recommended):

```bash
# Python 3
python3 -m http.server 8000
# then visit http://localhost:8000/Contact-Form.html
```

```bash
# Node.js (npx)
npx --yes serve .
# then visit http://localhost:3000 (or the URL shown in the terminal)
```

### Project structure
```text
─ Contact-Form.html
─ README.md
─ form.png
─ form_testing.mp4
```

### How it works
- The form lives in `Contact-Form.html` with embedded CSS and JS
- JavaScript attaches listeners for `input`, `blur`, and `submit`
- Email format is validated via a simple regex; other fields use length checks
- Submission is simulated with a 2s delay, then a success message is shown and form resets

### Validation rules
- **Full Name**: required, at least 2 characters
- **Email**: required, must match basic email pattern `^[^\s@]+@[^\s@]+\.[^\s@]+$`
- **Subject**: required, at least 3 characters
- **Message**: required, at least 10 characters

### Customize
- **Primary color**: `#dc2626` (buttons, borders, accents)
- **Success color**: `#10b981`
- **Typography**: `'Segoe UI', Tahoma, Geneva, Verdana, sans-serif`
- **Form width**: Max width is `470px`; adjust `.form-container { max-width: ... }`
- **Spacing and radii**: Tweak padding and `border-radius` in `.form-container`, inputs, and buttons

### Accessibility notes
- Labels use `for`/`id` to associate with inputs
- Clear focus styles and high-contrast error messaging
- Semantic elements and appropriate `required` attributes

### Browser support
- Works in modern evergreen browsers (Chrome, Firefox, Edge, Safari)
- No external libraries required

### License
Specify a license for your project (e.g., MIT). If unsure, add a `LICENSE` file later. 
