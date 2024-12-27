[繁體中文](./README_TW.md) | **简体中文** | [English](./README_EN.md) 

# Fabric-Bedrock-Miner
帮你 "挖掘" 基岩的客户端 Fabric mod！

# 我的世界版本支持

Minecraft 1.21.4

# 历史版本

Minecraft1.12.1[bunnyi116/fabric-bedrock-miner ](https://github.com/bunnyi116/fabric-bedrock-miner)

Minecraft1.20[LXYan2333/Fabric-Bedrock-Miner](https://github.com/LXYan2333/Fabric-Bedrock-Miner) 

# 说明
该项目复刻自 [LXYan2333/Fabric-Bedrock-Miner](https://github.com/LXYan2333/Fabric-Bedrock-Miner) 以及[bunnyi116/fabric-bedrock-miner ](https://github.com/bunnyi116/fabric-bedrock-miner)进行修改

## 默认方块列表清单

#### 破坏方块白名单（支持破坏）
- 基岩

#### 破坏方块黑名单 (不支持破坏)
- 暂无

#### 服务器方块黑名单（不支持破坏，无法通过指令更改，内置过滤器）
- 屏障
- 普通型命令方块
- 连锁型命令方块
- 循环型命令方块
- 结构空位
- 结构方块
- 拼图方块

#### 方块添加命令过滤器
- 空气
- 可替换方块

## 客户端指命说明
- `/bedrockMiner` 开启/关闭
- `/bedrockMiner disable` 禁用模组（开启后模组将不会继续处理）
- `/bedrockMiner block whitelist add <block>` 添加白名单方块列表
- `/bedrockMiner block whitelist remove <block>` 移除白名单方块列表
- `/bedrockMiner block blacklist add <block>` 添加黑名单方块列表
- `/bedrockMiner block blacklist remove <block>` 移除黑名单方块列表
- `/bedrockMiner blockName blacklist add <blockName>` 添加黑名单方块列表
- `/bedrockMiner blockName blacklist remove <blockName>` 移除黑名单方块列表
- `/bedrockMiner task add <x, y, z>` 添加任务
- `/bedrockMiner task clear` 清理任务
- `/bedrockMiner debug true` 开启调试模式
- `/bedrockMiner debug false` 关闭调试模式

# 视频教程
https://www.youtube.com/watch?v=b8Y86yxjr_Y
</br>
https://www.bilibili.com/video/BV1Fv411P7Vc

# 使用方法
使用前需准备好如下物品：
1. 效率 Ⅴ 钻石镐（下界合金也行）
2. 急迫 Ⅱ 信标
3. 一些活塞
4. 一些红石火把
5. 黏液块若干

**空手**右键基岩启动此模组（注意要空手）

启动后，左键基岩，模组会尝试自动破除基岩。

再次空手右键基岩关闭此模组。

如果本模组帮你节省了大量时间的话，请给个 Star 呗 QwQ。

# 更新内容

因Minecraft1.21.4更新

Fabric(yarn-1.21.4+build.2)API修改了Fabric(yarn-1.21.1+build.3)API `net.minecraft.network.packet.c2s.play`中的`PickFromInventoryC2SPacket`方法体，将其分为`PickItemFromBlockC2SPacket`和`PickItemFromEntityC2SPacket`。

新增` PickItemFromBlockC2SPacket`，还修改了` PlayerMoveC2SPacket.LookAndOnGround`方法的使用，修改了`EntityAttributes`中对药水效果的定义

