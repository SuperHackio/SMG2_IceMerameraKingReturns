# SMG2 IceMerameraKingReturns

## Baron Brrr in SMG2

Baron Brrr is here in SMG2!

Below is a list of everything that's included:
- The MegaMeramera class for ProductMapObjDataTable.bcsv.
- The ObjectData files for Baron Brrr and Countess Cinder (new fire variant).
- The JSON files for particle effects.

Below is a list of other things that you will need:
- A level editor.
- A particle editor with support for JSON files.
- ActionSound entries with all sound labels for IceMerameraKing, IceManIce, MerameraQueen and MagmaMeteorBall.
> *Note: MagmaMeteorBall already has two ActionSound entries in vanilla SMG2. For Countess Cinder, a 3rd entry with the trigger name `BmIcemerakingStoneBreak` is required.*

## Credits
- [@Gabbo](https://github.com/Gabbo089) - Decompilation.
- [@Super Hackio](https://github.com/SuperHackio) - Ported and enhanced SMG1 code to SMG2.

## Setup
It is adviced to reference the [template mod](https://youtu.be/PfwK-2djr4A) for this port. You can use the following parameters:

### IceMerameraKing / MerameraQueen
| Parameter | Description |
| --- | --- |
| Obj_arg0 | Power Star ID. Spawns the assigned Power Star when defeated. Optional. |
| Obj_arg1 | Damage type. The type of damage Mario takes when touching the boss. Refer to the [ACTMES types in Syati](https://github.com/SMGCommunity/Syati/blob/main/include/Game/LiveActor/HitSensor.h). For example: `ACTMES_ENEMY_ATTACK_FREEZE` has 0x6B, which is 107 in decimal. `ACTMES_ENEMY_ATTACK_FIRERUN_STRONG` has 0x67, which is 103 in decimal. |
| Obj_arg2 | Health. The amount of hits the boss can take. Default 3. |
| Obj_arg3 | Minion spawn health. The health left at which the boss will spawn minions. Default 1. |
| Obj_arg4 | Escape time. The amount of time in frames the boss will try to escape when blown out. Default 600. |
| SW_DEAD | Gets activated when defeated. |
| SW_A | When activated, the boss will attack Mario. It will stay idle when deactivated. |
> *Note: Custom particles, sounds and the projectile model can be defined via InitActor.bcsv.*
