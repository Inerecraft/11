---- Minecraft Crash Report ----
// There are four lights!

Time: 2020-05-20 14:23:30 CST
Description: Initializing game

java.lang.NoClassDefFoundError: hellfirepvp/astralsorcery/common/starlight/transmission/registry/TransmissionClassRegistry$TransmissionProvider
    at java.lang.Class.getDeclaredMethods0(Native Method)
    at java.lang.Class.privateGetDeclaredMethods(Class.java:2701)
    at java.lang.Class.privateGetPublicMethods(Class.java:2902)
    at java.lang.Class.getMethods(Class.java:1615)
    at net.minecraftforge.fml.common.eventhandler.EventBus.register(EventBus.java:82)
    at fr.frinn.modularmagic.ModularMagic.<init>(ModularMagic.java:40)
    at sun.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method)
    at sun.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:62)
    at sun.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45)
    at java.lang.reflect.Constructor.newInstance(Constructor.java:423)
    at java.lang.Class.newInstance(Class.java:442)
    at net.minecraftforge.fml.common.ILanguageAdapter$JavaAdapter.getNewInstance(ILanguageAdapter.java:191)
    at net.minecraftforge.fml.common.FMLModContainer.constructMod(FMLModContainer.java:599)
    at sun.reflect.GeneratedMethodAccessor5.invoke(Unknown Source)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:498)
    at com.google.common.eventbus.Subscriber.invokeSubscriberMethod(Subscriber.java:91)
    at com.google.common.eventbus.Subscriber$SynchronizedSubscriber.invokeSubscriberMethod(Subscriber.java:150)
    at com.google.common.eventbus.Subscriber$1.run(Subscriber.java:76)
    at com.google.common.util.concurrent.MoreExecutors$DirectExecutor.execute(MoreExecutors.java:399)
    at com.google.common.eventbus.Subscriber.dispatchEvent(Subscriber.java:71)
    at com.google.common.eventbus.Dispatcher$PerThreadQueuedDispatcher.dispatch(Dispatcher.java:116)
    at com.google.common.eventbus.EventBus.post(EventBus.java:217)
    at net.minecraftforge.fml.common.LoadController.sendEventToModContainer(LoadController.java:219)
    at net.minecraftforge.fml.common.LoadController.propogateStateMessage(LoadController.java:197)
    at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
    at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:498)
    at com.google.common.eventbus.Subscriber.invokeSubscriberMethod(Subscriber.java:91)
    at com.google.common.eventbus.Subscriber$SynchronizedSubscriber.invokeSubscriberMethod(Subscriber.java:150)
    at com.google.common.eventbus.Subscriber$1.run(Subscriber.java:76)
    at com.google.common.util.concurrent.MoreExecutors$DirectExecutor.execute(MoreExecutors.java:399)
    at com.google.common.eventbus.Subscriber.dispatchEvent(Subscriber.java:71)
    at com.google.common.eventbus.Dispatcher$PerThreadQueuedDispatcher.dispatch(Dispatcher.java:116)
    at com.google.common.eventbus.EventBus.post(EventBus.java:217)
    at net.minecraftforge.fml.common.LoadController.distributeStateMessage(LoadController.java:136)
    at net.minecraftforge.fml.common.Loader.loadMods(Loader.java:595)
    at net.minecraftforge.fml.client.FMLClientHandler.beginMinecraftLoading(FMLClientHandler.java:232)
    at net.minecraft.client.Minecraft.init(Minecraft.java:467)
    at net.minecraft.client.Minecraft.run(Minecraft.java:3931)
    at net.minecraft.client.main.Main.main(SourceFile:123)
    at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
    at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:498)
    at net.minecraft.launchwrapper.Launch.launch(Launch.java:159)
    at net.minecraft.launchwrapper.Launch.main(Launch.java:30)
Caused by: java.lang.ClassNotFoundException: hellfirepvp.astralsorcery.common.starlight.transmission.registry.TransmissionClassRegistry$TransmissionProvider
    at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:185)
    at java.lang.ClassLoader.loadClass(ClassLoader.java:424)
    at java.lang.ClassLoader.loadClass(ClassLoader.java:357)
    ... 48 more
