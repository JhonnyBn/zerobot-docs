---
sidebar_position: 7
---

# Engine
Control's the bot engine

```lua
Engine.isHealingEnabled()
Engine.isHealFriendEnabled()
Engine.getBotVersion()
Engine.isBotEnabled()
Engine.isTargetingEnabled()
Engine.isMagicShooterEnabled()
Engine.isEquipmentEnabled()
Engine.isTimerEnabled()
Engine.enableTargeting(enable)
Engine.enableMagicShooter(enable)
Engine.enableHealFriend(enable)
Engine.enableHealing(enable)
Engine.enableEquipment(enable)
Engine.enableTimer(enable)
Engine.enableBot(enable)
Engine.magicShooterSwitchProfile(profileIndex)
Engine.magicShooterGetProfile()
Engine.magicShooterGetProfileName(index)
Engine.targetingSwitchProfile(profileIndex)
Engine.targetingGetProfile()
Engine.targetingGetProfileName(index)
Engine.equipmentSwitchProfile(profileIndex)
Engine.equipmentGetProfile()
Engine.equipmentGetProfileName(index)
Engine.getScriptsDirectory()
Engine.healingSwitchProfile(profileIndex)
Engine.healingGetProfile()
Engine.healingGetProfileName(index)
Engine.getUserId()
Engine.getLicenseTime()
Engine.setAlarm(alarmType, enable)
Engine.isAlarmEnabled(alarmType)
Engine.loadScript(scriptName)
Engine.unloadScript(scriptName)
Engine.reloadScript(scriptName)
Engine.loadConfig(config)
Engine.isScriptLoaded(scriptName)
```

### Code

