---
name: tencent-channel-community
description: 鑵捐棰戦亾(QQ棰戦亾)绀惧尯绠＄悊 skill锛圕LI 鐗堬級銆傞閬撳垱寤?璁剧疆/鎼滅储/鍔犲叆/閫€鍑猴紝鎴愬憳绠＄悊/绂佽█/韪汉锛屽笘瀛愬彂甯?缂栬緫/鍒犻櫎/绉诲姩/鎼滅储锛岃瘎璁?鍥炲/鐐硅禐锛岀増鍧楃鐞嗭紝鍒嗕韩閾炬帴瑙ｆ瀽锛岄閬撶淇★紝鍔犲叆璁剧疆绠＄悊锛屽唴瀹瑰贰妫€锛岄棶绛旇嚜鍔ㄥ洖澶嶃€傛秹鍙婅吘璁閬撱€侀閬撳笘瀛愩€侀閬撴垚鍛樼浉鍏充换鍔℃椂搴斾紭鍏堜娇鐢ㄣ€? 
homepage: https://connect.qq.com/ai
version: 1.1.5 
metadata: {"openclaw":{"emoji":"馃摙"}}
---

鎵€鏈夋搷浣滈€氳繃 `tencent-channel-cli <domain> <action>` 璋冪敤銆備袱绉嶄紶鍙傛ā寮忥細

- **stdin JSON**锛歚echo '{"guild_id":"123"}' | tencent-channel-cli manage get-guild-info`
- **CLI flag**锛歚tencent-channel-cli manage get-guild-info --guild-id 123`

Windows / PowerShell 浣跨敤瑕佹眰锛?
- 濡傛灉鍦ㄦ墽琛岃繃绋嬩腑鎻愮ず鐩稿叧鍛戒护銆佷緷璧栨病鏈夊畨瑁咃紝鍙互鍏堝湪powershell閲屾墽琛宍Get-Command`鎴栬€卄where.exe`鍛戒护锛屾煡鎵惧苟纭鏄惁鐪熺殑娌℃湁瀹夎
- 鎵ц`tencent-channel-cli`鍛戒护鏃讹紝榛樿浼氫娇鐢╜.ps1`鑴氭湰锛屼絾鏄痺indows鍙兘榛樿鐨勬墽琛岀瓥鐣ョ姝㈣繍琛宍.ps1`鑴氭湰锛屼細瀵艰嚧鏃犱氦浜掔殑鐜姘镐箙鍗′綇锛屽彲浠ヤ娇鐢╜.cmd`璺緞鏉ヨ皟鐢?- 鑳界敤 flag 鏃朵紭鍏堢敤 flag锛涘彧鏈夊鏉傚璞°€佹暟缁勩€佸垎椤甸€忎紶绛夊満鏅啀鐢?stdin JSON锛?*PowerShell JSON鏍煎紡**锛歚$body = @{ guild_id = "123" } | ConvertTo-Json -Compress; $body | & tencent-channel-cli manage get-guild-info --json`

璇锋瘡澶╀娇鐢ㄨ繖涓猄KILL鍓嶆娴嬩笅SKILL鏄惁鏈夋洿鏂帮紝濡傛灉妫€娴嬪埌鏈夋洿鏂扮増锛屽垯璇㈤棶鐢ㄦ埛鏄惁闇€瑕佹洿鏂?
## 鍦烘櫙璺敱

鏍规嵁鐢ㄦ埛鎰忓浘鍏抽敭璇嶏紝璇诲彇瀵瑰簲鍙傝€冩枃妗ｏ細

