# zh 本地化术语表

批次 1（登录→角色选择/创建界面）定译。后续批次沿用；有修订时改此处并回填历史译文。

约定：简体中文；全角标点（，。：？！）用于中文句子内，省略号用"……"；`\n`、`\t` 等标记与 `$xxx$`、`%s`、`&amp;` 实体、快捷键标记原样保留；专名保留拉丁原文（见"待定名"区）。

## 通用词定译

Login / LOGIN → 登录
Password → 密码
Confirm Password → 确认密码
Forgotten Password → 忘记密码
Username → 用户名
Email Address → 电子邮箱
Account → 账号（Create/Edit/Upgrade Account → 创建/编辑/升级账号）
Free Trial Account → 免费试用账号
Submit → 提交
OK → 确定
Cancel → 取消
Back → 返回
Next → 下一步
Close → 关闭
Delete → 删除
Rename → 重命名
Exit → 退出
Help → 帮助
Support → 客服支持
Options → 选项
Configuration → 配置
Status → 状态
Version → 版本；Version Notes → 版本说明；Read Notes → 阅读说明
Client Version → 客户端版本
Online / Offline → 在线 / 离线
Connect → 连接；Connecting → 正在连接
Play → 开始游戏
Patch → 补丁；Patch Details → 补丁详情；Total Patch → 补丁总量
Required Files → 所需文件
Check Data → 检查数据
Level of Detail (LOD) → 细节等级
Game Resolution → 游戏分辨率
Normal → 普通
Career → 职业
Civilization → 种族（fix round 1 裁定：uiRand3 与同屏 uiSelCiv "你想扮演哪个种族？"统一用"种族"；wk 侧此标签为 CIVILISATION）
Race → 种族
Culture → 文化
Ecosystem → 生态系统
Gender → 性别
Name → 名字；Surname → 姓氏
Character → 角色
Empty Slot → 空槽位
Level → 等级
Body → 身体；Arms → 手臂；Legs → 腿部；Torso → 躯干
Face → 面部；Shape（脸栏目）→ 脸型
Hair → 头发；Haircut → 发型
Eye Color → 眼睛颜色
Eye（Fyros 脸型滑条 uiFace2Fy；wk 主文档为 EYES HEIGHT）→ 眼睛高度（fix round 1，与 uiFace1Fy 嘴部高度/uiFace3Fy 鼻子高度同族一致）
Tattoos → 纹身
Clothes → 服装
Height → 身高
Colors → 颜色
Score（HP/Sap 等状态数值，角色摘要表）→ 数值
Max / Maximum → 最大 / 最大值
Reg (Regeneration) → 回复
Fighter → 战士；Magician → 法师；Ranger → 游侠；Crafter → 工匠
General（职业页签）→ 概述；Specific（职业页签）→ 专项
Randomize → 随机生成；Manual creation → 手动创建；Random creation → 随机创建
End User Licence Agreement (EULA) → 最终用户许可协议；I ACCEPT → 我接受；DECLINE → 拒绝
Code of Conduct → 行为准则
Skip Intro → 跳过开场

## 专名（待定名区，批次 1 保留拉丁原文）

Fyros / FYROS → 原样保留（uiCultFy 标题大写 FYROS、正文 Fyros，随原文大小写）
Matis / MATIS → 原样保留
Tryker / TRYKER → 原样保留
Zoraï / ZORAÏ → 原样保留（含 ï）
Ryzom / RYZOM → 原样保留（uiSelectTitle 大写 RYZOM，随原文）
Atys → Atys
homin(kin) → homin（"hominkind" 译作 "homin 一族"）
kitins → kitin（"kitin 蜂群"）
Ryzom Arkitect → Ryzom Arkitect
Winch Gate (Property Limited) → Winch Gate（公司名不译）
Kami / Karavan / Homins → 未出现在批次 1，留待后续批次定译
Green Rising（Atys 大事件）→ 暂译"绿之复苏"，待定名
Great Dragon（en）/ Grand Arsonist（wk 法语 lore，同一角色）→ 暂译"巨龙"，待定名；fix round 1 裁定维持"巨龙"（与 en 回退显示一致优先于 wk 法语 lore），后续批次复核
Berserker（Fyros 战士职阶）→ 暂译"狂战士"，待定名
WorldPay / PayPal / Steam / SSL / GNU AGPL → 原样保留（许可证名"GNU Affero General Public License"译作"GNU Affero 通用公共许可证"）

## wk/en 源文本漂移记录（批次 1，fix round 1 补录）

**裁定：译文以 en.uxt 为基准**（fix round 1 修订，旧计划"以 wk 为准"作废；en 为客户端实际回退显示文本）。
下表由 `wk.uxt` 与 `translated/en.uxt` 对 140 条批次 1 标签逐键对比自行生成：**35 条文本差异（10 条仅排版/标点差异，25 条实质差异）+ 15 条 wk 缺失 + 90 条完全一致 = 140**。
注：审查报告口径为 38 条，与本次实测 35 条不符，待与审查者对账；本表为可复现实测（脚本 `wk_en_drift.py`，解析逻辑同 Task 5 提取器；en.uxt 中 140 标签各恰定义 1 次）。

### A. 实质文本差异（25 条）

