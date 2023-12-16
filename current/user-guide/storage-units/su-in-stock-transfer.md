# SU in Stock Transfer

Here, you can describe handling Storage Units in the Stock Transfer transaction.

---

## New SU

![Document Details](./media/new-su.png)

1. Set the Storage Unit details. You can choose the Destination Warehouse now (the Arrow Down) or do it during the Items collection or in the Put Away Items screen:

  ![Storage Unit details](./media/new-su-put-away.png)

  You can also scan the SSCC number to set a new number instead of the generic one.

2. The top line holds information on an SU to which Items are being added. Click it to leave the adding SU mode. When the bar is empty, Items are added without an SU assigned.

  ![Document Details](./media/scanning-sscc.png)

3. You can add Items by scanning barcodes or adding them manually:

  ![Document Details](./media/su-document-details.png)

4. Clicking an Item in the adding SU mode leads to the screen of Quantity, Batch, or Bin Locations (depends on Item type, Warehouse, and workflow):

  ![Batches](./media/su-batches.png)

5. Clicking SU details leads to its details. You can check the picked Items here. You can also go to the Storage Unit Details screen (B) to choose a Destination Warehouse. You can also leave the SU adding mode (A).

  ![Storage Unit Details](./media/new-su-details.png)

6. You can add the next SU and Items to it. You can also go back to the previous SU by scanning its SSCC or SU Code or by moving to it manually and clicking the magnifying glass icon.

  ![Document Details](./media/su-doc-details.png)

7. When you go out of the edit mode of an SU and go to its details (the Line details screen), you can see which Batches have been chosen, quantities, and if they are stored in another SU or loose. You can also delete from the list Items without SU or Items in new SUs, but you cannot delete Items in the previously existing SUs.

  ![Line Details](./media/line-details.png)

8. You can choose a Destination Warehouse after setting up the document details. You can skip this step by clicking the Right Arrow (which leads directly to the Put Away Items screen).

  ![Document Details](./media/doc-details-end.png)

9. Put Away Items screen: here, you can choose a location for each of the SUs (after clicking it), delete selecting all of the SUs (A), put all of the SUs in the chosen location (B), and go to the document saving (C).

  ![Put Away Items](./media/put-away-items-end.png)

10. 
Once the location is selected, it is marked on its line. After choosing a location for all SUs, you can go to the document summary (the Right Arrow icon).

  ![Put Away Items](./media/put-away-items-mark.png)

11. The document summary:

  ![Remarks](./media/new-su-remarks.png)

## Existing SU

1. Choose an existing SU. There are two ways to ways to do it:

    a. Scanning an SU or SSCC Code in the Document Details screen. This way, you add the whole SU and its content (it is still possible to change the selection later).

    ![Document Details](./media/stock-transfer-doc-det.png)

    b. Scanning an SU or SSCC Code or choosing an SU manually in the List of SUs screen:

    ![Document Details](./media/stock-counting-sus.png)

    Choosing this option opens a List of SUs in the current Warehouse (if there are Bin locations in the Warehouse, a list of Bin Locations is opened first):

    ![SU Locations](./media/su-locations.png)

    ![List of SUs](./media/list-of-sus.png)

2. Choosing an existing SU leads to the Storage Unit details screen. Here, you can choose to receive all the Items or just some of them (A), with a pallet or other collective packaging (B) or without it (C):

  ![Storage Unit Details](./media/storage-unit-details.png)

  Android version:

  ![Storage Unit - Android](./media/storage-unit-details-android.png)

3. In the following example screenshot, you can see that the Item in the first line has not been picked at all, the second one has been picked partially, and the third has been picked fully. The child SU (the fourth row) has not been picked at all:

  ![Storage Unit Details](./media/storage-details-picked.png)

4. You can choose the child SU and choose Items, quantities, Batches, and if we are picking it with (A) or without (B) the collective packaging:

  ![Storage Unit Details](./media/child-su-details.png)

    a. Here you can see an example where the child SU has been chosen with content and collective packaging (the child SU stays in the parent SU):

    ![Storage Unit Details](./media/child-su-details-2.png)

    b. Here you can see an example where the child SU has been chosen with content but without the collective packaging (the child SU content goes to the parent SU):

    ![Storage Unit Details](./media/child-su-details-no-packaging.png)

5. The chosen lines can be transferred along with the parent SU (A) - then, Active-Item-01 will be left in the source Warehouse, and the rest will be transferred. Or transfer alone, Active-Item-01 will stay in the Parent pallet (B).

  ![Storage Unit Details](./media/su-details-transfer.png)

6. Choose the required Items and SUs and go to the document summary:

  ![Document Details](./media/su-document-summary.png)

7. Now, choose a Destination: Warehouse, Warehouse, and Bin, or skip this step. 

  ![Destination Warehouse](./media/su-destination-warehouse.png)

  ![To Bin](./media/su-destination-bin.png)

  You can set the automatic skip of this step in Custom Configuration:

  ![WMS Custom Configuration](./media/su-config.png)

8. In the Put Away screen, you can put each Item in a specific location by clicking its line, delete the location selection (A), put all the Items in the previously chosen location (B), and go to the Document Details (C):

  ![Put away Items](./media/put-away-items.png)

9. You can then add remarks (optional) and save the document:

  ![Remarks](./media/su-remarks.png)
