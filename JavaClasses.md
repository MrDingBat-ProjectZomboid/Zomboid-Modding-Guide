# Project Zomboid Modding Guide
**_This document is very much a Work-In-Progress._**
* [Goto ToC](TOC.md) 

# Java Classes Exposed to Lua
* BufferedReader
* java.io.BufferedWriter
* DataInputStream
* DataOutputStream

* Double
* Long
* Float
* Integer
* Math
* Void

* SimpleDateFormat

* ArrayList
* Calendar
* java.util.EnumMap
* java.util.GregorianCalendar
* HashMap
* java.util.LinkedList
* Stack
* java.util.Vector
* java.util.Iterator

* fmod.fmod.FMODAudio
* fmod.fmod.FMODSoundBank
* fmod.fmod.FMODSoundEmitter

* org.joml.Vector3f

* se.krka.kahlua.vm.KahluaUtil

* sun.util.BuddhistCalendar

* zombie.audio.DummySoundBank
* zombie.audio.DummySoundEmitter
* zombie.audio.BaseSoundEmitter
* zombie.audio.GameSound
* zombie.audio.GameSoundClip

* zombie.behaviors.Behavior
* zombie.behaviors.Behavior.BehaviorResult
* zombie.behaviors.general.PathFindBehavior

* zombie.ai.states.AttackState
* zombie.ai.states.BurntToDeath
* zombie.ai.states.ClimbDownSheetRopeState
* zombie.ai.states.ClimbOverFenceState
* zombie.ai.states.ClimbOverFenceState2
* zombie.ai.states.ClimbSheetRopeState
* zombie.ai.states.ClimbThroughWindowState
* zombie.ai.states.ClimbThroughWindowState2
* zombie.ai.states.CrawlingZombieTurnState
* zombie.ai.states.DieState
* zombie.ai.states.FakeDeadZombieState
* zombie.ai.states.IdleState
* zombie.ai.states.JustDieState
* zombie.ai.states.LuaState
* zombie.ai.states.LungeState
* zombie.ai.states.OpenWindowState
* zombie.ai.states.PathFindState
* zombie.ai.states.PlayerControlState
* zombie.ai.states.ReanimatePlayerState
* zombie.ai.states.ReanimateState
* zombie.ai.states.SatChairState
* zombie.ai.states.SatChairStateOut
* zombie.ai.states.StaggerBackDieState
* zombie.ai.states.StaggerBackState
* zombie.ai.states.SwipeState
* zombie.ai.states.SwipeStatePlayer
* zombie.ai.states.ThumpState
* zombie.ai.states.WalkTowardState
* zombie.ai.states.WanderState
* zombie.ai.states.ZombieStandState

* zombie.characters.BodyDamage.BodyPartType
* zombie.characters.BodyDamage.BodyPart
* zombie.characters.BodyDamage.BodyDamage
* GameKeyboard
* fmod.fmod.EmitterType

* zombie.characters.CharacterTimedActions.LuaTimedAction
* zombie.characters.CharacterTimedActions.LuaTimedActionNew

* zombie.characters.Moodles.Moodle
* zombie.characters.Moodles.Moodles
* zombie.characters.Moodles.MoodleType

* ProfessionFactory
* ProfessionFactory.Profession

* PerkFactory
* PerkFactory.Perk
* PerkFactory.Perks

* zombie.characters.traits.ObservationFactory
* zombie.characters.traits.ObservationFactory.Observation

* TraitFactory
* TraitFactory.Trait

* zombie.characters.IsoDummyCameraCharacter
* zombie.characters.Stats
* SurvivorDesc
* zombie.characters.SurvivorFactory
* zombie.characters.SurvivorFactory.SurvivorType

* IsoGameCharacter
* IsoGameCharacter.PerkInfo
* IsoGameCharacter.XP
* IsoPlayer
* zombie.characters.IsoSurvivor
* IsoZombie

* zombie.core.Clipboard

* zombie.core.fonts.AngelCodeFont

* zombie.core.logger.ZLogger

* zombie.core.properties.PropertyContainer

* zombie.core.textures.ColorInfo
* Texture

* SteamFriend
* SteamUGCDetails
* SteamWorkshopItem

* zombie.core.Color
* zombie.core.Colors
* Core
* Language
* PerformanceSettings
* SpriteRenderer
* Translator

* DebugOptions
* DebugOptions.BooleanDebugOption

* zombie.erosion.ErosionConfig
* zombie.erosion.ErosionConfig.Debug
* zombie.erosion.ErosionConfig.Season
* zombie.erosion.ErosionConfig.Seeds
* zombie.erosion.ErosionConfig.Time
* ErosionMain
* zombie.erosion.season.ErosionSeason

