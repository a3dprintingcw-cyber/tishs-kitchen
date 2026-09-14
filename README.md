# Tish's Kitchen

A tap-to-sell order counter for Tish's Kitchen. She taps a meal each time one is
sold, and the app keeps a running total of the money made that day.

**Live app:** https://a3dprintingcw-cyber.github.io/tishs-kitchen/

## How it works

* **Sell** shows every item as a big card. One tap is one sale. A badge on the
  card shows how many of that item went out today.
* **Undo** in the bottom bar removes the last tap, for when a button is pressed
  by mistake.
* **Today** is the running receipt: how many of each item, what each line is
  worth, and the total for the day. The plus and minus buttons on a line fix a
  miscount. From here the day can be copied as text or sent on WhatsApp.
* **Close the day** files the day under History and sets the counter back to zero.
* **History** keeps every closed day with its total, plus a running total across
  all of them.

Everything is stored on the phone itself, so it keeps working with no internet.
Nothing is sent anywhere.

## Menu and prices

| Item | Price (XCG) |
| --- | --- |
| Pasta Porkchop + Drink | 35 |
| Pasta Chicken + Drink | 35 |
| Burrito Chicken, Takis + Drink | 35 |
| Biscoff Cookie Cake Cup | 15 |
| Strawberry Tres Leches Cup | 15 |
| Strawberry Lemonade | 5 |
| Peachy | 5 |
| Delivery Fee | 10 |

## Photos

Every item except the delivery fee has a photo in the `images` folder. To swap
one, drop a new square image in that folder and point the item at it in the
`MENU` list near the top of the script in `index.html`:

```js
{ id:"pasta-porkchop", name:"Pasta Porkchop + Drink", price:35, emoji:"🍝", img:"images/pasta-porkchop.webp" },
```

An empty `img` falls back to the emoji. Square images around 360x360 keep the
app light enough to load fast on mobile data.

## Changing a price or adding an item

Same `MENU` list. Each item needs a unique `id`, a `name`, a `price` and an
`emoji`. Days already closed keep the price they were sold at, so changing a
price does not rewrite past history.

## Putting it on her home screen

Open the live link in Chrome or Safari, then choose "Add to Home Screen". It
opens full screen like a normal app.
