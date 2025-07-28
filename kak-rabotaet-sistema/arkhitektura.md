# Architecture

<div data-full-width="false"><figure><img src="../.gitbook/assets/Безымянный-2025-05-20-1537 (1).png" alt=""><figcaption></figcaption></figure></div>

_<mark style="color:purple;">**Gateway**</mark>_ - Nginx for distributing requests to multiple servers

_<mark style="color:blue;">**PostgeSQL**</mark>_ - database (...)

_<mark style="color:purple;">Frontend</mark>_ - For the interface Nginx (JS, React)

_<mark style="color:orange;">Backend</mark>_ - API (Kotlin, Spring)

_<mark style="color:blue;">**\*\*\*\* checker**</mark>_ - service for checking tasks in the required language (Java, Javalin)