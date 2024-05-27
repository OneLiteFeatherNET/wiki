---
layout: landing
---

# Introduction

## What is Microtus?

[**Microtus**](https://github.com/OneLiteFeatherNET/Microtus) is not only the latin term of a [common vole](https://en.wikipedia.org/wiki/Microtus), it is the up to date, open source fork of the serversoftware [**Minestom**](https://minestom.net/) which aims for code quality & stability. In order to do so, you, the community are playing an important part! Unlike (Craft-) Bukkit, Spigot, Paper and their corresponding forks, Microtus is **not** a drop in replacement for a whole Minecraft Vanilla experience. The main reason behind this is that Microtus (and Minestom) contains no Minecraft/Mojang/Microsoft developed Code.

\
\-> Microtus is a framework or literally "construction kit", it is meant to help building your own features, servers or minigames. Like a sandbox, it contains tools like a shovel for sand to build your vision of a minigame or server implementation, **but without any vanilla logic!**

## Why Microtus ?&#x20;

Microtus has the ability to accommodate hundreds or thousands of players with little memory. It is also possible to achieve the result faster without a lot of cancellation logic. Everything that is known as NMS[^1] under Paper/Spigot is supplied as an interface with Microtus.

## Why Microtus and not Minestom?

Minestom decided some time ago to add functions such as

* Terminal
* Extensions
* (TinyLog)

**to be removed for various reasons**

Microtus and the team behind it believe that a terminal and extensions is a very good combination for a plugin-in hybrid system to speed up update cycles or development cycles.

It also allows you to deploy smaller jars instead of a large [monolithic](https://en.wikipedia.org/wiki/Monolithic\_application) application. In line with this, we are trying to incorporate or orientate [design patterns](https://refactoring.guru/design-patterns) such as [Modulith](https://dzone.com/articles/architecture-style-modulith-vs-microservices) and others.

In addition, we believe that it is a lesser evil to leak a partial component on the internet than a large jar file containing all dependencies or internal libs.

### TL;DR

We have reinstalled the above features and give full flexibility to the developers and re-document code from upstream or improve it.

## Our goals

Our aim is to bring Microtus closer to the concept of stability, maintainability, and modularity. Since many people see such terms as being empty words, I have described it as a concept.

The main goals can be found here on the [roadmap](https://github.com/orgs/OneLiteFeatherNET/projects/5).

**One of our biggest points is documentation, listening to the community and stimulating discussions. So you are welcome to discuss things on our** [**Discord**](https://discord.onelitefeather.net) **or** [**Github**](https://github.com/OneLiteFeatherNET/Microtus/discussions)**.**

[^1]: Native Minecraft Source
