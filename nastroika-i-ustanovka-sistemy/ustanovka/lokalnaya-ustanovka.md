# Local Installation

{% hint style="danger" %}
For the current competitions, use the [Production mode](production-ustanovka.md). \
It has stricter security policies and does not contain development tools.
{% endhint %}

## Docker

{% hint style="warning" %}
If you haven't installed Docker before, please do so. Nothing will work without it [\[Installation Guide Link\]](https://docs.docker.com/engine/install/)
{% endhint %}

### Choose Your Architecture

{% tabs %}
{% tab title="x64" %}
To install, you need to download the repository and deploy the Docker Compose Container.

Downloading images from the repository:

```bash
docker compose pull
```

Start:

```sh
docker compose up
```

{% endtab %}

{% tab title="others" %}
To install, you need to download the repository and deploy the Docker Compose Container.

Building images:

```bash
docker compose build
```

Start:

```sh
docker compose up
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
To run containers in the background, use the _<mark style="color:blue;">**-d**</mark>_ flag

Example:

{% code fullWidth="false" %}
```bash
docker compose up -d
```
{% endcode %}
{% endhint %}

After this, please configure the programming languages. This is described on the next page.