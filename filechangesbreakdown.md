# File changes breakdown
In case you wish to undo some of my changes but keep others, open the relevant .ini file with your text editor of choice. There are other tiny misc optimizations/changes that will not impact your experience so I've skipped those.

The top will always be the vanilla game values and the bottom will be my edit as found in the ready-to-use files.

## APB Reloaded\APBGame\Config\DefaultEngine.ini
### **Black Login Screen** <br >
```Map=APBLoginLevel.apb``` <br >
```LocalMap=APBLoginLevel.apb``` <br >
changed to <br >
```Map=UIDistrict_DistrictSelect.apb``` <br >
```LocalMap=UIDistrict_DistrictSelect.apb``` <br >

### **Disabled Bounty Notifications (left side of the screen)** <br >
```+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Ceremony"``` <br >
changed to <br >
```;+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_Ceremony"``` <br >

### **Disabled Dirty Money (top left under pledged contact)**
```+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_OpenWorld"``` <br >
changed to <br >
```;+GlobalDataStoreClasses="APBUserInterface.cUIDataStore_HUD_OpenWorld"``` <br >

## APB Reloaded\Engine\Config\BaseEngine.ini <br >

### **FPS** <br >
```MinSmoothedFrameRate=22``` <br >
```MaxSmoothedFrameRate=100``` <br >
```MaxClientFrameRate=128``` <br >
changed to <br >
```;bSmoothFrameRate=TRUE``` <br >
```;MinSmoothedFrameRate=22``` <br >
```MaxSmoothedFrameRate=128``` <br >
```MaxClientFrameRate=0``` <br >

### **Disabled Texture Streaming (DTS)** <br >
```bUseTextureStreaming=True``` <br >
```bUseLightingTextureStreaming=True``` <br >
changed to <br >
```bUseTextureStreaming=False``` <br >
```bUseLightingTextureStreaming=False``` <br >


### **Garbage Collection (GC/Stutter Fix)** <br >
```TimeBetweenPurgingPendingKillObjects=60``` <br >
changed to <br >
```TimeBetweenPurgingPendingKillObjects=0``` <br >

### **Bloom** <br >
```DefaultPostProcessName=APBPostEffectMaterials.APBPostEffect_Process``` <br >
changed to <br >
```;DefaultPostProcessName=APBPostEffectMaterials.APBPostEffect_Process``` <br >


## APB Reloaded\APBGame\Config\DefaultGame.ini
### **Disable Muzzle Flash** <br >
```m_bEnableMuzzleFlash=true``` <br >
```m_bEnableMagazineCasings=true``` <br >
changed to <br >
```m_bEnableMuzzleFlash=false``` <br >
```m_bEnableMagazineCasings=false``` <br >

### **Ragdolls** <br >
NPC/Civilian Ragdolls <br >
```m_cfg_fMinNPCRagdollDisplayTime=60.0``` <br >
```m_cfg_fMaxNPCRagdollDisplayTime=120.0``` <br >
```m_cfg_nMaxNumberOfNPCRagdolls=30``` <br >
```m_cfg_nHardMaxNumberOfNPCRagdolls=45``` <br >
```m_cfg_fMinNPCRagdollDespawnDelay=10.0``` <br >
changed to <br >
```m_cfg_fMinNPCRagdollDisplayTime=0.0``` <br >
```m_cfg_fMaxNPCRagdollDisplayTime=0.0``` <br >
```m_cfg_nMaxNumberOfNPCRagdolls=0``` <br >
```m_cfg_nHardMaxNumberOfNPCRagdolls=0``` <br >
```m_cfg_fMinNPCRagdollDespawnDelay=0``` <br >

Player Ragdolls <br >
```m_nMaxDeadRagDollPawns=8``` <br >
```m_bDeathAnimations=true``` <br >
changed to <br >
```m_nMaxDeadRagDollPawns=0``` <br >
```m_bDeathAnimations=false``` <br >
