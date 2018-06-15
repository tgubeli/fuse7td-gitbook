# Create an HTTP\(CSV\) to Red Hat Data Grid integration

* Click on the **`Integrations`** tab.
* Click on the **`Create Integration`** button.

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LDgEtlo1zua2etnJvxn%2F-LELUN0iQuZ-Lrgc8hhc%2F-LELUepgR8SpNSlYSgyo%2Fimage.png?alt=media&token=0f0657c7-c105-4e1d-aff8-e5142423f484)

* Select **`stockApp`** as the start connection.

![](../.gitbook/assets/image%20%2817%29.png)

* Select the only available action:  **`Periodic invoke URL.`**
* Enter the following values:

| **URL Path** | store\_1 |
| --- | --- |
| **Period** | 60 |

* Click on the **`Next`** button.

![](../.gitbook/assets/image%20%2823%29.png)

* Select **`RH Data Grid - Stock`** as the finish connection.
* Select the only available action:  **`Invoke URL`.**
* Enter the following values:

| **URL Path** | store\_1 |
| --- | --- |
| **Http Method** | PUT |

* Click on the **`Next`** button.
* Click on the **`Done`** button.
* 
