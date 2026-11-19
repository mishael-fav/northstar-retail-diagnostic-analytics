# Data Dictionary

## weekly_performance.csv
**Grain:** one row per Week_Start × Region × Channel × Device × Category.

Fields:
- Week_Start: Monday date for the reporting week.
- Region: Lagos, Abuja, or Port Harcourt.
- Channel: Organic Search, Paid Search, Paid Social, or Email.
- Device: Mobile or Desktop.
- Category: Electronics, Fashion, or Home & Living.
- Sessions: on-site sessions.
- Add_to_Cart: cart-add events.
- Checkout_Starts: checkout-start events.
- Orders: completed orders.
- Gross_Revenue: order value before discounts and refunds.
- Discount_Amount: discounts applied.
- Refund_Amount: refunds recognized.

## marketing_spend.csv
**Grain:** one row per Week_Start × Region × Paid Channel.

Important:
- Only Paid Search and Paid Social appear in this file.
- It is NOT split by Device or Category.
- Think carefully before joining this file to weekly_performance.csv.

Fields:
- Week_Start
- Region
- Channel
- Impressions
- Clicks
- Spend

## release_log.csv
Operational events that may be useful as context. Timing alone does not establish causation.
