# TF2 Bot Server Presets

Quick console commands for setting up TF2 bot practice servers.

---

## Presets

### Medic Fill
**Purpose:** Add healing bots to casual matches with friends  
**Use case:** LAN parties or small groups wanting extra medics
```console
tf_bot_kick all ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; tf_bot_add 2 medic hard ; mp_disable_respawn_times 1
```

---

### Medic Fill (Odd Teams)
**Purpose:** Fix unbalanced teams from the above command  
**Use case:** When you need 3 medics instead of 2 for even teams
```console
tf_bot_kick all ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; tf_bot_add 3 medic hard ; mp_disable_respawn_times 1
```

---

### Sixes Simulation
**Purpose:** Practice 6v6 competitive format  
**Use case:** Solo practice for competitive sixes

⚠️ **Important:** Select your class first, then reduce that class count by 1 in the command
```console
tf_bot_kick all ; tf_bot_add 4 soldier hard ; tf_bot_add 2 demoman hard ; tf_bot_add 2 medic hard ; tf_bot_add 4 scout hard ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; mp_disable_respawn_times 1
```

**Standard composition:** 2 Scouts, 2 Soldiers, 1 Demo, 1 Medic per team

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
- Respawn times are disabled for continuous action
