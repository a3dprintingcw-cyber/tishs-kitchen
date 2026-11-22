# Tish's Kitchen

Customer ordering site at https://tishxkitchen.com. Customers pick food, choose
pickup or delivery and a time, and send the order.

With `CONFIG.api` set, the order goes straight into Tish's app through the
order API (`backend/` in the `tishs-kitchen-admin` repo) and her phone buzzes.
Menu, prices, sold out and delivery fee are then loaded live from her app.
If the API cannot be reached, the order falls back to a WhatsApp message.
With `CONFIG.api` empty it works as before: WhatsApp only.

Payment: cash, or online with Sentoo links set in `CONFIG.sentoo` in `index.html`.

Tish's own order and money app lives in the `tishs-kitchen-admin` repo at
https://admin.tishxkitchen.com. `bridge.html` lets that app copy her old data
from this address the first time she opens it. Do not remove it.

Single `index.html`, no build step.
