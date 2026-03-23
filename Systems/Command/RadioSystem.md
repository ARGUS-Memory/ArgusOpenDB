[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Command](README.md) > Radio System

# Radio System

Station communications rely on a radio network covering both internal departments and ship-to-ship space frequencies. Each department operates on a dedicated encrypted channel, with a shared common frequency available to all crew. Encryption keys restrict who can transmit and receive on departmental channels.

---

## Frequency Reference

All frequencies are listed in kHz. The public range runs from 1441 to 1489 kHz. Frequencies outside this range are restricted to specific organizations.

| Frequency | Channel | Description |
|---|---|---|
| 1459 | Common | General crew communications; all headsets receive by default |
| 1353 | Command | Command staff and heads of staff |
| 1359 | Security | Security department |
| 1357 | Engineering | Engineering department |
| 1355 | Medical | Medical department |
| 1351 | Science | Research and science |
| 1349 | Service | Service department |
| 1347 | Supply | Cargo and supply |
| 1361 | Exploration | Exploration and away teams |
| 1485 | Medical (internal) | Medical secure channel |
| 1475 | Security (internal) | Security secure channel |
| 1461 | Entertainment | Station entertainment and events |
| 1345 | Emergency Response | Emergency Response Team; restricted |
| 1213 | Syndicate | Syndicate operative network; restricted |

### Channel Prefixes

When transmitting on a departmental channel, the radio system prefixes the message with the channel name. Default headset transmits on Common (no prefix). Encrypted key required to access departmental channels.

---

## Encryption Keys

Encryption keys slot into headsets to grant access to departmental channels. A standard headset has two key slots. Keys can be inserted and removed by hand.

| Key | Channels unlocked |
|---|---|
| Command | Command, Supply, Service, Security, Medical, Engineering, Science, Exploration |
| Captain | All departmental channels + AI Private |
| Security | Security |
| Engineering | Engineering |
| Medical | Medical |
| Science | Science |
| Service | Service |
| Supply | Supply, Service |
| Exploration | Exploration |
| Head of Personnel | Supply, Service, Command, Security, Exploration |
| Pathfinder | Exploration, Command |
| Pilot | Exploration, Engineering |
| Search and Rescue | Exploration, Medical |

Heads of staff carry multi-channel command keys that cover all relevant departments in their chain of command. The Captain and AI integrated headsets cover all channels simultaneously.

> [!NOTE]
> Holding a key does not grant physical access rights. Key possession is a matter of communications access only. Unauthorized possession of a departmental key is a security concern but is not itself an access violation.

---

## Headset Types

Each department issues three physical headset form factors: a standard over-ear headset, a bowman headset (worn as a collar or jaw mount), and an earbud. All three forms function identically. The encryption key preinstalled determines the default departmental channel; keys can be swapped if the wearer has physical access to the appropriate key.

| Department | Standard | Bowman | Earbud |
|---|---|---|---|
| General issue | Headset | Bowman headset | Earbud |
| Security | Security headset | Security bowman | Security earbud |
| Engineering | Engineering headset | Engineering bowman | Engineering earbud |
| Medical | Medical headset | Medical bowman | Medical earbud |
| Science | Science headset | Science bowman | Science earbud |
| Service | Service headset | Service bowman | Service earbud |
| Supply | Supply headset | Supply bowman | Supply earbud |
| Exploration | Exploration headset | Exploration bowman | Exploration earbud |
| Mining | Mining headset | -- | -- |

Mining headsets and exploration variants carry an **ad-hoc fallback** mode: when the primary station antenna is out of range or offline, these headsets fall back to short-range direct-band transmission between nearby units. This allows minimal communication within a working party even if station comms are down.

---

## Handheld Radio

Handheld radios can transmit and receive on any frequency without an encryption key, but do not decrypt locked channels. To transmit on a frequency the operator tunes the radio by hand. Handheld radios are useful for communicating on frequencies where no key is available, broadcasting general announcements, or communicating with parties who lack headsets.

Handheld radios cannot be worn; they must be held in hand or placed on a surface to transmit. They function identically to headsets in terms of range within the station.

---

## Intercoms

Wall-mounted intercom units are installed throughout the station at key locations. An intercom broadcasts to all crew within the local area and can also be set to transmit on the common frequency or any tuned frequency. Intercoms cannot be encrypted; anyone in range can hear and respond.

Intercoms are activated by clicking them. Volume and frequency can be adjusted with a screwdriver on the back panel. Intercoms can be used to communicate between areas without a headset, make local announcements, or broadcast emergency warnings.

---

## AI Integration

The station AI has integrated radio access covering all departmental frequencies simultaneously without requiring physical keys. The AI can monitor and transmit on any channel. AI radio access cannot be restricted through key management; disabling AI communications requires either a law-based order or direct hardware interference with the AI core.

---

*See also: [Chain of Command](../Command/ChainOfCommand.md), [Standard Operating Procedure](StandardOperatingProcedure.md), [Paperwork System](Paperwork.md)*
