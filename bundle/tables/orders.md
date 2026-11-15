---
type: Table
title: Orders Table
description: Purchase order records for the okf-sync fixture dataset.
tags:
- sales
- orders
---

The `orders` table records one row per purchase. Each order links to the
[customers](customers.md) table via `customer_id`. Update in proof/shared branch. 

# Schema

- `order_id`: INTEGER, Unique order identifier.
- `customer_id`: INTEGER, Purchaser. Links to the [customers](customers.md) table.
