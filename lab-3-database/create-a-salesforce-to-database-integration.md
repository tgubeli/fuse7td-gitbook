# Create a Salesforce to Database integration

* Click on the **`Integrations`** tab.
* Click on the **`Create Integration`** button.
* Select  **IgniteSalesforce** as start connection.

![](../.gitbook/assets/image%20%285%29.png)

* Select **`On Create`**action**.**
* Select **`Contact`** as **Object** **name**.
* Click on the **`Done`** button.

![](../.gitbook/assets/image%20%28156%29.png)

* Select **`IgniteDB`** as finish connection.

![](../.gitbook/assets/image%20%2867%29.png)

* Select **`Invoke SQL`** as action.
* Enter the following value:

| **SQL Statement** | INSERT INTO Contacts\(first\_name,last\_name,email,lead\_source\) values\(:\#first,:\#last,:\#email,:\#lead\) |
| --- |


* Click on the **Done** button.

![](../.gitbook/assets/image%20%28134%29.png)

* Click on the warning icon next to the **INVOKE SQL** connection.
* Click on the **Add a data mapping step** link.

![](../.gitbook/assets/image%20%2832%29.png)

* Perform the following mappings:

| **Source** | **Target** |
| --- | --- | --- | --- | --- |
| FirstName | first |
| LastName | last |
| Email | email |
| LeadSource | lead |

* Click on the **`Done`** button.

![](../.gitbook/assets/image%20%2885%29.png)

* Click on the **Publish** button.
* Enter **SalesforceToDB** as **Integration Name.**
* Click on the **Publish** button.

![](../.gitbook/assets/image%20%28149%29.png)





