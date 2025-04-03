### Verion

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
