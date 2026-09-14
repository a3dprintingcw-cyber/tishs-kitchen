# Tish's Kitchen

Order counter and back office for Tish's Kitchen, Curaçao.
Live at **https://tishxkitchen.com**

Open it on the phone, then **Add to Home Screen**. It opens like a real app and works with no internet.

---

## The five tabs

**Sell** — tap the food to build an order, then press **Charge**.
On the charge screen: pickup or delivery, customer name and phone, paid or not paid,
cash or card, cash received (it works out the change), a discount, and a note.

**Orders** — everything taken today. Filter by *To make*, *Owed*, or *Delivery*.
Open an order to take the money later, mark it made, send a WhatsApp receipt, or delete it.

**Money** — today's takings at a glance: total, in hand, still owed, cash vs card,
what sold today, and every earlier day. Send a summary to WhatsApp, or export a CSV.

**People** — every customer who gave a name or number: how many orders, how much they spent,
what they usually order, and what they still owe. One tap sends a friendly payment reminder.

**More** — the menu editor, the delivery fee, backups.

## Menu

Tish can change the menu herself in **More**: add items, change prices, rename,
regroup, or mark something **Sold out**. No code, no waiting on anyone.

Starting menu:

| Item | Price |
|---|---|
| Pasta Porkchop + Drink | XCG 35 |
| Pasta Chicken + Drink | XCG 35 |
| Burrito Chicken, Takis + Drink | XCG 35 |
| Biscoff Cookie Cake Cup | XCG 15 |
| Strawberry Tres Leches Cup | XCG 15 |
| Strawberry Lemonade | XCG 5 |
| Peachy | XCG 5 |
| Delivery fee | XCG 10 |

## Backups, important

Everything is stored in the phone's own browser. Nothing is sent anywhere, which is why
it works offline. It also means that if the phone is lost or the browser data is cleared,
the orders go with it.

**More → Save a backup** writes one small file. Keep it in WhatsApp, email or Drive.
The app asks for a backup once a week. **Restore** loads it back.

## Photos

Photos live in `images/`, square, about 320x320, WebP. To swap one, drop a new file in
`images/` and point the item at it in the menu editor (`images/your-file.webp`).

## Files

```
index.html      the whole app, no build step
manifest.json   home screen name, colours, icons
icon-192.png    app icon
icon-512.png    app icon
images/         product photos
CNAME           tishxkitchen.com
```

Hosted on GitHub Pages from `main` at the repository root.
