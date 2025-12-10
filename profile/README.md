> **Status:** 🚧 Draft — open to feedback and improvement.  
> This document will evolve as our community grows.  

# localcompose

**localcompose** is an umbrella above a toolset for running local Docker Compose apps in an offline-friendly, no-cloud-required way.  
It helps you stop juggling ports and IPs like `127.0.0.1:9000`, giving each app a clean domain name and a trusted HTTPS link.  
With minimal setup, your **local tools** feel like real websites — easier to browse, test, and connect across your system.

For example, you can turn `http://localhost:9000/` into `https://portainer.locom.self` — 
no cloud, no port hassle, just localhost done right.
Moreover, it's just as easy to map services like `http://it-tools:8080/` or `http://stirling-pdf:8080/` 
to clean HTTPS domains such as `https://it-tools.locom.self` and `https://stirling-pdf.locom.self`.
This makes them ready to install under Chrome's "Cast, Save, and Share" options — 
effectively turning your compose-stacked local tools into desktop-like applications.

🔧 Current focus:  
[`locom`](https://github.com/localcompose/locom) is the flagship tool in our ecosystem — a command-line orchestrator for local-only Docker Compose workflows.  
Currently on hold pending prerequisites, it remains our central focus, and its status is tracked transparently in the roadmap.

💡 Vision:  
Support developers, testers, and tinkerers who prefer local, private, and reliable environments — without unnecessary cloud complexity.  
See [strategic pyramid](../docs/strategic-pyramid.md) for visualization.

---

📌🔭 _This project and related repositories evolve at different paces.  
Some may be on hold (warm or cold), with their current **status** and context documented transparently in the [roadmap](https://github.com/orgs/localcompose/projects/5/views/4).  
Contributors and feedback are always welcome — watch [the `locom` repo](https://github.com/localcompose/locom) for updates!_

---

> 🧩 **Note:**  
> The policies and templates in this `.github` repository are **drafts**.  
> They are expected to evolve as our organization and projects
(like [_`locom`_](https://github.com/localcompose/locom) and [_`fastreleaser`_](https://github.com/localcompose/fastreleaser))
mature.  
> Suggestions and pull requests to improve them are **warmly welcome** — please open an
[issue](https://github.com/localcompose/.github/issues/new)
or [PR](https://github.com/localcompose/.github/edit/main/profile/README.md) in this repository.
>
> See also: [Meta repository of `localcompose` organization](https://github.com/localcompose/.github)
