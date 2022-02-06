# crash-report
---- Minecraft Crash Report ----
// Don't be sad, have a hug! <3

Time: 04/02/2022, 19:37
Description: Exception in server tick loop

java.lang.OutOfMemoryError: Java heap space
	at java.base/java.util.LinkedHashMap$LinkedValues.iterator(LinkedHashMap.java:626)
	at net.minecraft.server.MinecraftServer.method_20415(MinecraftServer.java:767)
	at net.minecraft.server.MinecraftServer.method_16075(MinecraftServer.java:756)
	at net.minecraft.class_1255.method_5383(class_1255.java:110)
	at net.minecraft.server.MinecraftServer.method_16208(MinecraftServer.java:740)
	at net.minecraft.server.MinecraftServer.method_3774(MinecraftServer.java:499)
	at net.minecraft.server.MinecraftServer.method_3735(MinecraftServer.java:330)
	at net.minecraft.class_1132.method_3823(class_1132.java:72)
	at net.minecraft.server.MinecraftServer.method_29741(MinecraftServer.java:657)
	at net.minecraft.server.MinecraftServer.method_29739(MinecraftServer.java:270)
	at net.minecraft.server.MinecraftServer$$Lambda$9412/0x00000001014f7740.run(Unknown Source)
	at java.base/java.lang.Thread.run(Thread.java:833)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
