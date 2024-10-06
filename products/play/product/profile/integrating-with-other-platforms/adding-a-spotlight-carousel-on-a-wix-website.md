## Adding a Spotlight Carousel on a Wix Website

To inform you, we only support adding widgets on a Wix website. 

Luckily, we have a workaround to support Spotlight carousels on Wix websites.

Here's how:

### Use an Iframe

Paste this code:

```html
<script>tolstoyAppKey="YOUR APPKEY"</script> 
<script src="https://widget.gotolstoy.com/widget/widget.js" defer></script>
```

Plus the carousel code:

```html
<tolstoy-carousel
id="PUBLISH ID"
class="tolstoy-carousel"
data-product-id="PRODUCT_ID">
</tolstoy-carousel>
```