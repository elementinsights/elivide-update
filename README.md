# Styles.css Integration Guide

This guide explains how to ensure `styles.css` is properly integrated into your Shopify theme.

## 1. Check `styles.css` file

Ensure that `styles.css` has the following code:

```
recharge-subscription-widget {
  max-width:100%;
}

/* .shopify-block.shopify-app-block.recharge-subscription-widget > recharge-subscription-widget {
  max-width:100%;
} */

.rc-purchase-option__sub-container {
  background:blue !important;
}

. rc-purchase-option__label {
  background:red !important;
}
```

## 2. Check `theme.liquid` for styles.css import

Ensure that `theme.liquid` file is correctly importing the `styles.css` file. Add the following at the bottom of the `<head>` tag:

```liquid
{{ 'styles.css' | asset_url | stylesheet_tag }}
