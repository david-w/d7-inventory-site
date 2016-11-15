
# Must have features

1. Easy way to deal with carton quantities.

  - An exact reprint of an SKU may result in different carton quantities. If that occurs and there is still previous stock in inventory, we end up with multiple carton quantities for the same SKU.
  
  - Customer usually orders by carton (2x Item C) but occasionally will order by exact quantity needed. (10,000 Item C)
  
  - Print orders rarely fill an even number of cartons.  We usually end up with one smaller "short" carton on each SKU.
  
  - Inventory quantities must not be negative, or at the very least have the "Sorry, this item is out of stock" replace the add to cart button on negative quantities.  Current D6 site only disables the add to cart button when quantity is exactly 0.

2. Inventory transactions.

  - For obvious reasons, we need a way to record all transactions to products in inventory.  With current D6 site, there has been no easy way to record transactions that ADD to inventory.  
  
  - Occasionally, products in inventory become obsolete and a new version is printed before the stock is depleted. This results in a "kill order" where the old product is destroyed and recycled.
