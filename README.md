# Styles.css Integration Guide

This guide explains how to ensure `styles.css` is properly integrated into your Shopify theme. All of the code can be found in the files above.

## 1. Check `styles.css` in `theme.liquid`

Verify that a current `styles.css` file exists with the correct code.

Ensure that your `theme.liquid` file is correctly importing the `styles.css` file. Add the following as the last item in the `<head>` tag:

```liquid
{{ 'styles.css' | asset_url | stylesheet_tag }}
```

## 2. Check `ultimate-dayalayer.liquid` in `theme.liquid`

Verify that a current `ultimate-datalayer.liquid` file exists with the correct code.

Ensure that your `theme.liquid` file is correctly importing the `ultimate-datalayer.liquid` file. Add the following as the last item in the `<head>` tag:

```liquid
{% render 'ultimate-datalayer' %}
```