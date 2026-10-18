# ShazCorp Mechanic’s Toolkit

Making a mechanic's exocortex life better one click at a time.

Dedicated exocortex sheets and guided preparation for Starfinder Second Edition
Mechanics and characters with the Mechanic archetype. Create and manage a
Drone, Mine Network or Turret without turning the mechanic’s character sheet
into a device tracker.

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

Install the latest public release using this stable manifest:

1. Back up your world and return Foundry to Setup.
2. Open **Add-on Modules → Install Module**, paste the manifest URL below and
   install it.
3. Launch your SF2e world, open **Manage Modules**, enable **ShazCorp Mechanic’s
   Toolkit**, then save and reload.

```text
https://github.com/Shazburg/Shazcorp-Mechanic-s-Toolkit/releases/latest/download/module.json
```

Release notes, installable packages and matching source archives are available at:

```text
https://github.com/Shazburg/Shazcorp-Mechanic-s-Toolkit/releases/latest
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

With weapon mounts fitted, use **Get weapon from mechanic** to choose an
available weapon that fits the free mounts. Confirming transfers one weapon
from the mechanic and mounts it; it does not create a copy. **Get ammunition
from mechanic** lists ammunition compatible with mounted weapons and lets you
choose a quantity. Each weapon also has **Get compatible ammunition**, which
filters specifically for that weapon. Load transferred ammunition using the
weapon’s existing loading controls.

Dragging equipment from an owned world actor to the drone also transfers it
after quantity selection and confirmation; it does not copy the source item.
Dropped weapons arrive unmounted: use **Mount** to confirm installation.
Compendium and standalone world-item drops still import items; dragging within
the same drone still sorts its inventory. Inaccessible or unsupported actor
sources are refused rather than silently copied. This correction does not
automatically remove duplicates created by earlier versions.

Use **Install attachment from mechanic** at a weapon to choose carried equipment
accepted by SF2e’s native compatibility check. Confirm the available attachment
slots, prerequisites and applicable installation activity; the system’s
compatibility check does not replace those table decisions.

Installed add-ons appear beside their weapon with rules, chat and native option
controls. **Adjust Sight** activates a scope for one commanded drone action;
the adjustment ends at the beginning of the mechanic’s next turn or when the
weapon is no longer wielded. Outside combat it expires after six seconds of
world time. **End adjustment** clears it early. Bipod and fireburst mode changes
also use the drone action tracker. Their manipulate activations require
**Manual Dexterity**; integrated mounts alone do not provide manipulation.

Confirmed new scope/bipod/fireburst installations start inactive. An older scope
whose native toggle is already enabled is labelled as untracked; use Adjust
Sight to start its tracked duration or End adjustment to disable it. The module
does not silently change existing add-ons when a sheet opens.

**Uninstall & Return** sends a drone attachment back to the mechanic without
moving its weapon or loaded ammunition. Confirm the removal activity. If a
detach/transfer stops partway through, inspect both inventories and the saved
recovery record rather than retrying. Turret upgrades retain their existing
custom-rig Uninstall destination.

Passive rules continue to use SF2e’s automation. Native toggles/suboptions are
exposed where available, including on turret upgrades, but turret activation
action costs and other add-ons’ triggers, saves, charges and non-native effects
still require table resolution. Rules/chat controls do not claim to execute
those effects. Requirements such as bipod placement and movement restrictions
remain part of the item's rules, not automatic movement enforcement.

**Return** sends equipment back to the linked mechanic instead of deleting it.
Returning a mounted weapon confirms the removal activity and carries its
attachments and loaded ammunition with it. Ammunition merely selected from a
separate inventory stack stays with its actor; that selection is cleared when
the weapon changes actors. Unlink ammunition before returning it if another
weapon still selects it.

Use **Command Drone on the mechanic**, then resolve attacks and local abilities
on the drone. Weapon mounts provide capacity, not extra hands or extra actions.
Support, service and feat-dependent controls appear where supported.

Native actions and feat cards are reused when present. Turret firing is under
**Remote Weapon Systems**, with native Damage and Critical Damage buttons on
its attack roll. Ordinary damage and healing use SF2e's normal controls.
Conditional mine/device effects and combined detonations use a specialized
resolution control only where needed. Do not apply the same damage twice.
**Review / Synchronize** removes obsolete module-generated cards without
removing native feats or your own custom actions. Existing actors are not
automatically changed. Specializations appear under **Passive Features**.

**Service & Control** groups its controls by purpose: **Command & Movement**,
**Support & Maneuvers**, **Repair & Reboot**, and **Battery Recharge**. Routine
repairs are separate from emergency procedures. **Reports & Recovery** is below
these groups and opens automatically for a pending action or service report;
GM-only recovery controls remain restricted to the GM.

Pause over a fitted customization, passive feature or Service & Control
control to see its rules and requirements. Tooltips use Foundry's normal hover
delay. Keyboard focus also opens help; Escape dismisses it. Reading a fitted
customization no longer requires opening an item sheet. Operational buttons
still perform their normal actions when clicked.

Mine and Turret sheets use the same delayed help for configuration, preparation,
recovery and weapon controls. Pause over fitted or loose turret upgrade names
for their native rules; installing, uninstalling, posting rules and native
activation options remain separate operational controls.

Weapon mount and ammunition guidance sits to the right of its readouts or
controls, stacking below them in narrow windows. For known manipulate add-ons,
a drone without Manual Dexterity sees a disabled block and an explanatory
warning; only **Uninstall & Return** remains usable. This does not automatically
rewrite existing native option states. Passive add-ons are not locked by this
check. **Mark customization** and **Unmark** explain their grouping-only role
on hover instead of showing detached instructions.

Mine preparation and detonation guidance and Turret storage, firing and custom
rig guidance follow the same adjacent layout. Stored or broken turrets show a
disabled firing block with its reason; array changes remain available. Stored
turret upgrade activations require deployment, not Manual Dexterity; rules and
uninstall remain accessible. Mine discard is unavailable with no carried stock,
and Detonate Mine is unavailable without a live deployed marker. Preparation
and missing-marker recovery remain available.

## Choose and retain exocortex artwork

Use **Portrait & Token** in the header of an owned Drone, Mine Network or Turret
sheet. Choose separate existing assets with **Browse**, or paste their paths.
**Apply Artwork** changes the portrait and prototype token, without changing
statistics, equipment, ownership, size, position or ring settings.

**Remember** saves the two asset paths on the linked mechanic for future
exocortices of that type. Existing actors are not silently changed. Rebuilds,
redeployment and turret array changes retain explicitly chosen art. To update
already-placed tokens too, select **Also update existing tokens**; this is off
by default and requires permission to update every matching token.

Owning players and GMs can use the editor. Browsing/uploading still uses normal
Foundry file permissions; without browsing access, paste a known accessible
asset path. Opening or cancelling does not change artwork. Resolve interrupted
device/build/inventory operations before editing. If a cosmetic update stops
partway through, reopen the editor and apply again; no resources are refunded
or spent by these controls.

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
Included game-rule descriptions, data and adaptations are licensed under **ORC**;
see `ORC-NOTICE.md` in the release archives for source attribution and license scope.
The 13 bundled generic default token images are offered under **CC0-1.0**.
See `LICENSE` for the complete GPLv3 text and `NOTICES.md` for scope and asset
notices. Game content, artwork and third-party materials are not automatically licensed under
the code’s GPL terms. A software license does not grant rights in Paizo or
Foundry material. The software is provided without warranty.

Report problems at:

```text
https://github.com/Shazburg/Shazcorp-Mechanic-s-Toolkit/issues
```

Include Foundry/system/module versions, the device type, steps to reproduce,
and any relevant error message. Remove credentials, player details, world
exports and campaign secrets before submitting screenshots or logs.
