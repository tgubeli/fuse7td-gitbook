# Create an AMQ to API integration

* Click on the **`Integrations`** tab.
* Click on the **`Create Integration`** button.

![](../.gitbook/assets/image%20%2878%29.png)

* Select **`AMQ Broker`** as the start connection.
* Select the **`Subscribe for messages`** action.

![](../.gitbook/assets/image%20%28132%29.png)

* Enter the following values:

| **Destination name** | invoices |
| --- | --- |
| **Destination Type** | Queue |

* Click on the **`Next`** button.

![](../.gitbook/assets/image%20%28156%29.png)

* Click on the **`Done`** button.
* Select the **`OpenCRX-Leads`** connection.
* Select the **`POST /invoice`** action**.**

![](../.gitbook/assets/image%20%2819%29.png)

* Click on the **`Done`** button**.**
* Hover over the **+** icon and click on the  **Add a Step** link.
* Select the **Log** step.

![](../.gitbook/assets/image%20%28140%29.png)

* Check **`Message Body`**.
* Enter "**`INVOICE`**" as **Custom Text.** 
* Click on the **`Done`**  button.

![](../.gitbook/assets/image%20%28120%29.png)

* Hover over the **+** icon and click on the **Add a Step** link.
* Select the **`Split`** step.
* Enter the following values:

| **Expression** | //invoice |
| --- | --- |
| **Language** | xpath |

* Click on the **`Done`** button.

![](../.gitbook/assets/image%20%2875%29.png)

* Hover over the **+** icon and click on the **`Add a connection`.**
* Select **`DataShape`** connector.
* Select the **`Datashape Endpoint`** action.
* Click on the **`Next`** button.
* Select **`XML Instance`** as the **Output Data Type.**
* Copy and paste **Labs\lab5\invoice.xml** into the definition field.
* Enter**`InvoiceXML`** as the **Data Type Name.**
* Click  on the **`Done`** button.

![](../.gitbook/assets/image%20%2884%29.png)

* Click on the **warning** icon in the **finish** connector.
* Click on the **`Add a data mapping step`** link.

![](../.gitbook/assets/image%20%2877%29.png)

* Expand **InvoiceXML** -&gt; **invoice** in the **Source** data structure.
* Expand **Request -&gt; body -&gt; org.opencrx.kernel.contract1.Invoice** in the **Target** data structure.

![](../.gitbook/assets/image%20%2843%29.png)

* Perform the following mappings:

| invoiceDescription | description |
| --- | --- | --- | --- | --- | --- |
| invoiceName | name |
| @number | contractNumber |
| totalAmountIncludingTax | totalAmountIncludingTax |
| totalBaseAmount | totalBaseAmount |
| totalTaxAmount | totalTaxAmount |

![](../.gitbook/assets/image%20%2880%29.png)

* Click on the **+** icon in the **`Constants`** tab.

![](../.gitbook/assets/image%20%28111%29.png)

* Enter the following:

| **Value** | true |
| --- | --- |
| **Value Type** | Boolean |

* Click on the **`Save`** button.

![](../.gitbook/assets/image%20%2894%29.png)

* Click on the **`true`** constant and map it to **`noAutoRecalc`**.

![](../.gitbook/assets/image%20%28119%29.png)

* Click on the **`Done`** button.
* Click on the **`Publish`** button.
* Enter **"`AMQtoAPI`"** as integration name.
* Click on the **`Publish`** button.





