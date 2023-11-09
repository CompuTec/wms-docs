# Stock Counting

Stock Counting is checking the quantity of Items available in a specific Warehouse. CompuTec WMS supports the SAP Business One Stock Counting function.

:::warning

Note that currently, CompuTec WMS supports only Stock Counting documents with Stock Counter set to User.

:::

1. Choose the Stock Counting option from the main menu:

  ![Main Menu](./media/st-StockCounting.png)

2. Choose the required document:

  ![Select](./media/st-SelectStockCounting.png)

3. Items available on the document are displayed.
The following data are displayed on the Item row: Item Name, Item Code, Bin, quantity in a Warehouse, and counted quantity.
Click an Item row to set up its details.

  ![Document](./media/st-DocDet-1.png)

4. If batches or serials do not manage the Item, choosing it leads to the Counted quantity form with the Total counted quantity:

  ![Counted quantity](./media/st-NotCountedQuantity.png)

  Click the Total Counted row or Plus icon to set up the quantity. Set it up by clicking '+' and '-' icons or by typing it in:

  ![Quantity](./medi/st-Quantity.png)

  Click the Save icon after setting up the quantity. Total counted will change:

  ![Counted Quantity](./media/st-CountedQuantity.png)

  Click the 'x' icon to go back to the Items list.

  ![Document Details](./media/st-DocDet-2.png)

5. If Serial Numbers manage the Item, choosing it leads to the Serials form. Click the '+' icon to add an Item with a Serial Number.

  ![Serials](./media/st-Serials.png)

  Enter a Serial Number and click the Save icon:

  ![Serial](./media/st-Serial.png)

  The Item is counted and added to the list:

  ![Serials](./media/st-Serials2.png)

  Click the 'x' icon to go back to the Items list.

6. If the Item is managed by Batches, choosing it leads to the Batches form. Click the '+' icon to set up quantity:

  ![Batches](./media/st-Batches.png)

  Enter the Batch number, set up the quantity by typing it in or by using the + or - icons, and click the Save icon:

  ![Batch Quantity](./media/st-Batch-Quantity.png)

  Quantity with a specified Batch is added to the document:

  ![Batches](./media/st-Batches-1.png)

  Click the 'x' icon to return to the list of Items.

7. You can add a new Item to the list by clicking the menu icon and then the '+' icon.

  ![Document Details](./media/st-DocDet-Add.png)

8. You can add a Storage Unit by clicking the menu icon and the highlighted icon:

  ![Document Details](./media/st-DocDet-AddS.png)

  Scan an SU barcode or enter a number and click Search or SSCC Search (depending on the type of the entered number).

  All the Items from the chosen SU will be added to the Item list.

  ![Add SU](./media/st-AddSU.png)

9. You can check already added SUs by clicking the menu icon and then the highlighted icon:

  ![Document Details](./media/st-DocDet-AddSt.png)

  ![Storage Unit](./media/st-SU-Empty.png)

10. Unlike most of the CompuTec WMS transactions, you do not save the document after completing work. Values are being saved at the moment of adding quantity. Click the 'x' icon to go back to the main menu:

  ![Document Details](./media/st-Finish.png)
