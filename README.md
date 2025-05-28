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

## 3. Check `recharge-styling-bottles.liquid'` and `recharge-styling-filter.liquid'` in the sections folder

Verify that a current `recharge-styling-bottles.liquid'` and `recharge-styling-filters.liquid` file exist with the correct code.

Ensure that product templates for bottles with a subscription have the correct code as found in the `product.recharge-bottle-subscription.json` file above.

Ensure that product templates for filters with a subscription have the correct code as found in the `product.recharge-filter-subscription.json` file above.

