# Production Setup

## Docker

{% hint style="warning" %}
If Docker has not been installed before, please install it. Nothing will work without it [\[Installation Guide Link\]](https://docs.docker.com/engine/install/)
{% endhint %}

### Set Environment Variables

Example: [https://github.com/CodeBattles-nn/codebattles/blob/new_backend/.env.example](https://github.com/CodeBattles-nn/codebattles/blob/new_backend/.env.example)

{% code title=".env.example" lineNumbers="true" %}
```properties
DB_USER=dfvdsdfvsdswvdfvdsvdfvdf
DB_PASSWORD=dvnsevhjeiwurowuqvhjevfvuodfb
DB_NAME=cb

```
{% endcode %}

{% stepper %}
{% step %}
### Create a .env File

The structure can be found in .env.example
{% endstep %}

{% step %}
### Set Complex Settings

In the .env file
{% endstep %}
{% endstepper %}

### Select Your Architecture

{% tabs %}
{% tab title="x64" %}
To install, you need to download the repository and deploy the Docker compose Container

pulling images from the repository:

```bash
docker compose -f prod-docker-compose.yml pull
```

starting:

```sh
docker compose -f prod-docker-compose.yml up
```

{% endtab %}

{% tab title="other" %}
To install, you need to download the repository and deploy the Docker compose Container

building images:

```bash
docker compose -f prod-docker-compose.yml build
```

starting:

```sh
docker compose -f prod-docker-compose.yml up
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
To run containers in the background, use the _<mark style="color:blue;">**-d**</mark>_ flag

Example:

{% code fullWidth="false" %}
```bash
docker compose up -f prod-docker-compose.yml -d
```
{% endcode %}
{% endhint %}

After this, please configure the programming languages. This is described on the next page