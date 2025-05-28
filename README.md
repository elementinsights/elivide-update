# Styles.css Integration Guide

This guide explains how to ensure `styles.css` is properly integrated into your Shopify theme.

## 1. Check `styles.css` in `theme.liquid`

Ensure that your `theme.liquid` file is correctly importing the `styles.css` file. Add the following as the last item the `<head>` tag:

```liquid
{{ 'styles.css' | asset_url | stylesheet_tag }}
```

Also verify that a current styles.css file exists.
