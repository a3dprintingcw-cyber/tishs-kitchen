# Tish's Kitchen

Customer ordering site at https://tishxkitchen.com. Customers pick food, choose
pickup or delivery and a time, and the order opens in WhatsApp to Tish.
Payment: cash, or online with Sentoo links set in `CONFIG.sentoo` in `index.html`.

Tish's own order and money app lives in the `tishs-kitchen-admin` repo at
https://admin.tishxkitchen.com. `bridge.html` lets that app copy her old data
from this address the first time she opens it. Do not remove it.

Single `index.html`, no build step.
