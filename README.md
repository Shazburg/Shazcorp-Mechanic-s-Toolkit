# ShazCorp Mechanic’s Toolkit

Making a mechanic's exocortex life better one click at a time.

Dedicated exocortex sheets and guided preparation for Starfinder Second Edition
Mechanics and characters with the Mechanic archetype. Create and manage a
Drone, Mine Network or Turret without turning the mechanic’s character sheet
into a device tracker.

**Public release status:** the first public package is still undergoing content
review. The installation URL below is reserved for that release and will not
work until its assets have been published.

## Requirements

- Foundry Virtual Tabletop 14; the development test environment uses 14.369.
- The Starfinder Second Edition system, version 1.6.1. The current package
  targets that exact system version, not arbitrary later releases or PF2e.
- A saved mechanic character with its native Tech Core class features and
  exocortex choice. Complete the character’s own choices before creating a device.
- The owning player or GM can create a device. Players need Foundry's
  **Create Actors** permission for their role and must own the mechanic.
  Operating a linked device requires ownership of both actors.

This is an unofficial software aid, not a replacement for the game’s rules.
Obtain rules and equipment through their authorized sources. No premium token
pack or animation module is required.

## Installation

Once the public release is available:

1. Back up your world and return Foundry to Setup.
2. Open **Add-on Modules → Install Module**, paste the manifest URL below and
   install it.
3. Launch your SF2e world, open **Manage Modules**, enable **ShazCorp Mechanic’s
   Toolkit**, then save and reload.

```text
https://github.com/Shazburg/Shazcorp-Mechanic-s-Toolkit/releases/latest/download/module.json
```

The package ID is `shazcorp-mechanics-toolkit`. Users of the former
`shazcorp-exocortex-drone` package must disable/uninstall that package and
start fresh. There is no automatic transfer of its device builds. Keep your
mechanic character; installing this module does not replace it or bulk-edit actors.

## Create your first exocortex

1. As the owning player or GM, open the saved mechanic’s character sheet and select **Exocortex**
   in its header.
2. If the character has more than one supported exocortex, choose which to open.
   An existing linked device opens instead of creating a duplicate.
3. For a new device, enter its name, make the available configuration choices,
   select **Review**, then confirm creation/preparation.
4. For Mechanic Dedication, the owner or GM confirms initial setup when prompted. Existing
   choices are retained; setup does not grant unrelated full-class features.

The new device receives its dedicated sheet and default artwork. Its ownership
is based on the mechanic’s explicit owners, rather than granting access to
every player. A player who creates the device keeps explicit ownership, including
when their access to the mechanic comes from its default ownership setting.
If Foundry denies actor creation, ask the GM to grant **Create Actors** for
your role or to create the device. The module does not bypass that permission.

## Prepare and use a drone

Use **Exocortex** on the mechanic to open the builder for its linked drone.
Choose a chassis, size and the customizations available to that character.
Parameter choices, such as a movement type, appear where needed. The builder
uses the mechanic’s level and actual feats to determine available selections.
Review the result before applying it.

Preparation and Undo post reports to chat. There is no once-per-day software
lock; the table is responsible for when preparation is allowed. Rebuilding a
loadout does not refill HP or ammunition. Repair/service controls are separate.
Undo is not a general rollback of combat, purchases or spent resources.

Add weapons and ammunition under **Mounted Equipment & Supplies**. Mount the
weapon, select compatible ammunition at that weapon’s inventory entry, and use
**Load / Reload** or **Select ammo**, as offered. Ammunition is managed there,
not separately on every Strike or Auto-Fire action. Confirm removal of equipment
when it is no longer needed. Armor upgrades require an available Upgrade Slot
and compatible installation.

Use **Command Drone on the mechanic**, then resolve attacks and local abilities
on the drone. Weapon mounts provide capacity, not extra hands or extra actions.
Support, service and feat-dependent controls appear where supported.

## Prepare and use a turret

Use the mechanic’s **Exocortex** header to create or open its linked turret.
Choose an available array and an eligible weapon grade, then review the setup.
Paid grades require a purchase/crafting confirmation; the module does not charge
credits or grant a free upgrade when the mechanic levels up.

Deployment, recall, repositioning and other mechanic commands belong on the
mechanic. Strike, Area Fire and device-local offensive abilities belong on the
turret. Deploy/recall are context-sensitive uses of the deployment command.
Scene placement asks for a position; Escape cancels selection.

To install an upgrade, put the actual compatible item in the mechanic’s
inventory, click an empty custom-rig upgrade slot on the turret, select the
item and confirm **Install**. This transfers the item; it is not merely a link
to view it. The module checks available slots and native compatibility.

Target the intended creature before firing. Select the correct shared multiple
attack penalty step. Turret rolls use the mechanic’s native SF2e statistics
with the device’s position and configuration. Use the resulting chat controls
for damage or critical damage.

## Prepare and use a mine network

Open **Exocortex** to create or open the mechanic’s Mine Network. Use commands
on the mechanic to deploy and manage mines; use the network’s local detonation
actions for deployed mines. Configuration and available controls follow the
character’s actual abilities.

Deploying creates a scene marker. Choose the deployed mine and confirm its
detonation options. Chat provides the relevant roll and save/template controls.
When applying an outcome, enter the actual save result and confirm the affected
target. Do not also apply the same damage through an ordinary damage button.

Mine triggers, legal areas, line of effect and reaction eligibility still need
table adjudication. Walking a token past a marker does not secretly detonate it.

## Changes and troubleshooting

- **The Exocortex button is missing:** confirm the module is enabled, the system
  version matches, you own the saved world character, and its native mechanic
  class/dedication and exocortex choice are present. Third-party sheets may not
  expose the supported header control; try the system’s standard character sheet.
- **A level or feat changed:** reopen the builder or use **Review / Synchronize**
  for the device. Check the proposed changes before confirming. The module does
  not rebuild devices when a world loads.
- **A purchase is unavailable:** eligibility does not supply equipment or pay
  for it. Add the actual item and confirm any required purchase separately.
- **An operation was interrupted:** stop retrying blindly. Use the relevant
  pending-report or GM recovery control and inspect the current state first.
  Recovery safeguards do not promise that every multi-document write is atomic.

The module supports level 1–20 progression, but situational actions are not all
fully automatic. Hits, saves, cover, line of effect, reaction triggers and legal
movement remain explicit decisions. Its action ledger is not a universal
three-action tracker. Back up your world and test your configuration before play.

## How this was developed

Developed using AI-assisted coding, debugging, and testing.

## License and reporting issues

Original software contributions are licensed under **GPLv3**.
See `LICENSE` for the complete GPLv3 text and `NOTICES.md` for scope and asset
notices. Artwork and third-party materials are not automatically licensed under
the code’s GPL terms. A software license does not grant rights in Paizo or
Foundry material. The software is provided without warranty.

Report problems at:

```text
https://github.com/Shazburg/Shazcorp-Mechanic-s-Toolkit/issues
```

Include Foundry/system/module versions, the device type, steps to reproduce,
and any relevant error message. Remove credentials, player details, world
exports and campaign secrets before submitting screenshots or logs.