Details:
	Minecraft Version: 1.18.1
	Minecraft Version ID: 1.18.1
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 17.0.1, Microsoft
	Java VM Version: OpenJDK 64-Bit Server VM (mixed mode), Microsoft
	Memory: 20893744 bytes (19 MiB) / 2147483648 bytes (2048 MiB) up to 2147483648 bytes (2048 MiB)
	CPUs: 12
	Processor Vendor: AuthenticAMD
	Processor Name: AMD Ryzen 5 3600 6-Core Processor              
	Identifier: AuthenticAMD Family 23 Model 113 Stepping 0
	Microarchitecture: Zen 2
	Frequency (GHz): 3.59
	Number of physical packages: 1
	Number of physical CPUs: 6
	Number of logical CPUs: 12
	Graphics card #0 name: NVIDIA GeForce GTX 1050 Ti
	Graphics card #0 vendor: NVIDIA (0x10de)
	Graphics card #0 VRAM (MB): 4095.00
	Graphics card #0 deviceId: 0x1c82
	Graphics card #0 versionInfo: DriverVersion=30.0.14.9709
	Memory slot #0 capacity (MB): 8192.00
	Memory slot #0 clockSpeed (GHz): 2.40
	Memory slot #0 type: DDR4
	Memory slot #1 capacity (MB): 8192.00
	Memory slot #1 clockSpeed (GHz): 2.40
	Memory slot #1 type: DDR4
	Virtual memory max (MB): 26555.36
	Virtual memory used (MB): 13022.21
	Swap memory total (MB): 10240.00
	Swap memory used (MB): 94.50
	JVM Flags: 9 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx2G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	Fabric Mods: 
		adorn: Adorn 3.2.0+1.18.1
		advanced_runtime_resource_pack: Runtime Resource Pack 0.2.9
		advancednetherite: Advanced Netherite 1.4.0-1.18.1
		amecsapi: Amecs API 1.3.3+mc1.18-pre1
		apoli: Apoli 2.2.2
		appleskin: AppleSkin 2.3.0+mc1.18.1
		aqupdgrizzly: Grizzly Bear mob 1.18-1.2.2
		architectury: Architectury 3.6.15
		backslot: BackSlot 1.2.4
		balm-fabric: Balm 2.4.1+0
		bclib: BCLib 1.2.5
		betterend: Better End 1.0.1
		blue_endless_jankson: jankson 1.2.1
		blur: Blur (Fabric) 2.4.1
		breakprogress: Break Progress 1.0.1
		byg: BYG 1.3.5.8
		calio: Calio 1.4.2
		capybara: Capybara 1.0.1
		cardinal-components-base: Cardinal Components API (base) 4.0.1
		cardinal-components-block: Cardinal Components API (blocks) 4.0.1
		cardinal-components-entity: Cardinal Components API (entities) 4.0.1
		cardinal-components-item: Cardinal Components API (items) 4.0.1
		carrier: Carrier 1.9.1
		cloth-basic-math: cloth-basic-math 0.6.0
		cloth-config: Cloth Config v6 6.1.48
		com_electronwill_night-config_core: core 3.6.4
		com_electronwill_night-config_toml: toml 3.6.4
		com_eliotlash_mclib_mclib: mclib 18
		com_eliotlash_molang_molang: molang 18
		com_typesafe_config: config 1.4.1
		confabricate: confabricate 2.2.0-SNAPSHOT+4.1.1
		copperarmorandtools: Copper Armor & Tools 1.9.2
		croptopia: Croptopia 1.8.0
		diggusmaximus: Diggus Maximus 1.5.2-1.18
		earthtojavamobs: Earth2Java 1.7.4+1.18
		enchantinginfuser: Enchanting Infuser 3.1.1
		expandedstorage: Expanded Storage 7.3.6
		fabric: Fabric API 0.46.4+1.18
		fabric-api-base: Fabric API Base 0.4.2+d7c144a865
		fabric-api-lookup-api-v1: Fabric API Lookup API (v1) 1.5.3+d7c144a865
		fabric-biome-api-v1: Fabric Biome API (v1) 6.0.2+d7c144a865
		fabric-blockrenderlayer-v1: Fabric BlockRenderLayer Registration (v1) 1.1.10+3ac43d9565
		fabric-command-api-v1: Fabric Command API (v1) 1.1.7+d7c144a865
		fabric-commands-v0: Fabric Commands (v0) 0.2.6+b4f4f6cd65
		fabric-containers-v0: Fabric Containers (v0) 0.1.19+d7c144a865
		fabric-content-registries-v0: Fabric Content Registries (v0) 0.4.8+d7c144a865
		fabric-crash-report-info-v1: Fabric Crash Report Info (v1) 0.1.9+3ac43d9565
		fabric-dimensions-v1: Fabric Dimensions API (v1) 2.1.10+a1d9bbf565
		fabric-entity-events-v1: Fabric Entity Events (v1) 1.4.6+d7c144a865
		fabric-events-interaction-v0: Fabric Events Interaction (v0) 0.4.17+d7c144a865
		fabric-events-lifecycle-v0: Fabric Events Lifecycle (v0) 0.2.9+d7c144a865
		fabric-game-rule-api-v1: Fabric Game Rule API (v1) 1.0.11+d7c144a865
		fabric-item-api-v1: Fabric Item API (v1) 1.3.1+691a79b565
		fabric-item-groups-v0: Fabric Item Groups (v0) 0.3.6+3ac43d9565
		fabric-key-binding-api-v1: Fabric Key Binding API (v1) 1.0.9+d7c144a865
		fabric-keybindings-v0: Fabric Key Bindings (v0) 0.2.7+b4f4f6cd65
		fabric-language-kotlin: Fabric Language Kotlin 1.7.1+kotlin.1.6.10
		fabric-lifecycle-events-v1: Fabric Lifecycle Events (v1) 1.4.13+713c266865
		fabric-loot-tables-v1: Fabric Loot Tables (v1) 1.0.9+d7c144a865
		fabric-mining-level-api-v1: Fabric Mining Level API (v1) 1.0.6+d7c144a865
		fabric-mining-levels-v0: Fabric Mining Levels (v0) 0.1.11+b4f4f6cd65
		fabric-models-v0: Fabric Models (v0) 0.3.4+d7c144a865
		fabric-networking-api-v1: Fabric Networking API (v1) 1.0.19+d7c144a865
		fabric-networking-v0: Fabric Networking (v0) 0.3.6+b4f4f6cd65
		fabric-object-builder-api-v1: Fabric Object Builder API (v1) 1.11.4+d7c144a865
		fabric-object-builders-v0: Fabric Object Builders (v0) 0.7.12+d7c144a865
		fabric-particles-v1: Fabric Particles (v1) 0.2.10+526dc1ac65
		fabric-permissions-api-v0: fabric-permissions-api 0.1-SNAPSHOT
		fabric-registry-sync-v0: Fabric Registry Sync (v0) 0.9.2+ad01bfbd65
		fabric-renderer-api-v1: Fabric Renderer API (v1) 0.4.11+b0b66fc365
		fabric-renderer-indigo: Fabric Renderer - Indigo 0.4.15+6825030165
		fabric-renderer-registries-v1: Fabric Renderer Registries (v1) 3.2.10+b4f4f6cd65
		fabric-rendering-data-attachment-v1: Fabric Rendering Data Attachment (v1) 0.3.5+d7c144a865
		fabric-rendering-fluids-v1: Fabric Rendering Fluids (v1) 0.1.19+3ac43d9565
		fabric-rendering-v0: Fabric Rendering (v0) 1.1.12+b4f4f6cd65
		fabric-rendering-v1: Fabric Rendering (v1) 1.10.6+713c266865
		fabric-resource-conditions-api-v1: Fabric Resource Conditions API (v1) 1.0.2+d7c144a865
		fabric-resource-loader-v0: Fabric Resource Loader (v0) 0.4.14+713c266865
		fabric-screen-api-v1: Fabric Screen API (v1) 1.0.8+d7c144a865
		fabric-screen-handler-api-v1: Fabric Screen Handler API (v1) 1.1.12+d7c144a865
		fabric-structure-api-v1: Fabric Structure API (v1) 2.1.3+d7c144a865
		fabric-tag-extensions-v0: Fabric Tag Extensions (v0) 1.2.8+d7c144a865
		fabric-textures-v0: Fabric Textures (v0) 1.0.10+3ac43d9565
		fabric-tool-attribute-api-v1: Fabric Tool Attribute API (v1) 1.3.8+fb3b57b465
		fabric-transfer-api-v1: Fabric Transfer API (v1) 1.5.9+d7c144a865
		fabricloader: Fabric Loader 0.12.12
		feature_nbt_deadlock_be_gone: Feature NBT Deadlock Be Gone - Fabric $version
		forgeconfigapiport: Forge Config API Port 3.1.1
		geckolib3: Geckolib 3.0.32
		graveyard: The Graveyard 1.5
		hologram-api: Hologram API 0.2.1+1.18-pre5
		inventoryhud: Inventory HUD + 3.4.2
		io_leangen_geantyref_geantyref: geantyref 1.3.11
		jankson: Jankson 4.0.0+j1.2.0
		java: OpenJDK 64-Bit Server VM 17
		kyrptconfig: Kyrpt Config 1.2.4-1.18
		libcd: LibCapableData 3.0.3+1.16.3
		libzoomer: LibZoomer 0.3.0+1.17.1
		magna: Magna 1.7.0-1.18-pre1
		maybe-data: Maybe data 1.0.1-1.17
		midnightlib: MidnightLib 0.3.1
		minecraft: Minecraft 1.18.1
		modmenu: Mod Menu 3.0.1
		mostructures: Mo' Structures 1.3.0-pre1+1.18
		mousetweaks: Mouse Tweaks 2.22
		ninjaphenix_container_lib: NinjaPhenix's Container Library 1.2.10
		no_null_processors: No Null Processors - Fabric 2.0.1+1.18.1
		notenoughanimations: NotEnoughAnimations 1.4.0
		nukes: Nukes 1.0.1
		okzoomer: Ok Zoomer 5.0.0-beta.3+1.17.1
		omega-config: OmegaConfig 1.2.2-1.18.1
		org_aperlambda_lambdajcommon: lambdajcommon 1.8.1
		org_jetbrains_kotlin_kotlin-reflect: kotlin-reflect 1.6.10
		org_jetbrains_kotlin_kotlin-stdlib: kotlin-stdlib 1.6.10
		org_jetbrains_kotlin_kotlin-stdlib-jdk7: kotlin-stdlib-jdk7 1.6.10
		org_jetbrains_kotlin_kotlin-stdlib-jdk8: kotlin-stdlib-jdk8 1.6.10
		org_jetbrains_kotlinx_kotlinx-coroutines-core-jvm: kotlinx-coroutines-core-jvm 1.5.2
		org_jetbrains_kotlinx_kotlinx-coroutines-jdk8: kotlinx-coroutines-jdk8 1.5.2
		org_jetbrains_kotlinx_kotlinx-serialization-cbor-jvm: kotlinx-serialization-cbor-jvm 1.3.1
		org_jetbrains_kotlinx_kotlinx-serialization-core-jvm: kotlinx-serialization-core-jvm 1.3.1
		org_jetbrains_kotlinx_kotlinx-serialization-json-jvm: kotlinx-serialization-json-jvm 1.3.1
		org_quiltmc_quilt-json5: quilt-json5 1.0.0
		org_spongepowered_configurate-core: configurate-core 4.1.1
		org_spongepowered_configurate-extra-dfu4: configurate-extra-dfu4 4.1.1
		org_spongepowered_configurate-gson: configurate-gson 4.1.1
		org_spongepowered_configurate-hocon: configurate-hocon 4.1.1
		origins: Origins 1.3.1
		packet_tweaker: Packet Tweaker 0.2.0+1.18-pre1
		placeholder-api: Placeholder API 1.1.3+1.17.1
		playerabilitylib: Pal 1.3.0
		polymer: Polymer (Core) 0.2.0-beta.21+1.18.1
		polymer-legacy: Polymer (Compatibility) 0.1.9+0.2.0-beta.21+1.18.1
		polymorph: Polymorph 0.0.19-1.18.1
		puzzleslib: Puzzles Lib 3.1.3
		reach-entity-attributes: Reach Entity Attributes 2.1.1
		repurposed_structures: Repurposed Structures 3.3.6+1.18.1
		roughlyenoughitems: Roughly Enough Items 7.2.418
		satin: Satin 1.7.0
		server_translations_api: Server Translations API 1.4.8+1.18-pre1
		sgui: sgui 1.0.0-rc6+1.18-pre5
		slotlink: slotlink 4.2.1
		spruceui: SpruceUI 3.3.0+1.17
		static-content: Static Content 1.0.2-1.16.2
		staticdata: Static Data 1.1.2
		terrablender: TerraBlender 1.1.0.73
		torohealth: ToroHealth Damage Indicators 1.18-fabric-2
		towers_of_the_wild_reworked: Towers of the Wild: Reworked 2.1.1
		tradingpost: Trading Post 3.1.2
		trashslot: TrashSlot 11.0.1
		universal-graves: Universal Graves 2.0.0-rc.1+1.18.1
		vanilla-hammers: Vanilla Hammers 3.2.0-1.18.1
		visualworkbench: Visual Workbench 3.1.0
		waystones: Waystones 9.0.3
		wthit: wthit 4.5.1
		xaerominimap: Xaero's Minimap 22.1.2
	Server Running: true
	Player Count: 0 / 8; []
	Data Packs: vanilla, Fabric Mods
	Type: Integrated Server (map_client.txt)
	Is Modded: Definitely; Client brand changed to 'fabric'; Server brand changed to 'fabric'
