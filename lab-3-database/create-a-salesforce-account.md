# Create a Salesforce account

* Go to [https://developer.salesforce.com/signup](https://developer.salesforce.com/signup) and create a free developer account.

![](../.gitbook/assets/image%20%2820%29.png)

* Go to your mail inbox and confirm the new account.
* Set a password for the account.
* Login to your Salesforce account.
* Click on the **Profile** icon \(upper-right side\).
* Click on the **`Switch to Salesforce Classic`** link.

![](../.gitbook/assets/image%20%2870%29.png)

* Click on the **`Setup`** link

![](../.gitbook/assets/image%20%28100%29.png)

* Go to the **Build** section and expand **Create**.
* Click on the **Apps** link.

![](../.gitbook/assets/image%20%286%29.png)

* Scroll down to the **Connected Apps** section.
* Click on the **`New`** button.

![](../.gitbook/assets/image%20%28134%29.png)

* Enter the following values:

| Connected App Name | IgniteApp |
| --- | --- | --- |
| API Name | IgniteApp |
| Contact Email | _&lt;any email address&gt;_ |

![](../.gitbook/assets/image%20%2834%29.png)

* Scroll down to the **API \(Enable OAuth Settings\)** area.
* Click on the **`Enable OAuth Settings`** checkbox.
* Add the following **OAuth Scopes**:

  * **`Access and manage your data (api)`**
  * **`Perform requests on your behalf at any time(refresh_token,offline_acces)`**

![](../.gitbook/assets/image%20%281%29.png)

* Click on the **`Enable for Device Flow`**checkbox.
* Enter `https://fuse-ignite.ignite1.rhtechofficelatam.com/api/v1/credentials/callback` as **Callback URL.**

![](../.gitbook/assets/image%20%289%29.png)

* Click on the **`Save`** button.

![](../.gitbook/assets/image%20%284%29.png)

* Take note of the **Consumer Key** and **Consumer Secret** \(you will need them later\).

![](../.gitbook/assets/image%20%2877%29.png)
