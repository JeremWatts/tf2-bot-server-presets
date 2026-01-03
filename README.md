# TF2 Bot Server Presets

Quick console commands for setting up TF2 bot practice servers.

---

## Presets

**What:** Medic fill
**Why:** More juicy hitboxes for your lanparty
```console
tf_bot_kick all ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; tf_bot_add 2 medic hard ; mp_disable_respawn_times 1
```

---

### What: Fix for odd medic fill
**Why:** the above command left you with odd teams
```console
tf_bot_kick all ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; tf_bot_add 3 medic hard ; mp_disable_respawn_times 1
```

---

### What: Sixes Simulation
**Why:** You like the idea of sixes but commiting to finding a group of 11 other people is rough

⚠️ **Important:** Select your class first, move the command that spawns your bot counterpart in this command to happen right after the "kick all", then reduce that class count by 1 in the command
```console
tf_bot_kick all ; tf_bot_add 4 soldier hard ; tf_bot_add 2 demoman hard ; tf_bot_add 2 medic hard ; tf_bot_add 4 scout hard ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; mp_disable_respawn_times 1
```


---

## Tested Maps

Maps confirmed to have working bot navigation meshes:

| Payload | King of the Hill | Control Points |
|---------|------------------|----------------|
| pl_upward | koth_viaduct | cp_dustbowl |
| pl_badwater | koth_slaughter_event | cp_process |
| pl_venice | koth_badlands | |
| pl_goldrush | | |
| pl_thundermountain | | |
| pl_pier | | |

---

## Usage

1. Open console in TF2 (`` ` `` key by default)
2. Copy and paste the desired preset
3. Press Enter

## Notes

- All presets disable random crits and use fixed weapon spreads
- Bots are locked to their assigned classes
- Respawn times are disabled
