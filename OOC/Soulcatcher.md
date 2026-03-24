[OOC Reference](README.md) > Soulcatcher

# Soulcatcher

A soulcatcher (soul gem) is a device that captures a consciousness from its physical body and contains it in a virtual interior space. The captured soul persists inside the device, aware and communicative, while the original body becomes mindless. This document covers the capture process, soul interaction capabilities, the virtual interior, and integration with NIF implants.

---

## Capture

Capturing a soul requires the target to have soulcatcher capture enabled in their personal preferences (SOULCATCHER_ALLOW_CAPTURE flag). A target who has opted out cannot be captured regardless of device capabilities.

When capture proceeds, a new mind container is created inside the soul gem and the target's consciousness is transferred into it. The original body remains in place but becomes unresponsive to direction. The soul is now inside the gem.

---

## Virtual Interior

The interior of a soul gem is a customizable private space. The predator (device holder) can set:

- **Interior description:** Text shown to captured souls describing their environment. Default is a small white room.
- **Capture message:** Shown to the soul at the moment of capture.
- **Release message:** Shown to the soul at release.
- **Transfer message:** Shown to the soul when moved to another device.
- **Deletion message:** Shown to the soul if the consciousness is destroyed.

The interior can be updated at any time while souls are inside.

---

## Soul Communication

Captured souls communicate through a private channel. Their speech appears to the device holder and to other souls in the same gem in a designated format: [SC] soul_name speaks, 'message'. Souls cannot use standard station radio or normal speech that would be heard by outside crew.

Standard emotes function within the private channel.

---

## Permissions and Flags

The device holder can configure which operations are allowed on the captured soul:

| Flag | Permission granted |
|---|---|
| SOULCATCHER_ALLOW_CAPTURE | Soul can be captured in the first place |
| SOULCATCHER_ALLOW_TRANSFER | Soul can be moved to another device |
| SOULCATCHER_ALLOW_DELETION | Soul consciousness can be destroyed |
| SOULCATCHER_ALLOW_DELETION_INSTANT | Soul can be destroyed immediately without delay |
| SOULCATCHER_ALLOW_TAKEOVER | Soul can assume control of the holder's body |

Transfer and deletion require both the flag to be set and appropriate operator action. Souls cannot self-transfer or self-delete.

---

## Return to Body

The device holder can release a soul back to its original body at any time, provided the body is alive and accessible. The soul is transferred back and the body resumes normal function.

If the original body has died or been destroyed while the soul was contained, standard resleeving options apply to provide the mind with a new body. See [Resleeving](../Systems/Medical/Resleeving.md).

---

## NIF Integration

A NIF implant with soulcatcher software installed provides additional features for contained souls:

| NIF Flag | Feature |
|---|---|
| NIF_SC_ALLOW_EARS | Soul can hear events in the physical space outside the gem |
| NIF_SC_ALLOW_EYES | Soul can see events in the physical space outside the gem |
| NIF_SC_BACKUPS | Automatic consciousness backups are enabled |
| NIF_SC_PROJECTING | Augmented reality projection from inside the gem is active |

These flags are set per-implant by the NIF software configuration. Without these flags, the soul has no sensory access to the outside world and exists solely in the virtual interior.

---

## Belly Integration

A soulcatcher can be linked to a predator's belly configuration. When linked, soul capture visuals and notification signals are tied to belly state updates. This allows a belly to serve simultaneously as a physical holding space and a soulcatcher-linked environment.

---

*See also: [Vore Overview](VoreOverview.md), [Belly Configuration](BellyConfiguration.md), [Resleeving](../Systems/Medical/Resleeving.md), [NIF Hardware Overview](../Systems/Science/NIF.md)*
