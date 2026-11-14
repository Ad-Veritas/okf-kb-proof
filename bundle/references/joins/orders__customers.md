---
type: Reference
title: Orders to Customers Join Path
description: Join relationship linking orders to their purchasing customer by customer_id.
tags:
- join
- sales
---

This join path links an order to the customer who placed it, letting a
query recover the customer name for every order row.

```sql
SELECT
  o.order_id AS order_id,
  o.customer_id AS customer_id,
  c.name AS customer_name
FROM
  orders AS o
JOIN
  customers AS c
ON
  o.customer_id = c.customer_id;
```
