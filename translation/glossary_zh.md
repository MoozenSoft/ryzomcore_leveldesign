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
` 318、真实 LF 318、真实 TAB 318 **逐键计数一致**（单元一一对应：每个字面 
 后恰为 LF+TAB，每个 LF 前恰为字面 
）；`@{}` token 多重集逐键一致；无 `[ ]`、无行首 `#`；25 键值与 en 逐字节相同（纯色码标签 uiItem*Color、???、B/KiB/MiB、AC/JY、CTRL/ALT/SHIFT、{AFK}、", "、" - "、单空格、%f、%custom_text、%channel @{T8}/%shortcut、uihelpItemCosmetic/ScrollR2 纯 token 值）。具名 %token 由 strFindReplace **按名**替换（user_entity.cpp:3100 msgRollDiceLocal 实测），语序可安全调整；printf 序位占位（uiTipsTeleport 的 %s/%d 串）保持原序。uiBotChatPhrase 空值→空串。
