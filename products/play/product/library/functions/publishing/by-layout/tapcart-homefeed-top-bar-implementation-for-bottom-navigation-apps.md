## Code for Homefeed Top Bar Implementation for Apps Using Bottom Navigation

### HTML Code

```html
<tolstoy-block
    data-publish-id=""**PROJECT_PUBLISH_ID**""
    data-block-type=""video-page""
    data-nav-type=""header-and-bottom-navbar""
></tolstoy-block>
```

### CSS Code

```css
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}
```

### JavaScript Code

```javascript
function createTolstoyBlock() {
    const script = document.createElement('script');
    script.setAttribute('type', 'module');
    script.setAttribute('defer', '');
    script.setAttribute('src', 'https://widget.gotolstoy.com/we/widget.js');
    script.setAttribute('data-app-key', 'TOLSTOY_APP_KEY');
    
    document.head.appendChild(script);
}

createTolstoyBlock();
```