* ChooseGameInfo.Mod
* ChooseGameInfo.Story
* zombie.gameStates.GameLoadingState
* zombie.gameStates.MainScreenState

* zombie.globalObjects.CGlobalObjects
* zombie.globalObjects.CGlobalObjectSystem
* zombie.globalObjects.GlobalObject
* zombie.globalObjects.SGlobalObjects
* zombie.globalObjects.SGlobalObjectSystem

* zombie.input.Keys
* Mouse

* zombie.inventory.types.Clothing
* zombie.inventory.types.ComboItem
* zombie.inventory.types.Drainable
* zombie.inventory.types.DrainableComboItem
* zombie.inventory.types.Food
* zombie.inventory.types.HandWeapon
* zombie.inventory.types.InventoryContainer
* zombie.inventory.types.Key
* zombie.inventory.types.KeyRing
* zombie.inventory.types.Literature
* zombie.inventory.types.AlarmClock
* zombie.inventory.types.WeaponPart
* zombie.inventory.types.Moveable
* zombie.inventory.types.Radio

* ItemContainer
* InventoryItem
* InventoryItemFactory
* zombie.inventory.FixingManager
* zombie.inventory.RecipeManager

* zombie.iso.areas.isoregion.IsoRegion
* zombie.iso.areas.isoregion.DataCell
* zombie.iso.areas.isoregion.DataChunk
* zombie.iso.areas.isoregion.ChunkRegion
* zombie.iso.areas.isoregion.MasterRegion

* zombie.iso.areas.IsoBuilding
* zombie.iso.areas.IsoRoom
* zombie.iso.areas.SafeHouse

* zombie.iso.objects.interfaces.BarricadeAble

* zombie.iso.objects.IsoBarbecue
* zombie.iso.objects.IsoBarricade
* zombie.iso.objects.IsoCrate
* zombie.iso.objects.IsoCurtain
* zombie.iso.objects.IsoCarBatteryCharger
* zombie.iso.objects.IsoDeadBody
* zombie.iso.objects.IsoDoor
* zombie.iso.objects.IsoFire
* IsoFireManager
* zombie.iso.objects.IsoFireplace
* zombie.iso.objects.IsoGenerator
* zombie.iso.objects.IsoJukebox
* zombie.iso.objects.IsoLightSwitch
* zombie.iso.objects.IsoMolotovCocktail
* zombie.iso.objects.IsoWaveSignal
* zombie.iso.objects.IsoRadio
* zombie.iso.objects.IsoTelevision
* zombie.iso.objects.IsoStove
* zombie.iso.objects.IsoThumpable
* zombie.iso.objects.IsoTrap
* zombie.iso.objects.IsoTree
* zombie.iso.objects.IsoWheelieBin
* zombie.iso.objects.IsoWindow
* zombie.iso.objects.IsoWindowFrame
* zombie.iso.objects.IsoWorldInventoryObject
* zombie.iso.objects.IsoZombieGiblets
* zombie.iso.objects.RainManager
* zombie.iso.objects.ObjectRenderEffects

* IsoSprite
* zombie.iso.sprite.IsoSpriteInstance
* zombie.iso.sprite.IsoSpriteManager
* zombie.iso.sprite.IsoSpriteGrid

* zombie.iso.SpriteDetails.IsoFlagType
* zombie.iso.SpriteDetails.IsoObjectType

* ClimateManager
* ClimateManager.DayInfo
* ClimateManager.ClimateFloat
* ClimateManager.ClimateColor
* ClimateManager.ClimateBool
* zombie.iso.weather.WeatherPeriod
* zombie.iso.weather.WeatherPeriod.WeatherStage
* zombie.iso.weather.WeatherPeriod.StrLerpVal
* ClimateManager.AirFront
* zombie.iso.weather.ThunderStorm
* zombie.iso.weather.ThunderStorm.ThunderCloud
* zombie.iso.weather.fx.IsoWeatherFX
* zombie.iso.weather.Temperature
* zombie.iso.weather.Temperature.PlayerTempVars
* zombie.iso.weather.ClimateColorInfo

* zombie.iso.BuildingDef
* IsoCamera
* IsoCell
* zombie.iso.IsoChunkMap
* IsoDirections
* IsoGridSquare
* zombie.iso.IsoHeatSource
* zombie.iso.IsoLightSource
* zombie.iso.IsoLot
* zombie.iso.IsoLuaMover
* zombie.iso.IsoMetaChunk
* zombie.iso.IsoMetaCell
* IsoMetaGrid
* IsoMetaGrid.Trigger
* IsoMetaGrid.Zone
* zombie.iso.IsoMovingObject
* IsoObject
* zombie.iso.IsoObjectPicker
* IsoPushableObject
* IsoUtils
* IsoWorld
* zombie.iso.LosUtil
* zombie.iso.MetaObject
* zombie.iso.RoomDef
* zombie.iso.SliceY
* Vector2
* zombie.iso.Vector3

