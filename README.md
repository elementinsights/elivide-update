# Styles.css Integration Guide

This guide explains how to ensure `styles.css` is properly integrated into your Shopify theme.

## 1. Check `styles.css` file

Ensure that `styles.css` has the following code:

```
{{ 'styles.css' | asset_url | stylesheet_tag }}
```

## 2. Check `theme.liquid` for styles.css import

Ensure that `theme.liquid` file is correctly importing the `styles.css` file. Add the following at the bottom of the `<head>` tag:

```liquid
{{ 'styles.css' | asset_url | stylesheet_tag }}
