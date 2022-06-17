---
toc: false
# disableReadmoreNav: true
draft: false
---

## Flow for Engineers

This methodology can be used as additional helper for [12-Factor app](https://12factor.net/) or can be used separately, as standalone practice. This methodology created by author [Sys-Adm.in](https://sys-adm.in) blog and is using in [Open BLD DNS](https://lab.sys-adm.in) project.

#### Main principles:

1. ### Automation

    Maximum coverage (if possible) of all aspects of using the application, examples of the main phases:

    * Assembly
    * Deploy
    * Deprecation
    * Configuration
    * Backup
    * Failover

    {{< alert style="info" >}} **Thesis**: Minimum human factor, automate be concise. {{< /alert >}}

2. ### Minimalism / Conciseness

    A minimum of third-party tools, a bias towards built-in tools in the platforms used (for example: bash on Linux, powershell on Windows, etc.). Close principles - KISS, Unix-way. The fewer components in the environment (points of failure), the better.

    {{< alert style="info" >}} **Thesis**: Make it simple, at minimum wages, but do not forget about safety. {{< /alert >}}

3. ### Security

    Approach examples:

    * Separation of powers
    * Granular Access
    * Using roles
    * Logging and notifications

    {{< alert style="info" >}} **Thesis**: More rake in the way of the attacker. {{< /alert >}}


4. ### Notifications

    Find out about the incident from a quick notification, the main principles are:

    * Granular triggering
    * Fast messaging
    * Messages within the nearest reach (for example, your favorite messenger)
    
    {{< alert style="info" >}} **Thesis**: Notify only about the important. {{< /alert >}}

5. ### Measurability

    Sets of internal metrics on which notification triggers or logged events are based. Examples:

    * Service stop
    * Port unreachable
    * Number of requests
    * CPU recycling

    {{< alert style="info" >}} **Thesis**: Have a minimum set of metrics to identify a problem or event. {{< /alert >}}

6. ### Self-healing

    Examples:

    * Service stopped - attempt to restart
    * Service unavailable - attempt to reconfigure
    * DoS / DDoS - an attempt to level or self-destruct

    {{< alert style="info" >}} **Thesis**: Internal monitoring (or self-diagnostics) for the purpose of self-healing or self-destruction (minimization of failover events). {{< /alert >}}

7. ### Flexibility

    Examples of flexibility:

    * Cross-platform
    * Unification
    * Binary applications (e.g. GoLang binaries)

    {{< alert style="info" >}} **Thesis**: Automation, conciseness, cross-platform give flexibility. {{< /alert >}}

8. ### Documentations

    Any kind/type of supporting documentation. Examples:

    * Self-documentation (for example: scripts, api, comments in the code, names of functions or methods, etc.)
    * Readme
    * Scheme / Diagram
    * Pen on paper
    * Photo (for example, a photo of the board where the diagrams were drawn during the discussion)
    * Screenshots
    * etc

