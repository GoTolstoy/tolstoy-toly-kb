## Tapcart Code Block for Homefeed Top Bar Implementation for Apps with Side Navigation

**HTML** code:

```html
<tolstoy-block
    data-publish-id="**PROJECT_PUBLISH_ID**"
    data-block-type="video-page"
    data-nav-type="header"
></tolstoy-block>
```

**CSS** code:

```css
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}
```

**JS** code:

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