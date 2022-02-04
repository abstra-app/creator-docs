# Configuring the Password Grant Type with Auth0

This lesson closely follows the original [auth0 post](https://auth0.com/docs/get-started/authentication-and-authorization-flow/call-your-api-using-resource-owner-password-flow#prerequisites).

We assume you have followed the steps in [configuring auth0](auth-with-auth0.md).

### Extra configuration needed

Go to your dashboard on Auth0 and select your application:

![](<../../.gitbook/assets/Kapture 2022-02-04 at 10.57.17.gif>)

Scroll down and change your **application type** to `Regular Web Application`. Scroll more to **advanced settings** and **Grant Types** and enable the `Password` grant. Save the changes.

![](<../../.gitbook/assets/Kapture 2022-02-04 at 11.00.07.gif>)

Go to **Authentication** > **Database** and take note of the Username-Password database connection. In this example it is `Username-Password-Authentication.`

![](<../../.gitbook/assets/Kapture 2022-02-04 at 11.07.13.gif>)

Finally go to **Settings** and scroll down to **API Authorization Settings** and paste the connection name in the **Default Directory** field. Save it.

![](<../../.gitbook/assets/Kapture 2022-02-04 at 11.12.51.gif>)

Thats it. Now you can use the [Username/Password Login action](../../docs/front-end/actions/sign-in-with-usename-password.md)
