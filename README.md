# Stitched by Donna

Brochure website for Donna Russell's handmade quilted items. It's one static page (`index.html`) with no build step, deployed to Hostinger from the `main` branch.

## Updating products and prices

Open `index.html` and find the `ITEMS` list near the bottom (search for `EDIT ME`). Each product is one line:

```js
{name:"Santa Paws treat bag", m:"dog", cat:"Treat bags", price:18, size:"22 × 19 cm", desc:"...", art:"bag", f:"f-dotred", img:"images/santa-paws.jpg"},
```

- `price`: a number such as `18` shows "$18". `null` shows "Ask for price".
- `img`: path to a photo in `images/`. Leave it as `""` to show the illustration instead.
- `cat`: the category. New categories appear as filter buttons automatically.
- `big:true`: shows the item as the large feature block. Use it on only one item.
- `size`, `desc`: optional details shown on the card.

## Photos

Put photos in `images/`. Square photos look best, around 1000 × 1000 px and under 300 KB each. Use lowercase names with hyphens, e.g. `reindeer-treat-bag.jpg`.

## Deploying

Pushing to `main` deploys automatically through Hostinger's Git integration (hPanel → Advanced → Git).
