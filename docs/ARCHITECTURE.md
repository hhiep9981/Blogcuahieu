# Architecture

## Module map
`index.html` (single page)
1. Header / nav (sticky, mobile menu)
2. Hero: asymmetric split (copy + image)
3. `#products`: bento grid (Tide large, Harbor, Roots)
4. Capabilities: tabs per product
5. `#founders`: offset founder pair
6. `#approach`: statement + 2x2 principles
7. `#contact`: email CTA block
8. Footer

Design tokens live in the `@theme` block inside `<style type="text/tailwindcss">`.

## FUNCTION REGISTRY

### index.html (inline script)
| Function | Signature | Purpose | Tags |
|----------|-----------|---------|------|
| `initReveal` | `() -> void` | Add `.in` to `.reveal` elements on viewport entry | `#ui #motion` |
| `initTabs` | `() -> void` | Accessible tabs with arrow-key navigation | `#ui #a11y` |
| `initMenu` | `() -> void` | Toggle mobile nav menu | `#ui` |
| `initCopyEmail` | `() -> void` | Copy contact email with success/error status | `#ui` |