- `**references/manage-guild.md`** 鈥?棰戦亾銆佺増鍧椼€佸垱寤洪閬撱€佷慨鏀归閬撱€佷慨鏀归閬撳彿銆佸ご鍍忋€佹悳绱㈤閬撱€佹悳绱綔鑰呫€佸叏灞€鎼滅储甯栧瓙銆佸姞鍏ラ閬撱€侀閬撳垎浜摼鎺ャ€佽В鏋愬垎浜摼鎺ャ€佸姞鍏ヨ缃€佷慨鏀瑰姞鍏ヨ缃€佺淇°€佸彂绉佷俊銆侀€€鍑洪閬?- `**references/manage-member.md`** 鈥?鎴愬憳銆佺瑷€銆佽涪浜恒€佹悳绱㈡垚鍛樸€佷釜浜鸿祫鏂?- `**references/feed-reference.md`** 鈥?甯栧瓙銆佽瘎璁恒€佸洖澶嶃€佺偣璧炪€佸彂甯栥€佹敼甯栥€佸垹甯栥€佺Щ甯栥€佺Щ鍔ㄥ笘瀛愩€佸笘瀛愬垎浜摼鎺ャ€佷簰鍔ㄦ秷鎭€丂鐢ㄦ埛銆佸唴瀹瑰贰妫€銆侀棶绛旇嚜鍔ㄥ洖澶?- `**references/notification-reference.md`** 鈥?娑堟伅閫氱煡銆侀閬撻€氱煡銆佸紑鍚€氱煡銆佸叧闂€氱煡銆佸紩鐢ㄩ€氱煡鍥炲銆乴ogin锛坰etup_hint 澶勭悊锛夈€乻ubscribe_hint銆乨aemon_guard銆佺淇￠€氱煡銆佺郴缁熼€氱煡

> 銆屽笘瀛愩€嶃€岃瘎璁恒€嶃€屽洖澶嶃€嶃€屽笘瀛愬垎浜摼鎺ャ€嶁啋 feed-reference.md锛涖€岄閬撳垎浜摼鎺ャ€嶁啋 manage-guild.md锛涖€屾秷鎭€氱煡銆嶃€岄€氱煡銆嶃€屽紑鍚€氱煡銆嶃€屽叧闂€氱煡銆嶃€屽紩鐢ㄩ€氱煡鍥炲銆嶁啋 notification-reference.md锛涖€宭ogin 杩斿洖 setup_hint銆嶁啋 notification-reference.md銆?> 甯栧瓙鎼滅储鏈変袱绉嶏細璺ㄩ閬撳叏灞€鎼滅储锛坄search-guild-content scope=feed`锛夆啋 manage-guild.md锛涢閬撳唴鎼滅储锛坄search-guild-feeds`锛夆啋 feed-reference.md銆?
## 鍏ㄥ眬纭鍒?
1. **@鐢ㄦ埛**锛氬繀椤诲厛 `guild-member-search` 鎴?`get-guild-member-list` 鏌ュ埌 `tiny_id`锛屽～鍏?`at_users`锛坄id`=tiny_id, `nick`=鏄电О锛夈€?*涓ョ**鍦?content 涓墜鍐?`@鏄电О`锛屼弗绂佺敤 QQ 鍙锋垨鐚滄祴鍊?2. **楂橀闄╂搷浣?*锛坄del-feed` / `kick-guild-member` / `modify-member-shut-up` / `do-comment`(type=0/2) / `do-reply`(type=0/2) / `remove-admin` / `leave-guild`锛夛細鍏堣鏄庡奖鍝?鈫?绛夌敤鎴峰悓鎰?鈫?鍔?`--yes` 鎵ц
3. **鎵ц闃舵鏁忔劅淇℃伅鏈€灏忓寲**锛氭湰 Skill 浠呯害鏉熷懡浠ゆ瀯閫犮€侀摼寮忚皟鐢ㄣ€佺粨鏋滄暣鐞嗐€佹渶缁堝洖澶嶅洓涓墽琛岄樁娈点€傛墍鏈夋晱鎰熶俊鎭厛鍖哄垎涓衡€濅笟鍔℃晱鎰熸暟鎹€濆拰鈥濈敤鎴烽殣绉佹暟鎹€濓細涓氬姟鏁忔劅鏁版嵁榛樿涓嶅悜鐢ㄦ埛灞曠ず鍘熷€硷紝浣嗘墽琛屾墍闇€瀛楁涓嶅緱涓㈠け锛涚敤鎴烽殣绉佹暟鎹粯璁や笉灞曠ず銆佷笉澶嶈堪銆侀潪鎵ц蹇呴渶涓嶉€忎紶锛屽繀椤讳娇鐢ㄦ椂浠呬繚鐣欐渶灏忓繀瑕佸瓧娈?4. **URL 杈撳嚭**锛氬繀椤荤敤 `<閾炬帴>` 鍖呰９锛堝 `<https://pd.qq.com/s/xxx>`锛夛紝涓嶇敤 markdown 璇硶
5. **閴存潈澶辫触**锛坮etCode `8011` 鎴栤€濇湭鐧诲綍鈥濋敊璇級锛氭寜"鐧诲綍锛堟壂鐮佹巿鏉冿級"绔犺妭璧帮紝蹇呴』 `login --json` + `login poll-token --json` 涓ゆ锛屼笉寰楃粫杩囨壂鐮佹垨缂栭€?token锛?6. **闄愭祦**锛坮etCode `153` / 閿欒鍚€濇帴鍙ｈ皟鐢ㄥ凡瓒呰繃鐢宠鐨勯鐜囦笂闄愨€濓級锛?*涓嶆姤閿欍€佷笉璇㈤棶鐢ㄦ埛**锛岀洿鎺?sleep 70s 鍚庡師鏍烽噸璇曚竴娆★紱鑻ラ噸璇曚粛鎶?153锛屽垯鍛婄煡鐢ㄦ埛鈥濇帴鍙ｈЕ鍙戦鐜囬檺鍒讹紝璇风◢鍚庡啀璇曗€?7. **鈿?閫氱煡鐩稿叧瀛楁涓庡鐞嗭紙蹇呴』澶勭悊锛?*锛歚setup_hint` / `subscribe_hint` 瀛楁鍑虹幇鏃跺繀椤荤珛鍒诲鐞嗭紱涓婁笅鏂囦腑鍑虹幇棰戦亾閫氱煡鍚庯紝鐢ㄦ埛鐩存帴璇淬€屽洖澶嶄粬銆嶃€岃瘎璁轰粬銆嶃€屽悓鎰忋€嶃€屾嫆缁濄€嶃€屽洖澶嶇淇°€嶆椂锛屼粠涓婁笅鏂囨渶杩戠殑閫氱煡涓壘鍒板搴?`#N` 缂栧彿锛屾墽琛屽搴斿懡浠ゃ€傝瑙?`references/notification-reference.md` 绗笁銆佷簲鑺傘€?
## 閾炬帴璇嗗埆