Caused by: java.lang.NullPointerException
    at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:176)
    ... 50 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
  Minecraft Version: 1.12.2
  Operating System: Windows 10 (amd64) version 10.0
  Java Version: 1.8.0_181, Oracle Corporation
  Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
  Memory: 135067152 bytes (128 MB) / 738197504 bytes (704 MB) up to 17163091968 bytes (16368 MB)
  JVM Flags: 11 total; -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=16M -XX:-UseAdaptiveSizePolicy -XX:-OmitStackTraceInFastThrow -Xmn128m -Xmx16364m -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump
  IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
  FML: MCP 9.42 Powered by Forge 14.23.5.2847 Optifine OptiFine_1.12.2_HD_U_F5 222 mods loaded, 222 mods active
       States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
       
       | State | ID                                | Version                  | Source                                                     | Signature                                |
       |:----- |:--------------------------------- |:------------------------ |:---------------------------------------------------------- |:---------------------------------------- |
       | LC    | minecraft                         | 1.12.2                   | minecraft.jar                                              | None                                     |
       | LC    | mcp                               | 9.42                     | minecraft.jar                                              | None                                     |
       | LC    | FML                               | 8.0.99.99                | forge-1.12.2-14.23.5.2847.jar                              | None                                     |
       | LC    | forge                             | 14.23.5.2847             | forge-1.12.2-14.23.5.2847.jar                              | None                                     |
       | LC    | jecharacters                      | 1.12.0-3.4.5             | [JEI拼音查询]JustEnoughCharacters-1.12.0-3.4.5.jar             | None                                     |
       | LC    | anothercommonbugfix               | 1.1.0                    | minecraft.jar                                              | None                                     |
       | LC    | smoothfontcore                    | mc1.12.2-2.1.1           | minecraft.jar                                              | None                                     |
       | LC    | advancedrocketrycore              | 1                        | minecraft.jar                                              | None                                     |
       | LC    | lesslag                           | 1.0                      | minecraft.jar                                              | None                                     |
       | LC    | openmodscore                      | 0.12.2                   | minecraft.jar                                              | None                                     |
       | LC    | foamfixcore                       | 7.7.4                    | minecraft.jar                                              | None                                     |
       | LC    | botania_tweaks_core               | -100                     | minecraft.jar                                              | None                                     |
       | LC    | smoothfont                        | mc1.12.2-2.1.1           | [平滑字体]SmoothFont-mc1.12.2-2.1.1.jar                        | None                                     |
       | LC    | crafttweaker                      | 4.1.20                   | [crt]CraftTweaker2-1.12-4.1.20.jar                         | None                                     |
       | LC    | mtlib                             | 3.0.6                    | MTLib-3.0.6.jar                                            | None                                     |
       | LC    | modtweaker                        | 4.0.17                   | [crt拓展兼容]modtweaker-4.0.17.jar                             | None                                     |
       | LC    | endertweaker                      | 1.2.0                    | [末影接口-魔改]EnderTweaker-1.12.2-1.2.0.jar                     | None                                     |
       | LC    | jei                               | 4.15.0.293               | [JEI物品管理器]jei_1.12.2-4.15.0.293.jar                        | None                                     |
       | LC    | ic2                               | 2.8.188-ex112            | [工业时代2]industrialcraft-2-2.8.188-ex112.jar                 | de041f9f6187debbc77034a344134053277aa3b0 |
       | LC    | redstoneflux                      | 2.1.0                    | RedstoneFlux-1.12-2.1.0.6-universal.jar                    | 8a6abf2cb9e141b866580d369ba6548732eff25f |
       | LC    | cofhcore                          | 4.6.3                    | [热力核心]CoFHCore-1.12.2-4.6.3.27-universal.jar               | None                                     |
       | LC    | libvulpes                         | 0.4.2.-74                | [高级火箭前置]LibVulpes-1.12.2-0.4.2-74-universal.jar            | None                                     |
       | LC    | advancedrocketry                  | 1.7.0.-209               | [高级火箭]AdvancedRocketry-1.12.2-1.7.0-209-universal.jar      | None                                     |
       | LC    | art                               | 1.0.0                    | [crt-高级火箭]ARTweaker-1.12.2-1.0.0.jar                       | None                                     |
       | LC    | ctgui                             | 1.0.0                    | [crt]CraftTweaker2-1.12-4.1.20.jar                         | None                                     |
       | LC    | crafttweakerjei                   | 2.0.3                    | [crt]CraftTweaker2-1.12-4.1.20.jar                         | None                                     |
       | LC    | inworldcrafting                   | 1.12.2-0.13.0            | [crt世界合成]inworldcrafting-1.12.2-0.13.0-universal.jar       | None                                     |
       | LC    | ctm                               | MC1.12.2-1.0.1.30        | CTM-MC1.12.2-1.0.1.30.jar                                  | None                                     |
       | LC    | chisel                            | MC1.12.2-1.0.1.44        | [凿子]Chisel-MC1.12.2-1.0.1.44.jar                           | None                                     |
       | LC    | tinkersextras                     | 1.12.2-1.1.0             | [匠魂2-特性配置]TinkersExtras-1.12.2-1.1.0.jar                   | b02331787272ec3515ebe63ecdeea0d746653468 |
       | LC    | endercore                         | 1.12.2-0.5.73            | [末影核心]EnderCore-1.12.2-0.5.73.jar                          | None                                     |
       | LC    | cofhworld                         | 1.3.1                    | CoFHWorld-1.12.2-1.3.1.7-universal.jar                     | 8a6abf2cb9e141b866580d369ba6548732eff25f |
       | LC    | thermalfoundation                 | 2.6.3                    | [热力基本]ThermalFoundation-1.12.2-2.6.3.27-universal.jar      | 8a6abf2cb9e141b866580d369ba6548732eff25f |
       | LC    | codechickenlib                    | 3.2.3.358                | CodeChickenLib-1.12.2-3.2.3.358-universal.jar              | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LC    | brandonscore                      | 2.4.17                   | [龙之核心]BrandonsCore-1.12.2-2.4.17.208-universal.jar         | None                                     |
       | LC    | draconicevolution                 | 2.3.24                   | [龙之进化]Draconic-Evolution-1.12.2-2.3.24.349-universal.jar   | None                                     |
       | LC    | thermalexpansion                  | 5.5.4                    | [热力膨胀5]ThermalExpansion-1.12.2-5.5.4.43-universal.jar      | 8a6abf2cb9e141b866580d369ba6548732eff25f |
       | LC    | baubles                           | 1.5.2                    | Baubles-1.12-1.5.2.jar                                     | None                                     |
       | LC    | thaumcraft                        | 6.1.BETA26               | [神秘时代6]Thaumcraft-1.12.2-6.1.BETA26.jar                    | None                                     |
       | LC    | enderio                           | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | enderiointegrationtic             | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | mantle                            | 1.12-1.3.3.55            | Mantle-1.12-1.3.3.55.jar                                   | None                                     |
       | LC    | tconstruct                        | 1.12.2-2.13.0.179        | [匠魂2]TConstruct-1.12.2-2.13.0.179.jar                      | None                                     |
       | LC    | base                              | 3.13.0                   | base-1.12.2-3.13.0.jar                                     | None                                     |
       | LC    | contenttweaker                    | 1.12.2-4.9.1             | [crt创物]ContentTweaker-1.12.2-4.9.1.jar                     | None                                     |
       | LC    | crafttweakersync                  | 1.0                      | [crt脚本同步]CraftTweakerSync-1.0.jar                          | None                                     |
       | LC    | jaopca                            | 1.12.2-2.2.8.103         | [JAOPCA]JAOPCA-1.12.2-2.2.8.103.jar                        | None                                     |
       | LC    | oredictinit                       | 1.12.2-2.2.1.71          | [JAOPCA]JAOPCA-1.12.2-2.2.8.103.jar                        | None                                     |
       | LC    | tinkersjei                        | 1.2                      | [JEI-匠魂]tinkersjei-1.2.jar                                 | None                                     |
       | LC    | jeid                              | 1.0.3-48                 | [JEIDs]JustEnoughIDs-1.0.3-48.jar                          | None                                     |
       | LC    | jetif                             | 1.5.1                    | [JEI丢弃查询]jetif-1.12.2-1.5.1.jar                            | None                                     |
       | LC    | moreoverlays                      | 1.15.1                   | [JEI怪物生成查看]moreoverlays-1.15.1-mc1.12.2.jar                | None                                     |
       | LC    | harvestcraft                      | 1.12.2zb                 | [潘马斯农场]Pam's+HarvestCraft+1.12.2zf.jar                     | None                                     |
       | LC    | jehc                              | 1.7.0                    | [JEI潘马斯]just-enough-harvestcraft-1.12.2-1.7.0.jar          | None                                     |
       | LC    | thaumicjei                        | 1.6.0                    | [JEI神秘]ThaumicJEI-1.12.2-1.6.0-27.jar                      | None                                     |
       | LC    | modnametooltip                    | 1.10.1                   | [mod名称显示]modnametooltip_1.12.2-1.10.1.jar                  | None                                     |
       | LC    | projectintelligence               | 1.0.9                    | [PI文档]ProjectIntelligence-1.12.2-1.0.9.28-universal.jar    | None                                     |
       | LC    | placebo                           | 1.6.0                    | [pl]Placebo-1.12.2-1.6.0.jar                               | None                                     |
       | LC    | inventorytweaks                   | 1.63+release.109.220f184 | [R键整理]InventoryTweaks-1.63.jar                             | 55d2cd4f5f0961410bf7b91ef6c6bf00a766dcbe |
       | LC    | tesla                             | 1.0.63                   | [特斯拉]Tesla-1.12.2-1.0.63.jar                               | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | theoneprobe                       | 1.4.28                   | [TOP]theoneprobe-1.12-1.4.28.jar                           | None                                     |
       | LC    | chameleon                         | 1.12-4.1.3               | [储物抽屉前置]Chameleon-1.12-4.1.3.jar                           | None                                     |
       | LC    | storagedrawers                    | 1.12.2-5.4.0             | [储物抽屉]StorageDrawers-1.12.2-5.4.0.jar                      | None                                     |
       | LC    | buildcraftlib                     | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | buildcraftcore                    | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | buildcraftenergy                  | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | toughasnails                      | 3.1.0.139                | [意志坚定]ToughAsNails-1.12.2-3.1.0.139-universal.jar          | None                                     |
       | LC    | forestry                          | 5.8.2.387                | [林业]forestry_1.12.2-5.8.2.387.jar                          | None                                     |
       | LC    | botania_tweaks                    | 1.8.6                    | [植物魔法修改]botaniatweaks-1.8.6.jar                            | None                                     |
       | LC    | botania                           | r1.10-363                | [植物魔法]Botania+r1.10-363.jar                                | None                                     |
       | LC    | guideapi                          | 1.12-2.1.8-63            | [指南]Guide-API-1.12-2.1.8-63.jar                            | None                                     |
       | LC    | bloodmagic                        | 1.12.2-2.4.3-105         | [血魔法2]BloodMagic-1.12.2-2.4.3-105.jar                      | None                                     |
       | LC    | topaddons                         | 1.12.2-1.12.0            | [TOP]topaddons-1.12.2-1.12.0.jar                           | None                                     |
       | LC    | mcjtylib_ng                       | 3.5.4                    | mcjtylib-1.12-3.5.4.jar                                    | None                                     |
       | LC    | xnet                              | 1.8.2                    | [xnet]xnet-1.12-1.8.2.jar                                  | None                                     |
       | LC    | ynot                              | 0.2.4                    | [xent气体]YNot-0.2.4.jar                                     | None                                     |
       | LC    | netherportalfix                   | 5.3.17                   | [下界传送门修正]NetherPortalFix_1.12.1-5.3.17.jar                 | None                                     |
       | LC    | bnbgaminglib                      | 2.17.6                   | [世界生成前置]BNBGamingLib-1.12.2-2.17.6.jar                     | None                                     |
       | LC    | topography                        | 1.10.1                   | [世界生成]Topography-1.12.2-1.10.1.jar                         | None                                     |
       | LC    | bedbugs                           | @VERSION@                | [修复卡床]BedBugs-1.12-1.0.1.jar                               | None                                     |
       | LC    | biggerpacketsplz                  | 1.2                      | [修复服务器数据包]biggerpacketsplz-since1.8-1.2.jar                | 266588b191a3e2974a4a577f282858a3bc07da42 |
       | LC    | powerchisels                      | 1.0.0-beta-3             | [凿子-能量凿子]powerchisels-1.0.0-beta-3.jar                     | None                                     |
       | LC    | fastbench                         | 1.7.3                    | [工作台性能优化]FastWorkbench-1.12.2-1.7.3.jar                    | None                                     |
       | LC    | actuallyadditions                 | 1.12.2-r151              | [实用拓展]ActuallyAdditions-1.12.2-r151-2.jar                  | None                                     |
       | LC    | mcmultipart                       | 2.5.3                    | [通用机械前置]MCMultiPart-2.5.3.jar                              | None                                     |
       | LC    | mekanism                          | 1.12.2-9.8.3.390         | [通用机械]Mekanism-1.12.2-9.8.3.390.jar                        | None                                     |
       | LC    | forgelin                          | 1.8.4                    | Forgelin-1.8.4.jar                                         | None                                     |
       | LC    | teslacorelib                      | 1.0.15                   | [特斯拉核心]tesla-core-lib-1.12.2-1.0.15.jar                    | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | industrialforegoing               | 1.12.2-1.12.2            | [工业先锋]industrialforegoing-1.12.2-1.12.13-237.jar           | None                                     |
       | LC    | appliedenergistics2               | rv6-stable-7             | [应用能源]appliedenergistics2-rv6-stable-7.jar                 | dfa4d3ac143316c6f32aa1a1beda1e34d42132e5 |
       | LC    | avaritia                          | 3.3.0                    | [无尽贪婪]Avaritia-1.12.2-3.3.0.33-universal.jar               | None                                     |
       | LC    | valkyrielib                       | 1.12.2-2.0.20.1          | [环境科技前置]valkyrielib-1.12.2-2.0.20.1.jar                    | None                                     |
       | LC    | environmentaltech                 | 1.12.2-2.0.20.1          | [环境科技]environmentaltech-1.12.2-2.0.20.1.jar                | None                                     |
       | LC    | plustic                           | 7.1.6.1                  | [匠魂2-扩充]plustic-7.1.6.1.jar                                | None                                     |
       | LC    | exnihilocreatio                   | 1.12.2-0.4.7.2           | [无中生有]exnihilocreatio-1.12.2-0.4.7.2.jar                   | None                                     |
       | LC    | tcomplement                       | 1.12.2-0.4.3             | [匠魂2-补充]TinkersComplement-1.12.2-0.4.3.jar                 | None                                     |
       | LC    | compactmachines3                  | 3.0.18                   | [压缩空间]compactmachines3-1.12.2-3.0.18-b278.jar              | None                                     |
       | LC    | vanillafix                        | 1.0.10-SNAPSHOT          | [原版修复]VanillaFix-1.0.10-99.jar                             | None                                     |
       | LC    | morphtool                         | 1.2-21                   | [变形工具]Morph-o-Tool-1.2-21.jar                              | None                                     |
       | LC    | cucumber                          | 1.1.3                    | [合成拓展前置]Cucumber-1.12.2-1.1.3.jar                          | None                                     |
       | LC    | extendedcrafting                  | 1.5.6                    | [合成拓展]ExtendedCrafting-1.12.2-1.5.6.jar                    | None                                     |
       | LC    | craftingtweaks                    | 8.1.9                    | [合成调整]CraftingTweaks_1.12.2-8.1.9.jar                      | None                                     |
       | LC    | bookshelf                         | 2.3.590                  | [实用物品前置]Bookshelf-1.12.2-2.3.590.jar                       | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | darkutils                         | 1.8.230                  | [实用物品]DarkUtils-1.12.2-1.8.230.jar                         | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | packagedauto                      | 1.12.2-1.0.2.9           | [封包合成]PackagedAuto-1.12.2-1.0.2.9.jar                      | None                                     |
       | LC    | mets                              | 1.53X                    | [工业时代2-更多电力设备]MoreElectricTools.v1.53X.jar                 | None                                     |
       | LC    | gravisuite                        | 3.1.1                    | [工业重力装甲]Gravitation+Suite-3.1.1.jar                        | None                                     |
       | LC    | advanced_solar_panels             | 4.3.0                    | [工业高级太阳能]Advanced+Solar+Panels-4.3.0.jar                   | None                                     |
       | LC    | p455w0rdslib                      | 2.3.161                  | [应用能源无线合成终端前置]p455w0rdslib-1.12.2-2.3.161.jar              | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | ae2wtlib                          | 1.0.34                   | [应用能源无线合成终端]AE2WTLib-1.12.2-1.0.34.jar                     | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | mousetweaks                       | 2.10                     | [鼠标手势]MouseTweaks-2.10-mc1.12.2.jar                        | None                                     |
       | LC    | wit                               | 1.0.2                    | [应用能源2-无线接口终端]WirelessInterfaceTerminal-1.12.2-1.0.2.jar   | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | wpt                               | 1.0.3                    | [应用能源2-无线样板终端]WirelessPatternTerminal-1.12.2-1.0.3.jar     | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | wft                               | 1.0.4                    | [应用能源2-无线流体终端]WirelessFluidTerminal-1.12.2-1.0.4.jar       | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | jee                               | 1.0.8                    | [应用能源JEI]JustEnoughEnergistics-1.12.2-1.0.8.jar            | None                                     |
       | LC    | bdlib                             | 1.14.3.12                | bdlib-1.14.3.12-mc1.12.2.jar                               | None                                     |
       | LC    | ae2stuff                          | 0.7.0.4                  | [应用能源实用前置]ae2stuff-0.7.0.4-mc1.12.2.jar                    | None                                     |
       | LC    | libnine                           | 1.1.5                    | [应用能源懒惰前置]libnine-1.12.2-1.1.5.jar                         | None                                     |
       | LC    | threng                            | 1.1.7                    | [应用能源懒惰前置]lazy-ae2-1.12.2-1.1.7.jar                        | None                                     |
       | LC    | wct                               | 3.12.97                  | [应用能源无线合成终端]WirelessCraftingTerminal-1.12.2-3.12.97.jar    | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | extracells                        | 2.6.5                    | [应用能源更多存储单元]ExtraCells-1.12.2-2.6.5.jar                    | None                                     |
       | LC    | spatialservermod                  | 1.3                      | [应用能源空间]spatialservermod-1.3.jar                           | None                                     |
       | LC    | buildcraftbuilders                | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | buildcrafttransport               | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | buildcraftsilicon                 | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | buildcraftcompat                  | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | buildcraftfactory                 | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | buildcraftrobotics                | 7.99.24.4                | [建筑]buildcraft-all-7.99.24.4.jar                           | None                                     |
       | LC    | buildinggadgets                   | 2.8.1                    | [建筑小帮手]BuildingGadgets-2.8.1.jar                           | None                                     |
       | LC    | openmods                          | 0.12.2                   | [开放式模组库]OpenModsLib-1.12.2-0.12.2.jar                      | d2a9a8e8440196e26a268d1f3ddc01b2e9c572a5 |
       | LC    | openblocks                        | 1.8.1                    | [开放式方块]OpenBlocks-1.12.2-1.8.1.jar                         | d2a9a8e8440196e26a268d1f3ddc01b2e9c572a5 |
       | LC    | slurp                             | 0.3                      | [意志坚定-啜饮]slurp-1.12-0.3.jar                                | None                                     |
       | LC    | tanaddons                         | 3.4.24                   | [意志坚定-热力]ToughExpansion-1.12-3.4.24.jar                    | None                                     |
       | LC    | carrots                           | 1.0.0b1                  | [意志坚定-盔甲内衬前置]carrotslib-mc1.12.2-1.0.0b1.jar               | None                                     |
       | LC    | armorunder                        | 1.0.0                    | [意志坚定-盔甲内衬]armorunder-mc1.12.2-1.0.0.jar                   | None                                     |
       | LC    | cookingforblockheads              | 6.5.0                    | [懒人厨房]CookingForBlockheads_1.12.2-6.5.0.jar                | None                                     |
       | LC    | excompressum                      | 3.0.31                   | [无中生有-压缩工具]ExCompressum_1.12.2-3.0.31.jar                  | None                                     |
       | LC    | infinitefluids                    | 1.2.0                    | [无限流体]infinitefluids-1.11-1.2.0.jar                        | None                                     |
       | LC    | extrautils2                       | 1.0                      | [更多实用设备2]extrautils2-1.12-1.9.9.jar                        | None                                     |
       | LC    | betterbuilderswands               | 0.11.1                   | [更好的建筑之杖]BetterBuildersWands-1.12-0.11.1.245+69d0d70.jar   | None                                     |
       | LC    | betteradvancements                | 0.1.0.77                 | [更好的进度]BetterAdvancements-1.12.2-0.1.0.77.jar              | None                                     |
       | LC    | fastfurnace                       | 1.3.1                    | [更快的熔炉]FastFurnace-1.12.2-1.3.1.jar                        | None                                     |
       | LC    | enderioconduits                   | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | gasconduits                       | 1.12.2-1.2.1             | [末影接口-气体管道]GasConduits-1.12.2-1.2.2.jar                    | None                                     |
       | LC    | lootcapacitortooltips             | 1.3                      | [末影接口-电容信息]lootcapacitortooltips-1.3.jar                   | None                                     |
       | LC    | enderiobase                       | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | enderioconduitsappliedenergistics | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | enderioconduitsopencomputers      | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | enderioconduitsrefinedstorage     | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | enderiointegrationforestry        | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | enderiointegrationticlate         | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | ftblib                            | 5.4.4.5                  | FTBLib-5.4.4.5.jar                                         | None                                     |
       | LC    | enderiomachines                   | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | enderiopowertools                 | 5.1.55                   | [末影接口]EnderIO-1.12.2-5.1.55.jar                            | None                                     |
       | LC    | fastleafdecay                     | v14                      | [树叶快速腐烂]FastLeafDecay-v14.jar                              | None                                     |
       | LC    | nuclearcraft                      | 2.18o                    | [核电工艺]NuclearCraft-2.18o-1.12.2.jar                        | None                                     |
       | LC    | manavisualizer                    | r1.0-1                   | [植物魔法-魔力显示]ManaVisualizer-r1.0-1.jar                       | None                                     |
       | LC    | hammercore                        | 2.0.6.7                  | HammerCore-1.12.2-2.0.6.7.jar                              | 9f5e2a811a8332a842b34f6967b7db0ac4f24856 |
       | LC    | botanicadds                       | 4r                       | [植物魔法拓展]BotanicAdditions-1.12.2-4r.jar                     | 4d7b29cd19124e986da685107d16ce4b49bc0a97 |
       | LC    | botanianeedsit                    | 1.12.2-3.0-release       | [植物魔法需要它]botanianeedsit-1.12.2-3.0-release.jar             | None                                     |
       | LC    | extrabotany                       | 56                       | [植物魔法额外植物学]ExtraBotany-r1.1-56.jar                         | None                                     |
       | LC    | advgenerators                     | 0.9.20.12                | [模块化发电机]generators-0.9.20.12-mc1.12.2.jar                  | None                                     |
       | LC    | modularmachinery                  | 1.11.1                   | [模块化机械]modularmachinery-1.12.2-1.11.1.jar                  | a0f0b759d895c15ceb3e3bcb5f3c2db7c582edf0 |
       | L     | modularmagic                      | 1.5.1                    | [模块化机械-魔法]modularmagic-1.5.1.jar                           | None                                     |
       | L     | sourcebottles                     | 1.0.1                    | [水瓶消耗水源]SourceBottles-1.0.2.jar                            | None                                     |
       | L     | norecipebook                      | 1.2.1                    | [没有合成书]noRecipeBook_v1.2.2formc1.12.2.jar                  | None                                     |
       | L     | foamfix                           | 0.10.10-1.12.2           | [泡沫修复]foamfix-0.10.10-1.12.2.jar                           | None                                     |
       | L     | toastcontrol                      | 1.8.1                    | [消息框控制]Toast+Control-1.12.2-1.8.1.jar                      | None                                     |
       | L     | lunatriuscore                     | 1.2.0.42                 | [游戏信息显示前置]LunatriusCore-1.12.2-1.2.0.42-universal.jar      | None                                     |
       | L     | ingameinfoxml                     | 2.8.2.94                 | [游戏信息显示]InGameInfoXML-1.12.2-2.8.2.94-universal.jar        | None                                     |
       | L     | gamestages                        | 2.0.119                  | [游戏阶段]GameStages-1.12.2-2.0.119.jar                        | None                                     |
       | L     | waterstrainer                     | 3.2.0                    | [滤水器]WaterStrainer-1.12-3.2.0.jar                          | None                                     |
       | L     | surge                             | 2.0.77                   | [潮涌]Surge-1.12.2-2.0.77.jar                                | None                                     |
       | L     | torchmaster                       | 1.8.1.81                 | [火炬大师]torchmaster_1.12.2-1.8.1.81.jar                      | None                                     |
       | L     | thermaldynamics                   | 2.5.5                    | [热动力学]ThermalDynamics-1.12.2-2.5.5.21-universal.jar        | None                                     |
       | L     | universalmodifiers                | 1.12.2-1.0.16.1          | [环境科技前置]valkyrielib-1.12.2-2.0.20.1.jar                    | None                                     |
       | L     | ding                              | 1.0.2                    | [界面进入提示]Ding-1.12.2-1.0.2.jar                              | None                                     |
       | L     | customskinloader                  | 14.11                    | [皮肤补丁]CustomSkinLoader_Forge-14.11.jar                     | None                                     |
       | L     | wanionlib                         | 1.12.2-2.2               | [矿辞统一]WanionLib-1.12.2-2.2.jar                             | None                                     |
       | L     | dummycore                         | 2.4.112.5.               | DummyCoreUnofficial-2.4.112.5.jar                          | None                                     |
       | L     | thaumicbases                      | 3.3.400.6r               | [神秘基础学]thaumicbases-3.3.352.6r.jar                         | None                                     |
       | L     | thaumictinkerer                   | 1.12.2-5.0-353c71c       | [神秘工匠]thaumictinkerer-1.12.2-5.0-353c71c.jar               | None                                     |
       | L     | tcinventoryscan                   | 2.0.10                   | [神秘库存扫描]ThaumicInventoryScanning_1.12.2-2.0.10.jar         | None                                     |
       | L     | brazier                           | 1.2.0                    | [神秘源质火盆]brazier-1.2.0.jar                                  | None                                     |
       | L     | thaumcraftjarchecker              | 1.0                      | [神秘源质罐子统计]ThaumcraftJarChecker-1.12.2-1.0a.jar             | None                                     |
       | L     | thaumicenergistics                | 2.2.3                    | [神秘能源]thaumicenergistics-2.2.3.jar                         | None                                     |
       | L     | nmsot                             | 1.2.2-mc1.12.2           | [禁止树上刷怪]NoMobSpawningOnTrees-1.2.2-mc1.12.2.jar            | None                                     |
       | L     | tooltweaks                        | 1.0.7                    | [禁用原版工具]tooltweaks-1.0.7.jar                               | None                                     |
       | L     | titlechanger                      | 1.1.4                    | [窗口标题]titlechanger-1.1.4.jar                               | None                                     |
       | L     | clumps                            | 3.1.2                    | [经验机制改革]Clumps-3.1.2.jar                                   | None                                     |
       | L     | custommainmenu                    | 2.0.9.1                  | [自定义主菜单]CustomMainMenu-MC1.12.2-2.0.9.1.jar                | None                                     |
       | L     | resourceloader                    | 1.5.3                    | [自定义资源位置]ResourceLoader-MC1.12.1-1.5.3.jar                 | None                                     |
       | L     | applecore                         | 3.2.0                    | [苹果核]AppleCore-mc1.12.2-3.2.0.jar                          | None                                     |
       | L     | appleskin                         | 1.0.9                    | [苹果皮]AppleSkin-mc1.12-1.0.9.jar                            | None                                     |
       | L     | nopotionshift                     | 1.2.0                    | [药水栏不移动背包GUI]nopotionshift_1.12.2-1.2.0.jar                | None                                     |
       | L     | bloodarsenal                      | 1.12.2-2.2.0-29          | [血液兵工厂]BloodArsenal-1.12.2-2.2.1-29.jar                    | None                                     |
       | L     | treegrowingsimulator              | 0.0.4                    | [跳舞树成长]TreeGrowingSimulator2017-1.0.1.jar                  | None                                     |
       | L     | mekanismgenerators                | 1.12.2-9.8.3.390         | [通用机械发电]MekanismGenerators-1.12.2-9.8.3.390.jar            | None                                     |
       | L     | controlling                       | 3.0.8                    | [键位冲突显示]Controlling-3.0.8.jar                              | None                                     |
       | L     | akashictome                       | 1.2-12                   | [阿卡什宝典]AkashicTome-1.2-12.jar                              | None                                     |
       | L     | autoreglib                        | 1.3-32                   | [阿卡什宝典前置]AutoRegLib-1.3-32.jar                             | None                                     |
       | L     | enchdesc                          | 1.1.19                   | [附魔描述]EnchantmentDescriptions-1.12.2-1.1.19.jar            | None                                     |
       | L     | ceramics                          | 1.12-1.3.7               | [陶瓷器]Ceramics-1.12-1.3.7.jar                               | None                                     |
       | L     | cyclopscore                       | 1.6.0                    | CyclopsCore-1.12.2-1.6.0.jar                               | None                                     |
       | L     | commoncapabilities                | 2.4.5                    | CommonCapabilities-1.12.2-2.4.5.jar                        | None                                     |
       | L     | integrateddynamics                | 1.1.1                    | [集成动力]IntegratedDynamics-1.12.2-1.1.1.jar                  | None                                     |
       | L     | integrateddynamicscompat          | 1.0.0                    | [集成动力]IntegratedDynamics-1.12.2-1.1.1.jar                  | None                                     |
       | L     | sqpatch                           | 1.0.0                    | [集成动力补丁]SqueezerPatch-1.12.2-1.0.0.jar                     | None                                     |
       | L     | integratedtunnels                 | 1.6.10                   | [集成管道]IntegratedTunnels-1.12.2-1.6.10.jar                  | None                                     |
       | L     | integratedtunnelscompat           | 1.0.0                    | [集成管道]IntegratedTunnels-1.12.2-1.6.10.jar                  | None                                     |
       | L     | sereneseasons                     | 1.2.18                   | [静谧四季]SereneSeasons-1.12.2-1.2.18-universal.jar            | None                                     |
       | L     | draconicadditions                 | 1.11.0                   | [龙之进化-拓展]Draconic-Additions-1.12.2-1.11.0.31-universal.jar | None                                     |
       | L     | ftbutilities                      | 5.4.0.124                | FTBUtilities-5.4.0.124.jar                                 | None                                     |
       | L     | itemfilters                       | 1.0.3.12                 | ItemFilters-1.0.3.12.jar                                   | None                                     |
       | L     | ftbquests                         | 1.8.0.237                | FTBQuests-1.8.0.237.jar                                    | None                                     |
       | L     | patchouli                         | 1.0-20                   | Patchouli-1.0-20.jar                                       | None                                     |
       | L     | immersiveengineering              | 0.12-92                  | [沉浸工程]ImmersiveEngineering-0.12-92.jar                     | None                                     |
       | L     | phosphor-lighting                 | 1.12.2-0.2.6             | [照明优化]phosphor-1.12.2-0.2.6+build50-universal.jar          | None                                     |
       | L     | wrapup                            | 1.12-1.1.3               | [JAOPCA前置]WrapUp-1.12-1.1.3.jar                            | None                                     |
       | L     | justthetips                       | 1.12-1.0.1.1             | [提示]justthetips-1.12-1.0.1.1.jar                           | None                                     |
       | L     | teslacorelib_registries           | 1.0.15                   | [特斯拉核心]tesla-core-lib-1.12.2-1.0.15.jar                    | None                                     |
       | L     | unidict                           | 1.12.2-2.9.6             | [矿辞统一]UniDict-1.12.2-2.9.6.jar                             | None                                     |
  Loaded coremods (and transformers): JustEnoughIDs Extension Plugin ([JEIDs]JustEnoughIDs-1.0.3-48.jar)
                                        org.dimdev.jeid.JEIDTransformer
                                      CTMCorePlugin (CTM-MC1.12.2-1.0.1.30.jar)
                                        team.chisel.ctm.client.asm.CTMTransformer
                                      DCLoadingPlugin (DummyCoreUnofficial-2.4.112.5.jar)
                                        DummyCore.ASM.DCASMManager
                                      CorePlugin ([平滑字体]SmoothFont-mc1.12.2-2.1.1.jar)
                                        bre.smoothfont.asm.Transformer
                                      IELoadingPlugin (ImmersiveEngineering-core-0.12-92.jar)
                                        blusunrize.immersiveengineering.common.asm.IEClassTransformer
                                      Botania Tweaks Core ([植物魔法修改]botaniatweaks-1.8.6.jar)
                                        quaternary.botaniatweaks.asm.BotaniaTweakerTransformer
                                      PhosphorFMLLoadingPlugin ([照明优化]phosphor-1.12.2-0.2.6+build50-universal.jar)
                                        
                                      SurgeLoadingPlugin ([潮涌]Surge-1.12.2-2.0.77.jar)
                                        
                                      SqueezerCore ([集成动力补丁]SqueezerPatch-1.12.2-1.0.0.jar)
                                        shadows.squeezer.Transformer
                                      SSLoadingPlugin ([静谧四季]SereneSeasons-1.12.2-1.2.18-universal.jar)
                                        sereneseasons.asm.transformer.EntityRendererTransformer
                                        sereneseasons.asm.transformer.WorldTransformer
                                      VanillaFixLoadingPlugin ([原版修复]VanillaFix-1.0.10-99.jar)
                                        
                                      AdvancedRocketryPlugin ([高级火箭]AdvancedRocketry-1.12.2-1.7.0-209-universal.jar)
                                        zmaster587.advancedRocketry.asm.ClassTransformer
                                      LesslagCorePlugin ([较少的滞后]lesslag-1.0-1.12.2.jar)
                                        
                                      MekanismCoremod ([通用机械]Mekanism-1.12.2-9.8.3.390.jar)
                                        mekanism.coremod.KeybindingMigrationHelper
                                      CustomSkinLoader ([皮肤补丁]CustomSkinLoader_Forge-14.11.jar)
                                        customskinloader.forge.loader.LaunchWrapper
                                      BiggerPacketsPlzCoreMod ([修复服务器数据包]biggerpacketsplz-since1.8-1.2.jar)
                                        net.elnounch.mc.biggerpacketsplz.BiggerPacketsPlzClassTransformer
                                      ForgelinPlugin (Forgelin-1.8.4.jar)
                                        
                                      HCASM (HammerCore-1.12.2-2.0.6.7.jar)
                                        com.zeitheron.hammercore.asm.HammerCoreTransformer
                                      AnotherCommonBugFix ([另一个通用bug修复]AnotherCommonBugFix-1.1.0-1.12.2.jar)
                                        com.anotherera.core.ACBFClassTransformer
                                      AppleCore ([苹果核]AppleCore-mc1.12.2-3.2.0.jar)
                                        squeek.applecore.asm.TransformerModuleHandler
                                      Do not report to Forge! (If you haven't disabled the FoamFix coremod, try disabling it in the config! Note that this bit of text will still appear.) ([泡沫修复]foamfix-0.10.10-1.12.2.jar)
                                        pl.asie.foamfix.coremod.FoamFixTransformer
                                      EnderCorePlugin (EnderCore-1.12.2-0.5.73-core.jar)
                                        com.enderio.core.common.transform.EnderCoreTransformer
                                        com.enderio.core.common.transform.SimpleMixinPatcher
                                      LoadingPlugin ([自定义资源位置]ResourceLoader-MC1.12.1-1.5.3.jar)
                                        lumien.resourceloader.asm.ClassTransformer
                                      OpenModsCorePlugin ([开放式模组库]OpenModsLib-1.12.2-0.12.2.jar)
                                        openmods.core.OpenModsClassTransformer
                                      Inventory Tweaks Coremod ([R键整理]InventoryTweaks-1.63.jar)
                                        invtweaks.forge.asm.ContainerTransformer
                                      JechCore ([JEI拼音查询]JustEnoughCharacters-1.12.0-3.4.5.jar)
                                        me.towdium.jecharacters.core.JechClassTransformer
  GL info: ' Vendor: 'NVIDIA Corporation' Version: '4.6.0 NVIDIA 445.87' Renderer: 'GeForce GTX 970/PCIe/SSE2'
  OpenModsLib class transformers: [llama_null_fix:FINISHED],[horse_base_null_fix:FINISHED],[pre_world_render_hook:FINISHED],[player_render_hook:FINISHED],[horse_null_fix:FINISHED]
  Pulsar/tconstruct loaded Pulses: - TinkerCommons (Enabled/Forced)
                                   - TinkerWorld (Enabled/Not Forced)
                                   - TinkerTools (Enabled/Not Forced)
                                   - TinkerHarvestTools (Enabled/Forced)
                                   - TinkerMeleeWeapons (Enabled/Forced)
                                   - TinkerRangedWeapons (Enabled/Forced)
                                   - TinkerModifiers (Enabled/Forced)
                                   - TinkerSmeltery (Enabled/Not Forced)
                                   - TinkerGadgets (Enabled/Not Forced)
                                   - TinkerOredict (Enabled/Forced)
                                   - TinkerIntegration (Enabled/Forced)
                                   - TinkerFluids (Enabled/Forced)
                                   - TinkerMaterials (Enabled/Forced)
                                   - TinkerModelRegister (Enabled/Forced)
                                   - chiselIntegration (Enabled/Not Forced)
                                   - craftingtweaksIntegration (Enabled/Not Forced)
                                   - theoneprobeIntegration (Enabled/Not Forced)
  AE2 Version: stable rv6-stable-7 for Forge 14.23.5.2768
  Pulsar/tcomplement loaded Pulses: - ModuleCommons (Enabled/Forced)
                                    - ModuleMelter (Enabled/Not Forced)
                                    - ModuleArmor (Enabled/Not Forced)
                                    - ModuleSteelworks (Enabled/Not Forced)
                                    - CeramicsPlugin (Enabled/Not Forced)
                                    - ChiselPlugin (Enabled/Not Forced)
                                    - ExNihiloPlugin (Enabled/Not Forced)
                                    - Oredict (Enabled/Forced)
  HammerCore Debug Information: Dependent Mods:
                                    -Botanic Additions (botanicadds) @4r
  Suspected Mods: Modular Magic (modularmagic)
  Launched Version: HMCL 3.3.166
  LWJGL: 2.9.4
  OpenGL: GeForce GTX 970/PCIe/SSE2 GL version 4.6.0 NVIDIA 445.87, NVIDIA Corporation
  GL Caps: Using GL 1.3 multitexturing.
           Using GL 1.3 texture combiners.
           Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
           Shaders are available because OpenGL 2.1 is supported.
           VBOs are available because OpenGL 1.5 is supported.
  Using VBOs: Yes
  Is Modded: Definitely; Client brand changed to 'fml,forge'
  Type: Client (map_client.txt)
  Resource Packs: Minecraft-Mod-Language-Modpack.zip
  Current Language: 简体中文 (中国)
  Profiler Position: N/A (disabled)
  CPU: 4x AMD Ryzen 3 1200 Quad-Core Processor
