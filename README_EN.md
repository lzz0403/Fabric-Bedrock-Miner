[繁體中文](./README_TW.md) | [简体中文](./README.md) | **English**

# Fabric-Bedrock-Miner
A Fabric client mod to "mine" bedrock!

# Minecraft Version Support

Minecraft 1.21.4

# History Version

Minecraft1.12.1[bunnyi116/fabric-bedrock-miner ](https://github.com/bunnyi116/fabric-bedrock-miner)

Minecraft1.20[LXYan2333/Fabric-Bedrock-Miner](https://github.com/LXYan2333/Fabric-Bedrock-Miner) 

# illustrate
This project fork modified from [LXYan2333/Fabric-Bedrock-Miner](https://github.com/LXYan2333/Fabric-Bedrock-Miner) and [bunnyi116/fabric-bedrock-miner ](https://github.com/bunnyi116/fabric-bedrock-miner) <br>

## Default block list list

#### Block whitelist (break supported)
- Bedrock

#### Block blacklist (Break is not supported)
- None

#### Server block blacklist (Break is not supported, cannot be changed by command, built-in filter)
- Command Block
- Chain Command Block
- Repeating Command Block
- Structure Void
- Structure Block
- Jigsaw Block

#### Block to add command filters
- Air
- Replaceable blocks

### Command description
- `/bedrockMiner` on/off
- `/bedrockMiner disable` disable the mod (the mod will not continue to process after it is turned on)
- `/bedrockMiner block whitelist add <block>` add whitelist block list
- `/bedrockMiner block whitelist remove <block>` remove whitelist block list
- `/bedrockMiner block blacklist add <block>` add blacklist block list
- `/bedrockMiner block blacklist remove <block>` remove blacklist block list
- `/bedrockMiner block blockName add <blockName>` add blacklist block list
- `/bedrockMiner block blockName remove <blockName>` remove blacklist block list
- `/bedrockMiner task add <x, y, z>` add a task
- `/bedrockMiner task clear` clear the task
- `/bedrockMiner debug true` enables debug mode
- `/bedrockMiner debug false` turn off debug mode

# Showcase
https://www.youtube.com/watch?v=b8Y86yxjr_Y  
https://www.bilibili.com/video/BV1Fv411P7Vc

# Usage
Have the following items ready:
1. Efficiency V diamond (or netherite) pickaxe
2. Haste II beacon
3. Pistons
4. Redstone torches
5. Slime blocks

Right click bedrock **with an empty hand** to switch on/off.

While the mod is enabled, left click bedrock to "mine" it.

If my mod saves you tons of time, please considering leave me a star.

# Compile
Checkout to the corresponding Minecraft version and compile following the Fabric wiki.

# Update Record

Due to Minecraft 1.21.4 update
The Fabric (yarn-1.21.4+build. 2) API has modified the body of the `PickFromInventoryC2SPacket` method in the Fabric (yarn-1.21.1+build. 3) API's `net.minecraft.network.packet.c2s.play`, dividing it into`PickItemFromBlockC2SPacket` and `PickItemFromEntityC2SPacket`.
Added `PickItemFromBlockC2SPacket` and modified `PlayerMoveC2SPacket.LookAndOnGround` and the definition of potion effects in `EntityAttributes`
