### `rtc_client_connected`

This option allows applications to show when a user enters the RTC session. When used in combination with [`rtc_client_disconnected`](#rtc_client_disconnected), a user interface of connected users can be kept up to date.

Only one `rtc_client_connected` event will be fired per client connection. Connecting to a session with multiple existing clients will fire separate `rtc_client_connected` events for each existing client. If a user connects using two or more editors (such as on desktop and on mobile), a separate `rtc_client_connected` event will be fired.

To help with generating a user interface for connected users, an object for user details is provided by the [`rtc_user_details_provider`](#rtc_user_details_provider) option.

{% if plugincode != "rtc" %}
Required plugin
: [Real-time Collaboration (`rtc`)]({{site.baseurl}}/plugins/premium/rtc/)
{% endif %}

Type
: Function

Input parameters
: {% include rtc/rtc-client-connect-inputs.md %}

> **Caution**: {{site.productname}} cannot guarantee the accuracy of data which comes from a remote object. {{site.companyname}} recommends only using the client information data for status flags. To obtain authentic client information, use the [`rtc_user_details_provider`](#rtc_user_details_provider) data returned through the `userDetails` field.

{% include rtc/rtc-client-connect-disconnect-example.md %}