* LuaEventManager
* MapObjects

* zombie.Quests.QuestCreator

* Server
* ServerOptions
* ServerOptions.BooleanServerOption
* ServerOptions.DoubleServerOption
* ServerOptions.IntegerServerOption
* ServerOptions.StringServerOption
* ServerOptions.TextServerOption
* zombie.network.ServerSettings
* ServerSettingsManager

* ZombiePopulationRenderer
* ZombiePopulationRenderer.BooleanDebugOption

* RadioAPI
* zombie.radio.devices.DeviceData
* zombie.radio.devices.DevicePresets
* zombie.radio.devices.PresetEntry
* ZomboidRadio
* RadioData
* zombie.radio.scripting.RadioScriptManager
* SLSoundManager
* zombie.radio.StorySounds.StorySound
* zombie.radio.StorySounds.StorySoundEvent
* zombie.radio.StorySounds.EventSound
* zombie.radio.StorySounds.DataPoint

* EvolvedRecipe
* zombie.scripting.objects.Fixing
* zombie.scripting.objects.Fixing.Fixer
* zombie.scripting.objects.Fixing.FixerSkill
* zombie.scripting.objects.GameSoundScript
* Item
* Item.ClothingBodyLocation
* zombie.scripting.objects.ItemRecipe
* Recipe
* Recipe.Result
* Recipe.Source
* zombie.scripting.objects.ScriptModule
* VehicleScript
* VehicleScript.Area
* VehicleScript.Part
* VehicleScript.Passenger
* VehicleScript.Position
* VehicleScript.Wheel

* ScriptManager

* zombie.ui.ActionProgressBar
* zombie.ui.Clock
* zombie.ui.UIDebugConsole
* zombie.ui.LuaUIWindow
* zombie.ui.ModalDialog
* zombie.ui.MoodlesUI
* zombie.ui.NewHealthPanel
* zombie.ui.ObjectTooltip
* zombie.ui.ObjectTooltip.Layout
* zombie.ui.ObjectTooltip.LayoutItem
* zombie.ui.RadarPanel
* zombie.ui.RadialMenu
* zombie.ui.SpeedControls
* TextManager
* UIElement
* zombie.ui.UIFont
* zombie.ui.UITransition
* UIManager
* zombie.ui.UIServerToolbox
* zombie.ui.UITextBox2
* zombie.ui.VehicleGauge
* zombie.ui.VirtualItemSlot
* zombie.ui.TextDrawObject

* zombie.util.list.PZArrayList

* BaseVehicle
* zombie.vehicles.PathFindBehavior2
* zombie.vehicles.VehicleDoor
* zombie.vehicles.VehicleLight
* VehiclePart
* zombie.vehicles.VehicleType
* VehicleWindow

* zombie.DummySoundManager
* GameSounds
* GameTime
* GameWindow
* SandboxOptions
* SandboxOptions.BooleanSandboxOption
* SandboxOptions.DoubleSandboxOption
* SandboxOptions.EnumSandboxOption
* SandboxOptions.IntegerSandboxOption
* SoundManager
* zombie.SystemDisabler
* VirtualZombieManager
* zombie.characters.DummyCharacterSoundEmitter
* zombie.characters.CharacterSoundEmitter
* SoundManager.AmbientSoundEffect
* BaseAmbientStreamManager
* AmbientStreamManager
* zombie.characters.BodyDamage.Nutrition
* zombie.iso.objects.BSFurnace
* zombie.iso.MultiStageBuilding
* zombie.iso.MultiStageBuilding.Stage
* SleepingEvent
* zombie.iso.objects.IsoCompost
* zombie.network.Userlog
* zombie.network.Userlog.UserlogType

* zombie.config.ConfigOption
* zombie.config.BooleanConfigOption
* zombie.config.DoubleConfigOption
* zombie.config.EnumConfigOption
* zombie.config.IntegerConfigOption
* zombie.config.StringConfigOption
* Faction

* LuaManager.GlobalObject.LuaFileWriter

* org.lwjgl.input.Keyboard
* zombie.network.DBResult
* zombie.iso.areas.NonPvpZone
* zombie.network.DBTicket
* zombie.core.stash.StashSystem
* zombie.core.stash.StashBuilding
* zombie.core.stash.Stash
* zombie.inventory.ItemType

* zombie.MapGroups

* zombie.chat.ChatMessage
* zombie.chat.ChatBase
* zombie.chat.ServerChatMessage

```
### PZ debug mode only
```

* Field
* Method
* Coroutine

----------------------------------------
* [Goto ToC](TOC.md)  
