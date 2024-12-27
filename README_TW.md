繁體中文 | [**簡體中文**](./README.md) | [English](./README_EN.md) 

# Fabric-Bedrock-Miner

幫你 "挖掘" 基巖的客戶端 Fabric mod！

# 我的世界版本支持

Minecraft 1.21.4

# 歷史版本

Minecraft1.12.1[bunnyi116/fabric-bedrock-miner ](https://github.com/bunnyi116/fabric-bedrock-miner)

Minecraft1.20[LXYan2333/Fabric-Bedrock-Miner](https://github.com/LXYan2333/Fabric-Bedrock-Miner) 

# 說明

該項目復刻自 [LXYan2333/Fabric-Bedrock-Miner](https://github.com/LXYan2333/Fabric-Bedrock-Miner) 以及[bunnyi116/fabric-bedrock-miner ](https://github.com/bunnyi116/fabric-bedrock-miner)進行修改

## 默認方塊列表清單

#### 破壞方塊白名單（支持破壞）

- 基巖

#### 破壞方塊黑名單 (不支持破壞)

- 暫無

#### 服務器方塊黑名單（不支持破壞，無法通過指令更改，內置過濾器）

- 屏障
- 普通型命令方塊
- 連鎖型命令方塊
- 循環型命令方塊
- 結構空位
- 結構方塊
- 拼圖方塊

#### 方塊添加命令過濾器

- 空氣
- 可替換方塊

## 客戶端指命說明

- `/bedrockMiner` 開啟/關閉
- `/bedrockMiner disable` 禁用模組（開啟後模組將不會繼續處理）
- `/bedrockMiner block whitelist add <block>` 添加白名單方塊列表
- `/bedrockMiner block whitelist remove <block>` 移除白名單方塊列表
- `/bedrockMiner block blacklist add <block>` 添加黑名單方塊列表
- `/bedrockMiner block blacklist remove <block>` 移除黑名單方塊列表
- `/bedrockMiner blockName blacklist add <blockName>` 添加黑名單方塊列表
- `/bedrockMiner blockName blacklist remove <blockName>` 移除黑名單方塊列表
- `/bedrockMiner task add <x, y, z>` 添加任務
- `/bedrockMiner task clear` 清理任務
- `/bedrockMiner debug true` 開啟調試模式
- `/bedrockMiner debug false` 關閉調試模式

# 視頻教程

https://www.youtube.com/watch?v=b8Y86yxjr_Y
</br>
https://www.bilibili.com/video/BV1Fv411P7Vc

# 使用方法

使用前需準備好如下物品：

1. 效率 Ⅴ 鉆石鎬（下界合金也行）
2. 急迫 Ⅱ 信標
3. 一些活塞
4. 一些紅石火把
5. 黏液塊若幹

**空手**右鍵基巖啟動此模組（註意要空手）

啟動後，左鍵基巖，模組會嘗試自動破除基巖。

再次空手右鍵基巖關閉此模組。

如果本模組幫你節省了大量時間的話，請給個 Star 唄 QwQ。

# 更新內容

因Minecraft1.21.4更新

Fabric(yarn-1.21.4+build.2)API修改了Fabric(yarn-1.21.1+build.3)API `net.minecraft.network.packet.c2s.play`中的`PickFromInventoryC2SPacket`方法體，將其分為`PickItemFromBlockC2SPacket`和`PickItemFromEntityC2SPacket`。

新增` PickItemFromBlockC2SPacket`，還修改了` PlayerMoveC2SPacket.LookAndOnGround`方法的使用，修改了`EntityAttributes`中對藥水效果的定義