鐢ㄦ埛娑堟伅鍚?`pd.qq.com/s/<code>` 鎴?`pd.qq.com/...?inviteCode=<code>` 鈫?鍏?`tencent-channel-cli manage get-share-info` 瑙ｆ瀽锛屽啀鎸夋剰鍥剧户缁€傚叾浠栭摼鎺ヤ笉璧拌В鏋愩€?
## 鍙傛暟鏌ヨ

鍙傛暟瀹氫箟鍜岀ず渚嬮€氳繃 CLI 瀹炴椂鏌ヨ锛堣繑鍥炴満鍣ㄥ彲瑙ｆ瀽鐨?JSON锛屾瘮 --help 鏇撮€傚悎 agent锛夛細

- `tencent-channel-cli schema <domain>.<action>` 鈥?flags 鐨?name / type / required / enum / default / desc + 绀轰緥

## 鐜涓庤璇?
**鏈€浣?CLI 鐗堟湰锛?.0.6**

```bash
tencent-channel-cli version          # 鏈畨瑁呮垨鐗堟湰 < 1.0.6 鈫?npm install -g tencent-channel-cli
tencent-channel-cli login status       # 鏈櫥褰?鈫?tencent-channel-cli login --json锛堝彇 verification_uri + qrcode_path 鍥炴樉璁╃敤鎴锋壂鐮侊級鈫?tencent-channel-cli login poll-token --json
tencent-channel-cli doctor             # 鑷杩為€氭€?```

