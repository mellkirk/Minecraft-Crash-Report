---- Minecraft Crash Report ----
// Shall we play a game?

Time: 6/15/15 4:10 PM
Description: Registering texture

java.lang.OutOfMemoryError: Java heap space
	at net.minecraft.client.renderer.texture.TextureUtil.func_110993_a(TextureUtil.java:241)
	at net.minecraft.client.renderer.texture.TextureUtil.func_110995_a(TextureUtil.java:232)
	at net.minecraft.client.renderer.texture.TextureUtil.func_110989_a(TextureUtil.java:194)
	at net.minecraft.client.renderer.texture.SimpleTexture.func_110551_a(SourceFile:48)
	at net.minecraft.client.renderer.texture.TextureManager.func_110579_a(SourceFile:72)
	at net.minecraft.client.renderer.texture.TextureManager.func_110577_a(SourceFile:40)
	at net.minecraft.client.LoadingScreenRenderer.func_73718_a(LoadingScreenRenderer.java:145)
	at net.minecraft.client.LoadingScreenRenderer.func_73719_c(LoadingScreenRenderer.java:94)
	at net.minecraft.client.Minecraft.func_71353_a(Unknown Source)
	at net.minecraft.client.Minecraft.func_71403_a(Unknown Source)
	at net.minecraft.client.Minecraft.func_71371_a(Unknown Source)
	at com.xcompwiz.mystcraft.MystcraftFirstRun.start(MystcraftFirstRun.java:57)
	at com.xcompwiz.mystcraft.error.MystcraftStartupChecker.onClientTick(MystcraftStartupChecker.java:117)
	at cpw.mods.fml.common.eventhandler.ASMEventHandler_388_MystcraftStartupChecker_onClientTick_ClientTickEvent.invoke(.dynamic)
	at cpw.mods.fml.common.eventhandler.ASMEventHandler.invoke(ASMEventHandler.java:54)
	at cpw.mods.fml.common.eventhandler.EventBus.post(EventBus.java:138)
	at cpw.mods.fml.common.FMLCommonHandler.onPreClientTick(FMLCommonHandler.java:325)
	at net.minecraft.client.Minecraft.func_71407_l(Unknown Source)
	at net.minecraft.client.Minecraft.func_71411_J(Unknown Source)
	at net.minecraft.client.Minecraft.func_99999_d(Unknown Source)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at net.minecraft.client.renderer.texture.TextureUtil.func_110993_a(TextureUtil.java:241)
	at net.minecraft.client.renderer.texture.TextureUtil.func_110995_a(TextureUtil.java:232)
	at net.minecraft.client.renderer.texture.TextureUtil.func_110989_a(TextureUtil.java:194)
	at net.minecraft.client.renderer.texture.SimpleTexture.func_110551_a(SourceFile:48)

-- Resource location being registered --
Details:
	Resource location: minecraft:textures/gui/options_background.png
	Texture object class: net.minecraft.client.renderer.texture.SimpleTexture
