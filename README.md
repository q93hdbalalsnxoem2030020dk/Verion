### Guide

How to use?
```
local verionCore = loadstring(game:HttpGet("https://raw.githubusercontent.com/q93hdbalalsnxoem2030020dk/Verion/refs/heads/main/Verion"))()
local VerionNot = loadstring(game:HttpGet("https://raw.githubusercontent.com/q93hdbalalsnxoem2030020dk/Verion/refs/heads/main/VerionNot"))()

local verion = verionCore()

verion.script([[

YOUR SCRIPT HERE, Without indentation or with indentation.

]])

-- Bypass & Execute:
verion.protect()
verion.script_load()

-- Verion statistics.
local stats = verion.get_stats()
print("ban attempts: " .. stats.BanAttempts)
print("kick attempts: " .. stats.KickAttempts)
print("protected UserId / UUID: " .. stats.UserId)

VerionNot()
```

> [!TIP]
> How to execute another script after executing the first one?
>
*Simple!*

```
local verionCore = loadstring(game:HttpGet("https://raw.githubusercontent.com/q93hdbalalsnxoem2030020dk/Verion/refs/heads/main/Verion"))()
local verion = verionCore()

verion.script([[

YOUR SCRIPT HERE, Without indentation or with indentation.

]])

-- Execute Only
verion.script_load()
```

### Verion GetStats()

Use this to get stats about the Verion instance:

  The `get_stats` function returns various stats to help you track protection.

  Example of how to use it:

  1. First, call the `get_stats` function.
  2. Then, print out the stats for Ban Attempts, Kick Attempts, UserId, Instance ID, etc.
```
local stats = verion.get_stats()

-- Print the number of blocked ban attempts
print("Ban Attempts Blocked: " .. stats.BanAttempts)

-- Print the number of blocked kick attempts
print("Kick Attempts Blocked: " .. stats.KickAttempts)

-- Print the UserId of the player running Verion
print("Protected UserId: " .. stats.UserId)

-- Print the unique instance ID for tracking the current Verion instance
print("Instance ID: " .. stats.InstanceId)

-- Print whether the protection is enabled (true or false)
print("Protection Enabled: " .. tostring(stats.Enabled))

-- Print whether the instance is protected (true or false)
print("Protection Status: " .. tostring(stats.Protected))
```
