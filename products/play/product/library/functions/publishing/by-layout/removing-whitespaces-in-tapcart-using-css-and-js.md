## Removing Whitespaces in Tapcart Using CSS and JS

Implement CSS and JS methods by adding the following:

Add the following code as a new line in CSS:

```css
html, body { height: 150px !important; }
```

If the CSS method doesn't work, remove the CSS code above and try the JS code (also a new line):

```javascript
setTimeout(() => { document.documentElement.style.setProperty('height', `150px`, 'important'); }, 500);
```