Stacktrace:
	at net.minecraft.client.renderer.texture.TextureManager.func_110579_a(SourceFile:72)
	at net.minecraft.client.renderer.texture.TextureManager.func_110577_a(SourceFile:40)
	at net.minecraft.client.LoadingScreenRenderer.func_73718_a(LoadingScreenRenderer.java:145)
	at net.minecraft.client.LoadingScreenRenderer.func_73719_c(LoadingScreenRenderer.java:94)
	at net.minecraft.client.Minecraft.func_71353_a(Unknown Source)
	at net.minecraft.client.Minecraft.func_71403_a(Unknown Source)
	at net.minecraft.client.Minecraft.func_71371_a(Unknown Source)
	at com.xcompwiz.mystcraft.MystcraftFirstRun.start(MystcraftFirstRun.java:57)
	at com.xcompwiz.mystcraft.error.MystcraftStartupChecker.onClientTick(MystcraftStartupChecker.java:117)
	at cpw.mods.fml.common.eventhandler.ASMEventHandler_388_MystcraftStartupChecker_onClientTick_ClientTickEvent.invoke(.dynamic)
	at cpw.mods.fml.common.eventhandler.ASMEventHandler.invoke(ASMEventHandler.java:54)
	at cpw.mods.fml.common.eventhandler.EventBus.post(EventBus.java:138)
	at cpw.mods.fml.common.FMLCommonHandler.onPreClientTick(FMLCommonHandler.java:325)
	at net.minecraft.client.Minecraft.func_71407_l(Unknown Source)
	at net.minecraft.client.Minecraft.func_71411_J(Unknown Source)
	at net.minecraft.client.Minecraft.func_99999_d(Unknown Source)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 8.1 (amd64) version 6.3
	Java Version: 1.8.0_45, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 19970000 bytes (19 MB) / 1060372480 bytes (1011 MB) up to 1060372480 bytes (1011 MB)
	JVM Flags: 6 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx1G -XX:+UseConcMarkSweepGC -XX:+CMSIncrementalMode -XX:-UseAdaptiveSizePolicy -Xmn128M
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP v9.05 FML v7.10.99.99 Minecraft Forge 10.13.4.1451 139 mods loaded, 139 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
	UCHIJA	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) 
	UCHIJA	FML{7.10.99.99} [Forge Mod Loader] (forge-1.7.10-10.13.4.1451-1.7.10.jar) 
	UCHIJA	Forge{10.13.4.1451} [Minecraft Forge] (forge-1.7.10-10.13.4.1451-1.7.10.jar) 
	UCHIJA	appliedenergistics2-core{rv2-stable-8} [AppliedEnergistics2 Core] (minecraft.jar) 
	UCHIJA	CodeChickenCore{1.0.7.46} [CodeChicken Core] (minecraft.jar) 
	UCHIJA	NotEnoughItems{1.0.5.111} [Not Enough Items] (NotEnoughItems-1.7.10-1.0.5.111-universal.jar) 
	UCHIJA	RB-Core{0.0.0.1} [RotatableBlocks Core] (minecraft.jar) 
	UCHIJA	ThaumicTinkerer-preloader{0.1} [Thaumic Tinkerer Core] (minecraft.jar) 
	UCHIJA	VeinMiner_coremod{0.27.1_build.unknown} [Core mod] (minecraft.jar) 
	UCHIJA	<CoFH ASM>{000} [CoFH ASM] (minecraft.jar) 
	UCHIJA	sapmanpack{2.5.1} [SanAndreasPs Manager Pack CORE edition] (SAPManPack-1.7.10-2.5.1.jar) 
	UCHIJA	battlegear2{1.7.10} [Mine & Blade Battlegear 2 - Bullseye] (1.7.10-MB_Battlegear2-Bullseye-1.0.8.0.jar) 
	UCHIJA	DamageIndicatorsMod{3.2.3} [Damage Indicators] ([1.7.10]DamageIndicatorsMod-3.2.3.jar) 
	UCHIJA	AnimationAPI{1.2.3} [AnimationAPI] (AnimationAPI-1.7.10-1.2.3.jar) 
	UCHIJA	appliedenergistics2{rv2-stable-8} [Applied Energistics 2] (appliedenergistics2-rv2-stable-8.jar) 
	UCHIJA	aquaticabyss{1.1.0} [Aquatic Abyss] (AquaticAbyss-1.7.2-1.1.0.jar) 
	UCHIJA	ArchimedesShips{1.7.10 v1.7.1} [Archimedes' Ships] (ArchimedesShips-1.7.1.jar) 
	UCHIJA	armourersWorkshop{1.7.10-0.33.0.84} [Armourer's Workshop] (Armourers-Workshop-1.7.10-0.33.0.84.jar) 
	UCHIJA	BetterFoliage{1.0.13} [Better Foliage] (BetterFoliage-mc1.7-1.0.13.jar) 
	UCHIJA	Baubles{1.0.1.10} [Baubles] (Baubles-1.7.10-1.0.1.10.jar) 
	UCHIJA	Thaumcraft{4.2.3.5} [Thaumcraft] (Thaumcraft-1.7.10-4.2.3.5.jar) 
	UCHIJA	betterstorage{0.13.1.126} [BetterStorage] (BetterStorage-1.7.10-0.13.1.126.jar) 
	UCHIJA	BiblioCraft{1.10.4} [BiblioCraft] (BiblioCraft[v1.10.4][MC1.7.10].jar) 
	UCHIJA	Mantle{1.7.10-0.3.2.jenkins184} [Mantle] (Mantle-1.7.10-0.3.2.jar) 
	UCHIJA	Natura{2.2.0} [Natura] (natura-1.7.10-2.2.0.1.jar) 
	UCHIJA	BiomesOPlenty{2.1.0} [Biomes O' Plenty] (BiomesOPlenty-1.7.10-2.1.0.1283-universal.jar) 
	UCHIJA	BiblioWoodsBoP{1.9} [BiblioWoods Biomes O'Plenty Edition] (BiblioWoods[BiomesOPlenty][v1.9].jar) 
	UCHIJA	BiblioWoodsNatura{1.5} [BiblioWoods Natura Edition] (BiblioWoods[Natura][v1.5].jar) 
	UCHIJA	CoFHCore{1.7.10R3.0.2} [CoFH Core] (CoFHCore-[1.7.10]3.0.2-262.jar) 
	UCHIJA	BuildCraft|Core{7.0.9} [BuildCraft] (buildcraft-7.0.9.jar) 
	UCHIJA	BuildCraft|Silicon{7.0.9} [BC Silicon] (buildcraft-7.0.9.jar) 
	UCHIJA	BuildCraft|Transport{7.0.9} [BC Transport] (buildcraft-7.0.9.jar) 
	UCHIJA	BuildCraft|Builders{7.0.9} [BC Builders] (buildcraft-7.0.9.jar) 
	UCHIJA	BuildCraft|Robotics{7.0.9} [BC Robotics] (buildcraft-7.0.9.jar) 
	UCHIJA	BuildCraft|Energy{7.0.9} [BC Energy] (buildcraft-7.0.9.jar) 
	UCHIJA	BuildCraft|Factory{7.0.9} [BC Factory] (buildcraft-7.0.9.jar) 
	UCHIJA	CarpentersBlocks{3.3.6} [Carpenter's Blocks] (Carpenter's Blocks v3.3.6 - MC 1.7.10.jar) 
	UCHIJA	kegare.caveworld{1.8.3} [Caveworld] (Caveworld_1.7.10-v1.8.3.jar) 
	UCHIJA	ChickenChunks{1.3.4.19} [ChickenChunks] (ChickenChunks-1.7.10-1.3.4.19-universal.jar) 
	UCHIJA	ForgeMultipart{1.2.0.345} [Forge Multipart] (ForgeMultipart-1.7.10-1.2.0.345-universal.jar) 
	UCHIJA	chisel{2.3.10.37} [Chisel 2] (Chisel2-2.3.10.37.jar) 
	UCHIJA	ChiselFacades{1.7.10-2.11-cricket} [Chisel Facades] (ChiselFacades-1.7.10-2.11-cricket.jar) 
	UCHIJA	chocolateQuest{1.0} [Chocolate Quest] (chocolateQuest-1.7.10-1.0.jar) 
	UCHIJA	claysoldiers{2.0.0-beta.2} [Clay Soldiers Mod] (ClaySoldiersMod-1.7.10-2.0.0-beta.2.jar) 
	UCHIJA	creativecore{1.0} [CreativeCore] (CreativeCore v1.1.4 mc1.7.10.jar) 
	UCHIJA	CustomSpawner{3.3.0} [DrZhark's CustomSpawner] (CustomMobSpawner 3.3.0.zip) 
	UCHIJA	props{2.0.2} [Decocraft] (Decocraft-2.0.2_1.7.10.jar) 
	UCHIJA	MoCreatures{6.3.1} [DrZhark's Mo'Creatures Mod] (DrZharks MoCreatures Mod v6.3.1.zip) 
	UCHIJA	dungeonmobs{4.1.2} [Dungeon Mobs] (Dungeon Mobs v4.1.2.jar) 
	UCHIJA	eplus{3.0.2-d} [Enchanting Plus] (EnchantingPlus-1.7.10-3.0.2-d.jar) 
	UCHIJA	MetallurgyCore{4.0.4} [Metallurgy Core] (MetallurgyCore-1.7.10-4.0.4.18.jar) 
	UCHIJA	Mekanism{8.1.5} [Mekanism] (Mekanism-1.7.10-8.1.5.237.jar) 
	UCHIJA	EnderIO{1.7.10-2.2.8.381} [Ender IO] (EnderIO-1.7.10-2.2.8.381.jar) 
	UCHIJA	EnderStorage{1.4.7.36} [EnderStorage] (EnderStorage-1.7.10-1.4.7.36-universal.jar) 
	UCHIJA	EnderZoo{1.7.10-1.0.11.28} [Ender Zoo] (EnderZoo-1.7.10-1.0.11.28.jar) 
	UCHIJA	EE3{0.3.507} [Equivalent Exchange 3] (EquivalentExchange3-1.7.10-0.3.507.jar) 
	UCHIJA	ThermalFoundation{1.7.10R1.0.0} [Thermal Foundation] (ThermalFoundation-[1.7.10]1.0.0-81.jar) 
	UCHIJA	ThermalExpansion{1.7.10R4.0.1} [Thermal Expansion] (ThermalExpansion-[1.7.10]4.0.1-182.jar) 
	UCHIJA	Waila{1.5.10} [Waila] (Waila-1.5.10_1.7.10.jar) 
	UCHIJA	TConstruct{1.7.10-1.8.5.build957} [Tinkers' Construct] (TConstruct-1.7.10-1.8.5.jar) 
	UCHIJA	ExtraUtilities{1.2.6} [Extra Utilities] (extrautilities-1.2.6.jar) 
	UCHIJA	Metallurgy{4.0.6} [Metallurgy 4] (Metallurgy-1.7.10-4.0.6.80.jar) 
	UCHIJA	harvestcraft{1.7.10i} [Pam's HarvestCraft] (Pam's HarvestCraft 1.7.10i.jar) 
	UCHIJA	ExtraTiC{1.4.5} [ExtraTiC] (ExtraTiC-1.7.10-1.4.5.jar) 
	UCHIJA	farseek{1.0.8} [Farseek] (Farseek-1.0.8.jar) 
	UCHIJA	FastCraft{1.21} [FastCraft] (fastcraft-1.21.jar) 
	UCHIJA	Steamcraft{0.28.7} [Flaxbeard's Steam Power] (Flaxbeard'sSteamPower-1.7.10-0.28.7.jar) 
	UCHIJA	ThaumicTinkerer{unspecified} [Thaumic Tinkerer] (ThaumicTinkerer-2.5-1.7.10-164.jar) 
	UCHIJA	ForbiddenMagic{1.7.10-0.562} [Forbidden Magic] (Forbidden Magic-1.7.10-0.562.jar) 
	UCHIJA	foxlib{1.7.10-0.7.0} [FoxLib] (FoxLib-1.7.10-0.7.0.jar) 
	UCHIJA	funkylocomotion{1.0} [Funky Locomotion] (funky-locomotion-1.7.10-beta-5c.jar) 
	UCHIJA	Growthcraft{2.1.0a} [Growthcraft] (growthcraft-core-1.7.10-2.1.0a.jar) 
	UCHIJA	Growthcraft|Cellar{2.1.0a} [Growthcraft Cellar] (growthcraft-cellar-1.7.10-2.1.0a.jar) 
	UCHIJA	Growthcraft|Apples{2.1.0} [Growthcraft Apples] (growthcraft-apples-1.7.10-2.1.0.jar) 
	UCHIJA	Growthcraft|Bamboo{2.1.0} [Growthcraft Bamboo] (growthcraft-bamboo-1.7.10-2.1.0.jar) 
	UCHIJA	Growthcraft|Bees{2.1.0} [Growthcraft Bees] (growthcraft-bees-1.7.10-2.1.0.jar) 
	UCHIJA	Growthcraft|Fishtrap{2.1.0a} [Growthcraft Fishtrap] (growthcraft-fishtrap-1.7.10-2.1.0a.jar) 
	UCHIJA	Growthcraft|Grapes{2.1.0} [Growthcraft Grapes] (growthcraft-grapes-1.7.10-2.1.0.jar) 
	UCHIJA	Growthcraft|Hops{2.1.0} [Growthcraft Hops] (growthcraft-hops-1.7.10-2.1.0.jar) 
	UCHIJA	Growthcraft|Rice{2.1.0a} [Growthcraft Rice] (growthcraft-rice-1.7.10-2.1.0a.jar) 
	UCHIJA	iChunUtil{4.2.2} [iChunUtil] (iChunUtil-4.2.2.jar) 
	UCHIJA	ImmersiveEngineering{0.1.9} [Immersive Engineering] (ImmersiveEngineering-0.1.9.jar) 
	UCHIJA	InfernalMobs{1.6.1} [Infernal Mobs] (InfernalMobs-1.7.10.jar) 
	UCHIJA	JABBA{1.2.1} [JABBA] (Jabba-1.2.1a_1.7.10.jar) 
	UCHIJA	journeymap{5.0.1} [JourneyMap] (JourneyMap5.0.1_Unlimited_MC1.7.10.jar) 
	UCHIJA	latticemod{1.0} [Lattice Mod] (latticemod-mc1.7.10-1.0.jar) 
	UCHIJA	littletiles{0.1} [LittleTiles] (LittleTiles v0.3.2 mc1.7.10.jar) 
	UCHIJA	LookingGlass{0.1.0.00} [Looking Glass] (lookingglass-1.7.10-0.1.0.00.jar) 
	UCHIJA	MagiaNaturalis{0.1.1} [§2Magia Naturalis] (MagiaNaturalis-1.7.10-0.1.2c.jar) 
	UCHIJA	malisiscore{1.7.10-0.12.3} [MalisisCore] (malisiscore-1.7.10-0.12.3.jar) 
	UCHIJA	malisisdoors{1.7.10-1.8.1} [Malisis' Doors] (malisisdoors-1.7.10-1.8.1.jar) 
	UCHIJA	MekanismGenerators{8.1.5} [MekanismGenerators] (MekanismGenerators-1.7.10-8.1.5.237.jar) 
	UCHIJA	MekanismTools{8.1.5} [MekanismTools] (MekanismTools-1.7.10-8.1.5.237.jar) 
	UCHIJA	morechisels{@VERSION@} [More Chisels] (MoreChisels-1.7.10-1.0-20.jar) 
	UCHIJA	Morph{0.9.1} [Morph] (Morph-Beta-0.9.1.jar) 
	UCHIJA	Mystcraft{0.11.12.00} [Mystcraft] (mystcraft-1.7.10-0.11.12.00.jar) 
	UCHIJA	NetherOres{1.7.10R2.3.0} [Nether Ores] (NetherOres-[1.7.10]2.3.0-12.jar) 
	UCHIJA	OmnisCore{0.1.0} [Omnis Core] (OmnisCore-1.7.10 - 0.0.6-universal.jar) 
	UCHIJA	clayspawn{1.7.2a} [Pam's Clay Spawn] (Pam's Clay Spawn 1.7.2a.zip) 
	UCHIJA	getalltheseeds{1.7.2a} [Pam's Get all the Seeds!] (Pam's Get all the Seeds 1.7.2a.zip) 
	UCHIJA	harvestthenether{1.7.10} [Pam's Harvest the Nether] (Pam's Harvest the Nether 1.7.10a.jar) 
	UCHIJA	randomplants{1.7.2a} [Pam's RandomPlants] (Pam's Random Pants 1.7.2a.zip) 
	UCHIJA	plantmegapack{4.23} [Plant Mega Pack] (plantmegapack-4.23-1.7.10-1448.jar) 
	UCHIJA	PneumaticCraft{1.8.1-83} [PneumaticCraft] (PneumaticCraft-1.7.10-1.8.1-83-universal.jar) 
	UCHIJA	ProjectBlue{1.1.4} [Project Blue] (ProjectBlue-1.1.4-mc1.7.10.jar) 
	UCHIJA	MrTJPCoreMod{1.0.9.18} [MrTJPCore] (MrTJPCore-1.0.9.18-universal.jar) 
	UCHIJA	ProjRed|Core{4.7.0pre1.84} [ProjectRed] (ProjectRed-1.7.10-4.7.0pre1.84-Base.jar) 
	UCHIJA	ProjRed|Transmission{4.7.0pre1.84} [ProjectRed-Transmission] (ProjectRed-1.7.10-4.7.0pre1.84-Integration.jar) 
	UCHIJA	ProjRed|Transportation{4.7.0pre1.84} [ProjectRed-Transportation] (ProjectRed-1.7.10-4.7.0pre1.84-Mechanical_beta.jar) 
	UCHIJA	ProjRed|Compatibility{4.7.0pre1.84} [ProjectRed-Compatibility] (ProjectRed-1.7.10-4.7.0pre1.84-Compat.jar) 
	UCHIJA	ProjRed|Integration{4.7.0pre1.84} [ProjectRed-Integration] (ProjectRed-1.7.10-4.7.0pre1.84-Integration.jar) 
	UCHIJA	ProjRed|Illumination{4.7.0pre1.84} [ProjectRed-Illumination] (ProjectRed-1.7.10-4.7.0pre1.84-Lighting.jar) 
	UCHIJA	ProjRed|Expansion{4.7.0pre1.84} [ProjectRed-Expansion] (ProjectRed-1.7.10-4.7.0pre1.84-Mechanical_beta.jar) 
	UCHIJA	quiverchevsky{b100} [QuiverBow] (QuiverBow_1.7.10_b100.zip) 
	UCHIJA	Roguelike{1.3.6.3} [Roguelike Dungeons] (roguelike-1.7.10-1.3.6.3.jar) 
	UCHIJA	RotatableBlocks{172-build-9} [Rotatable Blocks] (rotateableblocks-17x-build-9.jar) 
	UCHIJA	RWG{Alpha 1.3.2} [Realistic World Gen Alpha] (RWG-alpha-1.3.2.jar) 
	UCHIJA	StargateTech2{0.7.7-Alpha} [StargateTech 2] (StargateTech2-Alpha-0-7-8-MC1710-Forge1232.jar) 
	UCHIJA	streams{0.1.4} [Streams] (Streams-0.1.4.jar) 
	UCHIJA	Tails{1.7.10-1.3.1} [Tails] (Tails-1.7.10-1.3.1.jar) 
	UCHIJA	TaintedMagic{1.1.3.7} [Tainted Magic] (TaintedMagic-1.1.3.7.jar) 
	UCHIJA	ThaumcraftMobAspects{1.7.2-2A} [Thaumcraft Mob Aspects] (ThaumcraftMobAspects-1.7.2-2A.jar) 
	UCHIJA	ThaumicMachina{0.2.1} [Thaumic Machina] (Thaumic Machina-1.7.10-0.2.1.jar) 
	UCHIJA	thaumicenergistics{0.8.10.5} [Thaumic Energistics] (thaumicenergistics-0.8.10.5.jar) 
	UCHIJA	ThaumicExploration{0.6.0} [Thaumic Exploration] (ThaumicExploration-1.7.10-1.1-37.jar) 
	UCHIJA	thaumicinfusion{4.05} [Thaumic Infusion] (ThaumicInfusion-4.06.jar) 
	UCHIJA	ThaumicPipes{1.2.00} [Thaumic Pipes] (ThaumicPipes-1.7.10 - 1.2.1b-universal.jar) 
	UCHIJA	tinkersdefense{1.2} [Tinkers' Defense] (Tinkers-Defense-1.2.1.jar) 
	UCHIJA	Translocator{1.1.2.15} [Translocator] (Translocator-1.7.10-1.1.2.15-universal.jar) 
	UCHIJA	ttCore{MC1.7.10-0.1.0-67} [ttCore] (ttCore-MC1.7.10-0.1.0-67.jar) 
	UCHIJA	VeinMiner{0.27.1_build.unknown} [Vein Miner] (VeinMiner-1.7.10_0.27.1.unknown.jar) 
	UCHIJA	VeinMinerModSupport{0.27.1_build.unknown} [Mod Support] (VeinMiner-1.7.10_0.27.1.unknown.jar) 
	UCHIJA	wailaplugins{MC1.7.10-0.0.1-15} [WAILA Plugins] (WAILAPlugins-MC1.7.10-0.0.1-15.jar) 
	UCHIJA	wawla{1.1.1} [What Are We Looking At] (Wawla-1.1.1_1.7.10.jar) 
	UCHIJA	WR-CBE|Core{1.4.1.9} [WR-CBE Core] (WR-CBE-1.7.10-1.4.1.9-universal.jar) 
	UCHIJA	WR-CBE|Addons{1.4.1.9} [WR-CBE Addons] (WR-CBE-1.7.10-1.4.1.9-universal.jar) 
	UCHIJA	WR-CBE|Logic{1.4.1.9} [WR-CBE Logic] (WR-CBE-1.7.10-1.4.1.9-universal.jar) 
	UCHIJA	McMultipart{1.2.0.345} [Minecraft Multipart Plugin] (ForgeMultipart-1.7.10-1.2.0.345-universal.jar) 
	UCHIJA	ForgeMicroblock{1.2.0.345} [Forge Microblocks] (ForgeMultipart-1.7.10-1.2.0.345-universal.jar) 
	GL info: ' Vendor: 'ATI Technologies Inc.' Version: '4.2.12422 Compatibility Profile Context 13.152.1.1000' Renderer: 'AMD Radeon HD 7560D'
	AE2 Version: stable rv2-stable-8 for Forge 10.13.2.1291
	Mantle Environment: Environment healthy.
	CoFHCore: -[1.7.10]3.0.2-262
	ThermalFoundation: -[1.7.10]1.0.0-81
	ThermalExpansion: -[1.7.10]4.0.1-182
	TConstruct Environment: Environment healthy.
	NetherOres: -[1.7.10]2.3.0-12
	AE2 Integration: IC2:OFF, RotaryCraft:OFF, RC:OFF, BC:ON, RF:ON, RFItem:ON, MFR:OFF, DSU:ON, FZ:OFF, FMP:ON, RB:ON, CLApi:OFF, Waila:ON, InvTweaks:OFF, NEI:ON, CraftGuide:OFF, Mekanism:ON, ImmibisMicroblocks:OFF, BetterStorage:ON
	Launched Version: 1.7.10-Forge10.13.4.1451-1.7.10
	LWJGL: 2.9.1
	OpenGL: AMD Radeon HD 7560D GL version 4.2.12422 Compatibility Profile Context 13.152.1.1000, ATI Technologies Inc.
	GL Caps: Using GL 1.3 multitexturing.
Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
Anisotropic filtering is supported and maximum anisotropy is 16.
Shaders are available because OpenGL 2.1 is supported.

	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: []
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	Anisotropic Filtering: Off (1)
