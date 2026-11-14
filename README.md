# Lumen Test Supply (test store)

A fake, static shop for testing ShopLens price-drop tracking (docs/price-drop-tracking/ on
feature/price-drop-tracking). Published with GitHub Pages from the `main` branch.

**To drop a price:** open `products/<item>.html`, change `"price"` in the JSON-LD block at the top
and the visible `$` price in the page body, then commit. Pages republishes in about a minute.

Rules the price check applies: USD only, `InStock`, one offer per page, the product name must stay
the same, and a new price must be within 0.3x-3x of the price when tracking started.
