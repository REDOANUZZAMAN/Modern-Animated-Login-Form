# 🔐 Modern Animated Login Form

A stunning, futuristic login form with rotating neon borders, dynamic background effects, and smooth animations. Built with pure HTML and CSS - no JavaScript framework required.

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=flat&logo=css3&logoColor=white)
![Status](https://img.shields.io/badge/status-active-success.svg)

## ✨ Features

- **Rotating Neon Border** - Animated conic gradient in pink and cyan colors
- **Hover Expansion** - Form elegantly expands from compact box to full size
- **Dynamic Background** - Floating color blobs with animated grid overlay
- **Glassmorphism Design** - Modern translucent UI elements
- **Glowing Effects** - Icons and buttons with neon glow on hover
- **Smooth Animations** - CSS transitions and keyframe animations
- **Responsive Layout** - Clean, centered design
- **Single File** - Everything in one HTML file

## 🎬 Demo

The login form features:
- Compact initial state (400x200px)
- Expands on hover to reveal full form (450x500px)
- Dual-layer rotating neon borders (pink + cyan)
- Dark cyberpunk background with animated elements
- Glowing submit button
- Interactive links for "Forgot Password" and "Sign up"

## 🚀 Quick Start

1. **Clone the repository**
```bash
git clone https://github.com/redoanuzzaman/modern-login-form.git
cd modern-login-form
```

2. **Open the file**
```bash
# Simply open in your browser
open index.html
# or double-click the file
```

No build tools, no dependencies - just open and use!

## 📁 File Structure

```
modern-login-form/
├── index.html         # Complete login form
└── README.md         # Documentation
```

## 🎨 Customization

### Change Border Colors

Edit the conic gradient colors:

```css
/* Pink border */
.box {
  background: repeating-conic-gradient(
    from var(--a),
    #ff2770 0%,    /* Change this color */
    #ff2770 5%,
    transparent 5%,
    transparent 40%,
    #ff2770 50%
  );
}

/* Cyan border */
.box::before {
  background: repeating-conic-gradient(
    from var(--a),
    #45f3ff 0%,    /* Change this color */
    ...
  );
}
```

### Adjust Animation Speed

Modify the rotation speed:

```css
@keyframes rotating {
  0% { --a: 0deg; }
  100% { --a: 360deg; }
}

.box {
  animation: rotating 4s linear infinite; /* Change duration */
}
```

### Customize Background

Change blob colors and positions:

```css
body::before {
  background: 
    radial-gradient(circle at 30% 20%, rgba(255, 39, 112, 0.5) 0%, transparent 25%),
    radial-gradient(circle at 70% 80%, rgba(69, 243, 255, 0.5) 0%, transparent 25%),
    /* Add more gradients or modify colors */
}
```

### Adjust Hover Size

Change expanded dimensions:

```css
.box:hover {
  width: 450px;   /* Modify width */
  height: 500px;  /* Modify height */
}
```

## 🛠️ Technologies Used

- **HTML5** - Semantic structure
- **CSS3** - Advanced animations and effects
- **@property** - CSS Houdini for animatable custom properties
- **Font Awesome 6.5.1** - Icons
- **Google Fonts (Poppins)** - Typography

## 🌐 Browser Support

| Browser | Support |
|---------|---------|
| Chrome  | ✅ Full |
| Firefox | ✅ Full |
| Safari  | ✅ Full |
| Edge    | ✅ Full |
| Opera   | ✅ Full |

**Note:** `@property` CSS feature requires modern browsers (2020+)

## 💡 Integration Tips

### Add Form Functionality

Wrap inputs in a form tag and add JavaScript:

```html
<form id="loginForm">
  <input type="text" name="username" required>
  <input type="password" name="password" required>
  <input type="submit" value="Sign in">
</form>

<script>
document.getElementById('loginForm').addEventListener('submit', function(e) {
  e.preventDefault();
  // Add your login logic here
});
</script>
```

### Connect to Backend

Use fetch API to send credentials:

```javascript
fetch('/api/login', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ username, password })
})
.then(response => response.json())
.then(data => console.log(data));
```

## 🎯 Use Cases

- Landing pages
- Web applications
- Dashboard login
- Admin panels
- SaaS products
- Portfolio projects
- Learning CSS animations

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 💡 Future Enhancements

- [ ] Add form validation
- [ ] Social media login buttons
- [ ] Remember me checkbox
- [ ] Password strength indicator
- [ ] Multi-step authentication
- [ ] Dark/light theme toggle
- [ ] Mobile-optimized version
- [ ] Accessibility improvements (ARIA labels)

## 👨‍💻 Author

**Redoanuzzaman**
- GitHub: [@redoanuzzaman](https://github.com/redoanuzzaman)
- Email: redoanuzzaman707@gmail.com
- Website: [redoan.dev](https://redoan.dev)

## 🙏 Acknowledgments

- Font Awesome for beautiful icons
- Google Fonts for Poppins typeface
- CSS Houdini for making custom property animations possible
- The web design community for inspiration

## 💖 Show your support

Give a ⭐️ if you like this project!

---

Made with 💙 and CSS by Redoanuzzaman
