# Mission: Stock Count Reconciliation
**Run:** Mission (12 Iris → 03 Penny → 02 Bean) | **Gate:** one yes on the stock plan (section 02) | **Date:** 2026-10-23

## Brief
- **Codename:** Stockcount
- **Type:** Research → Decision
- **Objective:** Turn the Oct 21 physical count into one decision on what to do with Martha's World stock before the Dec 4 relaunch.
- **Success metric:** Makonnen says yes or no to one plan. Shopify quantities match the shelf.
- **Constraints:** $1,000 relaunch budget, already allocated. No new spend. Nothing deleted.
- **Inputs:** Products & Inventory (Notion, counted Oct 21), Shopify Admin (live Oct 23), Shopify analytics (12 months).

---

## 12 Iris — Data & Analytics

### Finding 1: the shelf holds 3.2x what Shopify says

| Group | Shopify units | Physical count | Variance |
|---|---|---|---|
| Character pins (6) | 114 | 386 | +272 |
| Character keychains (5) | 90 | 301 | +211 |
| Plush ball keychains (3) | 42 | 125 | +83 |
| Lola Plush | 13 | 8 | −5 |
| **Live products, 15** | **259** | **820** | **+561** |

Per product:

| Product | Shopify | Physical | Var | New price (Oct 21–22) |
|---|---|---|---|---|
| Ruby Pin | 19 | 72 | +53 | $14 |
| Merri Jane Pin | 20 | 69 | +49 | $14 |
| Crystal Pin | 19 | 67 | +48 | $14 |
| Martini Pin | 19 | 65 | +46 | $14 |
| Lola Pin | 18 | 65 | +47 | $14 |
| Martha's World Gold Pin | 19 | 48 | +29 | $22 |
| Martini Keychain Lavender | 20 | 67 | +47 | $18 |
| Crystal Keychain Orange | 16 | 64 | +48 | $18 |
| Merri Jane Keychain Yellow | 18 | 60 | +42 | $18 |
| Ruby Keychain Tan | 18 | 56 | +38 | $18 |
| Lola Keychain Lime | 18 | 54 | +36 | $18 |
| Green Plush Ball Keychain | 14 | 42 | +28 | $32 |
| Yellow Plush Ball Keychain | 14 | 42 | +28 | $32 |
| Pink Plush Ball Keychain | 14 | 41 | +27 | $32 |
| Lola Plush | 13 | 8 | −5 | $25 (discontinued Oct 22) |

[Verified] Physical counts from Products & Inventory, entered Oct 21 from count photos. Shopify quantities and prices pulled live Oct 23.
[Inference] The Shopify quantities for pins and keychains (16–20 each) were placeholders set when the listings went up in March 2026, never a count. That's why every row is off by roughly the same amount.

### Finding 2: "updated the website" = prices, not inventory

Shopify changed on Oct 21 23:34 and Oct 22 14:57 UTC:
- Pins $3 → $14. Gold pin $3 → $22. Character keychains $3 → $18. Plush ball keychains $12 → $32.
- Inventory quantities: **unchanged**. Shopify still thinks there are 259 units, not 820.
- Lola Plush: still live at $25 with 13 units, though it's discontinued.

[Verified] Product updatedAt timestamps and prices, Shopify Admin.

### Finding 3: the 13 hidden products were not counted

Draft and archived products with stock on Shopify: pin pack (48), flight-tag pack (48), both ringer tees (38 + 25), four skullies/truckers (17, 13, 11, 7, 4), four sock colorways (15, 14, 13, 11). 264 units in the system, about $5,600 at list. Physical count: blank on all 13. Makonnen closed the count Oct 21 without them. Status is **unknown, not zero**.

### Finding 4: the store does not currently sell

| Period | Orders | Paid orders | Net sales |
|---|---|---|---|
| Last 12 months | 27 | 8 | $118 |
| Last 180 days | 4 | 3 | $63 |
| Black Friday week 2025 (Nov 20–Dec 5) | 2 | 0 | $0 |

Units sold in the last 180 days: 5 (one Merri Jane keychain, one of each plush ball, one Lola plush). 19 of the 27 orders were $0 (gifts or manual). Hidden stock sold 0 because it's hidden.
At 5 units per 180 days, 820 units is a 80-year supply.

[Verified] ShopifyQL, sales and inventory tables.

### What Iris hands to Penny
The constraint is traffic, not price and not stock. There is one traffic event on the calendar: the Nov 16 tease and the Dec 4 drop. Every stock decision should attach to that event.

---

## 03 Penny — Finance

### Stock on hand at the new prices

| Group | Units | At old price | At new price |
|---|---|---|---|
| Pins | 386 | $1,158 | $5,788 |
| Character keychains | 301 | $903 | $5,418 |
| Plush ball keychains | 125 | $1,500 | $4,000 |
| Lola Plush (free with purchase) | 8 | $200 | $0 |
| **Live stock** | **820** | **$3,761** | **$15,206** |
| Hidden stock (uncounted, Shopify figure) | 264 | $5,612 | $5,612 |

[Inference] The price move quadruples the paper value. It changes nothing about cash until someone buys. The store sold 5 units in six months at $3; at $14–$32 it will sell fewer per visitor, so the relaunch has to bring more visitors than ever before for this to net out. That's a marketing problem (Fizz), not a pricing one.

### Old-stock options (the 13 hidden products, ~264 units)

