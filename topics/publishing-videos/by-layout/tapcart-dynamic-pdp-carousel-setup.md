## Tapcart Dynamic PDP Carousel Setup

The **PROJECT_PUBLISH_ID** in the HTML code needs to be replaced with the publish ID from the TV project, which you can find in the Tolstoy app. Make sure to replace the **TOLSTOY_APP_KEY** in the JS code with your Tolstoy app key.

You can use this [Guidde video walkthrough](https://app.guidde.com/share/playbooks/omfqybH3Rr2yFVjgejuSTg?origin=7hK1MO5mPsQuiT0iQVou54jqkwJ3).

**HTML code:**

```html
<tolstoy-carousel
    class="tolstoy-carousel"
    data-publish-id="PROJECT_PUBLISH_ID"
    style="display: none">
</tolstoy-carousel>
```

**CSS code:**

```css
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
  font-family: Helvetica;
}

.tolstoy-carousel iframe {
  display: block !important;
}
```

**JS code:**

```javascript
function setBlockHeight(height) {
  document.documentElement.style.setProperty(
    "height",
    `${height}px`,
    "important"
  );
}

function updateCarousel() {
  const carouselElement = document.querySelector(".tolstoy-carousel");

  if (carouselElement) {
    const productId = window?.Tapcart?.variables?.product?.id;
    if (productId) {
      carouselElement.setAttribute("data-product-id", productId);
    }
  }
}

function appendScriptsToHeader() {
  const tolstoyAppKeyScript = document.createElement("script");
  tolstoyAppKeyScript.innerHTML =
    'tolstoyAppKey="TOLSTOY_APP_KEY"';
    
  const widgetScript = document.createElement("script");
  widgetScript.src = "https://widget.gotolstoy.com/widget/widget.js";

  const head = document.getElementsByTagName("head")[0];
  head.appendChild(tolstoyAppKeyScript);
  head.appendChild(widgetScript);
}

function checkElementExistence() {
  let attempts = 0;
  const intervalId = setInterval(function () {
    attempts++;
    const element = document.querySelector(".tolstoy-carousel-container");
    if (element) {
      setBlockHeight(490);
      const carousel = document.querySelector(".tolstoy-carousel");
      if (carousel) {
        carousel.style.display = "block";
      }
      clearInterval(intervalId);
    } else if (attempts >= 50) {
      clearInterval(intervalId);
    }
  }, 200);
}

function loadContent() {
  setBlockHeight(0);
  updateCarousel();
  appendScriptsToHeader();
  checkElementExistence();
}

loadContent();
```
