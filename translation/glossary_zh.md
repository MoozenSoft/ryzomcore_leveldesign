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
Kami / Karavan → 保留拉丁（批次 2 c2 定录，见"批次 2"节）；Homins → 未出现，留待后续批次定译
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

## 批次 2（游戏内主界面 ingame）定译 —— c2 分片（R2ED 场景编辑器 / Ring 窗口 / 前哨站）

### 前哨站（Outpost）

Outpost → 前哨站；BUILDINGS → 建筑；SQUADS → 小队；STATUS → 状态；OUTPOST（标题）→ 前哨站
Attack/Defense Phase → 攻击/防御阶段；Attack/Defense Time → 攻击/防御时间；Before/After Attack（Defense）→ 攻击前/攻击后（防御前/防御后）
Attacker / Defender → 攻击方 / 防御方
Round → 回合；Round Level → 回合等级；Current Round → 当前回合；Minimum Threshold → 最低阈值
Coffer(s) → 金库；WAR COFFER → 战争金库；Change Coffer → 更改金库
dapper(s) → 达珀（暂译·音译，待定名；Ryzom 货币单位）
Guild → 公会；Guild Leader → 公会会长；High Officer → 高级军官
squad → 小队；squad spawn → 小队出动；SQUAD SPAWN POSITION → 小队出动位置；ACTIVE SQUADS → 已出动小队；PENDING SQUADS → 待命小队；RECRUIT / SQUAD RECRUITMENT → 招募 / 小队招募
DECLARE WAR → 宣战；COST OF DECLARING → 宣战费用；WAR SCHEDULE → 战争时间表；WAR STATUS → 战争状态；War Declared → 已宣战；Peace → 和平
Marauding Tribe → 劫掠部落（暂译）；hostile tribe → 敌对部落
Time Zone → 时区；LOCAL（时间语境）→ 当地时间；Auto / automatic mode → 自动 / 自动模式

### Ring / R²ED 场景编辑器

**Scenario → 场景**（正式定录入册）。裁定依据：批次 1 已审定 outv2 输出即实译（"SCENARIO EDITOR"→"场景编辑器"、"Resume Scenario"→"继续场景"），分片任务名亦为"R2ED 场景编辑器"；任务书括号虽将 Scenario 列入专名，按既译一致优先。R²ED、Ring、Ryzom、Ryzom Ring Points（含缩写 RRP）仍保留拉丁。
Ring Terminal → Ring 终端；Ring Destinations → Ring 目的地；destination → 目的地；Ring Scenario → Ring 场景
场景难度段位：Novice / Apprentice / Confirmed / Advanced / Expert / Master → 新手 / 学徒 / 熟手 / 进阶 / 专家 / 大师
评分五维（Ratings → 评分）：Accessibility → 可达性（暂译）；Difficulty → 难度；Direction → 指引性（暂译）；Fun → 趣味性；Originality → 原创性
Reward Points → 奖励点数；Author RRP → 作者 RRP；Owner RRP → 所有者 RRP；Scenario RRP → 场景 RRP
Requirements → 要求；Listing Options → 列表选项；Control（uiR2EDRules 标签）→ 控制权（暂译；其 tooltip "Mastering" → 主持方式）
Adventure Master → 冒险主持人；Animator → 主持人；Mastered / Masterless → 有主持 / 无主持
newcomer → 新人；ALLOW NEWCOMERS → 允许新人；Non-guild players → 非公会玩家
Shard → 服务器；Mainland → 主大陆；allegiance → 信仰（信奉 Kami/Karavan；no allegiance → 无信仰）
Kami / Karavan → 保留拉丁（批次 1 待定名区遗留项，本次定录）
台词条目（尾随空格保留，运行时在其后拼接玩家名）：Send a 'tell' to → "发送密语给 "；Kick → "踢出 "；Unkick → "取消踢出 "；Teleport to → "传送到 "；tell → 密语；KICK / UNKICK → 踢出 / 取消踢出
Fit columns → 适应列宽；Resize → 调整大小；Connected player → 在线玩家；Nb. Players → 玩家人数；Players tracking → 玩家追踪；Launch date → 启动日期
"My Scenarios"（文件系统文件夹名）与 "Pioneer Scenarios"（加载树分类名）保留拉丁

### c2 实测：值内换行/标记保留

源值含两类换行标记：字面 `\n`（反斜杠+n 两字符）与"真实换行+真实制表"对（`\n`+`\t`），典型组合形如 `\n`⏎⇥；译文逐键等数复现，不合并不清理。c2 全 245 键合计：55×`@{` 色码、40×真实换行、40×真实制表、1×`%time`；无 `$`、无 `&`。核对脚本 `make_zh_c2.py`，日志 `check_c2.txt`、`check_c2_extra.txt`（色码载荷序列逐键比对、数字集合逐键比对、残留拉丁词扫描）。

## 批次 2（游戏内主界面 ingame）定译 —— c3 分片（动作栏/聊天/任务/公会等其余 ingame 界面）

### 与 c2 已定译对齐（沿用）

Scenario → 场景；tell → 密语；dapper(s) → 达珀；Outpost → 前哨站；DECLARE WAR → 宣战；Mainland → 主大陆；High Officer → 高级军官（Officer → 军官）；Guild Leader → 公会会长（Leader → 会长）；Kami/Karavan/Ring 保留拉丁

### 通用 UI / 系统（c3 新增）

Action(s) → 动作；Action Bar → 动作栏；Key → 按键；Assign/Delete/Edit Key → 指定/删除/编辑按键；Macro → 宏；Shortcut Bar → 快捷栏；Shortcut Number → 快捷位编号；Run Shortcut → 执行快捷操作
Chat → 聊天；Main Chat → 主聊天；Tell Mode/Tell Window/Reply Tell → 密语模式/密语窗口/回复密语；Talk → 交谈；Say → 说话；Shout → 大喊；Universe (Channel) → 宇宙（频道）；Territory → 领地；Contact List → 联系人列表
Desktop（多套界面布局）→ 桌面；Popup / Popin → 弹出 / 停靠；Dock/Undock → 停靠/解除停靠
Compass → 罗盘；Map → 地图；Landmark → 地标；Zoom in/out → 放大/缩小；Rear View → 后视角；View（键位组）→ 视角；Camera → 镜头
Mission(s) → 任务；Mission Journal → 任务日志（uiJournal 标题译"任务"）；Ritual Task → 仪式任务；Rite → 仪式；Tracking → 追踪
Guild XP → 公会经验；Guild Points → 公会点数；Rank（公会职级）→ 职位；Headquarters → 总部；Bearer → 旗手（暂译）；Recruiter → 招募官
Fame → 名望；Target（名）→ 目标 /（动）锁定；Assist → 协助；Bonus/Malus → 增益/减益；Powers/Auras → 能力/光环；Dodge/Parry → 闪避/招架；Death Penalty → 死亡惩罚；Coma → 昏迷；Respawn → 复活（uiDeathWarningContent 文内"RESPAWN 按钮"译"复活"按钮，与 uiRespawn 一致）
Resale → 转售；Resale Margin → 转售差价；Bonus On Resale → 转售加成；Base Price → 基础价格
品质档位 Class（botchat 筛选）：Basic/Fine/Choice/Excellent/Supreme → 初级/优良/上选/优秀/极品（Class → 品级，与 Quality=品质 区分）
Encyclopedia → 百科全书；Album → 合集；Theme → 主题；Action Progression → 动作进阶；Progression → 进度
Debug → 调试；Profile → 性能分析；Primitive → 图元；Render Mode → 渲染模式；Screenshot → 截图；Movie → 影片

### 采集/制造/动物（c3 新增）

Raw Material → 原材料；Craft → 制造；Harvest → 采集；Extract → 提取；Plan（制造图样槽）→ 图样；Stanza（"Root Stanza"）→ 根节（暂译）
Mount → 坐骑（名）/骑乘（动）；Mount / Dismount → 骑乘 / 下骑；Stable → 马厩；Packer（驮兽）→ 驮兽；Pack（驮兽驮包栏）→ 驮包；Demon（ANIMAL_TYPE::Demon 宠物型）→ 恶魔（暂译）；Free（放归宠物）→ 放生；Quarter（剖割尸体）→ 剖割

