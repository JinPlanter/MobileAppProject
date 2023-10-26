Table of Contents:
* [Architectural Decision Record (ADR)](#architectural-decision-record-adr)
  * [Hardware](#hardware)
    * [Context](#context)
    * [Decision](#decision)
    * [Rationale](#rationale)
    * [Consequences](#consequences)

# Architectural Decision Record (ADR)
## Hardware

### Context

- Due to the fact that mobile phones come with hardware, we should look into the possibility of using them for our mobile app.

### Decision

- After some deliberation, we have decided that the only hardware features we need is touch screen functionality and local storage. The touch screen is for the user to interact with our application, while the local storage is to hold all the user information. There is no need for speakers, a fingerprint scanner or other hardware features.

<br/>

### Rationale

- Our app does not need a lot of the hardware components as it is an app that calculates expenses (which is done using the software components)

<br/>

### Consequences

- There will be no negative, nor positive consequences.
