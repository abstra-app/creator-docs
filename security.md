---
description: This page explains how Abstra applications work and how we deal with security
---

# Security

![](<.gitbook/assets/image (51).png>)

Abstra is mostly a frontend editor, that said, almost all sensitive data you deal with your applications are not stored with us. In fact, most of it does not even pass through our servers.

There are some exceptions:

* Data stored using our [hosted tables](docs/front-end/actions/hosted-tables.md). Each application has it own database. We don't apply any automatic encryption, therefore, **never store passwords or other sensitive data before talking to us**.
* Backend connectors. Credentials and connections are done by our backend. In this case, **we don't collect any data that passes through** our serves.

As with any development platform, you should always be aware of best security practices, such as:

* **Never store API credentials on the frontend** because these configurations are client-side.
* Be mindful that **page protection is client-side**, therefore you should **always protect your connectors and queries**.
* Be sure to use only HTTPS/encrypted endpoints, even with backend connectors.
* All page URLs are accessible even if there is no link to them in the application. The same is appliable to components not in use.

We apply industry best standards to store and protect data when needed, but we strongly recommend getting in touch before using any sensitive data with Abstra apps, so we can help you to configure using the safest practices.
