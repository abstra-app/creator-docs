# Redirect Sign in/Sign up

The `Redirect Sign in / Sign up` action is used to sign in your application's users.

![](<../../../.gitbook/assets/image (56).png>)

You can choose page that the user will be redirected to after a successful login or a failed login.

![](<../../../.gitbook/assets/image (65).png>)

{% hint style="warning" %}
**Warning**. When using this action in the preview mode (inside the project editor) the behaviour will be different from releases and production: on the preview mode this action will behave just like the [Popup Login](sign-in-sign-up.md) action. When in releases or production it will redirect to the login page instead of opening the popup.
{% endhint %}

After the `Redirect Sign in / Sign up` action execution the `user` and `error` variables will be exposed and can be used to do operations with other actions.