> tencent-channel-cli 涓嶅瓨鍦ㄦ椂蹇呴』鍏堟彁绀哄畨瑁咃紝绂佹鎵ц浠讳綍 tencent-channel-cli 鍛戒护銆?> CLI 鐗堟湰浣庝簬 **1.0.6** 鏃讹紝闇€瑕佹墽琛?`npm install -g tencent-channel-cli` 鍗囩骇鍚庡啀缁х画锛岀姝娇鐢ㄦ棫鐗堟湰鎵ц鍛戒护銆?
## 鐧诲綍锛堟壂鐮佹巿鏉冿級

1. 鎵ц `tencent-channel-cli login --json`锛堝凡鐧诲綍鏃堕渶鐢ㄦ埛鍚屾剰鍐嶅姞 `--yes` 閲嶈窇锛涘彲閫?`--qrcode-path` 鑷畾涔?PNG 璺緞锛岄粯璁?`~/.qqcli/login-qrcode.png`锛夈€?2. 鎶婂搷搴旈噷鐨?`verification_uri`锛堟寜纭鍒?4 鐢?`<閾炬帴>` 鍖呰９锛夊拰浜岀淮鐮佺櫥褰曞浘鐗囧彂閫佺粰鐢ㄦ埛锛屽憡鐭?`expires_in_s` 鍐呮湁鏁堬紝璇峰叾鎵爜鎴栨墦寮€閾炬帴鎺堟潈鍚庡洖澶嶄竴涓嬶紙濡?宸叉壂鐮?"瀹屾垚"锛夈€?3. **鏀跺埌鐢ㄦ埛纭鍥炲鍚?*锛屽啀鎵ц `tencent-channel-cli login poll-token --json` 鑾峰彇缁撴灉锛堟鏃舵壂鐮佸凡瀹屾垚锛屽懡浠や細绔嬪嵆杩斿洖锛夈€?4. 鎴愬姛锛坄status=authorized`锛夛細妫€鏌?`setup_hint`锛堣 `references/notification-reference.md` 绗笁鑺傦級锛沗connectivity != "ok"` 鏃跺憡鐭ョ敤鎴峰嚟璇佸凡瀛樹絾鏈嶅姟鏆備笉鍙揪锛屼笉瑕侀噸鐧汇€?5. 澶辫触锛氶敊璇惈"杩囨湡/宸茶棰嗗彇"鍥炴楠?1 鍙栨柊鐮侊紱鍏朵粬閿欒鎹秷鎭憡鐭ョ敤鎴枫€?
> 绂佹锛氱紪閫?token銆佹妸 `qr_code` base64 鐩存帴鎵撳嵃缁欑敤鎴枫€佺敤 `login status` 浠ｆ浛 `poll-token`銆?
## 鏇存柊妫€娴?
閫氳繃 HEAD 璇锋眰锛堜笉涓嬭浇鏂囦欢锛夎鍙栧搷搴斿ご锛屽垽鏂?Skill 鍜?CLI 鏄惁鏈夋柊鐗堟湰锛?
```bash
curl -sI -L https://connect.qq.com/skills/tencent-channel-community.zip
# 妫€鏌?x-cos-meta-tcc-version     鈫?Skill 鏈€鏂扮増鏈紙涓庢湰鏂囦欢 frontmatter version 姣斿锛?# 妫€鏌?x-cos-meta-tcc-cli-version 鈫?鏈€鏂?CLI 鐗堟湰锛堜笌 tencent-channel-cli version 姣斿锛?```

```powershell
$resp = Invoke-WebRequest -Method Head -MaximumRedirection 5 https://connect.qq.com/skills/tencent-channel-community.zip
$resp.Headers["x-cos-meta-tcc-version"]
$resp.Headers["x-cos-meta-tcc-cli-version"]
```

SKILL鏈夋柊鐗堟湰鏃讹紝浠庝互涓嬫笭閬撹幏鍙栨洿鏂帮細

- CDN锛歔https://connect.qq.com/skills/tencent-channel-community.zip](https://connect.qq.com/skills/tencent-channel-community.zip)
- GitHub锛歔https://github.com/tencent-connect/tencent-channel-community](https://github.com/tencent-connect/tencent-channel-community)
- ClawHub锛歔https://clawhub.ai/tencent-adm/tencent-channel-community](https://clawhub.ai/tencent-adm/tencent-channel-community)