```lua
--- Returns if healing function is enabled
-- This function is a wrapper around the external function engineIsHealingEnabled.
function Engine.isHealingEnabled()

--- Returns if heal friend function is enabled
-- This function is a wrapper around the external function return IsHealFriendEnabled.
function Engine.isHealFriendEnabled()

--- Returns current bot version
-- This function is a wrapper around the external function engineGetBotVersion.
function Engine.getBotVersion()

--- Returns if bot is enabled
-- This function is a wrapper around the external function engineIsBotEnabled.
function Engine.isBotEnabled()

--- Returns if targeting function is enabled
-- This function is a wrapper around the external function engineIsTargetingEnabled.
function Engine.isTargetingEnabled()

--- Returns if magic shooter function is enabled
-- This function is a wrapper around the external function engineIsMagicShooterEnabled.
function Engine.isMagicShooterEnabled()

--- Returns if equipment function is enabled
-- This function is a wrapper around the external function engineIsEquipmentEnabled.
function Engine.isEquipmentEnabled()

--- Returns if timer function is enabled
-- This function is a wrapper around the external function engineIsTimerEnabled.
function Engine.isTimerEnabled()

--- Enables or disables the targeting system.
-- This function is a wrapper around the external function engineTargetingEnable.
-- @param enable (boolean) - A flag indicating whether to enable (true) or disable (false) the targeting system.
function Engine.enableTargeting(enable)

--- Enables or disables the magic shooter system.
-- This function is a wrapper around the external function engineMagicShooterEnable.
-- @param enable (boolean) - A flag indicating whether to enable (true) or disable (false) the magic shooter system.
function Engine.enableMagicShooter(enable)

--- Enables or disables the heal friend system.
-- This function is a wrapper around the external function engineHealFriendEnable.
-- @param enable (boolean) - A flag indicating whether to enable (true) or disable (false) the heal friend system.
function Engine.enableHealFriend(enable)

--- Enables or disables the healing system.
-- This function is a wrapper around the external function engineHealingEnable.
-- @param enable (boolean) - A flag indicating whether to enable (true) or disable (false) the healing system.
function Engine.enableHealing(enable)

--- Enables or disables the equipment system.
-- This function is a wrapper around the external function engineEquipmentEnable.
-- @param enable (boolean) - A flag indicating whether to enable (true) or disable (false) the equipment system.
function Engine.enableEquipment(enable)

--- Enables or disables the timer system.
-- This function is a wrapper around the external function engineTimerEnable.
-- @param enable (boolean) - A flag indicating whether to enable (true) or disable (false) the timer system.
function Engine.enableTimer(enable)

--- Enables or disables all bot functions.
-- This function is a wrapper around the external function engineBotEnable.
-- @param enable (boolean) - A flag indicating whether to enable (true) or disable (false) all bot functions.
function Engine.enableBot(enable)

--- Switches the profile of magic shooter by index.
-- This function is a wrapper around the external function engineMagicShooterSwitchProfile.
-- @param profileIndex (number) - The index of the profile to switch to (from 0 to 9).
function Engine.magicShooterSwitchProfile(profileIndex)

--- Gets the current profile index selected on magic shooter.
-- This function is a wrapper around the external function engineMagicShooterGetProfile.
-- @return (number) - The index of current selected profile.
function Engine.magicShooterGetProfile()

--- Gets the current magic shooter profile name.
--- This function is a wrapper around the external function engineMagicShooterGetProfileName.
--- @param index (number) - The index of the profile to get the name from (from 0 to 9).
--- @return (string) - The name of the current selected profile.
function Engine.magicShooterGetProfileName(index)

--- Switches the profile of targeting by index.
-- This function is a wrapper around the external function engineTargetingSwitchProfile.
-- @param profileIndex (number) - The index of the profile to switch to (from 0 to 9).
function Engine.targetingSwitchProfile(profileIndex)

--- Gets the current profile index selected on targeting.
-- This function is a wrapper around the external function engineTargetingGetProfile.
-- @return (number) - The index of current selected profile.
function Engine.targetingGetProfile()

--- Gets the current targeting profile name.
-- This function is a wrapper around the external function engineTargetingGetProfileName.
-- @param index (number) - The index of the profile to get the name from (from 0 to 9).
-- @return (string) - The name of the current selected profile.
function Engine.targetingGetProfileName(index)

--- Switches the profile of equipment by index.
-- This function is a wrapper around the external function engineEquipmentSwitchProfile.
-- @param profileIndex (number) - The index of the profile to switch to (from 0 to 9).
function Engine.equipmentSwitchProfile(profileIndex)

--- Gets the current profile index selected on equipment.
-- This function is a wrapper around the external function engineEquipmentGetProfile.
-- @return (number) - The index of current selected profile.
function Engine.equipmentGetProfile()

--- Gets the current equipment profile name.
-- This function is a wrapper around the external function engineEquipmentGetProfileName.
-- @param index (number) - The index of the profile to get the name from (from 0 to 9).
-- @return (string) - The name of the current selected profile.
function Engine.equipmentGetProfileName(index)

--- Gets the default scripts directory.
-- This function is a wrapper around the external function engineGetScriptsDirectory.
-- @return (string) - The path to default scripts directory.
function Engine.getScriptsDirectory()

--- Switches the profile of healing by index.
--- This function is a wrapper around the external function engineHealingSwitchProfile.
--- @param profileIndex (number) - The index of the profile to switch to (from 0 to 9).
function Engine.healingSwitchProfile(profileIndex)

--- Gets the current profile index selected on healing.
--- This function is a wrapper around the external function engineHealingGetProfile.
--- @return (number) - The index of current selected profile.
function Engine.healingGetProfile()

--- Gets the current healing profile name.
--- This function is a wrapper around the external function engineHealingGetProfileName.
--- @param index (number) - The index of the profile to get the name from (from 0 to 9).
--- @return (string) - The name of the current selected profile.
function Engine.healingGetProfileName(index)

--- Gets the last user ID.
-- This function is useful to identify current user. You can use engineGetUserId directly if you need to avoid hooks.
-- @return (string) - The last generated user ID, non-sensitive data.
function Engine.getUserId()

--- Gets the remaining time of the license.
--- This function is a wrapper around the external function engineGetLicenseTime.
--- To allow this function, the user should consent to share this information with the script by enabling "Allow Scripts Access License Time" on Engine tab.
--- @return (string) - The last visible license time from ZeroBot overview tab. If this information is not available, it will return nil.
function Engine.getLicenseTime()

--- Enables or disables specific alarm type.
--- @param alarmType (number) - The alarm type to enable or disable.
--- @param enable (boolean) - A flag indicating whether to enable (true) or disable (false) the alarm type.
function Engine.setAlarm(alarmType, enable)

--- Get the status of a specific alarm type.
--- @param alarmType (number) - The alarm type to check. Refer to Enums.AlarmType.
--- @return (boolean) - Returns true if the alarm type is enabled, false otherwise.
function Engine.isAlarmEnabled(alarmType)

--- Load specific script.
-- This function is a wrapper around the external function engineLoadScript.
-- This function runs asynchronously, so it may take some time to load the script, so if you will use Engine.unloadScript right after this function, you should wait for the script to be loaded, wait some delay.
-- @param scriptName (string) - The name of the script to load. This name is based on "Available Scripts" list in "Scripting" tab.
-- @return (boolean) - Returns true if the script is loaded successfully, false if the script doesn't exists.
function Engine.loadScript(scriptName)

--- Unload specific script.
-- This function is a wrapper around the external function engineUnloadScript.
-- @param scriptName (string) - The name of the script to unload. This name is based on "Enabled Scripts" list in "Scripting" tab.
-- @return (boolean) - Returns true if the script was unloaded successfully, false if the script doesn't exists.
function Engine.unloadScript(scriptName)

--- Reload specific script.
--- This function is a wrapper around the external function engineReloadScript.
--- @param scriptName (string) - The name of the script to reload. This name is based on "Enabled Scripts" list in "Scripting" tab.
--- @return (boolean) - Returns true if the script was reloaded successfully, false if the script doesn't exists.
function Engine.reloadScript(scriptName)

--- Load specific configuration by name. For privacy reasons we don't have a function to list available configurations.
--- This function is a wrapper around the external function engineLoadConfig.
--- @param config (string) - The name of the config file to load. This name is based on available configurations list in "Settings" tab.
function Engine.loadConfig(config)

--- Check if a specific script is loaded.
--- This function is a wrapper around the external function engineIsScriptLoaded.
--- @param scriptName (string) - The name of the script to check. This name is based on "Enabled Scripts" list in "Scripting" tab.
--- @return (boolean) - Returns true if the script is loaded, false otherwise.
function Engine.isScriptLoaded(scriptName)
```