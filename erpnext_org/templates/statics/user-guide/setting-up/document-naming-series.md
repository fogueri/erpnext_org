Data records are broadly classified as “Master” or “Transaction”. A master
record is a record that has a “name”, for example a Customer, Item, Supplier,
Employee etc. A Transaction is a record that has a “number”. Examples of
transactions include Sales Invoices, Quotations etc. You make transactions
against a number of master records.

ERPNext allows you to make prefixes to your transactions, with each prefix
forming its own series. For example a series with prefix INV12 will have
numbers INV120001, INV120002 and so on.

You can have multiple series for all your transactions. It is common to have a
separate series for each financial year. For example in Sales Invoice you
could have:

  * INV120001
  * INV120002
  * INV-A-120002

etc. You could also have a separate series for each type of Customer or for
each of your retail outlets.

To setup a series, go to:

> Setup > Tools > Update Numbering Series

![Document Naming Series](assets/erpnext_org/images/erpnext/naming-series.png)

In this form,

  1. Select the transaction for which you want to make the series The system will update the current series in the text box.
  2. Edit the series as required with unique prefixes for each series. Each prefix must be on a new line.
  3. The first prefix will be the default prefix. If you want the user to explicitly select a series instead of the default one, check the “User must always select” check box.

![Document Numbering Series](assets/erpnext_org/images/erpnext/naming-series-1.png)

You can also update the starting point of a series by entering the series
name and the starting point in the “Update Series” section.

For Example: If you wish to change the prefix of a Delivery Note follow the following process.

Step 1: Go to Setup.

Step 2: Click on Update Numbering Series.

Step 3: Under Select Transaction; Select the Document you wish to give new series name, example: Delivery Note.

Step 4: Under Series List for the Transaction: Type the required Series type. For Example, DE/.DD./.MM./.YY./.##### 

Step 5: Click on Update button. Go to the respective document and select your series. You will get this series DE/09/01/13/00001 where 09 is the day, 01 is the month and 00001 is the series.