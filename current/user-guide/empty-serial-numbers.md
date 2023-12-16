# Empty Serial Numbers

Here, you can find a description of managing Empty Serial Numbers Items through CompuTec WMS.

---

## Item Master Data Configuration

![Item Master Data](./media/item-master-data.png)

## Transactions supported in CompuTec WMS

    GRPO
    Delivery
    Pick and Pack
    Stock Transfer (Transfer Request)
    Stock Counting (planned to be supported).

### GRPO from Purchase Order

![Order Selection](./media/GRPO-1.png)

![Document Details](./media/GRPO-2.png)

![Storage Info](./media/GRPO-3.png)

![Automatic Creation](./media/GRPO-4.png)

![Storage Info](./media/GRPO-5.png)

![Document Details](./media/GRPO-6.png)

![Remarks](./media/GRPO-7.png)

#### Result in SAP Business One

![Goods Receipt PO](./media/GRPO-SAP.png)

![Serial Number](./media/GRPO-SAP-2.png)

### Stock Transfer / From Transfer Request

![Source Warehouse](./media/stock-transfer-1.png)

![From Bin](./media/stock-transfer-2.png)

![Serials](./media/stock-transfer-3.png)

![Serials](./media/stock-transfer-4.png)

![Empty Serials Wizard](./media/stock-transfer-5.png)

![Serials](./media/stock-transfer-6.png)

![Document Details](./media/stock-transfer-7.png)

![Destination Warehouse](./media/stock-transfer-8.png)

#### All to one Bin Location

![To Bin](./media/stock-transfer-to-one-bin-1.png)

![Put Away Items](./media/stock-transfer-to-one-bin-2.png)

#### To different Bin Locations

![Destination Warehouse](./media/stock-transfer-to-different-bins-1.png)

![To Bin](./media/stock-transfer-to-different-bins-2.png)

![Put Away Items](./media/stock-transfer-to-different-bins-3.png)

![Serials](./media/stock-transfer-to-different-bins-4.png)

![To Bin](./media/stock-transfer-to-different-bins-5.png)

![Put Away Items](./media/stock-transfer-to-different-bins-6.png)

![Serials](./media/stock-transfer-to-different-bins-7.png)

![To Bin](./media/stock-transfer-to-different-bins-8.png)

![Put Away Items](./media/stock-transfer-to-different-bins-9.png)

![Remarks](./media/stock-transfer-to-different-bins-10.png)

### Delivery from Sales Order

![Order Selection](./media/delivery-from-sales-order-1.png)

![Order Selection](./media/delivery-from-sales-order-2.png)

![Storage Info](./media/delivery-from-sales-order-3.png)

![From Bin](./media/delivery-from-sales-order-4.png)

![Serials](./media/delivery-from-sales-order-5.png)

<!-- ![Empty Serials Wizard](./media/delivery-from-sales-order-6.png) -->

#### Empty

<!-- ![Storage Info](./media/delivery-from-sales-order-empty.png) -->

#### Named

<!-- ![Empty Serials Wizard](./media/delivery-from-sales-order-named-1.png) -->

<!-- ![Serials](./media/delivery-from-sales-order-named-2.png) -->

<!-- ![Serials](./media/delivery-from-sales-order-named-3.png) -->

<!-- ![Empty Serials Wizard](./media.delivery-from-sales-order-named-4.png) -->

<!-- ![Serials](./media/delivery-from-sales-order-named-5.png) -->

![Storage Info](./media/delivery-from-sales-order-named-6.png)

![Document details](./media/delivery-from-sales-order-named-7.png)

![Remarks](./media/delivery-from-sales-order-named-8.png)

#### In SAP Business One

![Serial Number](./media/delivery-from-sales-order-named-9.png)

## Pick and Pack

(In this transaction, it is not possible to choose Serial Numbers; it is only possible to choose it.)

Warehouses without Bin Locations are supported.

Preallocation when choosing the following option:

![Option](./media/option.png)

Or Bin Locations when this option is turned on:

![Bin Location](./media/bin-location-1.png)

![Bin Location](./media/bin-location-2.png)

![Pick Lists](./media/bin-location-3.png)

- With preallocation:

  ![Storage Info](./media/with-preallocation-1.png)

  ![Quantity](./media/with-preallocation-2.png)

  ![Document Details](./media/with-preallocation-3.png)

- Without preallocation

  ![Storage Info](./media/without-preallocation-1.png)

  ![From Bin](./media/without-preallocation-2.png)

Let's choose, e.g., one named (empty Serial Numbers, and the one on the list must always be chosen separately, meaning you cannot pick one already called and one empty and proceed).

![Serials](./media/without-preallocation-3.png)

Let's choose the next three from the same location (different Bins):

![Storage Info](./media/without-preallocation-4.png)

![Serials](./media/without-preallocation-5.png)

![Empty Serials Wizard](./media/without-preallocation-6.png)

![Serials](./media/without-preallocation-7.png)

![Storage Info](./media/without-preallocation-8.png)

![Empty Serials Wizard](./media/without-preallocation-9.png)

![Storage Info](./media/without-preallocation-10.png)

![Document Details](./media/without-preallocation-11.png)

In the next step, it is possible to go to Delivery from the Pick List and create a Delivery document:

![Document](./media/delivery-from-pick-list-1.png)

![Document Details](./media/delivery-from-pick-list-2.png)

![Storage Info](./media/delivery-from-pick-list-3.png)

![Empty Serials Wizard](./media/delivery-from-pick-list-4.png)

![Storage Info](./media/delivery-from-pick-list-5.png)

![Serials](./media/delivery-from-pick-list-6.png)

![Storage Info](./media/delivery-from-pick-list-7.png)

![Serials](./media/delivery-from-pick-list-8.png)

![Empty Serials Wizard](./media/delivery-from-pick-list-9.png)

![Serials](./media/delivery-from-pick-list-10.png)

![Storage Info](./media/delivery-from-pick-list-11.png)

![Document Details](./media/delivery-from-pick-list-12.png)

![Remarks](./media/delivery-from-pick-list-13.png)

The result Delivery in SAP Business One:

![Serial Number Transaction Report](./media/result-delivery-in-sapb1.png)
