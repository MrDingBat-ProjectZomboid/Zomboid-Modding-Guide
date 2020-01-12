# Project Zomboid Modding Guide
**_This document is very much a Work-In-Progress._**
# Lua Methods

* [Goto ToC](TOC.md)  
## Contents

----------------------------------------------------------------------------------
----------------------------------------------------------------------------------

## List of Lua Methods

* addChallenge(KahluaTable challenge ) void
* addSound(IsoObject source, int x, int y, int z, int radius, int volume ) void
* backToSinglePlayer( ) void
* breakpoint( ) void
* checkSaveFileExists(String f ) boolean
* cloneItemType(String newName, String oldName ) Item
* createHordeFromTo(float x, float y, float x2, float y2, int count ) void
* createNewScriptItem(String base, String name, String display, String type, String icon ) Item
* createStory(String storyName ) void
* createWorld(String worldName ) void
* debugLuaTable(Object param, int depth ) void
* debugLuaTable(Object param ) void
* deleteLastStandSave( ) void
* deletePlayerSave(String fileName ) void
* deleteSave(String file ) void
* disconnect( ) void
* doChallenge(KahluaTable challenge ) void
* doKeyPress(boolean doIt ) void
* doTutorial(KahluaTable tutorial ) void
* drawOverheadMap(UIElement ui, float zoom, float xpos, float ypos ) void
* endFileInput( ) void
* endFileOutput( ) void
* endTextFileInput( ) void
* fileExists(String filename ) boolean
* forceChangeState(GameState state ) void
* forceDisconnect( ) void
* getActivatedMods( ) ArrayList
* getAllSavedPlayers( ) List
* getButtonCount(int joypad ) int
* getCallframeTop(Coroutine c ) int
* getCameraOffX( ) float
* getCameraOffY( ) float
* getCell( ) IsoCell
* getClassField(Object o, int i ) Field
* getClassFieldVal(Object o, Field field ) Object
* getClassFunction(Object o, int i ) Method
* getControllerCount( ) int
* getControllerName(int joypad ) String
* getCore( ) Core
* getCoroutineCallframeStack(Coroutine c, int n ) LuaCallFrame
* getCoroutineObjStack(Coroutine c, int n ) Object
* getCoroutineObjStackWithBase(Coroutine c, int n ) Object
* getCoroutineTop(Coroutine c ) int
* getCurrentCoroutine( ) Coroutine
* getDebug( ) boolean
* getEvolvedRecipes( ) Stack
* getFileInput(String filename ) DataInputStream
* getFilenameOfCallframe(LuaCallFrame c ) String
* getFilenameOfClosure(LuaClosure c ) String
* getFileOutput(String filename ) DataOutputStream
* getFileReader(String filename, boolean createIfNull ) BufferedReader
* getFileSeparator( ) String
* getFileWriter(String filename, boolean createIfNull, boolean append ) FileWriter
* getFirstLineOfClosure(LuaClosure c ) int
* getGameFilesInput(String filename ) DataInputStream
* getGameFilesTextInput(String filename ) BufferedReader
* getGameSpeed( ) int
* getGameTime( ) GameTime
* getHourMinute( ) String
* getItemText(String txt ) String
* getLastPlayedDate(String filename ) String
* getLineNumber(LuaCallFrame c ) int
* getListOfCommands(String command ) String
* getLoadedLua(int n ) String
* getLoadedLuaCount( ) int
* getLocalVarCount(Coroutine c ) int
* getLocalVarName(Coroutine c, int n ) String
* getLocalVarStack(Coroutine c, int n ) int
* getMapDirectoryTable( ) KahluaTable
* getMapInfo(String mapDir ) KahluaTable
* getMethodParameter(Method o, int i ) String
* getMethodParameterCount(Method o ) int
* getModDirectoryTable( ) KahluaTable
* getModFileReader(String modId, String filename, boolean createIfNull ) BufferedReader
* getModFileWriter(String modId, String filename, boolean createIfNull, boolean append ) FileWriter
* getModInfo(String modDir ) ChooseGameInfo.Mod
* getMouseX( ) int
* getMouseXScaled( ) int
* getMouseY( ) int
* getMouseYScaled( ) int
* getMyDocumentFolder( ) String
* getNumActivePlayers( ) int
* getNumClassFields(Object o ) int
* getNumClassFunctions(Object o ) int
* getOnlineUsername( ) String
* getPerformance( ) PerformanceSettings
* getPlayer( ) IsoPlayer
* getRenderer( ) SpriteRenderer
* getSandboxOptions( ) SandboxOptions
* getSaveDirectoryTable( ) KahluaTable
* getSaveInfo(String saveDir ) KahluaTable
* getScriptManager( ) ScriptManager
* getServerList( ) KahluaTable
* getServerModData( ) void
* getServerSpawnRegions( ) KahluaTable
* getShortenedFilename(String str ) String
* getSoundManager( ) BaseSoundManager
* getSpecificPlayer(int player ) IsoPlayer
* getSprite(String sprite ) IsoSprite
* getStoryDirectoryTable( ) KahluaTable
* getStoryInfo(String storyName ) ChooseGameInfo.Story
* getStorySavedTable( ) KahluaTable
* getText(String txt ) String
* getTextManager( ) TextManager
* getTexture(String filename ) Texture
* getTextureFromSaveDir(String filename, String saveName ) Texture
* getVirtualAndRealZombieCount( ) int
* getVirtualZombieManager( ) VirtualZombieManager
* getWorld( ) IsoWorld
* getWorldSoundManager( ) WorldSoundManager
* hasBreakpoint(String file, int line ) boolean
* hasDataBreakpoint(KahluaTable table, Object key ) boolean
* hasDataReadBreakpoint(KahluaTable table, Object key ) boolean
* initUISystem( ) void
* instanceItem(Item item ) InventoryItem
* instanceItem(String item ) InventoryItem
* instanceof(Object obj, String name ) boolean
* isAdmin( ) boolean
* isClient( ) boolean
* isCurrentExecutionPoint(String file, int line ) boolean
* isDemo( ) boolean
* isJoypadDown(int joypad ) boolean
* isJoypadLeft(int joypad ) boolean
* isJoypadPressed(int joypad, int button ) boolean
* isJoypadRight(int joypad ) boolean
* isJoypadUp(int joypad ) boolean
* isKeyDown(int key ) boolean
* isModActive(ChooseGameInfo.Mod mod ) boolean
* isMouseButtonDown(int number ) boolean
* isoToScreenX(float x, float y, float z ) float
* isoToScreenY(float x, float y, float z ) float
* isServer( ) boolean
* istype(Object obj, String name ) boolean
* isXBOXController( ) boolean
* localVarName(Coroutine c, int n ) String
* openUrl(String url ) void
* ping(String username, String pwd, String ip, String port ) void
* reloadLuaFile(String filename ) void
* reloadServerLuaFile(String filename ) void
* require(String f ) void
* save(boolean doCharacter ) void
* saveGame( ) void
* saveModsFile( ) void
* scoreboardUpdate( ) void
* screenZoomIn( ) void
* screenZoomOut( ) void
* sendClientCommand(String module, String command, KahluaTable args ) void
* SendCommandToServer(String command ) void
* sendServerCommand(String module, String command, KahluaTable args ) void
* sendWorldMessage(String message ) void
* serverConnect(String user, String pass, String server, String port ) void
* serverFileExists(String filename ) boolean
* setActivePlayer(int id ) void
* setGameSpeed(int NewSpeed ) void
* setPlayerJoypad(int player, int joypad ) void
* setPlayerMovementActive(int id, boolean bActive ) void
* setProgressBarValue(IsoPlayer player, int value ) void
* setShowPausedMessage(boolean b ) void
* stopPing( ) void
* tabToX(String a, int tabX ) String
* takeScreenshot(String fileName ) void
* takeScreenshot( ) void
* toggleBreakOnChange(KahluaTable table, Object key ) void
* toggleBreakOnRead(KahluaTable table, Object key ) void
* toggleBreakpoint(String file, int line ) void
* toggleModActive(ChooseGameInfo.Mod mod, boolean activate ) void
* toggleSafetyServer( ) void
* translatePointXInOverheadMapToWindow(float x, UIElement ui, float zoom, float xpos ) float
* translatePointXInOverheadMapToWorld(float x, UIElement ui, float zoom, float xpos ) float
* translatePointYInOverheadMapToWindow(float y, UIElement ui, float zoom, float ypos ) float
* translatePointYInOverheadMapToWorld(float y, UIElement ui, float zoom, float ypos ) float
* triggerEvent(String event, Object param, Object param2, Object param3, Object param4 ) void
* triggerEvent(String event, Object param, Object param2, Object param3 ) void
* triggerEvent(String event, Object param, Object param2 ) void
* triggerEvent(String event, Object param ) void
* triggerEvent(String event ) void
* useTextureFiltering(boolean bUse ) void
* writeLog(String loggerName, String logs ) void
* ZombRand(double max ) double
* ZombRand(double min, double max ) double
* ZombRandBetween(double min, double max ) double
* ZombRandFloat(float min, float max ) float 

----------------------------------------
* [Goto ToC](TOC.md)  
