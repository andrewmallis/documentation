---
title: Configuring SAML SSO for Pantheon with Okta
description: Detailed information to enable SAML single sign-on for your organization with Okta.
category:
  - developing
---

Starting in the Okta admin dashboard area, do the following:

1. Login to Okta admin area
2. Select **Applications**
3. Click **Add Application**
4. Click **Create New App**
2. Select **SAML 2.0** and click **Create**
3. Name your app **Pantheon** and click **Next**
4. Fill in the following settings:
  * **Single sign on URL**: `https://dashboard.pantheon.io/saml/example.com/consume`
  <div class="alert alert-warning" role="alert"> <strong>Note:</strong>  Replace <code>example.com</code> with the domain you control</div>
  * **Audience URI (SP Entity ID)**: `https://dashboard.pantheon.io`
  * **Name ID format**: `EmailAddress`
  * **Application username**: `Email`
  ![Okta settings](/source/docs/assets/images/okta-4.png)
5.  Click **Show Advanced Settings** then select `Compressed` for **Request compression** and click **Next.**
 ![Okta settings](/source/docs/assets/images/okta-5.png)

6. Open a support ticket with Pantheon requesting SAML Setup for your Organization and provide the following information found in the Okta Pantheon app **Sign On** tab >> **View Setup Instructions**
 * **Identity Provider Single Sign-On URL**
 * **X.509 Certificate**


7. Coordinate a time with Pantheon Support to complete setup and ensure everything is working

## See Also
* [Single Sign-On for Pantheon Organizations](/docs/articles/organizations/saml-for-orgs/)
