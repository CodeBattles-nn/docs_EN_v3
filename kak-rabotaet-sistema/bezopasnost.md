# Security

<figure><img src="../.gitbook/assets/Безымянный-2025-05-20-1537 (2).png" alt=""><figcaption></figcaption></figure>

The Codebattles platform ensures the security of executable programs using several tools.

### Docker

[**Docker**](https://www.docker.com) - an application for containerization.

The checker application runs in an isolated container. The checkers' container network is launched in isolation from the general subnet.

### Bubblewrap

[**Bubblewrap**](https://github.com/containers/bubblewrap) - a sandbox for applications. Used, for example, in [Flatpak](https://flatpak.org/)

Within Docker, a sandbox with network and file system isolation is used.

***

Using the above methods of protection from malicious actors, one can be confident in the system's security.