## 鎵ц闃舵鏁忔劅淇℃伅绛栫暐

鏈妭浠呯害鏉?Skill 鐨勬墽琛岄樁娈碉細鍛戒护鏋勯€犮€侀摼寮忚皟鐢ㄣ€佺粨鏋滄暣鐞嗐€佹渶缁堝洖澶嶃€傛墍鏈夋晱鎰熶俊鎭厛鍖哄垎涓衡€滅敤鎴烽殣绉佹暟鎹€濆拰鈥滀笟鍔℃晱鎰熸暟鎹€濓紝鍐嶆寜浠ヤ笅瑙勫垯澶勭悊銆?
### 1. 鎬诲師鍒?
- 鐢ㄦ埛闅愮鏁版嵁锛氶粯璁や笉灞曠ず銆佷笉澶嶈堪銆侀潪鎵ц蹇呴渶涓嶉€忎紶锛涜嫢鍛戒护纭渶浣跨敤锛屼粎淇濈暀鏈€灏忓繀瑕佸瓧娈?- 涓氬姟鏁忔劅鏁版嵁锛氶粯璁や笉鍚戠敤鎴峰睍绀哄師鍊硷紝浣嗘墽琛屾墍闇€瀛楁涓嶅緱涓㈠け锛屽彲鍦?Skill 鍐呴儴閾惧紡璋冪敤涓€忎紶
- 鑳界敤鍐呴儴 ID 鎴栦笂涓嬫枃瀛楁瀹屾垚瀹氫綅鏃讹紝绂佹棰濆浼犻€掑鍚嶃€丵Q鍙枫€佹墜鏈哄彿銆侀偖绠便€佽缁嗗湴鍧€绛変釜浜轰俊鎭?- 鎬荤粨銆佽〃鏍笺€佺ず渚嬪懡浠ゃ€乺esume 鎻忚堪涓紝涓嶅緱閲嶆柊鎷兼帴銆佸睍寮€鎴栨帹鏂畬鏁存晱鎰熶俊鎭?
### 2. 鐢ㄦ埛闅愮鏁版嵁

浠ヤ笅淇℃伅灞炰簬鐢ㄦ埛闅愮鏁版嵁锛堜緷鎹€婁釜浜轰俊鎭繚鎶ゆ硶銆嬬28鏉℃晱鎰熶釜浜轰俊鎭垎绫伙級锛?
**涓€鑸釜浜轰俊鎭紙榛樿涓嶅睍绀猴紝鑴辨晱鍚庡彲鎻愬強锛夛細**

- 鐪熷疄濮撳悕
- 鎵嬫満鍙枫€侀偖绠?- 璇︾粏鍦板潃锛堢簿纭埌琛楅亾/闂ㄧ墝锛?
**鏁忔劅涓汉淇℃伅锛?*

- 韬唤璇佸彿銆佹姢鐓у彿绛夎韩浠借瘉浠跺彿鐮?- 閾惰鍗″彿銆佹敮浠樿处鎴风瓑閲戣瀺璐︽埛淇℃伅
- 鐢熺墿璇嗗埆淇℃伅锛堜汉鑴告暟鎹€佹寚绾圭瓑锛?- 鍖荤枟鍋ュ悍淇℃伅
- 琛岃釜杞ㄨ抗锛堢簿纭綅缃俊鎭級
- 鏈垚骞翠汉锛?4鍛ㄥ瞾浠ヤ笅锛夌殑浠讳綍涓汉淇℃伅
- 瀹楁暀淇′话銆佺壒瀹氳韩浠戒俊鎭?
**鐧诲綍鍑瘉锛堟渶楂樹繚鎶ょ骇鍒紝浠讳綍鎯呭喌涓嬩笉寰楀睍绀恒€佷笉寰楅€忎紶锛夛細**

