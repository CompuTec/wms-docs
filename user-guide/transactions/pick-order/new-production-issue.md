# New Production Issue

The Pick Order transaction allows generating a ProcessForce Production Issue.

:::note
The order and availability of some of the forms during a document's creation may vary depending on individual settings. Click here to find out more.
:::

1. To create a Production Issue from a Pick Order, click Pick Order in the main menu.

  ![Start](./media/PickOrder2.png)

  ![New](./media/NewProductionIssue2.png)

2. The Opened Pick Orders window will appear.

  Choose a desired Pick Order by clicking its row. Only opened or started Manufacturing Orders are displayed.

  ![Manufacturing Order](./media/ManufOrder2.png)

  :::warning

  You can use the Filter field to search the records by typing in at least a part of a name or a document number.

  It is also possible to search by document date. In this case, a date without separators has to be typed in the filter field, e.g., 20190107 instead of 2019-01-07.

  :::

3. The 'Items to pick order' form will appear with Manufacturing Orders connected to the chosen Pick Order.

  Click an Item row or scan a barcode with an Item prefix to choose it from the list and set its quantity.

  ![Items to pick Order](./media/ItemsToPickOrder2.png)

  ![Batches](./media/PickOrder_Batches2.png)

  The required quantity is automatically entered in the quantity field.

  ![Quantity](./medi/Quantity_Flour2.png)

  Click the '+' icon to add Manufacturing Orders not connected to the chosen Pick Order.

  ![Pick Order](./media/PickOrder_AddItem2.png)

  You can also add a Manufacturing Order by scanning a barcode with a document number prefix. Only Manufacturing Orders with the status Open can be added.

  Click a required row or scan a barcode with a document number prefix to add a Manufacturing Order to the Items to Pick list.

  ![Manufacturing Order](./media/ManufOrder2.png)

  Click the Storage Unit icon to add an SU to a current document. You can add an SU by scanning a barcode with an SU prefix. Only SU with Items from Pick Order and the same Warehouse as on the Items rows can be added.

  ![Pick Order](./media/PickOrder-AddSU2.png)

  Click a required SU row to add it to the document. You can add it by scanning a barcode with an SU prefix.

  ![Pick Order SU](./medi/PickOrder-SU2.png)

  ![SU](./media/SUDetails2.png)

  ![SU](./media/SUAdded2.png)

  Scanning a barcode without a prefix in the Items to Pick list results in checking it for storage unit information.

4. Choosing a Storage Unit or a Batch in the FIFO method is possible. You can skip this step by clicking the right arrow icon.

  You can hide this form by using the related Custom Configuration [ADD LINK] option option.

  ![FIFO](./media/FIFO2.png)

  ![FIFO](./media/FIFO-SU2.png)

  ![FIFO](./media/SUInfo2.png)

5. If the Item is managed by Bin Locations, the 'From Bin' form will appear.

  Click a desired Bin row to choose it. You can also scan a barcode (with prefixes or not).

  ![From Bin](./media/FromBIN2.png)

6. If the Item is managed by Batches, the Batch form will appear.

  Click the desired Batch row. A batch can be chosen by scanning a barcode with a prefix.

  ![Batches](./media/Batches2.png)

7. The Quantity form will appear.

  The field is automatically filled in with the required quantity. Type in the desired quantity or set it by clicking the plus and minus buttons.

  Quantity can be set by scanning a barcode with a quantity prefix. Click the 'Right Arrow' icon after selecting the quantity.

  ![Quantity](./media/Quantity12.png)

8. In the 'Items to pick order' form, click the 'Right Arrow' button after setting the required quantities for every item.

  ![Ready](./media/Done2.png)

9. Remarks form will appear.

  Issue series can be chosen from the drop-down list. This value can be preset in ProcessForce form Document Numbering: Main Menu > Administration > System Initialization > Document Numbering. If the series is not picked, the default ones will be selected.

  Remarks can be added.

  ![Remarks](./media/Remarks02.png)

10. Click the Save icon after setting all the details.

  ![Remarks](./media/Remarks2.png)

11. A message about a document creation will be displayed.

  Click 'Ok' to finish the creation of a document.

  ![Created](./media/Created2.png)

12. Goods Issue has been created and recorded and can be viewed in SAP Business One.