### NPC 语境菜单 uimGcm*（c3 新增）

Role Master → 职业导师（Hire/Upgrade Role Master → 雇佣/升级职业导师；Learn Guild Action → 学习公会动作）
Zone Charge（ZC；客户端经 START_CHOOSE_DUTY 通道，义务/税捐性质）→ 领地税责（暂译：Review Charges → 查看领地税责、Abandon Charge → 放弃领地税责、Charge Attribution → 税责发放）
Pact → 契约（Make a Pact → 缔结契约、Trade Pact → 交易契约）；Building Trade → 建筑交易；Loot → 拾取；Disengage → 脱离战斗；Cosmetics → 外观道具

### c3 实测：换行/标记保留

源值含字面 `
`（反斜杠+n）与"真实换行+真实制表"组合（同 c2），典型段落分隔单元 `
`⏎⇥ 共 13 处逐键等数复现；`@{6F6F}`/`@{FFFF}` 色码各 8 处逐键复现；`%item`、`%fac` 占位符原样；尾随空格（列表标题/动态拼接前缀）逐键保留。全 633 键自查：键集合一致、结构字符（$/%/&/@{/字面
/换行/tab/<>"/反斜杠）逐键计数一致、纯数字值与空值原样；8 条英文缩写撇号随中译消失（预期，非占位符）。核对脚本 `make_c3_zh.py`。

### c3 暂定待复核

领地税责（Zone Charge）、恶魔（Demon）、根节（Root Stanza）、旗手（Bearer）、常用语（Talk Memorized）、购买自/出售给/学习自（Buy from/Sell to/Learn from 列表标题，尾随空格保留）

## 批次 2（游戏内主界面 ingame）定译 —— c1a 分片（游戏配置/任务栏/背包/罗盘/玩家信息/交互）

### 组队与社交
Team → 小队（TEAM INVITATION → 小队邀请；Leave Team → 离开小队；Team Members → 小队成员；注：c2 已定 squad → 小队，两英文词并行映射同词，同屏冲突待复核）
Party Chat → 群聊（CREATE NEW PARTY CHAT → 创建新群聊；join party chat → 加入群聊）
Guild → 公会（与 c2 一致）；GUILD & TEAM → 公会 & 小队（`&` 按契约原样保留）
League → 联盟；Clan（PvP 语境）→ 氏族；Tribe → 部落
Friend → 加为好友；friend list → 好友列表；Ignore → 屏蔽；IGNORE LIST → 屏蔽列表；Contact List → 联系人列表；Add contact → 添加联系人
tell → 密语（与 c2 一致）；Say → 说话；Shout → 喊话；Universe（聊天频道）→ 宇宙；Around → 周围；AROUND ME → 我周围；Dynamic Channel N → 动态频道 N；Communication → 通讯；Emote → 表情动作

### 声望与效忠
Fame → 声望；allegiance（Fame/PvP 语境）→ 效忠：Civilization allegiance → 种族效忠；Cult allegiance → 教派效忠；Cult → 教派；Allegiances: → 效忠：
（范围注：c2 已定 Ring 会话浏览器 allegiance → 信仰；c1a 的 Fame/PvP 国家/教派宣誓语境用"效忠"，两处分治，待统一复核）
Become Neutral → 成为中立；Set Civilization/Cult Allegiance to Neutral → 将种族/教派效忠设为中立；Faction and Nation Points → 阵营与国家点数；Nation → 国家

### 背包/装备
Inventory → 背包（沿用批次 1）；Bulk → 体积（Bag Bulk → 背包体积，尾随空格保留）；EQUIPMENT → 装备；ROOM → 房间；JEWELRY → 首饰；ARMOR → 护甲；HANDS → 手部；Mount → 坐骑；Corpses → 尸体

### 角色数值与战斗
CHARACTERISTICS → 属性；八维：Constitution 体质 / Metabolism 新陈代谢 / Intelligence 智力 / Wisdom 智慧 / Strength 力量 / Balance 平衡 / Dexterity 灵巧 / Will 意志
HP → HP（保留）；Sap → 树液；Stamina → 耐力；Focus → 专注；SAP/FOCUS DISPLAY → 树液/专注显示；REGENERATION → 回复（沿用批次 1）
Dodge → 闪避；Parry → 格挡；Critical Hit → 暴击；Disengage → 脱离战斗；Extract（采集提取动作）→ 提取；Identity（窗口）→ 身份
PROTECTIONS → 防护；RESISTANCES → 抗性；Max. Absorbed → 最大吸收；White/Black stars → 白星/黑星；Named Creature → 命名生物；Boss Creature → 首领生物

### 地标（Landmark → 地标）
Amber 琥珀 / Bandit 强盗 / Bark 树皮 / Citizen 公民 / Construction 建筑 / Fauna 动物 / Fiber 纤维 / Food 食物 / Forage 采集（沿用）/ Excellent Materials 优质材料 / Supreme Materials 极品材料 / Goo 胶质 / Insect 昆虫 / Kitin → kitin（保留拉丁）/ Miscellaneous 杂项 / Mission 任务 / Harmful 有害 / Node 节点 / Oil 油料 / Passage 通道 / Portal 传送门 / Preservative 防腐剂 / Resin 树脂 / Seed 种子 / Shell 甲壳 / Teleporter 传送点 / Wood 木材

### Ring / R²ED（与 c2 对齐）
Ring Scenario → Ring 场景；Ring Terminal → Ring 终端（均沿用 c2）；Ratings → 评分；Ring Ratings → Ring 评分；AM Rating → AM 评分（AM 缩写保留；全称 Adventure Master 见 c2"冒险主持人"）；Author/Organizer Rating → 作者/组织者评分
RRP 等级（en 含 "level" 故加"级"后缀，词根对齐 c2 段位）：Novice / Apprentice / Confirmed / Advanced / Expert / Master level → 新手级 / 学徒级 / 熟手级 / 进阶级 / 专家级 / 大师级
Reward Points (RRP) → 奖励点数（RRP）（对齐 c2）；KNOWLEDGE OF ATYS → Atys 知识
生态：Desert 沙漠 / Forest 森林 / Jungle 丛林 / Lakes 湖泊 / Prime Roots 原始根须（暂译待复核）

### PvP
allies / enemies / neutrals → 友方 / 敌方 / 中立方（PvP Allies in Guild/Team → 公会内/小队内 PvP 友方）；spire → 尖塔；PvP Logo → PvP 徽标；Neutral → 中立

### 图形/系统配置
Bloom → 泛光；Square Filter → 方形滤镜；Gamma → 伽马值；Contrast → 对比度；Luminosity → 亮度；Far Clip → 远景裁剪；Micro-Vegetation → 微植被；Landscape → 地形；Special Effects → 特效；Opacity → 不透明度（Mouse-Over Opacity → 悬停不透明度）
Max. Tracks（声音性能区，game_config.xml maxtrack）→ 最大音轨数；Max. High Def. → 高清角色上限（意译）；Max. Polygons → 最大多边形数
服务器状态：Authenticating 正在验证 / Logging in 正在登录 / Synchronizing 正在同步 / Probing 正在探测 / Stalled 停滞
其他：OTHER GIVES → 对方给予（player_trade.xml 交易接收侧）；NOT YET → 暂不（免费试用升级提示按钮，与 Upgrade Now 配对）；Quit Now → 立即退出；MY INFO SYSTEM → 我的信息系统；Item text → 物品文本；Roleplay Tags → 角色扮演标签；Prerequisites → 前置条件；Mission Journal → 任务日志
保留原文值：HP / HUD / NPC / PING / N/A / FPS / 25m·50m·125m·250m / /hello / Ryzom Ring / Hiha（拟声表情名，暂不译）/ Kami / Karavan / Fyros / Matis / Tryker / Zoraï（含 ï）/ Atys / kitin

### c1a 实测：值内换行/标记保留
与 c2 同型：字面 `\n` + "真实换行+真实制表"对，逐键等数复现。c1a 全 490 键合计：39 键含标记（`@{` 色码 32 键 77 处、字面 `\n` 31 键 50 处、真实换行/制表随行、`%n`/`%p` 11 键 16 处、`&` 1 键）；无 `$`。管线注意：经 heredoc 直写时 `\n` 会被折叠为 `\n`（本片初稿曾中招 50 处，已程序化回补为字面 `\n` + 真实换行/制表并全量复检通过）。

## 批次 2（游戏内主界面 ingame）定译 —— c1b 分片（游戏配置/任务栏/背包/罗盘/玩家信息/交互 · 后半）

### 与 c1a/c2/c3 对齐沿用（本批实测落地）

Team → 小队（Leave Team → 离开小队；Team Members → 小队成员；TEAM SHARE → 小队分配）；Party Chat → 群聊；tell/Say/Shout → 密语/说话/喊话；Universe → 宇宙；Around → 周围；Dynamic Channel N → 动态频道 N；Fame → 声望；Bulk → 体积；Dodge/Parry → 闪避/格挡；HP（缩写）→ HP 保留（TARGET HP → 目标 HP），Hit Points/health points（全称）→ 生命值；Emote → 表情动作；Stable → 马厩；Free（动物）→ 放生；Mount → 坐骑（名）/骑乘（动）；dapper(s) → 达珀；Mainland → 主大陆；Scenario Editor → 场景编辑器；Faction（Fame/PvP 语境）→ 阵营；PvP allies/enemies/neutrals → 友方/敌方/中立方；spire → 尖塔；PvP Logo → PvP 徽标；Jewelry/jewels → 首饰；Extract/Extraction → 提取（Harvest/Forage → 采集）；地标名沿用 c1a 表（本批 tooltip 引用 'Portal'→传送门、'Teleporter'→传送点、'Named Creature'→命名生物、'Boss Creature'→首领生物）

### c1b 新定译

战斗状态：Stamina → 耐力；Focus → 专注；Sap → 树液；Satiety → 饱食度；Bonus/Malus → 增益/减益；Total Malus → 总减益；Action Malus → 动作减益；Resistance score → 抗性分数；Magic domain → 魔法领域；Magical protection → 魔法防护；Affliction → 诅咒（暂定）；Elemental → 元素；Melee attack → 近战攻击；Special attack → 特殊攻击；Default attack → 默认攻击；Regeneration → 回复（沿用批次 1）
物品/背包：Quality → 品质；Materials → 材料；Armor → 护甲；Weapons → 武器；Tools → 工具；Slot → 槽位；Weight → 重量；BAG（INVENTORY 内页签）→ 背包；Pin（窗口）→ 固定；Consume Item → 使用物品；Teleporter Pact → 传送契约
装备部位：Chest covering 胸部护甲 / Sleeves 护臂 / Leg covering 腿部护甲 / Boots 靴子 / Gloves 手套 / Helmet 头盔 / Diadem 头冠 / Necklace 项链 / Earring 耳环 / Anklet 脚环 / Ring 戒指 / Bracelet 手镯（左右成对：左 X / 右 X）
社交/界面：Taskbar → 任务栏（底部主栏沿原名）；Action Bar → 动作栏；MY BARS（量表窗口，en 帮助文档作 "My Gauges"）→ 我的数值条；KEYBINDINGS → 按键绑定；Tabs → 页签；Groups → 群组；Block/Unblock → 屏蔽/取消屏蔽；Team Leader → 小队队长；Successor → 继承人；Validation(s) → 确认（数）；Title（角色）→ 称号；Guild Symbol → 公会徽记；Roleplay Tags → 角色扮演标签；PvP Tag → PvP 标记
传送/罗盘：TELEPORT LOCATIONS → 传送地点；Compass Target → 罗盘目标；Compass Range → 范围（罗盘探测范围）
暂定待复核：Source Life → 来源储量；Stanza → 节（c3 已定 Root Stanza → 根节，本批 "boost stanzas" → 强化节，同根）；Dismiss（动物）→ 遣散；Catalyzer → 催化器；Crystallize → 晶化；Enchant → 附魔；Recharge → 充能；Weak trading → 受限交易；Mobs → 怪物；FS（前端服务缩写）保留拉丁
保留原文值：DEUTSCH/ENGLISH/FRANCAIS/ESPANOL/РУССКИЙ（语言自名）、HUD、PVP、16:9、4:3、%、x；单位后缀 " m"→" 米"、" characters"→" 个字符"（前导空格保留）；尾随空格标签（Total Malus 、Speed Factor ）保留

### c1b 关键考证

- SHARING SEEDS 的 seeds = dappers（货币别称）：interaction.xml:627 队伍聊天队长菜单 `share_seeds`，people_interraction.cpp:2115 处理器注释 "The leader enable / disable seeds sharing" → 译"分享金钱"。
- uimwProgression `$P’S IDENTITY` 的 `$P` 为玩家名占位符（de.uxt:9039 `$P’S IDENTITÄT`、ru.uxt:9041 `ПАРАМЕТРЫ $p` 均保留占位符）→ 译"$P 的身份"。
- uittEarl：c1b 输入初版误作 "Left anklet"，en.uxt:8653 实为 `Left earring`（fr/de/es/ru 同证；会话中途输入文件已修正）→ 译"左耳环"；uittAnklel/uittAnkler（en.uxt:8677/8681）为真实 anklet 条目 → 左脚环/右脚环。
- uiWorkshop "ACTIONS & INVENTORY" 的 `&` 意译为"与"（动作与背包），本批唯一 `&` 计数偏差项，已在校验脚本 DEVIATIONS 白名单备案。

### c1b 实测：值内换行/标记保留

全 491 键自查（make_c1b.py 产译 + 独立复核脚本）：键集合与顺序一致；`@{` 色码 254 处、`$` 1 处（$P 占位符）、`%` 18 处、字面 \n 68 处、真实换行 68 处、真实制表 68 处（典型单元为 字面\n+真实换行+真实制表，同 c2/c3/c1a 型）、`&` 1 处（备案偏差）——除备案项外逐键计数一致；12 条值与原文相同（x、%、%、DEUTSCH、ENGLISH、FRANCAIS、ESPANOL、РУССКИЙ、HUD、16:9、4:3、PVP）均属规则保留集。

## 批次 2.8-r2（rem_en_r2 758 条：if*/mpcat*/mpfam* 原材料名族）定译

**构词模式**：物种拉丁名 + 材料中文，中西边界以空格连接（"Abhaya 木材""腐化 Yber 骨""新鲜 kitin 茧"）；Kitin→kitin（小写，沿用既有裁定）。"X Wood Node"→"X 木节"（区别于地标 Node→节点）。

**状态/加工词**：Fresh 新鲜 / Dry、Dried 干燥 / Damp 潮湿 / Rotting 腐烂 / Living 活体 / Dead 死亡 / Old 陈旧 / Blooming 盛开 / Redhot 炽热 / Refined 精炼 / Modified 改性 / Purificated 净化 / Corrupted 腐化 / Crystallized 晶化（沿用 c1b）/ Goo 胶质（沿用 c1a）/ Glue 黏胶 / Stellar 星辰 / Silvery 银色 / Golden 金色 / Loose Soil 松土 / Dry|Damp Wood Sawdust 干燥|潮湿木屑。

**部位/材料词**（新定，供同根沿用）：Skull 头骨 / Bone 骨 / Claw 爪 / Fang 獠牙 / Nail 趾甲 / Hoof 蹄 / Horn 角 / Tail 尾巴 / Wing 翅膀 / Skin 皮 / Leather 皮革 / Fur 毛皮 / Hair、Hairs 毛发 / Blood 血液 / Meat、Flesh 肉（不区分，备案）/ Beak 喙 / Rostrum 吻 / Spur 距 / Mandible 颚 / Jaw 颌 / Sting 毒刺 / Pincer 螯 / Sack 囊 / Carapace 甲壳 / Ligament 韧带 / Pelvis 骨盆 / Abdomen 腹部 / Spine 脊柱 / Trunk、Trunks 长鼻 / Crest 冠羽 / Head 头部 / Eye 眼睛 / Tongue 舌头 / Tooth 牙齿 / Parasite 寄生虫 / Larva 幼虫 / Egg 卵 / Cocoon 茧 / Saliva 唾液 / Secretion 分泌物 / Spider 蜘蛛 / Web 网 / Silk 丝 / Pollen 花粉 / Resin 树脂 / Sap 树液 / Wood 木材（沿用 c1a 地标）/ Bark 树皮 / Amber 琥珀 / Oil 油 / Fiber 纤维 / Seed 种子 / Leaf 叶（Green|Dead|Rotting Leaf 绿叶|枯叶|腐叶）/ Shell 甲壳 / Moss 苔藓 / Mushroom 蘑菇 / Cotton 棉 / Linen 亚麻 / Sponge 海绵 / Stem 茎 / Bud 花蕾 / Pistil 花蕊 / Berry 浆果 / Fruit 果实 / Honey 蜂蜜 / Wax 蜡 / Cereal 谷物 / Thorn 尖刺 / Reed 芦苇 / Straw 稻草 / Dust 尘土 / Pigment 颜料 / Fossil 化石 / Residue 残渣 / Splinter 碎片（Splinter Shell 碎屑甲壳）/ Bramble 荆棘 / Liana 藤蔓 / Lichen 地衣 / Strand 丝束（暂定）/ Gum 树胶 / Juice 汁液 / Acid 酸蚀（沿用 2.6 七系，作物品名待复核）/ Nodule 结节 / Part 部件 / Fish Scale 鱼鳞 / Firefly 萤火虫 / Dandelion 蒲公英 / Flower Petal 花瓣。

**甲壳虫族名译出**（英语描述性物种名，非拉丁专名）：Big 大型 / Bitters 苦味 / Champion 冠军 / Hero 英雄 / Horny 多角 / Insects 昆虫 / Smart 聪慧 / Sliders 滑行者 / Slamers 猛击者 / Whisperers 低语者 / Cuty、Cute 可爱（两物种合并译名，若为不同生物则撞车，待复核）+ 甲壳。

**订单/勋章/系统件**：Order Form 订购单 / Military Package 军用包裹 / Royal-Imperial-Theocratic-Federation Token 王室-帝国-神权-联邦令牌 / Merit Badge 功勋徽章 / Nano Builders 纳米建造器 / Sap Power Crystal 树液能量水晶（暂定）/ Crystallized Sap 晶化树液 / Atrium 中庭（暂定）/ System 系统 / Oath Bark 誓言树皮、Moon Resin 月亮树脂（普通名词性物种名译出，与 Silverweed/Tansy/Enola/Isabella 等留拉丁的分界待统一）/ Primitive Necklace 原始项链 / Jewelry 首饰（沿用 c1b）/ Taming-Training Tool 驯服-训练工具 / Living Seed 活体种子 / Melee weapon-Range weapon 近战-远程武器（沿用 2.6）/ Melee Warrior 近战战士 / Exotic 奇异（mpcat，暂定）/ Crafter 工匠（沿用批次 1）/ Upgrade 升级 / Undefined 未定义（沿用 2.6）/ Raw Material 原材料（沿用 2.5）/ Eucomina 留拉丁（纯专名，全片唯一与 en 逐字节同值键）。

**实测**：全 758 键自查（make_rem_zh_r2.py，token 引擎+未知词即错，337 不重复词全覆盖）：键集合与顺序一致；值内无任何标记（$ %@{}&<>、字面\n、换行/制表实测 en 为 0，逐键一致）；U+FFFD=0；非保留拉丁残留=0。报告 `.superpowers/sdd/2026-09-03-chinese-localization/task-b28-r2-report.md`。

## 批次 2 汇合裁定（分治词按多数派统一 · 最终定译，覆盖上文各分片记录中的冲突行）

合并 4 分片（c1a 490 / c1b 491 / c2 245 / c3 633 = 1859 键）时统计各分治词覆盖键数，**多数派胜出**；语境合理者保留并备案。改动清单（6 键，已落入 ingame_zh_all.json 与 translated/zh.uxt）：

| 词 | 裁定 | 票数 | 改动 |
|---|---|---|---|
| Shout | **喊话** | 喊话4 : 大喊1 | uiTalkCmdModeShout 大喊→喊话 |
| Parry | **格挡** | 格挡6 : 招架1 | uiToggleDodgeParry 招架→格挡 |
| Fame | **名望** | 名望4 : 声望3 | uiJoinClanProposalDesc / uiMk_interaction4 / uimwFame 声望→名望（c1b 记录行"Fame → 声望"作废） |
| Emote | **表情动作** | 表情动作10 : 表情0 | 全体一致，无改动 |
| allegiance | **效忠** | 效忠8 : 信仰2 | uiRingFilterReligionNeutral "无信仰的玩家"→"未效忠任何阵营的玩家" |

语境例外（保留不动）：uiRAP_CharReligionTooltip 的 en 源词为 **religion**（非 allegiance），"宗教信仰"属语境正确译法，不计入分治；uiBrowseRedoButton "Next→下一页" 沿用批次 1 已裁定的语境化分译。c2 的 Ring 会话浏览器 allegiance→信仰 记录由本裁定统一为效忠。


## 批次 2.5（客户端 C++/Lua 硬引用 474 条）定译

聊天命令帮助（cmd* / uiAddPartyChatCmd / uiRemovePartyChatCmd / uiInviteCmd / uiRandomBadParameter）：**完整成句翻译**；命令名与参数占位保留拉丁原样（/createGroup、group_name、destination、bag/player_room/guild/pet_animal1-4、'random'、<invite>、<add_to_party_chat>、<remove_party_chat>、ROOT 槽、"WRITE ME" 未写文占位）。
引擎/弹窗正式完整句：can_t_create_*、agp_trouble、uiDesktopNotIn32、uiUpdateDisplayDrivers* 系列（Ryzom 启动失败与显卡驱动弹窗）。
聊天引导词族（拼接前后缀）：says/shouts/tells you → 说/喊话/密语给你；You say/You shout/You tell/You tell %name → 你说/你喊话/你密语/你密语 %name（沿用批次2汇合裁定 Shout=喊话、tell=密语）。
单位定译：m→米、km→公里、bits→位、h/m/s（任务计时标签）→小时/分钟/秒、" h "/" m "/" s. "/" second(s) "/" meter(s)"→" 小时 "/" 分钟 "/" 秒。"/" 秒 "/" 米"；字节单位 B/KiB/MiB、纪元缩写 AC/JY、键名 CTRL/ALT/SHIFT、{AFK} 保留原样。
计量/武器术语：Sap Load→树液储量；Dodge/Parry Modifier→闪避/格挡修正；Adv. Dodge/Parry Modifier→对手闪避/格挡修正；Max. vs Slash/Smash/Pierce→对劈砍/砸击/穿刺最大吸收；Hit/Minute→命中/分钟；Magazine→弹匣容量；Reach→攻击距离；Command Range→指令距离；Max Packers→最大驮兽数；Action Cost/Credit→动作花费/动作点数；Kg→千克。
原材料（mp* / MP）：Raw Material Source/Target→原材料来源/目标；Item Parts→原材料部件；Can be used to Craft→可用于制造（Craft=制造沿用 c3；Forage 技能名→沙漠/森林/丛林/湖泊/原始根须采集）。
Ring（沿用 c2 场景）：ASK FOR INVITE→请求邀请；Mastered/Masterless→有主持/无主持（沿用 c2）；Entry point→进入点；场景取向：Hack'n'Slash→砍杀（暂定）、Story telling→叙事（暂定）、Mystery→悬疑、Guild/Newbie training→公会/新手训练；Connected (on the same/another) Mainland or Ring Scenario→在（同一/其他）主大陆或 Ring 场景中连接。
战斗飘字：Evade→规避（暂定，与 Dodge=闪避 区分）、Resist→抵抗。
botchat：SELL TO MERCHANT→出售给商人；Retire Price→回收价格；Resale Time Left→剩余转售时间；MAKE A PACT→缔结契约、BUILDING→建筑、GUILD ROLE MASTER→公会职业导师（沿用 c2/c3）。
称号（Title=称号沿用 c1b、Stanza=节沿用 c1b）：Stanzas/Skills Needed→所需节数/所需技能；Free to play account→免费游玩账号（暂定；与 Free Trial Account=免费试用账号区分）。
日期胶水词：uiTheSeasonIs→"现在是 "、uiAndTheWeatherIs→"，天气为 "（**备案偏差**：后者删前导空格，中文句子间拼接不需要；其余逐键首尾空格全保留）。uiDate/uiNowDate/uiApplyingDelta 等日期与补丁日志行按完整句。

### 批次 2.5 实测：标记与结构保留

全 474 键自查（make_cpp_zh.py + cpp_tr_p1..p5.py 程序化产译，规避 heredoc 折叠坑）：键集合一致；`@{` 931、`%` 486、`&` 38（=19 对 &CHK&/&SYS&/&BC&/&ISE&/&CHKCB& 频道前缀）、字面 `
` 318、真实 LF 318、真实 TAB 318 **逐键计数一致**（单元一一对应：每个字面 \n 后恰为 LF+TAB，每个 LF 前恰为字面 
）；`@{}` token 多重集逐键一致；无 `[ ]`、无行首 `#`；25 键值与 en 逐字节相同（纯色码标签 uiItem*Color、???、B/KiB/MiB、AC/JY、CTRL/ALT/SHIFT、{AFK}、", "、" - "、单空格、%f、%custom_text、%channel @{T8}/%shortcut、uihelpItemCosmetic/ScrollR2 纯 token 值）。具名 %token 由 strFindReplace **按名**替换（user_entity.cpp:3100 msgRollDiceLocal 实测），语序可安全调整；printf 序位占位（uiTipsTeleport 的 %s/%d 串）保持原序。uiBotChatPhrase 空值→空串。


### 批次 2.8-r3（剩余词条全量对齐 r3 片，758 键）新增定译

**原材料/生物族（mpfam787-819 / mpgroup / mpsapload）**：Corrupted→**腐化**（长尾族统一，兼对齐 uiMoreMFy CORRUPTER→腐化者）；queen（kitin 语境）→**蜂后**（la reine，批次 1"kitin 蜂群"延伸）；Lair→**巢穴**；Deposit→**矿藏**；Exotic（raw mats）→**异域**（Desert/Forest/Jungle/Lakes Exotic Raw Materials→X异域原材料，生态名沿用 c1a）；物种名保留拉丁：Koorin/Manath/Miakoda/Mitexi/Moojoo/Motega/Nita/Olathe/Omalita/Paddooa/Patee/Mooshy/Cray/Arma/Lumper/Mektoub/Moor；人名 Lixie/Sirgio/Pei 保留；Oath Wood→**誓言木**、Moon Linen→**月光亚麻**、Wood Knot→**树瘤**；Marauder(s)→**劫掠者**（与 c2 劫掠部落同族）；Token→**凭证**、Pack（组）→**驮包**（c3）、Meat→**肉**、Fur→**毛皮**、Blood→**血液**、Skull→**头骨**、Creature→**生物**、Aggressive Plant→**攻击性植物**、Mineral→**矿物**、Paper→**纸张**；树液储量档 Low/Medium/High/Very High→低/中/高/极高（与 uiConfigPoor/Medium/Super 对齐）。
**历法/地名族**：place_* 19 键全部**逐字节保留拉丁**（城市专名，Arena 亦作地名保留）；region_* 8 键译描述名：瞬息花园/困惑之林/异端陋室/隐秘之源/异见之丘/威严花园/**Matis 森林**（Matisian→Matis）/上部沼泽；uiContinent*：Abyss of Ichor→**灵液深渊**、Witherings→**枯萎之地**、Sicklands→**疫病之地**（uiMoreMMa 疫病者同族）、Fyros/Tryker Lands→X 之地、Living Islands→活岛、Sources→源泉、Forgotten Lands→遗忘之地；Silan→**Silan 保留**（Ruins of Silan→Silan 废墟）。
**部落名（uiFame_tribe_* 53）**：描述性名按语义直译（远古树妖/反 Kami 者/黑环/蟑螂/永恒之树社团/海盗/沙丘骑手/生态战士/纵火者/初代逃兵/Frahar 猎手/胶质脑袋/绿之种/死之种子的 Hamazan/圣像崇拜者/守护者/kitin 采集者/泻湖兄弟/不法之徒/胶质大师/Matis 边境守卫/转夜者/绿洲掘井者/火术士/回收者/变节者/守望者(Watchers)/根须采割者/神圣树液/树液拾取者/树液奴隶/焚烧者/暗影行者/杂草同胞/淤泥雕刻者/奴隶贩子/走私者/旱地 Matis/刀耕火种/训导师/破水者/编织缰绳/海滩拾荒者/吠叫者/暗化树液）；构词专名 6 个保留拉丁：Cholorogoos、Cuzans、Fraiders、Gibads、Leviers、Kuilde。Theist/Atheist→有神论者/无神论者；Hominist→**homin 至上者**；Tryton 保留。
**职业/人物族**：rpjob "Apprentice X"→**学徒X**（屠夫/花匠/挑水工/磁性制图师/工具匠/医师/幼虫采集者(Larvester)/卷轴匠）；攻击/增益/治疗施法者（ATTACK/BUFFER/HEALER CASTER）、近战/远程战士、采集者(Harvester)、商人(Merchant)——BUFFER CASTER→增益施法者（暂定）；range_warrior "Range Warrior"→**远程战士**（与 Ranger→游侠 按源词区分）；职阶头衔族 uiMore*：持剑者/浪荡剑客/Kami 之拳/腐化者/疫病者/惑心者/Kami 之怒/绯红猎手（Kamic→Kami 之）。
**下载器 uiBGD_*（49）**：Ryzom Downloader→**Ryzom 下载器**；Torrent Mode→Torrent 模式（BitTorrent、Torrent 保留拉丁）；package→数据包；{0} 格式占位逐键保留；" a {0}/s"→" 速度 {0}/秒"。
**配置 uiConfig*（75）**：bits→位（2.5）；AGP/EAX/FMod/OpenGL/Direct3D/FX/Hz/FPS/VRAM→Mb 数值保留；Renderer→渲染器；Poor/Medium/Normal/Super→低/中/普通/高（LOD 档沿用 2.6）；& 助记符 5 处逐键保留（&应用/&取消/&默认/&确定/&关于 Ryzom 配置...）；菜单尾 "..." 保留 ASCII 三点。
**经 de/es.uxt 官方译文消歧的暂定词**：uiFair=晴（**天气词**，de klar/es Despejado，非品质）；uiCap=上限（de GRENZE）；uiAcceptZCCharge=接受税责？（de Gebühr annehmen，沿用 c3 领地税责）；uiFinished=完成（de Abschließen 为按钮）；uiMasterFilter→大师筛选（暂定）；uiEnterCrZoneProposal→提交危险区域提案（de 证实 ENTER=提交义）。
**本批暂译待复核**：所受效果（Affected）、全部系列（All Sets）、应用区域（App Zone，de/es 亦未译）、臂甲（ARMPAD）、鞍垫（Milko PAD）、职阶（Grade/Echelon）、勘探（Prospection）、精炼（Refine）、增幅器（Amplifier）、筒仓（Silo）、归属旗帜（Claims Flag）、毁灭者（Destroyer）、掌控中（Under Control）、税责已就任/已当选（Charge applied/elected）、领地税责就任语境、工坊（Workshop，de Werkstatt 佐证）、幼虫采集者（Larvester）、异域（Exotic）、灵液（Ichor）、第 N 桌面（1st DESKTOP）、与…交谈（TALK TO，动态拼接风险）、主聊天沿用 c3、Ranger 后缀族、TODO : 前缀（802-814 法语长尾，保留 "TODO : " 字面，正文意译）。
**保留拉丁专名新增**：Moor、Kitins'→kitin 巢穴、Frahar、Hamazan、Kami/Karavan/Fyros/Matis/Tryker/Zoraï/Atys/Ring/Ryzom/Silan/Tryton/Lixie/Sirgio/Pei/BETA。Homins→homin（复数并入 homin 单形，批次 1 规则）。
**实测**：全 758 键（make_r3_zh.py 产译、check_r3.py 独立复核）：键集合与顺序一致；`@{XXXX}` 色码 15 键（@{6F6F}/@{FFFF}/@{C02F}）token 多重集逐键一致；`{0}` 10 键、%day/%month/%year、&（5 Qt 助记 + uiGuildInfoTitle 1 字面 &）、字面 `
`/真实 LF/真实 TAB **逐键计数一致**且单元同构（每个字面 \n 后恰为 LF+TAB）；数字序列逐键一致；首尾空白逐键一致（uiMFMailContent 修正为无尾空格，en 实值无尾随）；空串 6 键保空；单字母/专名/URL/纯 token 值 52 键逐字节保留；U+FFFD=0。

## 批次 2.8-r1（全量对齐收口·片 r1：758 条）新定译

**角色称号阶梯（character_title 族，前缀式）**：Novice X → 新手X；Apprentice X / X Apprentice → X学徒（尾随空格逐键保留）；Advanced X → 进阶X；Expert X → 专家X；Master X → 大师X；Master of X → X大师。词根沿用 c2 段位（新手/学徒/熟手/进阶/专家/大师），en 无 level 字样故不带"级"后缀。
**战斗称号词根**：Warrior → 武士（与 Fighter=战士 区分）；Fighter → 战士；Close Fighter → 近身斗士（暂定，与 Melee Fighter=近战战士 错峰）；Range Fighter → 远程战士；Hand to Hand Fighter → 徒手斗士；Ire Fighter → 狂战士（de 值即 Berserker，沿用批次 1 暂译）。武器使用者：弓手/重弓手/弩手/火枪手/步枪手/手枪射手/神枪手/炮手/重炮手/锤手/斧手/剑士/矛手/长矛手/短刃手（暂定）/蛮士（暂定）/轻·重武器手/劈砍手/砸击手/穿刺手/串刺手/钝击手/斩裂手（暂定）/剑客/持刃者/烈焰枪兵。拳跤：Boxing/Wrestling → 拳击/摔跤。
**制造职阶**：Armorer → 甲匠（重/轻/中甲匠）；Weaponsmith → 武器匠（近战/远程、轻/重）；Shieldsmith → 盾牌匠；Gunsmith → 枪械匠；Munitioner → 弹药匠；Jeweler → 珠宝匠；Forager → 采集者（与 Harvest→采集、Harvester→采集者 同词根，三词同译备案）；Crafter/Craftsman/Faber → 工匠（沿用批1）。
**魔法称号**：Attack/Buffer/Healer Caster → 进攻/增益/治疗施法者；Offensive/Defensive Magician → 进攻/防御法师；Mentalist → 心灵师；Mind Lord → 心灵主宰；Biomancer → 生物术士（暂定）；Warlock → 术士；Witherer → 枯萎者；Disturber → 扰乱者；Affliction Bringer → 降咒者（暂定）；Fouler → 污染者（暂定；fr=Contamineur、ru=Осквернитель，非"缩绒匠"）；Faker → 佯攻者（fr=Feinteur）；Life Stealer → 汲血者（沿用 2.5 汲血）；Cure/Curse/Sickness → 治愈/诅咒/疾病（Curse 与 Affliction=诅咒 同文，语境分治备案）；Sap → 树液（树液水晶/树液大师）；Wind Child → 风之子；Green/Scarlet/Shadow Hunter → 绿色/绯红/暗影猎人。
**fct_* NPC 职业后缀**（前导空格逐键保留，括号用全角）：Guard/Guard Chief/Intendant → 卫兵/卫兵队长/行政官；Welcomer → 迎宾员；Trainer → 培训师 与 Instructor → 教官 区分；Supplier/Messenger → 补给官/信使；Outlands → 荒野（暂定）；pact giver → 契约授予者（Pact=契约沿用 c3）；Kami Adept → Kami 信徒（暂定）；composition merchant → 配方商人（暂定，p* 复合键族）；Rookie Guard → 见习卫兵；foreman/Overseer → 监工；journeyman → 熟练工匠；prospector → 探矿者；patroller → 巡逻兵；stable boy/girl → 男/女马夫；barman/maid → 男/女酒保；Corporal/Sergeant/Captain → 下士/中士/队长（军阶暂定按西化三档，待实机复核）；Sage → 贤者；Scout → 斥候；Hawker → 行商；Steward → 管家；Cutthroat → 割喉者；tax collector → 收税官；Guild Clerk → 公会书记官；City/Village/Outpost/tribe welcomer → 城市/村庄/前哨站/部落迎宾员；Kitin threat watcher → Kitin 威胁监视者（Kitin 随原文大写、保留拉丁）。
**gn_class 守卫/佣兵阶级矩阵**（本批裁定）：Young/Senior/Veteran → 新锐/资深/老练；Regular/Strong/Powerful/Master/Elite → 普通/强健/强力/大师/精英；Warrior/Shooter/Magician/Healer → 武士/射手/法师/治疗师。**备案偏差**：gn_class 键名含军阶面名（conscript/private/corporal/sergent/captain/major/legionnaire…）但显示值是"经验+强度+职业"三元组，译文按值不按键（fr/de 同法）；"Veteran Strong Wrrior"、"Matis/Zoraï Voluteer" 源拼写错按语义正译（沿批次 2.7 惯例）。
**gn_bandit 匪帮名（136 条）**：全部创造性意译；人名/地名/生僻虚构生物保留拉丁（Tyler/Eva/Jena/Diller/Vinni/Cooky/Zora/Dyron/Frahar/Pyr/Thesos/Natae/Davae/Avalae/Highcliff/Nexus/Fount/Windy Gate/Cristabell/Stalia/Muse/Kovans/Mektoubs/Slathes/Lams/Jaks/Stavons/Ichor/Homin）。词根沿用：巨龙之眼（Great Dragon=巨龙）、树液哨卫/树液刮取者（Sap=树液）、原始根须亲王、胶质擒拿者/多情胶质滴（Goo=胶质）、自由游侠（Ranger=游侠）、劈砍手（Slashing=劈砍）、暗影强盗、割喉者、穿刺手、躲龙帮（泛称 Dragon→龙，与"巨龙"区分）。
**聊天前缀三件套**：Say/Shout/Whisper → 说话：/喊话：/低语：（汇合裁定 说话/喊话 沿用；Whisper=低语 与 tell=密语 区分；尾随空格逐键保留，冒号后空格随原文）。
**职员称号**：G/SG/GM/SGM → 向导/资深向导/游戏管理员/资深游戏管理员（CSR 官职，character_title.h BeginGmTitle 段实证）。FBT 键值 'Elder of Atys' → Atys 长老（与批2.7 uiEM_FBT 保留拉丁的键无关，此处译值）。
**其它新定译**：Chosen of Atys → Atys 天选者（暂定）；Celestial Guardian → 天界守护者；Avatar of Destruction/Sorrow → 毁灭/悲伤化身；Kamic Fist/Fury/Guardian → Kami 之拳/之怒/守护者；Imperial/Frontier/Local/Outlands Supplier → 帝国/边境/本地/荒野补给官；Warden → 监管官（暂定，de=Aufseher）；Escort/Comrade/Warmaster → 护卫/战友/战争大师；Green Seed → 绿种（暂定，fr=Graine Verte）；Leviers 保留拉丁；if 类目：Stanza→节（沿用 c1b）、Carrion→腐肉、Dead Seed→死种（暂定）、Crafting/Harvesting Tool→制造/采集工具；Sickness→疾病；PropertyNotFound→未找到属性（句号为译文正文）；TRAINING STATS/CHARACTERISTICS → 训练数值/训练属性；MAGIC ALTERATION SKILLS → 魔法变化技能（暂定）；Dune Caravaneer → 沙丘行商；Runner/Faker（Trader 支线）→ 跑者/佯攻者。
**实测**：全 758 键（make_rem_zh_r1.py 产译 + check_rem_r1.py 独立复核）：键集合与顺序一致；本片值域干净——`$ % & @{ 字面
 真实LF 真实TAB` 全批次总量为 0，逐键计数恒一致；219 键首尾空白逐键回填一致；空串 1 键（fct_civil）保空；恒等值 5 键（32 连字符分隔线 ___faber_skill_sep___、Homin、ifAI、Zora Kovans、fct_civil）；U+FFFD=0；fct_tb/tc_intendant 源键名与值地名列/反（tb 值 Crystabell、tc 值 Avendale），按值翻译并在产译脚本备案。


## 批次 2.8-r4（剩余词条全集 · 片4，755 键）新定译（暂译待汇合复核）

**沿用裁定**：名望/效忠/密语/喊话/格挡/闪避/场景/契约/职业导师/领地税责/达珀/前哨站/主大陆/服务器（Shard）/节（Stanza）/未定义/诅咒（Affliction）/七系元素（酸蚀 冰霜 腐蚀 火焰 毒素 闪电 冲击波）/提取/采集/转售/附魔/充能/树液储量/命中/分钟/弹匣容量/攻击距离/对劈砍·砸击·穿刺最大吸收/旗手—无/评分五维（可达性 难度 指引性 趣味性 原创性）/有主持·无主持/主持方式/新手训练·叙事·悬疑·公会训练·其他。

**新词族定译（本片新增）**：
- **魔法领域**：X Domain → X领域（沙漠领域/森林领域/丛林领域/湖泊领域/原始根须领域）；Elemental Magic→元素魔法、Affliction Magic→诅咒魔法。领域内咒法类型词（暂定）：Blind→致盲、Madness→疯狂、Sleep→催眠、Slow Move→缓行、Rooting→定身、Slow Attack→迟缓、Stun→眩晕、Fear→恐惧。
- **名望效忠 tooltip（uittFame*）**：magistrate→行政官（暂译）、priest→祭司（暂译）、bonze→僧侣（暂译）、sage→贤者（暂译）；stateless person→无国籍者、unbeliever→无信者、undetermined→待定（效忠语境）；swear allegiance→宣誓效忠、renounce→放弃效忠、enroll→招收。
- **Marauder/Ranger 组织族**：Organization→组织（暂译）、Organization Points→组织点数、Marauders→**劫掠者**（与 r3 及 c2 劫掠部落同根对齐；本片初稿"掠夺者"已废）、Ranger（组织）→游侠（与职业 Ranger 同译，同屏撞名待复核）。
- **RP 行业族**：Occupation→行业（与 Career=职业 分治，暂译）；基础/高级/角色扮演行业。
- **制造动作窗（phrase 编辑器）**：EFFECTS→效果、CREDITS→动作点数（2.5 沿用）、Add Credit→增加点数、Add Option→增加选项、Forget Action→遗忘动作、Remove Stanza→移除节、Success Rate→成功率、Spell Level→法术等级、Needed points/Total cost→所需点数/总花费、unshaded→不再灰显（暂译）、magic amplifier→魔法增幅器（暂译）、sap crystal→树液水晶（暂译）。
- **Sheath 族**：Sheath→**工具鞘**（暂译；Next/Previous Sheath→下一/上一工具鞘，uimMtSheath→工具鞘）。
- **PvP 状态**：Faction PvP→阵营 PvP、PvP Tagged→PvP 标记（c1b 沿用）、PvP Flagged→**PvP 挂旗**（暂译）、Not PvP Tagged→未被 PvP 标记。
- **聊天**：Whisper→低语（暂译）、Support Chat→客服聊天、NEW PARTY CHAT→新建群聊、NEW/REMOVE USER CHAT→新建/删除玩家聊天、/saveChannel 与 /name 命令词保留拉丁。
- **PvP 区域基地 tooltip（uiPvPEffect_region_*，78 键）**："Base of <区域名>"→"<区域名> 基地"，**Atys 地名一律保留拉丁**（Bounty Beaches/Nexus/Silan/Frahar/Umbra/Ichor/Loria/Oflovak/Muse 等；与 2.6 加载语专名保留、批1 正文 Fairhaven/New Lands 保留一致）。effect 句式"X提升/降低 @{2F2F}%p"；aggressivity of extractions→提取敌意（暂译）、thorny shield→荆棘之盾（暂译）、throwing weapons→投掷武器。
- **天气词**：Rainy→多雨、Snowy→多雪、Thundery→雷暴、Wind→大风、Sand storm→沙暴、Sap storm→树液风暴。
- **uiit_* 区域短标签 54 键**：逐字节保留拉丁小写 token（fr/de/es/ru 官方译文行为相同，实为专名键非漏翻）。
- **长尾/遗留键语境考证**：uiSelectPackage→选择安装包（client_install 工具 CClientInstallForm 引用实证）；uimTouchpad→触控板、uimCall→呼叫、uimItemTextDisplay→阅读、uimJournal→日志、uimFreezeJob/uimSwapJob→冻结职业/交换职业、uimwBuff→受效状态、uimwBGDownloader→补丁程序、uiScores→数值、uiPeople→人物、uiSeeding→保留"Seeding"（de/es/ru 官方均保留）、uiTechno→科技、uiSelPos→新手之地、uiProgressionTitle→我的成长、uiS2→黑与白之季、uiS2E0→第1集：Nexus 重见天日、uiInBag→收入背包/放出背包——**均未在现存 UI/代码中找到引用（遗留文本），语境内存疑待实机复核**。
- **welcome_phrase**（Matis 出生地 NPC 长对白，{break} 标记保留）：Mission Officers→任务军官（暂译）、Masters→导师（暂译）、Guards→卫兵、lift→升降梯。
- **Tryton 文档（uiTryton2..4）**：Mega Corp、E. Tryton 保留拉丁；"the New Beginning of Mankind"→人类的新开端（暂译）；uiMoreR* 游侠头衔：翠绿猎手/暗影猎手/Atys 守护者（暂译）。

**实测与备案偏差**：
- 全 755 键自查（make_r4_zh.py 产译 [字典 604+模板 97+保留 54]、check_r4.py 独立复核）：键集合与顺序一致；字面 `\n` 330/真实 LF 330/真实 TAB 330（单元一一对应：每个字面 \n 后恰为 LF+TAB，en/zh 双侧核验）、`@{` 829、色码 token 序列逐键多重集一致、`%` 157、`$` 0、`<name>`/`<party_chat>` 3 对、`{break}` 1——**逐键计数一致，0 偏差**；U+FFFD=0；逐字节保留 86 键（uiit* 54、等级段 6、种族名 4、Kami/Karavan 2、ZIG 标题 6、"00"/"???"/","/"NPC"/"Seeding"/"AppZone"/空串×8 等）。
- 备案偏差 2 项：`uiR2EDso_hack_slash` "&"→"与"（c1b 先例，白名单）；`uittInfoArmor{Blunt,Pierc,Slash}` 文内 ASCII 引号 "smashing"→全角引号"砸击"（c3 撇号消失先例延伸，白名单）。
- `uiRAP_WaitChars0..2` 尾随 ASCII "."/".."/"..." 为帧动画计数，**原样保留**（2.6 uiRAP_WaitMsg 同案）；`uiThousandsSeparator` "," 为程序化千分位值，逐字节保留。

## 批次 2.8 合并对账（4 片汇合 · 跨片一致性裁定 · 最终译值）

**合并基数**：r1 758 + r2 758 + r3 758 + r4 755 = **3029**；跨片键零重叠、zh/en 键集相等；键集 == pending diff ADD 块 label 集（6A9B6AD3，全等硬断言通过，diff 即剩余全集）。rem_zh_all.json 为唯一填充字典。

### 基准漂移备案（en 基准 vs diff/wk 原文）
- diff 块内嵌值为 **translated/wk.uxt**（原始工作文本，含法文残段与 sheet-id 占位），本批译文基准为 **translated/en.uxt**（上游策展英文明文）——两文件在 3029 键中漂移 **1039** 条（纯措辞 1019、空白 2、**结构标记计数差 18**）。
- 18 条逐一核查 + oracle 实证：en.uxt 为策展文本（wk 占位如 `gn_r_03_38_bandit`=r_03_38_bandit、`uittOrganization`="Organization tooltip"、`uiTextCommand2..3` 为法文长段而 en 已定空串）；**官方 de/fr/es 全部按 en 系文本翻译（ru 个别抄 wk 占位）**，zh 依 en 基准与上游主流一致。`welcome_phrase` 的 `<**`/`**>` 富文本标记 en 基准即无（zh 同步，`{break}` 保留）；`uittOutpostWar*` 数字差为 en"1 天"vs wk 法文"6666"（措辞性非标记）。
- 填充标记断言以 **zh vs en 基准**为准：3029 键 0 偏差（白名单外）；白名单 = 批次契约已批的 2 项（`uiR2EDso_hack_slash` &→与；`uittInfoArmor{Blunt,Pierc,Slash}` ASCII 引号→全角）。LF⇐`\n` 双侧约定 0 违规。

### 跨片族一致性裁定（最终值，已写入 rem_zh_all.json；补丁共 103 键）
| # | 族/键 | 冲突 | 裁定与依据 | 终值 |
|---|---|---|---|---|
| 1 | `uiPvPEffect_region_*`×76 + `gn_bandit_*`×6 + hovel×2 | r4 区域名保留拉丁 vs r3 region_*×8 直译 | **官方 de/fr/es/ru 4/4 在 Base-of 复合词中直译区域名**；r3 region_* 与 r3 uiContinentBagne 为批内先例；批1 规则"描述名直译、纯专名留拉丁"；按此统一，r1 bandit 名内区域引用同步对齐（Ichor/Windy Gate/Fount/Hovel×2 共 6 键改中文词根） | 见下表 39 名 |
| 2 | Cute/Cuty（mpfam284/307/31） | 两物种撞译"可爱" | 官方 3/3 将 Cute/Cuty 作**物种专名保留拉丁**（Cute-Schädel/Crâne de Cute/Concha de Cuty）；撞名即消解 | Cute 头骨 / Cute 毛发 / Cuty 甲壳 |
| 3 | Meat/Flesh（mpfam263-332 等 46 键） | 同译"肉" | 可接受（同义归并）；oracle：de 亦合并为 Fleisch（fr 区分 Viande/Chair，不取） | 均 肉（备案） |
| 4 | `uiMissionTimerDay` | r3 单字母逐字节保留 vs 2.5 家族已译 | **2.5 旧值 Hour/Minute/Second=小时/分钟/秒**（旧 zh.uxt 实证），族根一致压倒单字母保留规则 | 天 |
| 5 | `uiMK_Action_3` TALK TO | 与…交谈 拼接风险 | **全工作区零引用**（code/ryzom、client data、patchman、leveldesign game_element 全 grep 无 uiMK 消费点，整族为死键保险翻）——无运行时拼接点，风险为零；官方 de/fr/es 为前缀式（REDE MIT/Parler à/HABLAR CON），中文介宾结构不可前缀化 | 维持 与…交谈（若上游复活消费点再改） |
| 6 | Forager/Harvester→采集者 | 与 2.6"新手采集者" | 旧 zh.uxt 词根核对一致；r1 族内 31 键全 采集者 无例外；Forager=Harvester 系同职双标签（gn_class_forager/harvester/Forager en 异词同指），同文可接受 | 采集者（备案） |
| 7 | Curse/Affliction→诅咒 | 同文 | 旧 2.6/2.7 家族根 mpstat28-31、uihelpItemMagicBonus*Affliction、uittMagicResistTable"affliction（诅咒）"全为 诅咒；本批 Curse=诅咒 一致；Affliction_Bringer=降咒者 为构词派生 | 诅咒（确认） |
| 8 | kitin 大小写 | 16 键 kitin vs 源 Kitin | 批1 规则"kitin 保留拉丁、**随原文大小写**"——r2/r3 违例回改（mpfam77/309-312/310/695/716/774/797-801、mpgroup31/42、uiFame_tribe_kitin_gatheres） | Kitin |
| 9 | 组织 Ranger vs 职业 Ranger | 同译"游侠" | 官方 4/4 对 uiOrganization_7 保留"Ranger"（专名），**但批2.8 用户裁定"全部照翻，官方未译不构成豁免"（r1 匪帮名先例）**且 r3/r4 家族（uiWelcome_ranger、uittIdentityOrganization、fct_h_welcomer）已全译 游侠——批内多数派 + 裁定优先于 oracle；同词异指备案 | 游侠（备案，待实机） |
| 10 | Silan 废墟/遗迹 | r4 批内自撞 ×4:×1 | uiBuildingRuins=废墟 多数派 | 身处 Silan 废墟时… |
| 11 | Ichor | r1 留拉丁 vs r3 灵液 | 旧"汲血"实为 VAMPIRISM（r1 报告援引不成立）；r3 uiContinentBagne=灵液深渊 为批内唯一 Ichor 译根 | 灵液（深渊/杀手） |
| 12 | Fount→泉源 | 避开 uiContinentSources=源泉（r3） | 双词分治 | 泉源 |

**PvP 区域名终表**（slug→en→zh）：bountybeaches 丰饶海滩 · citiesofintuition 直觉之城 · dewdrops 露珠 · dunesofexil 流亡沙丘 · enchantedisle 魔法之岛 · fleetinggarden 瞬息花园* · forbidden_depths 禁忌深处 · frahartowers Frahar 之塔 · gate_of_obscurity 晦暗之门 · groveofconfusion 困惑之林* · groveofumbra 幽影之林 · havenofpurity 纯净庇护所 · hereticshovel 异端陋室* · hiddensource 隐秘之源* · imperialdunes 帝国沙丘 · knollofdissent 异见之丘* · knotofdementia 痴乱之结 · lagoonsofloria Loria 泻湖 · libertylake 自由湖 · maidengrove 处女之林 · majesticgarden 威严花园* · nexus Nexus（官方 4/4 留） · oflovaksoasis Oflovak 绿洲 · outlawcanyon 亡命峡谷 · restingwater 静水 · sawdustmines 木屑矿场 · the_abyss_of_ichor 灵液深渊* · the_elusive_forest 迷踪之林 · the_land_of_continuty 延续之地 · the_sunken_city 沉没之城 · the_trench_of_trials 试炼之堑 · the_under_spring 地下之泉 · the_windy_gate 狂风之门 · thefount 泉源 · thesavagedunes 蛮荒沙丘 · thescorchedcorridor 焦土走廊 · thevoid 虚空 · upperbog 上部沼泽* · windsofmuse Muse 之风（r1 保留先例）。*=r3 先例复用。uiit_* 54 键逐字节保留（官方 54/54 与 en 同值，程序关键词）。r1..r4 地名直译违例扫描（多词拉丁残留 43 种）：除本表外无违例，仅 Winch Gate Property Limited（版权公司名，留）。

### 合并/填充/merge 结果
- fill_rem_diff.py（全量版）：3029/3029 ADD 填充、**零删除、零重编号**、SWAP 3603 行原样保留、仅删尾标记 2 行；**merge 模拟终态 == translated/wk.uxt 标签序列（逐位一致）**——与历轮"剥 SWAP 尾部追加"不同，本批 zh.uxt 顺序自此对齐 wk 空间。
- AA_clean（12690 注释行扫描保留，0 删除——计数为扫描数）→ B_merge：日志无 not translated；merge 后 zh.uxt **6646** 条、标签唯一、LanguageName=简体中文、顺序==wk、**旧 3617 条 0 改动**、新 3029 条与 rem_zh_all.json 逐字节一致；其余 6 语言文件 0 变化（git 实证）；diff 归档 history/。
- **对齐审计：en.uxt 键集 − zh.uxt 键集 = ∅；zh − en = ∅**——uxt 域与 en 完全对齐，引用盲区闭合，**无残差清单**。
