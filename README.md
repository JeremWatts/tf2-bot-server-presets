# tf2-bot-server-presets


what:  medic fill
why:  more juicy hitboxes for your lanparty
```
tf_bot_kick all ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; tf_bot_add 2 medic hard ; mp_disable_respawn_times 1
```

what:  fix for odd medic fill
why:  the above command left you with odd teams
```
tf_bot_kick all ; tf_bot_reevaluate_class_in_spawnroom 0 ; tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; tf_bot_add 3 medic hard ; mp_disable_respawn_times 1
```

what:  sixes simulation
why:  you like the idea of sixes but commiting to finding a group of 11 other people is rough
note:  have your selected class first, and reduce the number by one
```
tf_bot_kick all ; tf_bot_add 4 soldier hard ; tf_bot_add 2 demoman hard ; tf_bot_add 2 medic hard ; tf_bot_add 4 scout hard ; tf_bot_reevaluate_class_in_spawnroom 0 ;  tf_use_fixed_weaponspreads 1 ; tf_weapon_criticals 0 ; mp_disable_respawn_times 1
```

what:  iconic maps that seem to have working navmeshes
```
pl_upward
koth_viaduct
pl_badwater
koth_slaughter_event
cp_dustbowl
pl_venice
cp_process
pl_goldrush
koth_badlands
pl_thundermountain
pl_pier
```