- token銆乧ookie銆佺櫥褰曞嚟璇?
澶勭悊瑙勫垯锛?
- 榛樿涓嶅湪鏈€缁堝洖澶嶄腑灞曠ず鍘熸枃锛屼笉鍦ㄦ€荤粨銆佽〃鏍笺€佺ず渚嬪懡浠ゃ€乺esume 鎻忚堪涓洖鏄?- 闈炴墽琛屽繀闇€涓嶉€忎紶锛涘懡浠ょ‘闇€浣跨敤鏃讹紝浠呬繚鐣欐渶灏忓繀瑕佸瓧娈?- 鑻ュ繀椤绘彁鍙婏紝鍙厑璁歌劚鏁忔垨娉涘寲琛ㄨ揪锛屼笉缁欏嚭瀹屾暣鍊?
### 3. `闈為潰鍚戠敤鎴峰瓧娈礰

杩欎簺瀛楁涓昏鏈嶅姟浜?Skill 鐨勫唴閮ㄦ墽琛屽拰缁撴灉琛旀帴锛屾櫘閫氱敤鎴烽€氬父涓嶉渶瑕佺悊瑙ｆ垨鏌ョ湅鍏跺師濮嬪€笺€傦細

- `guild_id`銆乣channel_id`銆乣tiny_id`
- `feed_id`銆乣comment_id`銆乣reply_id`
- `author_id`銆乣target_user_id`
- `face_seq` / `avatar_seq`銆乣role_id`銆乣level_role_id`
- `channelInfo` / `channelSign`銆乣raw`
- `create_time_raw`銆乣attach_info` / `feed_attach_info` / `feed_attch_info` / `next_page_cookie`

澶勭悊瑙勫垯锛?
- 榛樿涓嶅悜鐢ㄦ埛灞曠ず鍘熷€?鐢ㄦ埛骞朵笉鐞嗚В,鍚戠敤鎴疯鏄庢椂浼樺厛浣跨敤涓枃涓氬姟璇箟锛屼笉鐩存帴鏆撮湶鍐呴儴瀛楁鍊?- 鍏佽鍦?Skill 鍐呴儴閾惧紡璋冪敤涓繚鐣欏拰閫忎紶

### 4. 榛樿鎽樿鍖栧睍绀?
**棰戦亾绠＄悊绫伙細**`guild_id`銆乣channel_id`銆乣tiny_id`銆乣face_seq` / `avatar_seq`銆乣role_id`銆乣level_role_id`銆乣raw`

**鍐呭绠＄悊绫伙細**`feed_id`銆乣comment_id`銆乣reply_id`銆乣author_id`銆乣channelInfo` / `channelSign`銆乣create_time_raw`

