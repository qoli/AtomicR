# 已知 Bugs

##### 在 Terminal 運行命令可能閃退

在 Terminal 運行中有可能遇到 libssh2_channel_read 錯誤而導致 App 閃退

再次執行相同指令即可，目前此 Bugs 為偶發性。

##### 在 HND 機型上未支持 Shadowsock 控制面板

等待 App 更新。



# 計劃進度

##### 當前計劃

##### 1.0

* 界面支持簡體中文
* 添加線路功能
* Setting 頁面完工
* 多 SSH 配置檔支援
* Add Collection View 支援本地化顯示名稱
* 增加 HND 機型支援

##### 已排程計劃

##### 1.1

* json 腳本支援預先配置模式一鍵執行



# 更新日誌

##### 2019年03月04日

##### App（Build 25）

* 修正移除訂閱服務器后，由於運行中的服務器不存在列表上而閃退

##### App（Build 24）

* 修正 Terminal 在無服務器設定下的閃退

##### 2019年03月03日

##### 脚本源

**修改** Shadowsock 相关脚本修改来源版本

**增加** L2TP/IPSec VPN 一键安装脚本

**增加** 系统操作脚本

##### App（Build 23）

* 增加更新日誌
* 使用 SSH 模式讀取配置，嘗試改善兼容性。
* 嘗試修正 R6300V2 機型閃退

##### App（Build 21）

Build 21 版本發佈

* 增加了歡迎界面
* 改善 JSON Screen 載入性能
* 改善 iPhone SE 兼容性

##### 早期發佈（Build 21 之前）

* 支援 ACL（訪問控制）設定
* 支援線路切換
* 支援 Status（國外連線狀態）顯示
* 基於 JSON 調用 Terminal 以及 UI 呈現的 JSON Screen
* JSON Screen Add List

