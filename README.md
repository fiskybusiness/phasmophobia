# PhasmoPhobia Configurable Mods

Making Multi-player rooms and other silly stuff availible to the user in a slightly easier to use fashion

## Getting Started

Step 0: Make a copy of your original Assembly-CSharp.dll so you can easily switch back to non-modded game
Step 1: Copy the Assembly DLL and modconfig.cfg to your Phasmophobia install location, and overwrite the DLL (<SteamInstallLocation>\steamapps\common\Phasmophobia\Phasmophobia_Data\Managed)
Step 2: Configure the values in modconfig.cfg
Step 3: Start Game!

### serverPlayers

Maximum Capacity you want your Server to Have

```
serverPlayers=16
```

### numGhosts

Number of Ghosts in the Level. Each will have Bone Evidence and it's own ghost room

```
numGhosts=20
```

### idleTimerLow/IdleTimer High
Much of the Ghosts behaivour is determined by making a State Transition from the "Idle" State. Ghosts will by default stay in this mode for 2 - 6 seconds before doing something else like moving to a new room or interacting with an object.
Set the minimum and maximum time in the idle state to increase/decrease total activity of all Ghosts

```
//super high activity
idleTimerLow=0
idleTimerHigh=1

//super low activity
idleTimerLow=10
idleTimerHigh=20

```

### numCharges

Use these to control how many times you can use cameras or salt. This will not affect other players, only you

```
numChargesSalt=100
numChargesPhoto=9
```
