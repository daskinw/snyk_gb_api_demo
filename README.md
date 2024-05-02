# Snyk API Docs Demo

{% synced-block url="https://app.gitbook.com/o/-MA1LVuAa2r7iEH23aFf/synced-block/syb_wrng0" %}
[Untitled](https://app.gitbook.com/o/-MA1LVuAa2r7iEH23aFf/synced-block/syb\_wrng0)
{% endsynced-block %}

## Create a new user

<mark style="color:green;">`POST`</mark> `/users`

\<Description of the endpoint>

**Headers**

| Name          | Value              |
| ------------- | ------------------ |
| Content-Type  | `application/json` |
| Authorization | `Bearer <token>`   |

**Body**

| Name   | Type   | Description      |
| ------ | ------ | ---------------- |
| `name` | string | Name of the user |
| `age`  | number | Age of the user  |

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "id": 1,
  "name": "John",
  "age": 30
}
```
{% endtab %}

{% tab title="400" %}
```json
{
  "error": "Invalid request"
}
```
{% endtab %}
{% endtabs %}

{% swagger src=".gitbook/assets/snyk_api.json" path="/custom_base_images" method="get" %}
[snyk_api.json](.gitbook/assets/snyk_api.json)
{% endswagger %}

{% swagger src=".gitbook/assets/snyk_api.json" path="/custom_base_images/{custombaseimage_id}" method="get" %}
[snyk_api.json](.gitbook/assets/snyk_api.json)
{% endswagger %}

{% swagger src=".gitbook/assets/snyk_api.json" path="/groups/{group_id}/apps/installs/{install_id}" method="delete" %}
[snyk_api.json](.gitbook/assets/snyk_api.json)
{% endswagger %}

{% swagger src=".gitbook/assets/snyk_api.json" path="/groups/{group_id}/audit_logs/search" method="get" %}
[snyk_api.json](.gitbook/assets/snyk_api.json)
{% endswagger %}
