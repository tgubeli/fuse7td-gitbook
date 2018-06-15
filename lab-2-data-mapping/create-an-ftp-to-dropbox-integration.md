# Create an FTP to Dropbox Integration

* Click on the **`Integrations`** tab.
* Click on the **`Create Integration`** ``button.

![](../.gitbook/assets/image%20%28158%29.png)

* Select **`Openshift FTP`** as the start connection.

![](../.gitbook/assets/image%20%2884%29.png)

* Select the only available action: **`Download`**
* Enter the following values:

| File Name Expression | customer.xml |
| --- | --- | --- |
| FTP Directory | incoming |
| Delete file after download | Yes |

* Click on the **`Next`** button.

![](../.gitbook/assets/image%20%2849%29.png)

* Select **`XML Instance`** as **Type.**
* Paste the contents of the **Lab2\customer.xml** in the **`Definition`** field.

```text
<customer id="c1">
  <name>Pablo Szuster</name>
  <address>Ing. Butty 240</address>
</customer>
```

* Enter **`Customer`** as **Data Type Name**.
* Click on the **`Done`** button.

![](../.gitbook/assets/image%20%2862%29.png)

* Select **`DropboxIgnite`** as the finish connection.
* Select the only available action: **`Upload`**.
* Enter **`/customer.json`** as **Remote Path**.
* Click on the **`Next`** button.

![](../.gitbook/assets/image%20%28101%29.png)

* Select **`JSON Instance`** as **Type.**
* Paste the contents of **Lab2\customer.json** into the **Definition** field.

```text
{
"customer": {"id": "","firstName": "", "lastName": "","address":""}
}
```

* Enter **`Customer_JSON`** as **Data Type Name**.
* Click on the **`Done`** button.

![](../.gitbook/assets/image%20%2855%29.png)

{% hint style="warning" %}
Notice there is a warning icon next to the finish connection. This is because its input data shape is different than the start connector's output data shape.
{% endhint %}

* Click on the warning icon in the finish connection.
* Click on the ``**`Add a data mapping step`** link.

![](../.gitbook/assets/image%20%28147%29.png)

* Expand both the **Source** and **Target** data shapes.
* Click on the **@id** field in the **Source** data shape.
* Click on the **id** field in the **Target** data shape.

![](../.gitbook/assets/image%20%288%29.png)

* Click on the **address** field in the **Source** data shape.
* Click on the **address** field in the **Target** data shape.
* Click on the **`Add Transformation`** button.

![](../.gitbook/assets/image%20%28127%29.png)

* Select the **Uppercase** transformation.

![](../.gitbook/assets/image%20%2829%29.png)

* Click on the **name** field in the **Source** data shape.
* Click on the **firstName** field in the **Target** data shape.

![](../.gitbook/assets/image%20%28113%29.png)

* Go to the **Action** section in **Mapping Details.**
* Select **`Separate`** as the action.
* Leave the default separator \(Space\[ \]\).
* Click on the **`Add Target`** button.

![](../.gitbook/assets/image%20%28129%29.png)

* Click on the new **Target** field and enter "**lastName"**.
* Select the field suggestion

![](../.gitbook/assets/image%20%2865%29.png)

* Click on the **`Done`** button.
* Click on the **`Publish`** button.
* Enter **`FTP to DropBox`** as integration name.
* Click on the **`Publish`** button.

