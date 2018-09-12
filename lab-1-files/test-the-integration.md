# Test the integration

* Using an FTP client, or a web-based console if available, log in and navigate to the root directory of your web hosting service account.

* Navigate to the **./htdocs** subdirectory and create 2 folders: **incoming** and **outgoing** folders.

* Then navigate to the **incoming** folder.

* Upload **Labs\Lab1\file1.xml** to the FTP server.

* Now navigate to the **outgoing** folder.
* You should have a file with the current date as filename.

* Go back to **Fuse Ignite**  console.
* Click on the **`Integrations`** tab.
* Click on the **`Activity`** tab.

![](../.gitbook/assets/image%20%28156%29.png)

{% hint style="success" %}
Notice that there's been one activity in the deployed integration
{% endhint %}

* Click on the **`Metrics`** tab.

![](../.gitbook/assets/image%20%28163%29.png)

{% hint style="success" %}
In the metrics section, you can see one message has been processed by the deployed integration.
{% endhint %}

