
# Must have features

1. Easy way to deal with carton quantities.

  - An exact reprint of an SKU may result in different carton quantities. If that occurs and there is still previous stock in inventory, we end up with multiple carton quantities for the same SKU.
  
  - Customer usually orders by carton (2x Item C) but occasionally will order by exact quantity needed. (10,000 Item C)
  
  - Print orders rarely fill an even number of cartons.  We usually end up with one smaller "short" carton on each SKU.
  
  - Inventory quantities must not be negative, or at the very least have the "Sorry, this item is out of stock" replace the add to cart button on negative quantities.  Current D6 site only disables the add to cart button when quantity is exactly 0.

  - Stock threshold notifications are wacked. For example, some PI's are small so there are a large number per box. If the qty for the entire printing is 10,000 and we get 5,000 per carton, then the threshold notification is worthless really. Originally the plan was to have an email sent when the stock reached 20% of the printed amount. Ordering carton quanties only really makes this difficult.

2. Inventory transactions.

  - For obvious reasons, we need a way to record all transactions to products in inventory.  With current D6 site, there has been no easy way to record transactions that ADD to inventory.  
  
  - Occasionally, products in inventory become obsolete and a new version is printed before the stock is depleted. This results in a "kill order" where the old product is destroyed and recycled. We need an easy way to track this.
  
  - Rarely, a product in inventory will be revised and a new version printed but the customer requests that both versions of the item are kept in inventory.  I'm not exactly sure why this happens, but could possibly be products that they ship internationally vs. domestic??  Whatever the case, we need a way to flag these items to make sure the customer knows there are 2 versions (besides having seperate nodes).  Also, this should be noted on the pick order so we are sure to pull the correct item.

3. Locations

  - We have multiple locations where we store inventory.  We need a simple way to track locations that show on a pick order.  This can be done in D6 and D7 currently.  I'm just putting this here as a reminder.
  
  - Occasionally when a job gets reprinted and there is still some product left in inventory, space limitations dictate that the new printing is stored in a seperate area.  We need a way to track more than one location per SKU.
  
  
