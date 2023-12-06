# New Stock Counting

New Stock Counting transactions have been available since the WMS 2.10.15_R1 version.

## Requirements

### CompuTec WMS database objects installation

Click [here](./../../../administror-guide/installation/wms-server/wms-server.md/#wms-server) to find out more.

### AppEngine plugin installation (http://localhost:54000/webcontent/uaa/webapp/Index.html)

Click (ADD LINK) here to download the installation file.

Click [here](./plugin-installation.md) to find out more about the installation.

### Stock Counting Document

The new Stock Counting is created based on an empty document created in CompuTec WMS. Next, it is sent to SAP Business One. In the old Stock Counting, an SAP Business One user created a document based on which a list was displayed in CompuTec WMS.

![Document](./media/new-stock-counting-document.png)

### Custom Configuration option

You can choose to use either the new or the old Stock Counting. To use the old one, go to Custom Configuration → Stock Counting and check the Use old stock counting checkbox:

![Custom Configuration](./media/custom-configuration-new-stock-counting.png)

After enabling the old Stock Counting, you can use all of the checkboxes from this view (both for the old and new option versions):

After saving, auto return to: – choose where to return after saving Item Details on a document; you can select the main menu for this operation or the Item list

Display message after adding batches – configure a message displayed on adding a Batch. The message can be based on an SQL query

Scan DocNum on Base Document selection window – checking this option allows you to scan a document by Docnum, not by DocEntry, if a base document was chosen

Force manual quantity confirmation – after reviewing required prefixes (Warehouse, Vendor, Item, Quantity, Batch number), the application forces manual confirmation of quantity (instead of confirmation after scanning a barcode with quantity)

Stock Counting: automatically choose Bin Location on Batch scanning – automatically chooses Bin Location on Batch scanning

Mark updated rows as counted during Stock Counting – self-explanatory

Hide In Warehouse Quantity Information – hides quantities on the Item lines (click here to learn more).

## Usage

### Interface

CompuTec WMS → Stock Counting:

![Start](./media/new-stock-counting-main-menu.png)

![Select](./media/select-stock-counting.png)

Click the x icon to go back or the + icon to add another document. You can also choose an already created Stock Counting:

![Select Stock Counting](./media/new-stock-counting-list.png)

![Select Stock Counting](./media/new-stock-counting-list-of-document.png)

To add a new Stock Counting document, click the plus icon, type in its name, and click the save icon (lower right corner):

![Add Stock Counting](./media/adding-new-stock-counting.png)

Click the left icon to go back or the right icon to save.

You can edit the name or delete the document by clicking the highlighted icon and then the i icon:

![Document Details](./media/document-details-options.png)

![Document Details](./media/document-details-info.png)

![Edit Stock Counting](./media/stock-counting-delete-document.png)

Deleting a document does not cause a status change in SAP Business One (you cannot reverse the process):

![Close Counting](./media/to-close-stock-counting.png)

Closing the document in SAP Business One deletes the Stock Counting document in CompuTec WMS:

![Stock Counting Status](./media/stock-counting-status.png)

The following document can have the same name, but there cannot be two or more with the same name at the same time:

![Stock Counting Exist](./media/stock-counting-exist.png)

You can browse the list or use the filter option to find a specific document:

![Select Stock Counting](./media/stock-counting-filer.png)

Leaving the document does not delete already set quantities.

Saving to SAP Business One is planned to be performed through the AppEngine plugin. Now, to do this, use the save icon:

![Document Details](./media/document-details-save.png)

After that, you get a confirmation:

![Save Stock Counting](./media/save-stock-counting-to-sap.png)

### Adding new Items to the Stock Counting list

Manually

Choose a Stock Transfer document, click the list icon, and click the plus icon.

![Document Details](./media/stock-counting-adding-items.png)

Choose a Warehouse (or a Warehouse and a Bin location) for the Stock Counting (this has to be done for each of the Items):

![Warehouse and Bin](./media/stock-counting-bin.png)

![Warehouse and Bin](./media/stock-counting-bin-add.png)

Choose an Item and click the plus icon:

![New Item](./media/stock-counting-new-item.png)

![Counted quantity](./media/stock-counting-new-item-quantity.png)

Set quantity and click the save icon:

![Quantity](./media/stock-counting-new-item-quantity-save.png)

The Item is now present in the Stock Counting view:

![Document Details](./media/stock-counting-new-item-document-details.png)

You can edit the quantity for an Item line in two ways:

![Counted Quantity](./media/stock-counting-counted-quantity.png)

Remove the line with its quantity by clicking this icon:

![Quantity](./media/stock-counting-counted-quantity-add2.png)

The confirmation:

![Confirmation](./media/stock-counting-delete-item.png)

Adding an Item managed by Batch (a Warehouse has to be chosen every time):

![New Item](./media/stock-counting-add-item.png)

![Batches](./media/stock-counting-add-batch.png)

Type in the Batch name and click the save icon:

![Quantity](./media/stock-counting-quantity.png)

![Document Details](./media/stock-counting-quantity-line.png)

You can edit the Batch quantity by entering its line (you cannot change the Batch name now, but it is possible to delete it along with the counted quantity by clicking the icon next to the save icon).

![Batches](./media/stock-counting-batch.png)

![Quantity](./media/stock-counting-batch-quantity.png)

![Confirmation](./media/stock-counting-delete-batch.png)

You can add another Batch by clicking the plus icon.

![Batches](./media/stock-counting-add-batch-plus.png)

![Quantity](./media/stock-counting-add-batch-plus2.png)

The counter on the Document Details form shows a sum of quantity from all of the Batches of this Item.

![Batches](./media/stock-counting-batch-line.png)

![Stock Counting](./media/stock-counting-batch-details.png)

Adding an Item managed by Serial Numbers:

Choose a Warehouse, then a Serial Number Item, and click the plus icon:

![New Item](./medi/stock-counting-new-item-line.png)

![Serials](./media/stock-counting-new-item-plus.png)

Type in the Serial Number and click the save icon:

![Serial](./media/stock-counting-new-serial-plus.png)

It is not possible to change the Serial Number name. You can only remove it by clicking its line and then the icon next to the save icon:

![Serials](./media/stock-counting-delete-serial.png)

![Serial](./media/stock-counting-delete-serial2.png)

You can add another Serial Number by clicking the plus icon:

![Serials](./media/stock-counting-plus.png)

Adding quantity for a specific Item is performed by entering its line.

If a specific Item is present in another Warehouse or Bin location, you have to add it again with the required Warehouse and Bin location.

![Document Details](./media/stock-counting-serial-another-warehouse.png)

![Document Details](./media/stock-counting-serial-another-warehouse2.png)

### Information on the Item lines

![Document Details](./media/stock-counting-serial-item-line-information.png)

You can hide the Warehouse quantities by checking the Hide in Warehouse Quantity Information in Custom Configuration.

### Adding Storage Units

You can add new or already existing SU and edit Items and their quantities. You can also create multi-level SUs.

Important: Items added to SUs are unavailable in the Items list. They are available after entering a specific SU.

If a specific Item is added outside of an SU, it will be added to the total counted quantity:

![Document Details](./media/stock-counting-serial-adding-sus2.png)

![SU Document Details](./media/stock-counting-serial-adding-sus.png)

![Counted quantity](./media/stock-counting-serial-adding-sus3.png)

Use this icon to add an SU:

![Document Details](./media/stock-counting-serial-document-details-menu.png)

In the following form, you can see already added SUs, and you can add a new one by clicking the plus icon.

![List of SUs](./media/stock-counting-adding-sus.png)

![Add SU](./media/stock-counting-adding-sus2.png)

If you do not put anything in the SU Code or SSCC field and click the right arrow, a new SU will be created. Then choose a Warehouse and a Bin location (if required).

Choose the newly created SU in the List of SUs:

![List of SUs](./media/stock-counting-created-su.png)

![SU Document Details](./media/stock-counting-created-su-details.png)

Use this icon to remove an SU from the list (this does not cause the removal of an SU from the system):

![SU Document Details](./media/stock-counting-created-su-details2.png)

You can delete or edit each Item by entering its line.

### Adding already existing SUs

Type SSCC or SU Code (you can also scan a related barcode).

CompuTec WMS checks if the SU exists, is already added, and is already added to another document.

![SU not found](./media/stock-counting-created-su-not-found.png)

![SU already exists](./media/stock-counting-created-su-exist.png)

![SU already exists](./media/stock-counting-created-su-exist-in-another-sc.png)

After scanning, choose a Warehouse and Bin location (if required). If the SU was present in another Warehouse and now is in a different one, it can be fixed here.

![Warehouse](./media/stock-counting-created-warehouse-bin.png)

The following steps are the same as in the case of creating a new SU.

![List of SUs](./media/stock-counting-list-of-sus.png)

![SU Document Details](./media/stock-counting-list-of-sus-document-details.png)

Add an Item by clicking the plus icon:

![SU Document Details](./media/stock-counting-list-of-sus-document-details-plus.png)

The Warehouse choosing step is skipped because a Warehouse was already selected from during the SU creation.

![New Item](./media/stock-counting-new-item-list.png)

Similarly, you can add three types of Items: Serial-managed Items, Batch-managed Items, Items without Serial Numbers, or Batch.

The way of adding an Item is the same as in the case of adding Items that are not present in SUs.

![SU Document Details](./media/stock-counting-su-document-details.png)

You can change the location of an SU (with its content) by clicking the following icon and choosing another Warehouse (this applies only to the highest-level SUs):

![SU Document Details](./media/stock-counting-su-document-details-warehouse.png)

![Warehouse and Bin](./media/stock-counting-su-document-details-warehouse-save.png)

![SU Document Details](./media/stock-counting-su-document-details-warehouse-date.png)

You can add an SU to another SU by clicking this icon:

![SU Document Details](./media/stock-counting-su-second-level-su.png)

You can add an existing SU or click the right arrow icon to create a new one.

![Add SU](./media/stock-counting-su-exisitng.png)

You can access a lower-level SU by entering its line in the higher-level SU:

![SU Document Details](./media/stock-counting-su-line.png)

Here you can delete only a lower-level SU (with its content):

![SU Document Details](./media/stock-counting-su-remove.png)

Adding Items works the same way as in the highest-level SU case.

### Scanning

You can scan an SU barcode only in the Add SU form:

![Add SU](./media/stock-counting-scan-su.png)

Prefix 93 for an SU Code, e.g. (93)00000000000000000016

Prefix 00 for an SSCC, e.g. (00)0000000000000154

Upon scanning a code, you will get information (not present in the system or already added in this or another document), or the system will move to a related Warehouse.

Choosing an already added SU in the List of SUs form:

![List of SUs](./media/stock-counting-scan-list-of-sus.png)

Adding Items by scanning:

Possible cases:

In the Document details form:

![Document Details](./media/stock-counting-scan-adding-items-by-scanning.png)

Scan a Warehouse code, an Item code and a quantity code.

You can add a Warehouse along with the Bin location in the code.

![Quantity](./media/stock-counting-scan-adding-items-warehouse-bin.png)

![Quantity](./media/stock-counting-scan-adding-items-warehouse-bin2.png)

Click the save icon to approve.

Scanning with the 01(GS1GTIN) code:

![Quantity](./media/stock-counting-scan-adding-items-prefix-01.png)

Item code and quantity scanning:

![Document Details](./media/stock-counting-scan-adding-items-quantity.png)

Scan quantity always after entering an Item line:

![Counted Quantity](./media/stock-counting-scan-adding-items-quantity-item-line.png)

![Quantity](./media/stock-counting-scan-adding-items-quantity-item-line2.png)

Batch scanning:

Warehouse, Item, Batch, and Quantity:

![Quantity](./media/stock-counting-scan-warehouse-item-batch-quantity.png)

![Document Details](./media/stock-counting-scan-warehouse-item-batch-quantity2.png)

Batch and quantity:

![Batches](./media/stock-counting-scan-warehouse-batch-quantity.png)

Only quantity:

![Quantity](./media/stock-counting-scan-quantity.png)

Only Batch:

![Quantity](./media/stock-counting-scan-batch.png)

Scanning a Serial Number:

Warehouse, Item, Serial Number.

![Serials](./media/stock-counting-scan-warehouse-item-serial.png)

Item and Serial Number.

![Serials](./media/stock-counting-scan-item-serial.png)

Only Serial Number in the Serial Numbers form and when adding a new one:

![Serials](./media/stock-counting-scan-serial.png)

![Serials](./media/stock-counting-scan-serial2.png)
