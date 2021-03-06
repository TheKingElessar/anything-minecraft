# Intro

Here we will go through how to pick what server jar to use. A server jar contains all the code for the server, there are server jars for modloaders, like forge or fabric, and some that allow you to use plugins.

## Picking your server jar

The first step to finding the right server jar for you is to know what kind of server you want to run, is it survival, prisons, minigames and what Minecraft version is it? We will show you some basic ones then you can look at (link to the page of server jars) for more in-depth explanations etc.

### For MC 1.16.X

If you are planning on creating a survival server for your friend group [Fabric](https://fabricmc.net/). Fabric is mostly known for modded servers but you can install basic plugin port mods on server side and optimization mods for making chunks load faster, creating lighting better etc. Theres also mods for essentials port and many more plugins you would need on a regular server...
If instead you are planning on running a public server where you plan to have a **lot of plugins or custom gamemodes** you should go for a spigot fork like [PaperMC](https://papermc.io), or my personal favorite: [Purpur](https://github.com/pl3xgaming/Purpur). Purpur has all the optimization, fixes, and features of Paper, Tuinity, Spigot as well as their own features. We really recommend, it's the best fork we know of.

### For MC 1.13+

A good server jar to use is [Purpur](https://github.com/pl3xgaming/Purpur), it optimizes performance a lot and adds a lot of features (FLYING SQUIDS :D) to help optimize even further or just some fun cool things to do.

### For MC 1.12 and below

[PaperMC](https://papermc.io) is generally the best fork for these versions and not much more is needed.

**JUST PLEASE DONT USE VANILLA JAR!**

## Optimizing your .jar specific configurations to YOUR NEEDS (may be moved to its own md)

Every .jar comes with its own set of configurations you can tweak to suit your needs, and keep in mind that, YOUR NEEDS. You probably wont find as efective the config of a minigames server in a survival server. You should read every config, understand it, and choose if you need to use it or not. This is extremely important in survival servers as some config values can ruin your mob spawning rates or destroy your players custom redstone circuits.

Heres a [guide](https://www.spigotmc.org/threads/guide-server-optimization⚡.283181/) made by a well-known member of the community that can help you further in this optimization. Or join [this discord](https://discord.gg/yev2rN3eZH), they have an amazing discord bot that tells you how to optimize your server based on your timings report!

Another important thing in survival servers is to pre-generate your world, because chunk generation consumes a lot! This can be done in several ways but heres an example:

1. Download [Fast Chunk Pregenerator](https://www.spigotmc.org/resources/fast-chunk-pregenerator.74429/)
2. Set your desired world limit.
3. Use the command: /fcp start (radius) (world) (chunkX) (chunkZ)
4. Wait for it to finish, it may take a long time and the server will lag while it works. This **MUST** be done with the server empty / closed to public.

You should also use correct startup flags, the [Aikars flags](https://aikar.co/2018/07/02/tuning-the-jvm-g1gc-garbage-collector-flags-for-minecraft/)!