```
OPTION A: Standalone Black Friday clearance (the plan on the board, TASK-7)
UPFRONT COST: $0 (promo budget is reserved for the relaunch)
PROJECTED REVENUE: $0–$300
BASIS: last Black Friday with no push = 2 orders, $0. 50% off ~$5,600 list = $2,800 ceiling at 100% sell-through, which does not happen.
RISK: burns the "Martha's World is closing" tease on a sale nobody sees. Splits attention two weeks before the drop.
CONFIDENCE: High that it underperforms [Verified on last year's numbers]

OPTION B: Fold old stock into the Dec 4 drop as "Vault" add-ons + gift-with-purchase
UPFRONT COST: $0
PROJECTED REVENUE: raises average order value on the relaunch instead of standing alone. Example: spend $65 (one hoodie) → pick a free Vault item (socks, skully, trucker). Spend $100 → pin pack or flight-tag pack free. Packs also listed at $15/$25 in a Vault collection.
RISK: Vault items are off-concept (no Light/Dark). Mitigate: name it "The Vault" or "Archive" and keep it below the fold.
CONFIDENCE: Medium [Inference]. The gift-with-purchase mechanic is standard; the lift depends on relaunch traffic.

OPTION C: Gift / donate
UPFRONT COST: $0. Shipping if mailed to fans: ~$5 each.
PROJECTED REVENUE: $0. Clears space. Goodwill with fans and creators (Fizz already has $450 earmarked for gifting).
TAX: donated inventory is generally deductible at cost basis, not retail, for a pass-through business. [Inference] Confirm with the tax preparer. Keep a receipt from the receiving org.
CONFIDENCE: High on mechanics, low on any revenue effect.
```

### Penny's call
B for the sellable old stock (packs, skullies, truckers, socks). C for the ringer tees and the 8 Lola plush, which are already out of the brand. A is dead on the data.

Also: the 820 live units are the relaunch's bundle fuel. A "Pick a side" starter set (1 pin + 1 keychain + 1 plush ball) at $49 moves three units per order at a price that still beats the old $3 by 3x each. Nothing new gets made. No new spend.

---

## 02 Bean — Operations

### One plan, one yes

1. **Sync Shopify to the shelf.** Set the 15 live products to the physical count (820 units). Set Lola Plush to 0 and hide it, or convert it to a $0 gift-with-purchase. No money. I do it the moment you say yes.
2. **Kill the standalone Black Friday clearance.** TASK-7 becomes "Vault + gift-with-purchase tiers inside the Dec 4 drop." Nov 27–30 becomes part of the tease, not a sale.
3. **Old stock routing.**
   - Pin pack (48), flight-tag pack (48), skullies, truckers, socks → **Vault**. Listed in a hidden collection, published Dec 4 alongside the capsule, gift-with-purchase at $65 / $100.
   - Ringer tees (63 units), Lola Plush (8) → **gift or donate**. Out of the store. Archive on Dec 1 (TASK-14 stays, scope narrows to these).
4. **Bundle the live stock.** Ember + Fizz get one card: "Pick a side" starter set at $49 (pin + keychain + plush ball) built from existing stock. Goes in the Nov 16 tease.
5. **Count the 13 hidden products.** 30 minutes, same sheet. Or tell me "they're gone" and I zero them. Vault pricing waits on this.

**Gate:** steps 1–4 need your yes. Step 5 needs your hands.

### Workflow after yes
```
WORKFLOW: Stock plan → Dec 4
TRIGGER: Makonnen says yes
STEPS:
  1. Bean → set Shopify quantities to physical count → 15 products synced → Iris verifies
  2. Bean → rewrite TASK-7 (Vault + GWP) and TASK-14 (archive tees + Lola only) → board matches plan
  3. Ember → "Pick a side" starter set spec + Vault collection list → Fizz (tease copy) + Store Ops (hidden collection, by Nov 9)
  4. Makonnen → count hidden 13 → Bean sets Vault quantities
  5. Sully → one-line check on GWP terms and donation receipt → done
SUCCESS: Shopify = shelf. Board = plan. Vault ready by Nov 9 product-page build.
FALLBACK: if hidden stock is gone, Vault = pin pack + flight-tag pack only (those two rows had 48 each in Shopify; confirm physically).
```

---

## Open items
- **Gate:** yes/no on the plan above (Bean, steps 1–4).
- **Needs your hands:** count or confirm the 13 hidden products.
- **Sully:** gift-with-purchase terms and donation receipt, one line, after the yes. AI-generated legal analysis, not legal advice. Consult a licensed attorney.
- **Fizz:** the price move needs traffic to work. Relaunch promo plan should be sized against "5 units in 180 days" as the baseline, not the old $98/week figure.

## Labels
- [Verified] All counts, prices, timestamps, sales and inventory figures above come from Notion (Oct 21) and Shopify (Oct 23).
- [Inference] Placeholder-quantity explanation; Option B lift; starter-set price; tax treatment of donations.
- [Speculation] None.

---

## ✅ Executed — Oct 23, 2026 (Makonnen said yes)

| Step | Done |
|---|---|
| 1. Sync Shopify to shelf | 14 live products set to the Oct 21 count (812 units). Lola Plush set to 0 and hidden (Draft). Writes pinned to the prior quantity; none collided. Products & Inventory "Shopify units" column updated to match. |
| 2. Kill standalone clearance | TASK-7 rewritten: "Vault + gift-with-purchase inside the Dec 4 drop." Nov 27–30 is tease, not sale. |
| 3. Old stock routing | TASK-14 narrowed to ringer tees + Lola Plush. Everything else stays listed in the Vault until zero. |
| 4. Starter set | New card for Ember: "$49 Pick a side starter set + Vault collection spec," due Oct 30. |
| 5. Hidden 13 | New Needs You card, due Oct 28: count them or say "gone." |

Gate card closed. Command Log work report filed. Bean back to standby.
