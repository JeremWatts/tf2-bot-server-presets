# tf2 bot server presets
quick console commands for setting up tf2 bot practice servers.
---


**what:** medic fill

**why:** more juicy hitboxes for your lanparty
```console
tf_bot_kick all ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; tf_bot_add 2 medic hard ; mp_disable_respawn_times 1
```
---

**what:** fix for odd medic fill

**why:** the above command left you with odd teams
```console
tf_bot_kick all ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; tf_bot_add 3 medic hard ; mp_disable_respawn_times 1
```
---

**what:** sixes simulation

**why:** you like the idea of sixes but commiting to finding a group of 11 other people is rough

⚠️ **important:** select your class first, move the command that spawns your bot counterpart in this command to happen right after the "kick all", then reduce that class count by 1 in the command
```console
tf_bot_kick all ; tf_bot_add 4 soldier hard ; tf_bot_add 2 demoman hard ; tf_bot_add 2 medic hard ; tf_bot_add 4 scout hard ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; mp_disable_respawn_times 1
```
---

## tested maps
iconic maps that seem to have working navmeshes:
| payload | king of the hill | control points |
|---------|------------------|----------------|
| pl_upward | koth_viaduct | cp_dustbowl |
| pl_badwater | koth_slaughter_event | cp_process |
| pl_venice | koth_badlands | |
| pl_goldrush | | |
| pl_thundermountain | | |
| pl_pier | | |
---

## usage
1. open console in tf2 (`` ` `` key by default)
2. copy and paste the desired preset
3. press enter


## notes
- all presets disable random crits and use fixed weapon spreads
- bots are locked to their assigned classes
- respawn times are disabled