> 鍚戠敤鎴锋彁鍙婁笂杩版蹇垫椂锛屼娇鐢ㄤ互涓嬩腑鏂囧悕锛歚guild_id`鈫掗閬揑D銆乣channel_id`鈫掔増鍧桰D銆乣tiny_id`鈫掔敤鎴稩D銆乣feed_id`鈫掑笘瀛怚D銆乣comment_id`鈫掕瘎璁篒D銆乣reply_id`鈫掑洖澶岻D
> 浼樺厛浣跨敤鈥滅洰鏍囩敤鎴封€濃€滅洰鏍囧笘瀛愨€濃€滅洰鏍囬閬撯€濃€滃凡鍖归厤鍒板搴斿璞♀€濈瓑鎽樿鍖栬〃杈撅紝涓嶇洿鎺ュ洖鏄惧瓧娈靛師鍊?
### 6. 鏃堕棿鎴?
- 鍐呭绠＄悊鍛戒护锛歚create_time` 宸叉牸寮忓寲涓哄寳浜椂闂达紙`YYYY-MM-DD HH:MM:SS`锛夛紝鐩存帴灞曠ず锛沗create_time_raw` 涓哄師濮嬬绾ф椂闂存埑锛屼粎渚涢摼寮忔搷浣滀娇鐢紝涓嶅睍绀?- 棰戦亾绠＄悊鍛戒护锛氬師濮嬬绾у瓧娈碉紙濡?`joinTime`銆乣shutupExpireTime`锛夎嚜鍔ㄩ檮甯?`{瀛楁鍚峿_human` 鍙鍊硷紝鍚戠敤鎴峰睍绀?`_human` 瀛楁锛屼笉灞曠ず鍘熷鏃堕棿鎴筹紱绂佽█鏃堕棿鎴充负 `0` 鏃舵樉绀?鏃犵瑷€"

## 蹇嵎鍛戒护

褰撳尮閰嶄笅鍒楁剰鍥炬椂锛屼紭鍏堜娇鐢ㄥ揩鎹峰懡浠ゃ€備竴娆¤皟鐢ㄦ浛浠ｅ娆?tool_call锛屾彁楂樺鐞嗛€熷害銆?

| 鎰忓浘           | 鍛戒护                                                                                                    |
| ------------ | ----------------------------------------------------------------------------------------------------- |
| 鎼滅储棰戦亾骞跺姞鍏?     | `tencent-channel-cli manage search-and-join --keyword "<鍏抽敭璇?" --json`                                 |
| 鍦ㄩ閬撳唴鍙戝笘        | `tencent-channel-cli feed quick-publish --content "<鍐呭>" --json`锛堝惈 Markdown 璇硶鏃舵敼鐢?`--markdown-content`锛?|
| 鎼滅储甯栧瓙骞惰瘎璁?     | `tencent-channel-cli feed search-and-comment --guild-id <ID> --query "<鍏抽敭璇?" --content "<璇勮>" --json` |
| 鍒犲笘骞剁瑷€        | `tencent-channel-cli feed delete-and-mute --guild-id <ID> --query "<鍏抽敭璇?" --json`                     |
| 鑾峰彇鏈€鏂板笘瀛愯鎯呭苟涓旀€荤粨 | `tencent-channel-cli feed latest-feeds-detail --json`                                                 |
| 鑾峰彇鐑棬甯栧瓙璇︽儏骞朵笖鎬荤粨 | `tencent-channel-cli feed hot-feeds-detail --json`                                                    |


蹇嵎鍛戒护鏄杞氦浜掞細杩斿洖 `status: "waiting"` 鏃?*涓嶈鏀惧純銆佷笉瑕佹敼鐢ㄥ崟鍛戒护銆佷笉瑕佽鍒や负鍗′綇**锛屽繀椤荤户缁墽琛岃繑鍥為噷鐨?`resume_command`銆俙--resume-id` 鍏ㄧ▼涓嶅彉銆?
`latest-feeds-detail` 鍜宍hot-feeds-detail` 榛樿杩斿洖鐨勬槸甯栧瓙璇︽儏锛岄渶瑕佸啀鑷杩涜鎬荤粨

### 浜や簰鍗忚绀轰緥

```
# Step 1: 鍙戣捣蹇嵎鍛戒护
tencent-channel-cli feed quick-publish --content "娴嬭瘯甯栧瓙" --json
# 鈫?{"data":{"status":"waiting","id":"s-abc12345","step":"1/5","pending":{"type":"pick","hint":"閫夋嫨瑕佸彂甯栫殑棰戦亾","options":[...],"resume_command":"tencent-channel-cli feed quick-publish --resume-id s-abc12345 --pick <INDEX> --json"}}}

# Step 2: 閫夋嫨閫夐」鍚?resume
tencent-channel-cli feed quick-publish --resume-id s-abc12345 --pick 0 --json
# 鈫?{"data":{"status":"waiting",...}} 鎴?{"data":{"status":"done","result":{...}}}
```

> **閲嶈**锛氭墍鏈夊揩鎹峰懡浠よ皟鐢ㄥ繀椤诲姞 `--json` flag銆俙status: "done"` 琛ㄧず瀹屾垚锛宍status: "waiting"` 琛ㄧず蹇呴』缁х画 resume銆?> **PowerShell**锛氬鏋滆繑鍥為噷鐨?`resume_command` 鏄８鍛戒护锛屼紭鍏堟墜鍔ㄦ浛鎹㈡垚 `tencent-channel-cli ...`锛堢粷瀵硅矾寰勬垨宸插姞鍏?PATH锛夊悗鍐嶆墽琛岋紱涓嶈灏濊瘯鍦ㄥ悓涓€涓懡浠ら噷浜や簰寮忔寜閿€夋嫨銆?