| label | wk.uxt 值 | en.uxt 值（译文基准） |
|---|---|---|
| `uiAppearTitle` | `HOW DO WANT TO LOOK LIKE ?` | `WHAT DO YOU WANT TO LOOK LIKE?` |
| `uiCaNaBoldC` | `CRAFTSMAN` | `CRAFTER` |
| `uiCultFy` | `FYROS: WARRIORS OF FIRE AND MASTERS OF THE BURNING DESERT\n\n\t\n\n\tThe Fyros are the warrior race.…`（共 253 字符） | `FYROS: WARRIORS OF FIRE AND MASTERS OF THE BURNING DESERT\n\n\t\n\n\tThe Fyros are the warrior race.…`（共 250 字符） |
| `uiEulaAccept` | `ACCEPT` | `I ACCEPT` |
| `uiEulaContent` | `LICENCE RYZOM\n\n\t\n\n\tAVIS À L'UTILISATEUR : CE DOCUMENT EST UN CONTRAT. AVANT DE CLIQUER SUR LE …`（共 21470 字符） | `RYZOM LICENSE\n\n\t\n\n\tA NOTICE TO THE USER: THIS DOCUMENT IS A CONTRACT. BEFORE CLICKING ON THE "…`（共 19569 字符） |
| `uiExplcarac` | `CARACTERISTICS\n\n\t\n\n\tYou have 20 points to add to your caracteristics.\n\n\t\n\n\tRULES:\n\n\t-…`（共 235 字符） | `CHARACTERISTICS\n\n\t\n\n\tYou have 20 points to add to your characteristics.\n\n\t\n\n\tRULES:\n\n\…`（共 237 字符） |
| `uiEyes` | `EYES COLOR` | `EYE COLOR` |
| `uiFace1Fy` | `MOUTH HEIGHT` | `MOUTH LEVEL` |
| `uiFace2Fy` | `EYES HEIGHT` | `EYE` |
| `uiFace3Fy` | `NOSE HEIGHT` | `NOSE LEVEL` |
| `uiFace7Fy` | `EYES WIDTH / EYEBROWS` | `EYE WIDTH / EYEBROWS` |
| `uiForgetPwd` | `I FORGOT MY PASSWORD` | `FORGOTTEN PASSWORD` |
| `uiFreeTrial` | `FREE TRIAL` | `CREATE YOUR FREE TRIAL ACCOUNT` |
| `uiGameConfiguration` | `GAME CONFIGURATION` | `CONFIGURATION` |
| `uiOnPatchDetail` | `PATCH DETAIL` | `PATCH DETAILS` |
| `uiOnPatchOpt` | `OPTIONALS: Add/Remove Files From Patch` | `OPTIONAL: Add/Remove Files From Patch` |
| `uiOnRelease` | `RELEASE NOTE` | `VERSION NOTES` |
| `uiRand3` | `RACE` | `CIVILIZATION` |
| `uiRand4` | `SEX` | `GENDER` |
| `uiReleaseNote` | `READ NOTE` | `READ NOTES` |
| `uiSelInfos` | `INFORMATIONS\n\n\t\n\n\tYou have 5 slots to save 5 different characters.\n\n\tTo create a new charac…`（共 253 字符） | `INFORMATION\n\n\t\n\n\tYou have 5 slots to save 5 different characters.\n\n\tTo create a new charact…`（共 251 字符） |
| `uiTatoos` | `TATOOS` | `TATTOOS` |
| `uiZoCulture` | `ZORAI-CULTURE` | `ZORAÏ-CULTURE` |
| `uiZoEco` | `ZORAI-ECOSYSTEM` | `ZORAÏ-ECOSYSTEM` |
| `uiZoName` | `ZORAI` | `ZORAÏ` |

### B. 仅排版/标点/大小写差异（10 条，语义相同）

| label | wk.uxt 值 | en.uxt 值（译文基准） |
|---|---|---|
| `uiCareerTitle` | `WHAT DO YOU WANT TO BECOME ?` | `WHAT DO YOU WANT TO BECOME?` |
| `uiDelChar` | `DELETE THIS CHARACTER ?` | `DELETE THIS CHARACTER?` |
| `uiDeleteTitle` | `DO YOU REALLY WANT TO DELETE ?` | `DO YOU REALLY WANT TO DELETE?` |
| `uiLocationTitle` | `WHERE DO YOU WANT TO GO ?` | `WHERE DO YOU WANT TO GO?` |
| `uiManCrea` | `Manual Creation` | `Manual creation` |
| `uiRanCrea` | `Random Creation` | `Random creation` |
| `uiRebootConfirm` | `Ryzom will now relaunch. Please wait until Ryzom is fully restarted` | `Ryzom will now relaunch. Please wait until Ryzom is fully restarted.` |
| `uiSelCiv` | `WHAT RACE DO YOU WANT TO PLAY ?` | `WHAT RACE DO YOU WANT TO PLAY?` |
| `uiSummaryTitle` | `WHAT NAME DO YOU WANT ?` | `WHAT NAME DO YOU WANT?` |
| `uiTryton1` | `For many centuries I have voyaged through the quiescent corridors of Ryzom. I bore witness to the Gr…`（共 540 字符） | `For many centuries I have voyaged through the quiescent corridors of Ryzom. I bore witness to the Gr…`（共 525 字符） |

### C. wk.uxt 缺失（15 条，wk 无此标签、en 独有）

`uiAcceptTermsOfUse1`, `uiAcceptTermsOfUse2`, `uiCreateAccountWelcome`, `uiEmail`, `uiLOGLod`, `uiLOGResolution`, `uiLodValue`, `uiRequiredFiles`, `uiResValue`, `uiScanData`, `uiSubmitNewAccount`, `uiSubmitSucces1`, `uiSubmitSucces2`, `uiTotalPatch`, `uittBrowseFaq`

> 长文本（uiEulaContent、uiCultFy、uiTryton1、uiSelInfos、uiExplcarac）仅示前 100 字符，全文见源文件；其中 uiCultFy 的 wk 值含 "the Grand Arsonist"（wk.uxt:5118），en 值为 "the Great Dragon"——译文按 en 取"巨龙"，见待定名区。
