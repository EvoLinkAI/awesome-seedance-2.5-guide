<div align="center">

<a href="https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=banner&utm_campaign=awesome-seedance-2.5-guide"><img src="assets/banner.png" alt="Seedance 2.5 Early Access guide" width="100%"></a>

# Seedance 2.5 官方 Guide

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)
[![Get Seedance 2.5 Early Access](https://img.shields.io/badge/Get_Seedance_2.5-Early_Access-black)](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=badge&utm_campaign=awesome-seedance-2.5-guide)
[![Official Guide](https://img.shields.io/badge/Official_Guide-36_Media_Assets-7C3AED)](data/seedance-2-5-manifest.json)
[![API Key](https://img.shields.io/badge/API_Key-EvoLink-orange)](https://evolink.ai/signup?utm_source=github&utm_medium=badge&utm_campaign=awesome-seedance-2.5-guide)

[English](README.md) · [Español](README.es.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Türkçe](README.tr.md) · [简体中文](README.zh-CN.md) · **繁體中文** · [Русский](README.ru.md)

</div>

## 🍌 介紹

Seedance 2.5 early access 已透過 EvoLink 開放。本倉庫把官方 Seedance 2.5 發布素材整理成適合 GitHub 閱讀與複用的 guide，面向創作者、開發者和 AI 影片團隊。

本 guide 覆蓋 36 個官方素材，包含首屏 demo、官方作品展示、敘事控制、多語種表達和可控編輯。因為全部都是官方案例，所以單個 case 不寫作者或來源行。

[Get Seedance 2.5 Early Access](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide) · [取得 API Key](https://evolink.ai/signup?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide) · [目前 Seedance API 範例](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)

> [!NOTE]
> 目前可執行的 API 程式碼仍使用穩定的 Seedance 2 API path；Seedance 2.5 early access 正在 rollout。不要把已驗證的 `seedance-2.0-*` model id 替換成未驗證的 2.5 model id。

## 📑 目錄

- 介紹
- 快速開始
- 原 Seedance 2 Guide
- Seedance 2.5 官方 Guide
- 倉庫結構
- 致謝

## 🚀 快速開始

你可以用這個倉庫查看 2.5 官方案例、複製 prompt 結構，並進入 Seedance 2.5 early access。

> [!NOTE]
> 這裡的 Quick Start 有意保留目前已驗證的 `seedance-2.0-text-to-video` model id 和目前 Seedance 2 API path。Seedance 2.5 API access 正透過 early access rollout；暫時不要把可執行的 2.0 model id 替換成未驗證的 2.5 model id。

```bash
export EVOLINK_API_KEY="your_key_here"

curl --request POST \
  --url https://api.evolink.ai/v1/videos/generations \
  --header "Authorization: Bearer ${EVOLINK_API_KEY}" \
  --header 'Content-Type: application/json' \
  --data '{
    "model": "seedance-2.0-text-to-video",
    "prompt": "A cinematic product reveal, slow dolly-in, reflective glass table, premium commercial lighting",
    "duration": 5,
    "quality": "720p",
    "aspect_ratio": "16:9",
    "generate_audio": true
  }'
```

## 🧭 原 Seedance 2 Guide

新的 Seedance 2.5 官方 guide 已放在最前面。完整的原 Seedance 2 guide 已作為 legacy 跳轉入口保留，涵蓋目前 API path、用例寫法、prompt 模板、參數說明和多模態 workflow。

- [打開完整原 Seedance 2 guide](seedance-2-guide/README.zh-TW.md)
- [打開原 55 個 case 索引](use-cases/README.md)
- [英文 Seedance 2 用例](use-cases/en/README.md)
- [簡體中文 Seedance 2 用例](use-cases/zh-CN/README.md)
- [繁體中文 Seedance 2 用例](use-cases/zh-TW/README.md)
- [目前 Seedance API 範例](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)

## 🎬 Seedance 2.5 官方 Guide

## 首屏視頻

### Case 1: 首屏影片 1

[![首屏影片 1](assets/thumbnails/01-hero-demo-1-official-launch-film-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group2/2.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group2/2.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
一段高級、極具電影感的30秒3D動態圖形序列，採用精緻的蒸氣龐克與復古微縮景觀風格，搭配連續流暢的環繞與穿透運鏡。
[0-10秒]： 古董黃銅鐘面微距特寫，奇蹟般層層展開為相互嚙合的旋轉齒輪環與體積霧。鏡頭向下穿透齒輪，一架機械撲翼機（Ornithopter），正從做舊古籍堆疊而成的微縮峽谷中盤旋升空。
[10-20秒]： 鏡頭跟隨撲翼機的軌跡向前滑行，無縫穿透入一個高速旋轉的華麗黃銅幻影箱（Zoetrope），內部投射出飛馳的機械駿馬動態光影。光影躍出箱體，場景瞬間化為一輛黃銅質感懸浮纜車，正沿著微光銅軌穿梭於機械齒輪森林，沐浴在電影級的黃金時刻光線中。
[20-30秒]： 鏡頭優雅向下平移，纜車下方出現一艘精美的發條木製機械帆船，在深藍色玻璃材質的起伏海浪中破浪前行。海浪盡頭無縫演變為一輪發光巨月，一群舉著搖曳提燈的探險者剪影，正沿著星空下的水晶礦脈山脊艱難跋涉。鏡頭平滑螺旋拉遠，穿過空靈雲朵，回到滴答作響的宏大黃銅鐘面。
技術規格： 超寫實機械紋理，豐富黃銅與金色調，電影級淺景深。平滑連貫的無縫穿梭運鏡，極強的史詩感與奇幻冒險氛圍。
```

---

### Case 2: 首屏影片 2

[![首屏影片 2](assets/thumbnails/02-hero-demo-2-official-launch-film-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group1/1.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group1/1.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
一部配合动感电子节拍的快节奏、电影级无缝转场（Match-cut）短片。画面正中始终固定一颗完美无瑕的水晶球，内部刻有发光的‘seedance’标志。水晶球保持极致对焦，随着强劲的音乐鼓点，背景高速无缝切换：
場景1： 微距特寫，電影質感的水花在水晶球周圍飛濺，折射複雜光影。
场景2： 晨间复古咖啡馆，水晶球置于原木桌面，背景是升腾的咖啡热气与窗外模糊的通勤人流。
场景3： 傍晚黄金时刻，滑板青年单手抛握水晶球，背景为极速倒退的街景与绝美的夕阳逆光。
场景4： 狂热音乐节现场，人手高举水晶球，折射出背景绚丽的舞台激光。
场景5： 热闹的家庭派对餐桌，水晶球静置中央，背景是欢聚干杯、拿取食物的模糊人影。
场景6： 昏暗电影院中，双手捧着水晶球，巨大银幕的微光在其表面流转。
场景7： 水晶球置于强烈震动的音响振膜上，随音乐高潮无缝切换至旋转的DJ打碟机中央。
场景8： 户外露营之夜，背景化作温暖的篝火与摇曳的灯串光斑（Bokeh）。
拋起落幕： 隨音樂最終重音，水晶球被高高拋出畫面上方；瞬間切至純黑背景，畫面正中浮現極簡的黑底白字“seedance”，
紧贴动感BGM律动剪辑（卡点转场），顶级电影感调色（Cinematic Color Grading）。逼真的玻璃折射与透射材质，复杂光线追踪（Ray tracing），全局照明。主體極致清晰，背景帶有強烈的動態模糊，視覺衝擊極強。
```

---

### Case 3: 首屏影片 3

[![首屏影片 3](assets/thumbnails/03-hero-demo-3-official-launch-film-3.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group3/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group3/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 5

**Prompt:**

```text
電影級品牌概念短片。<<<image_1_1>>>為首幀，畫面微微晃動，鏡頭逐漸推近，來到窗外快速後退的樹影，樹影後退速度越來愈快，突然切到<<<image_2_2>>>，速度突然放緩，鏡頭順著溪流緩緩前進，鳥語花香。
鏡頭下移，來到水下，音效有水中氣泡的聲音，一群橘色的水母從鏡頭前優美地遊過<<<image_3_3>>>，鏡頭緩緩後拉，有一群小魚晃過鏡頭後從水里穿到窗內<<<image_4_4>>>，少女左看右看，在觀賞小魚
鏡頭緩緩後拉，畫面虛焦，隨後又重新對焦畫面變清晰，跟隨音樂節奏切換：中式園林花窗<<<image_5_5>>>光線轉圈、教堂玻璃彩窗、飛機舷窗、穹頂天窗、飄窗、百葉窗、歐洲老虎窗、門上貓眼、相機取景框、鳥類眼睛、人類眼睛特寫。
畫面停留在人類眼睛特寫，隨後眼睛閉上，畫面黑屏，再突然一睜眼，眼睛中央出現「seedance」帶重音
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

## 使用者作品

### Case 4: 視覺特效 1

[![視覺特效 1](assets/thumbnails/04-official-showcase-4-visual-effects.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-1.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-1.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
一段15秒無縫循環的創意文字動畫視頻，4K，30fps。每種語言約1.2秒，轉場透過文字溶解、變形或粒子飄散實現，無硬切。背景音樂節奏感明顯，強卡點
0-1.2s 中文「創造」· 歐普視錯覺純黑背景，黑白同心圓從中心向外擴散形成視覺隧道。白色立體漢字"創造"從圓心深處緩慢凸出推向鏡頭，粗體無襯線，邊緣有微妙陰影。同心圓隨文字推進產生波紋扭曲，如水面漣漪。文字完全凸出後停頓，隨即溶解為藍色蠟筆顆粒飄散。
1.2-2.4s 英文「CREATE」· 手繪蠟筆暖黃色牛皮紙紋理背景，粗糙的藍色蠟筆筆觸逐筆寫出大寫英文"CREATE"。筆觸帶有明顯的蠟筆顆粒感和重疊痕跡，E的最後一橫略微上揚。寫完後字母表面有輕微蠟質光澤，背景浮現淡淡的鉛筆輔助線。文字隨後被吸入CRT掃描線消失。
2.4-3.6s 西班牙語「CREAR」· 復古街機深色街機框體，中央CRT螢幕有細微掃描線和螢光粉顆粒感。藍紫漸層的立體像素字"CREAR"從底部升起，字母表面有海浪般的白色波紋動畫，邊緣發出霓虹藍光。螢幕左上角有"CREDIT 00"，右下角閃爍"INSERT COIN"。文字隨後像素化崩解為靛藍色蠟染紋樣。
3.6-4.8s 印尼語「CIPTAKAN」· 蠟染布料深靛藍色傳統印尼蠟染布料背景，布面有精細的拋物線花紋。白色襯線字體"CIPTAKAN"從布料下方緩緩浮起，如燙金壓印，布料隨文字浮現產生真實的褶皺波動。文字顯現後，布料被風吹起，金色碎屑向四周飄散，轉為伊斯蘭幾何圖案。
4.8-6.0s 馬來語“CIPTA”· 伊斯蘭幾何。深綠色絲絨背景，金色阿拉伯式幾何花紋從四角向中心蔓延。白色古典襯線字"CIPTA"從中心旋轉浮現，字母周圍有星形圖案環繞，金粉粒子飄落。文字隨後被金色雕刻刀逐字刻入黑色金屬牌匾。
6.0-7.2s 泰語「สร้างสรรค์」· 金箔雕刻黑色背景，泰文"สร้างสรรค์"以金色牌匾，從古老牌匾上呈現彷彿雕刻。文字表面有細微的金箔剝落動畫，露出下方暗紅色底漆，金色碎屑向四周飄散。雕刻完成後，文字熔化為銀色汞液滴落。
7.2-8.4s 阿拉伯語「إبداع」· 機械翻頁。黑色金屬翻頁顯示器佔據整個畫面，機械葉片喀喀作響依序翻轉。白色像素格組成的阿拉伯文"إبداع"從右至左逐字顯現，每個字母翻轉伴隨精確的機械運動和輕微震動。翻頁完成後，文字被彩色桑巴羽毛風暴席捲。
8.4-9.6s 葡萄牙語「CRIAR」· 狂歡羽毛。黑色背景，彩色桑巴羽毛從畫面邊緣向中心匯聚形成巨大羽毛扇。白色粗體字"CRIAR"從羽毛扇中心爆裂而出，羽毛隨文字衝擊向四周飛散，文字表面有Carnival亮片反光，巴西國旗綠黃藍光斑閃爍。文字隨後被黑色水墨沖刷。
9.6-10.8s 越南語“SÁNG TẠO”· 水墨絲綢。米白色絲綢背景，黑色水墨從畫面頂部緩緩流淌，逐漸形成越南語"SÁNG TẠO"。水墨在絲綢上產生自然的暈染邊緣，部分墨滴向下滴落形成懸掛的墨珠。完成後絲綢被風吹起，露出下方蓮花暗紋，文字凝結為透明玻璃球。
10.8-12.0s 日文「創造」· 光學玻璃純黑背景中央懸浮一顆完美的透明光學玻璃球，球體折射出彩虹色散光斑。玻璃球後方，日文漢字"創造"以彩虹色散投影呈現，隨玻璃球緩慢旋轉，文字產生扭曲拉伸分離的光學畸變。玻璃球表面有細微灰塵顆粒，隨後球體熔化為銀色液態金屬。
12.0-13.2s 韓文「창조」· 液態金屬。深邃星空背景，銀色液態汞從畫面頂部滴落，在空中自然凝聚成韓文"창조"。液態字表面有強烈的鏡面反射，倒映周圍星星。文字形成後，部分汞液繼續向下滴落，形成懸掛的金屬珠，最終所有金屬液匯聚成一顆巨大的銀色球體。
```

---

### Case 5: 影視 2

[![影視 2](assets/thumbnails/05-official-showcase-5-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-1.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-1.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
【整體風格設定】
一段極具電影感與高級質感的30秒高訂品牌級視覺大片。畫面強調夢幻光點（Bokeh）、絲滑的動感模糊轉場（Motion blur）、體積光（Volumetric lighting）以及超寫實的材質細節表現力。
【分鏡描述】
[0-5秒]：夢幻序章與微距特寫
極高畫質的微距特寫。一隻纖細的手伸向空中，指尖觸碰著如星辰般璀璨、閃爍的彩色光斑。伴隨光影流轉，無縫絲滑轉場至一位穿著純白薄紗裙的優雅女性，她正沉醉地彈奏一架復古鋼琴。淺景深，背景虛化為唯美的藍綠色調。
[5-15秒]：隨後切入流暢的跟隨運鏡（Follow shot）：一名戴著法式寬簷草帽、身披飄逸白裙的女子，在開滿粉橘色玫瑰與藍色繡球花的繁密花徑中輕盈奔跑。光線透過樹葉灑下斑駁光影，完美展現柔和的微風、真實的裙擺布料飄動物理演算以及花瓣的超寫實紋理。
[15-24秒]：靜謐美學與光影折射
鏡頭節奏放緩，進入極致唯美的慢動作（Slow-motion）。一位少女坐在歐式復古流金噴泉旁的黑色鐵藝桌前靜靜閱讀。空氣中漂浮著漫天晶瑩剔透的肥皂泡泡，泡泡表面完美折射出周圍的繁花與溫暖的陽光。水滴濺落的瞬間清晰可見，展現模型對透明材質、水體折射與複雜光照的頂級渲染能力。
```

---

### Case 6: 後期特效 3

[![後期特效 3](assets/thumbnails/06-official-showcase-6-post-production-vfx.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-1.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-1.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
深海珊瑚礁場景，藍色主調的熱帶海底世界，大面積健康繁盛的彩色活珊瑚，包含枝狀珊瑚、腦珊瑚、盤狀珊瑚和柔軟海扇珊瑚，大量熱帶魚群自然穿梭其中，近景清晰鮮活，遠景逐漸偏藍偏灰、對比減弱，上方自然光經過海水過濾形成柔和體積光，海水中有細小懸浮顆粒和擺動淡淡的小光， 8-12 只，大小各異。傘狀體帶有柔和的生物螢光效果，觸鬚隨波浪輕柔飄動，觸鬚末端有微弱的紫色光點。水母大小與珊瑚和魚類比例協調，發光效果柔和不刺眼，在深色海水背景中形成夢幻的光點。水母群的運動軌跡自然，呈現緩慢上升螺旋狀，部分水母從鏡頭前方遊過產生輕微的鏡頭光暈效果。保持水下的藍色調光照，水母的發光與周圍珊瑚的微弱反光和諧共存。 水母群遊動過程中產生了氣泡，氣泡上浮，在海中形成了「Seedance」字樣
```

---

### Case 7: 影視 4

[![影視 4](assets/thumbnails/07-official-showcase-7-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-2.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-2.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
電影質感，高級感，清晨金色沙漠，一座極簡主義白色美術館建築漂浮在沙丘上方，建築表面有細膩石材紋理和柔和反射。陽光穿過沙塵形成體積光，遠處沙丘層次分明。鏡頭從超廣角沙漠全景開始，緩慢向前推進，穿過飛揚的沙粒，進入漂浮建築內部。室內有懸浮雕塑、半透明絲綢裝置和身穿白色長袍的角色，布料隨風自然擺動。鏡頭圍繞著角色進行平滑環繞運動，最後建築牆面緩慢打開，露出巨大的天空和沙漠。高端藝術廣告風格，真實光照，精緻材質，電影級構圖，優雅運動，超現實但真實可信。
```

---

### Case 8: 廣告宣傳 5

[![廣告宣傳 5](assets/thumbnails/08-official-showcase-8-advertising.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-2.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-2.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
一部極具視覺張力的30秒高級品牌概念短片。开场采用超现实的颠倒视角，镜头随重力翻转，展现模特穿着复古麂皮靴的双脚轻踏在起伏的赤色沙丘上，微距镜头特写靴子表面的磨砂绒感与沾染的粗糙红沙颗粒。随后切入一系列充满失重感与梦幻色彩的蒙太奇：年轻的男女模特在暗流涌动的琥珀色风沙与冷冽的边缘轮廓光中轻盈向后坠落；镜头迅速切入面部的极锐利特写——风沙吹拂过沾着微小金沙的睫毛，模特佩戴着复古金属框架墨镜，弧形镜片中清晰地反射出荒野的烈日与风暴。隨後，戴上做舊厚重銀戒的手指，輕柔拂過粗糲滄桑的岩壁與隨風狂舞的蘆葦叢。
画面大量运用极具表现力的镜头语言：通过极低视角的微距镜头，透过边缘虚化且剔透的天然矿石晶体仰拍深邃的浩瀚星空与肆意穿行的探险者。在宏大场景中密集穿插高质感的局部特写：风中猎猎作响的粗纺亚麻衬衫纹理、模特紧绷冷峻的下颌线，以及颈部肌肤在逆光下闪烁的汗水光泽。結合魚眼鏡頭、快速的旋轉運鏡與絲滑的視覺錯位轉場，營造出前衛且充滿野性張力的神秘動感。
短片高潮处，镜头极具戏剧性地拉远，打破‘第四面墙’，揭示这其实是一个搭建了巨型LED星轨环形天幕与真实红沙阵列的高级虚拟影棚，将旷野的苍茫感与先锋的工业片场感完美碰撞。结尾处节奏放缓，回归细腻的质感特写：一位披发女子倚靠在复古越野车旁，镜头缓缓扫过车身斑驳剥落的重金属烤漆，女子随性地让掌心的细沙从指缝间滑落。清冷而皎洁的月光（Moonlight）侧光精准勾勒出做旧皮革外套粗犷的面料毛孔、重金属拉链折射的冷光，以及女子冷峻立体的面部轮廓。整体呈现复古胶片级的色彩美学，深邃的幽夜蓝与炽热的矿石橘交织，画面大气、自由，充满极高质感的品牌张力。最後畫面中央優雅浮現「seedance」文字。
```

---

### Case 9: 影視 6

[![影視 6](assets/thumbnails/09-official-showcase-9-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-2.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-2.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
京劇非遺短片，電影感，東方美學，溫暖克制。傳統戲班後台與手工作坊裡，老師傅安靜製作京劇頭飾、整理戲服、勾勒臉譜，手部細節細膩，絲線、珠飾、顏料和刺繡都很有質感。一個年輕學徒在旁邊認真看著，隨後小心接過工具，在老師傅指導下完成細小步驟。老師傅為他扶正頭面、整理衣襟，像把一門手藝和一份情感輕輕交到他手裡。最後年輕人穿戴整齊，站在即將上場的戲台邊，微光照亮戲服與側臉，老師傅在身後安靜注視。整體氣氛安靜、深情、有傳承感，少字幕，穿插合適的台詞。
```

---

### Case 10: 遊戲 7

[![遊戲 7](assets/thumbnails/10-official-showcase-10-game-trailer.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-3.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-3.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
落劇場（Oceanic Civilization）》
（史詩科幻 / Dune × Interstellar / 無真人 / 雕塑生命體）
【0–5秒｜宇宙級開場 · 海洋作為星球記憶】
深藍色海洋佔據畫面全景，極深層水體呈現分層結構，如同星球內部的液態宇宙。
鏡頭從高空緩慢垂直下墜，穿過雲層與海霧，進入海面。
海面像金屬薄膜般波動，折射出不規則的太陽光裂縫，極具史詩感體積光。
【5–10秒｜進入深海文明斷層】
鏡頭穿透海面，進入深海。
巨大的「海底文明結構」逐漸顯現：
斷裂的環形巨構建築、沉沒的石穹頂、漂浮的幾何遺跡平台。
結構風格融合古代神殿 + 外星文明科技感（類似 Dune 遺跡語）。
海水中懸浮著微光顆粒，如星塵在水中緩慢漂移。
【10–15秒｜雕塑生命體出現（非人類）】
在劇場中央，矗立著巨型雕塑生命體：
由白色石材與半透明礦物構成的“人形神像”，但無生命細節（無皮膚、無真實人類特徵）。
其姿態如古代儀式結構，身體呈現分段幾何結構，類似文明記憶載體。
雕塑表面被水流長期侵蝕，佈滿海藻與珊瑚晶化結構。
鏡頭緩慢環繞雕塑，形成「神靈降臨感」。
【15–20秒｜文明被喚醒 · 光流啟動】
整個海底遺跡開始「甦醒」。
雕塑內部出現微弱能量流動光紋，如神經網路般點亮。
斷裂石柱緩慢上升重組，形成環形劇場結構。
水體開始出現“秩序性流動”，彷彿空間被重新計算。
鏡頭由靜態環繞 → 輕微加速旋轉。
【20–24秒｜海面反轉 · 上升突破】
鏡頭突然向上加速衝出海面。
海水被撕開般向兩側分離，形成巨型水幕。
一艘古代文明巨型飛船/神殿船體從海底升起：
外形象融合石質神殿與科幻船艦的混合體，表面覆蓋珊瑚與礦化結構。
船體帶著海水瀑布般上升。
【24–27秒｜史詩旋轉鏡頭（視覺高潮）】
鏡頭圍繞巨船高速旋轉上升（spiral orbit shot）。
太陽從雲層裂隙中穿透，形成神聖光柱。
水流被旋轉拉成螺旋形態，如星系結構。
船體緩慢翻轉，展現其龐大結構：
類似「移動文明遺跡」而非交通工具。
【27–30秒｜終極遠景 · 文明尺度揭示】
鏡頭極速拉遠至太空級視角。
海洋、遺跡、升起的巨船、雕塑神殿在同一畫面垂直排列：
形成「海底文明—海面—天空光層」的三段宇宙結構。
整個世界像一個被喚醒的古老星球記憶系統。
最終畫面緩慢收束進入黑屏，僅剩微弱光點殘留。
史詩科幻美學 / Dune風沙海文明結構感 / Interstellar 級空間尺度 / 無人物敘事 / 雕塑文明遺跡 / 外星神殿結構 / 體積光穿透海水 / 巨構建築崩塌與重組 / 神聖儀式感鏡頭 / 螺旋運鏡 / 星塵粒子海洋 / 高動態範圍電影級真實感
```

---

### Case 11: 影視 8

[![影視 8](assets/thumbnails/11-official-showcase-11-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-3.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-3.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
主題是「機械花開」。畫面需要突顯生成影片模型在光影、美術細節、真實感、鏡頭運動和角色電影感的優勢。整體風格為高階科技品牌廣告，具有強烈視覺衝擊力。影片採用一鏡到底的微距推進鏡頭，從黑暗中的金屬花苞開始，逐漸進入花瓣內部的精密機械結構，最後以機械花完全綻放、光線向外擴散作為高潮畫面。要求真實物理光照、精緻金屬和玻璃材質、細膩機械運動、穩定構圖、電影級調色、無字幕
```

---

### Case 12: 科普 9

[![科普 9](assets/thumbnails/12-official-showcase-12-educational-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-3.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-3.mp4) · 點擊縮圖即可播放影片。

**Prompt:**

```text
整體風格需求：岩彩平面動畫，東方與絲路裝飾美學，礦物顏料質感，硃砂紅、赭石、石綠、群青、金色點綴，紙本與壁畫肌理，平面分層，不要真實攝影，不要 3D 寫實。畫面節奏由靜到動，再由動回歸沉靜，突出 “從土地到杯中” 的旅程感與豐盛感，音樂歡快，西域風格。
鏡頭一：枝頭初現，豐盛開場（0-4 秒）
絲路畫作紙上暈開赭石與朱紅色塊，一株石榴枝條從畫面右側舒展出來，葉片厚重，帶有明顯礦物顏料層次。枝頭一顆飽滿石榴緩緩顯現，外殼紅中帶金，輪廓圓潤安靜。陽光以金色圓斑和金箔碎點落在果皮上，石榴表面泛出溫潤光澤，像一枚被時光養熟的果實，開場氣質豐盛而克制。
鏡頭二：輕輕摘下，旅程開始（4-7 秒）
石榴被一位西域侍女輕輕摘下，動作平穩優雅。背景逐漸浮現卷草紋、古老紋樣和裝飾性長卷構圖，暗示它來自久遠土地。畫面從靜態枝頭自然過渡到旅程展開，山嶺、道路與城鎮開始在背景中平面鋪陳，像一幅絲路長卷慢慢被打開。
鏡頭三：穿越古道，跨越山河（7-13 秒）
駝隊剪影緩慢前行，鈴鐺以細小金點表現節奏，石榴出現在駱駝的背包裡。古道穿過沙丘、綠洲與城門，風沙以流動紋樣掠過，金線勾出的道路不斷向遠方延展。色彩濃烈而高級，像絲路壁畫與岩彩插畫融合在一起。石榴在漫長路途中始終鮮豔飽滿，像把遙遠土地的陽光、熱度與豐盛一直保存到了今天。
鏡頭四：古今轉場，抵達當下（13-16 秒）
背景中的古代紋樣與建築輪廓逐漸簡化，時間悄悄過渡到現代空間。石榴被放在現代案台上，桌面與器皿以簡潔平面幾何呈現，古今視覺在同一畫面中完成連接，畫面節奏從 “遠行” 轉為 “抵達”。
鏡頭五：切開石榴，視覺高潮（16-20 秒）
一隻手輕輕切開石榴，動作緩慢克制，果皮裂開的一瞬間極具儀式感。
鏡頭六：榨成果汁，豐沛流動（20-24 秒）
籽粒進入器皿，被壓榨成濃鬱石榴汁，液體流動呈現深紅通透質感，帶有細膩岩彩顆粒。石榴汁緩緩倒入現代玻璃杯中，玻璃輪廓清晰簡潔，紅色液體在杯中升高，表面泛起微微波紋與高光。幾顆冰塊落入杯中，冷白色與深紅色形成鮮明對比，杯壁出現細密水珠，清爽感拉滿。
鏡頭七：現代飲用，旅程落地（24-27 秒）
背景切入現代生活場景，窗光、桌面、織物與植物保持平面裝飾性和溫潤配色。果汁杯置於畫面中央，周圍隱約疊加古道、駝隊、城門紋樣，暗示這杯果汁來自漫長旅程。氛圍豐盛、溫暖、沉靜。
鏡頭八：時間匯合，海報式收束（27-30 秒）
背景中的古道紋樣與現代空間逐漸融合，像時間在這一杯果汁裡匯合。畫面短暫回閃枝頭石榴、古道駝影和紅色籽粒，形成 「從土地到杯中」 的完整迴路。最後收束成廣告海報式構圖：深紅濃豔的石榴汁置於中央，杯旁是一顆裂開的石榴，周圍疊加古道紋樣、金色光點與現代生活元素，畫面安靜卻充滿生命力，像一段跨越時間與土地的旅程終於抵達當下，廣告詞“seedance，來自西域的禮物”。
```

---

## 突破敘事邊界

### Case 13: 突破敘事邊界-30s連貫直出-輸出-1

[![突破敘事邊界-30s連貫直出-輸出-1](assets/thumbnails/13-narrative-control-13-30-second-continuous-output-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group1/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group1/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 8

**Prompt:**

```text
一鏡到底，鏡頭平穩地跟著一個穿著黑色大衣的人（參考<<<image_1_1>>>）從左向右穿過六個相連的不同色調、不同氛圍的房間。每個房間結構相同：白牆、人字拼淺色木地板、法式雙開落地窗、白紗簾，參考<<<image_2_2>>>但窗外風景和室內氛圍完全不同。主角全程勻速走動，穿過牆上敞開的每一扇門。
0-5秒，第一個房間，主題為美漫打鬥，主角進入屋內與人物（<<<image_3_3>>>）打鬥，人物落敗；
5-10秒，第二個房間，主題為溫暖，毛氈風格，窗外場景為向日葵田（<<<image_4_4>>>），室內光線暖橙柔光，有一個畫家正在畫向日葵（<<<image_5_5>>>）。主角进入后也变成毛毡风格；
10-15秒，第三個房間，主題為悲傷，整個畫面為黑白漫畫定格動畫風格，窗外陰雨，室內光線冷灰低沉，一個人獨自坐在空房間中央地板上，低頭抱膝，身旁一隻手機亮著無人接聽的通話界面。主角進入房間後關上房間的燈，馬上開燈，房間內變成彩色，瞬間生長出滿屋鮮花；
15-20秒，第四個房間，主題為歡樂，整個場景為浸泡在海裡的房間，參考<<<image_6_6>>>，主角遊進房間，身旁有美麗的珊瑚礁和魚群；
20-25秒，第五個房間，主題為驚喜，窗外場景漫天煙火夜空，參考<<<image_7_7>>>，室內光線彩色閃爍映射，主角被捲入歡呼氣氛。
25-30秒，最後主角來到一個空白房間，站在中央打了個響指，同時音效為響指聲，畫面整體黑屏，中間出現“seedance”字樣，參考<<<image_8_8>>>。
整體電影質感，高級時裝廣告風格，光線完全由窗外場景決定形成強烈情緒反差，畫面無文字。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 14: 突破敘事邊界-30s連貫直出-輸出-2

[![突破敘事邊界-30s連貫直出-輸出-2](assets/thumbnails/14-narrative-control-14-30-second-continuous-output-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group2/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group2/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 3

**Prompt:**

```text
製作一支關於足球三千年演變史的 30 秒科普短視頻，全片用同一個球作為視覺主線，球從古代一路滾動、穿越、變形，串聯不同文明與時代。整體節奏緊湊，畫面高級，歷史科普短片與藝術化轉場結合，突顯一個球跨越三千年的感覺，口播簡潔有力。
開場，一顆古老的球從黑色背景中緩緩出現，表面帶有歲月紋理，隨後滾入中國戰國時期的蹴鞠場景，畫面轉為水墨風，參考<<<image_1_1>>>的風格，古人穿古裝在庭院中蹴鞠，動作優雅，球在腳下彈起。口播：足球故事，從蹴鞠開始。
接著，這顆球繼續向前滾動，畫面自然過渡到古希臘球類遊戲場景，畫面為古典油畫風格，風格參考<<<image_2_2>>>，廣場與石柱背景明顯，人們穿著古希臘長袍踢球，畫面厚重、有歷史感。口播：希臘人也熱愛球類運動。
然後球滾入中世紀歐洲，畫面仍保持油畫風格，村莊、泥地、普通民眾追逐皮球，氣氛熱烈而粗糲，像民間古足球延續火種。口播：歐洲民間把球賽延續下來。
接著球被一腳踢出，畫面切換為黑白紀錄片風格，參考<<<image_3_3>>>，來到1863 年的英國，紳士、俱樂部、草地球場逐漸出現，象徵現代足球正式誕生，這顆球第一次呈現出現代足球的標準外觀。口播：1863 年，現代足球定型。
隨後畫面快速進入現代，球在空中旋轉，依序帶出關鍵發展節點，燈光、球場、觀眾、獎盃、全球不同場景交織，表現足球從地方運動走向全球。
結尾，這顆球在現代球場中央，世界各地的人群、歡呼聲在背景中融合，形成 “一個球連接世界” 的感覺，畫面大氣、有史詩感。口播：現在，足球連結了全世界。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 15: 突破敘事邊界-30s連貫直出-輸出-3

[![突破敘事邊界-30s連貫直出-輸出-3](assets/thumbnails/15-narrative-control-15-30-second-continuous-output-group-3.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group3/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group3/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 6

**Prompt:**

```text
一段 30 秒的膠囊咖啡機安裝使用教學影片。
0-2秒，開頭大標題文字為：seedance 膠囊咖啡機安裝使用教學課程
2-5秒，步驟 1：安裝水箱，參考<<<image_1_1>>>鏡頭： 中景，微俯視角位置： 機身背面動作： 將水箱對準機身背部卡槽，垂直向下推入，聽到 "咔" 聲卡緊，要求： 清晰展示水箱底部卡扣與機身卡槽的對位關係，水箱透明部分可見水位線
旁白： "首先，安裝水箱。"
5-9秒，步驟 2：安裝滴水盤，參考<<<image_2_2>>>鏡頭： 近景，正視角，位置： 機身底部前方，動作： 將滴水盤平行推入機身底部導軌，推至底部完全貼合，要求： 展示導軌對齊過程，突出滑入動作的順暢感
旁白： "接下來將托盤對準底部導軌。"
9-13秒，步驟 3：安裝廢棄膠囊收集盒，參考<<<image_3_3>>>鏡頭： 近景，微仰視角，位置： 滴水盤下方空腔，動作： 將收集盒對準凹槽推入，與滴水盤齊平，要求： 展示收集盒與機身的嵌合關係，確認安裝到位
旁白： "然後裝入膠囊收集盒。"
13-18秒，步驟 4：首次注水，參考<<<image_4_4>>>鏡頭： 特寫，側視角，位置： 機身頂部 / 背部水箱，動作： 打開水箱蓋，倒入清水至 MAX 水位線，合上水箱蓋，要求： 突出水位線標識，水流倒入清晰可見
旁白： "打開水箱蓋，倒入清水。注意不要超過最大水位線。"
畫面高亮最大水位線。
18-25秒，步驟 5：通電開機，參考<<<image_5_5>>>鏡頭： 中景，正視角，位置： 機身正面，動作： 插入電源線，按下電源鍵，指示燈由閃爍變為常亮（預熱完成），要求： 特寫電源按鍵與指示燈狀態變化，體現等待到就緒的過程
旁白： "接通電源，按下電源鍵。"
25-30秒，步驟 6：首次沖洗（不放膠囊），參考<<<image_6_6>>>鏡頭： 中景轉特寫，正側視角，位置： 機身正面，杯子在出水口下方，動作： 不放入膠囊，直接按萃取鍵，熱水流出沖洗管路，水流入杯中，要求： 強調 "無需放膠囊" 的提示標註，展示沖洗水流出全過程
旁白： "最後一步，首次沖洗。不需要放入膠囊，直接按下萃取鍵。您的咖啡機可以正式使用了。"
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 16: 突破敘事邊界-更多參考輸入-輸出-1

[![突破敘事邊界-更多參考輸入-輸出-1](assets/thumbnails/16-narrative-control-16-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 17

**Prompt:**

```text
核心指令： 全程 26 秒一鏡到底（One-Shot）敘事短片，穩定跟拍，參考<<<video_1_1>>>與平滑環繞運鏡，參考<<<video_2_2>>>交織。平滑行進感。鏡頭內實現晝夜交替與四季流轉。主角是歐洲女子<<<image_1_3>>>，置身充滿煙火氣的人海，凸顯極致的孤獨感與電影攝影質感。
分段運鏡與場景描述：
0-3 秒（平穩背跟）： 老舊木門<<<image_2_4>>>「吱呀」推開，鏡頭緊跟著歐洲女人穿著<<<image_3_5>>>的背影步出。他在門檻處微停，前方街巷光影斑駁，叫賣與人潮聲撲面而來。她神情疏離，緩緩邁步融入街頭。
3-6 秒（背側方跟拍）： 鏡頭保持平滑跟進，她步入擁擠的早市，氛圍參考<<<video_3_6>>>。兩側擠滿色澤濃鬱的水果攤與香料鋪，一隊街頭雜耍藝人正噴吐火龍，參考<<<image_4_7>>>，火光照亮人群，但她目不斜視，步伐勻速穿過。
6-9 秒（側邊平滑環繞）： 鏡頭開始向側前方平滑環繞，捕捉主角的側臉。她走過喧鬧的肉舖<<<image_5_8>>>，一位年輕母親抱著嬰兒<<<image_6_9>>>與他擦肩，嬰兒好奇地緊盯她，她卻只是微微垂下眼眸避開視線，沒有絲毫停留。
9-12 秒（正前方倒退跟拍）： 鏡頭繼續繞至主角正前方，進行倒退跟拍。前方人群突然如摩西分海般自然退至兩側，一隻披著華麗紅布的巨大大象<<<image_7_10>>>邁著沉穩的步伐，從畫面右側出現，佔據了大半個畫面。
12-15 秒（縫隙穿透與繞回）： 女人與大象即將相撞的瞬間，鏡頭巧妙地貼著大象與女人之間的狹窄縫隙滑過，重新繞回她的背影。大象龐大而安靜地掠過，頑童們歡呼追逐。象鈴聲、笑聲鼎沸，她卻連腳步都未曾放緩。
15-18 秒（環境光影漸變）： 伴隨她的行走，長鏡頭內的光影奇幻變幻－盛夏的刺眼陽光瞬間柔和，一陣微風捲起漫天金黃的落葉<<<video_2_2>>>0 ，季節在同一個長秋鏡頭中無縫過渡至深秋鏡頭。落葉拂過她的肩膀。
18-21 秒（360度沉浸環繞）： 前方驟然陷入一場盛大的街頭慶典<<<video_2_2>>>1 。空中噴吐出漫天彩帶與碎紙，攤販探出身子歡呼。鏡頭在此刻展開一段連貫的 360 度環繞運鏡，將安靜孤寂的主角與狂熱的周圍形成極其強烈的視覺撕裂。
21-24 秒（繞回側後方）： 當鏡頭環繞一週結束回到她側後方時，飄落的彩帶已悄悄化作漫天飛雪－瞬間入冬<<<video_2_2>>>2 。行人們紛紛撐起傘或戴上兜帽，女人微微瑟縮，豎起大衣衣領，服裝變成<<<video_2_2>>>3 ，在雪地中繼續孤身前行。
24-26 秒（慢推跟拍）： 隨著她走向長街盡頭，天色在行進中以肉眼可見的速度暗下，白晝無縫沉入黑夜。兩側昏黃的路燈與小攤的燈泡次第亮起<<<video_2_2>>>4 ，小販收拾貨物，喧鬧聲彷彿被大雪慢慢吸收、拉遠，她的腳步逐漸放緩。夜空驟然綻放盛大的煙火<<<video_2_2>>>5 ，煙火綻放聲音參考<<<video_2_2>>>6 五彩光斑在樓牆與她的眼眸中閃爍跳躍。世界熱鬧依舊，而她安靜仰望，鏡頭緩緩拉遠，在此溫柔收束。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 17: 突破敘事邊界-更多參考輸入-參考影片-1-1

[![突破敘事邊界-更多參考輸入-參考影片-1-1](assets/thumbnails/17-reference-asset-17-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference1.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference1.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 17

**Prompt:**

```text
核心指令： 全程 26 秒一鏡到底（One-Shot）敘事短片，穩定跟拍，參考<<<video_1_1>>>與平滑環繞運鏡，參考<<<video_2_2>>>交織。平滑行進感。鏡頭內實現晝夜交替與四季流轉。主角是歐洲女子<<<image_1_3>>>，置身充滿煙火氣的人海，凸顯極致的孤獨感與電影攝影質感。
分段運鏡與場景描述：
0-3 秒（平穩背跟）： 老舊木門<<<image_2_4>>>「吱呀」推開，鏡頭緊跟著歐洲女人穿著<<<image_3_5>>>的背影步出。他在門檻處微停，前方街巷光影斑駁，叫賣與人潮聲撲面而來。她神情疏離，緩緩邁步融入街頭。
3-6 秒（背側方跟拍）： 鏡頭保持平滑跟進，她步入擁擠的早市，氛圍參考<<<video_3_6>>>。兩側擠滿色澤濃鬱的水果攤與香料鋪，一隊街頭雜耍藝人正噴吐火龍，參考<<<image_4_7>>>，火光照亮人群，但她目不斜視，步伐勻速穿過。
6-9 秒（側邊平滑環繞）： 鏡頭開始向側前方平滑環繞，捕捉主角的側臉。她走過喧鬧的肉舖<<<image_5_8>>>，一位年輕母親抱著嬰兒<<<image_6_9>>>與他擦肩，嬰兒好奇地緊盯她，她卻只是微微垂下眼眸避開視線，沒有絲毫停留。
9-12 秒（正前方倒退跟拍）： 鏡頭繼續繞至主角正前方，進行倒退跟拍。前方人群突然如摩西分海般自然退至兩側，一隻披著華麗紅布的巨大大象<<<image_7_10>>>邁著沉穩的步伐，從畫面右側出現，佔據了大半個畫面。
12-15 秒（縫隙穿透與繞回）： 女人與大象即將相撞的瞬間，鏡頭巧妙地貼著大象與女人之間的狹窄縫隙滑過，重新繞回她的背影。大象龐大而安靜地掠過，頑童們歡呼追逐。象鈴聲、笑聲鼎沸，她卻連腳步都未曾放緩。
15-18 秒（環境光影漸變）： 伴隨她的行走，長鏡頭內的光影奇幻變幻－盛夏的刺眼陽光瞬間柔和，一陣微風捲起漫天金黃的落葉<<<video_2_2>>>0 ，季節在同一個長秋鏡頭中無縫過渡至深秋鏡頭。落葉拂過她的肩膀。
18-21 秒（360度沉浸環繞）： 前方驟然陷入一場盛大的街頭慶典<<<video_2_2>>>1 。空中噴吐出漫天彩帶與碎紙，攤販探出身子歡呼。鏡頭在此刻展開一段連貫的 360 度環繞運鏡，將安靜孤寂的主角與狂熱的周圍形成極其強烈的視覺撕裂。
21-24 秒（繞回側後方）： 當鏡頭環繞一週結束回到她側後方時，飄落的彩帶已悄悄化作漫天飛雪－瞬間入冬<<<video_2_2>>>2 。行人們紛紛撐起傘或戴上兜帽，女人微微瑟縮，豎起大衣衣領，服裝變成<<<video_2_2>>>3 ，在雪地中繼續孤身前行。
24-26 秒（慢推跟拍）： 隨著她走向長街盡頭，天色在行進中以肉眼可見的速度暗下，白晝無縫沉入黑夜。兩側昏黃的路燈與小攤的燈泡次第亮起<<<video_2_2>>>4 ，小販收拾貨物，喧鬧聲彷彿被大雪慢慢吸收、拉遠，她的腳步逐漸放緩。夜空驟然綻放盛大的煙火<<<video_2_2>>>5 ，煙火綻放聲音參考<<<video_2_2>>>6 五彩光斑在樓牆與她的眼眸中閃爍跳躍。世界熱鬧依舊，而她安靜仰望，鏡頭緩緩拉遠，在此溫柔收束。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 18: 突破敘事邊界-更多參考輸入-參考影片-1-2

[![突破敘事邊界-更多參考輸入-參考影片-1-2](assets/thumbnails/18-reference-asset-18-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference2.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference2.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 17

**Prompt:**

```text
核心指令： 全程 26 秒一鏡到底（One-Shot）敘事短片，穩定跟拍，參考<<<video_1_1>>>與平滑環繞運鏡，參考<<<video_2_2>>>交織。平滑行進感。鏡頭內實現晝夜交替與四季流轉。主角是歐洲女子<<<image_1_3>>>，置身充滿煙火氣的人海，凸顯極致的孤獨感與電影攝影質感。
分段運鏡與場景描述：
0-3 秒（平穩背跟）： 老舊木門<<<image_2_4>>>「吱呀」推開，鏡頭緊跟著歐洲女人穿著<<<image_3_5>>>的背影步出。他在門檻處微停，前方街巷光影斑駁，叫賣與人潮聲撲面而來。她神情疏離，緩緩邁步融入街頭。
3-6 秒（背側方跟拍）： 鏡頭保持平滑跟進，她步入擁擠的早市，氛圍參考<<<video_3_6>>>。兩側擠滿色澤濃鬱的水果攤與香料鋪，一隊街頭雜耍藝人正噴吐火龍，參考<<<image_4_7>>>，火光照亮人群，但她目不斜視，步伐勻速穿過。
6-9 秒（側邊平滑環繞）： 鏡頭開始向側前方平滑環繞，捕捉主角的側臉。她走過喧鬧的肉舖<<<image_5_8>>>，一位年輕母親抱著嬰兒<<<image_6_9>>>與他擦肩，嬰兒好奇地緊盯她，她卻只是微微垂下眼眸避開視線，沒有絲毫停留。
9-12 秒（正前方倒退跟拍）： 鏡頭繼續繞至主角正前方，進行倒退跟拍。前方人群突然如摩西分海般自然退至兩側，一隻披著華麗紅布的巨大大象<<<image_7_10>>>邁著沉穩的步伐，從畫面右側出現，佔據了大半個畫面。
12-15 秒（縫隙穿透與繞回）： 女人與大象即將相撞的瞬間，鏡頭巧妙地貼著大象與女人之間的狹窄縫隙滑過，重新繞回她的背影。大象龐大而安靜地掠過，頑童們歡呼追逐。象鈴聲、笑聲鼎沸，她卻連腳步都未曾放緩。
15-18 秒（環境光影漸變）： 伴隨她的行走，長鏡頭內的光影奇幻變幻－盛夏的刺眼陽光瞬間柔和，一陣微風捲起漫天金黃的落葉<<<video_2_2>>>0 ，季節在同一個長秋鏡頭中無縫過渡至深秋鏡頭。落葉拂過她的肩膀。
18-21 秒（360度沉浸環繞）： 前方驟然陷入一場盛大的街頭慶典<<<video_2_2>>>1 。空中噴吐出漫天彩帶與碎紙，攤販探出身子歡呼。鏡頭在此刻展開一段連貫的 360 度環繞運鏡，將安靜孤寂的主角與狂熱的周圍形成極其強烈的視覺撕裂。
21-24 秒（繞回側後方）： 當鏡頭環繞一週結束回到她側後方時，飄落的彩帶已悄悄化作漫天飛雪－瞬間入冬<<<video_2_2>>>2 。行人們紛紛撐起傘或戴上兜帽，女人微微瑟縮，豎起大衣衣領，服裝變成<<<video_2_2>>>3 ，在雪地中繼續孤身前行。
24-26 秒（慢推跟拍）： 隨著她走向長街盡頭，天色在行進中以肉眼可見的速度暗下，白晝無縫沉入黑夜。兩側昏黃的路燈與小攤的燈泡次第亮起<<<video_2_2>>>4 ，小販收拾貨物，喧鬧聲彷彿被大雪慢慢吸收、拉遠，她的腳步逐漸放緩。夜空驟然綻放盛大的煙火<<<video_2_2>>>5 ，煙火綻放聲音參考<<<video_2_2>>>6 五彩光斑在樓牆與她的眼眸中閃爍跳躍。世界熱鬧依舊，而她安靜仰望，鏡頭緩緩拉遠，在此溫柔收束。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 19: 突破敘事邊界-更多參考輸入-參考影片-1-6

[![突破敘事邊界-更多參考輸入-參考影片-1-6](assets/thumbnails/19-reference-asset-19-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference6.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference6.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 17

**Prompt:**

```text
核心指令： 全程 26 秒一鏡到底（One-Shot）敘事短片，穩定跟拍，參考<<<video_1_1>>>與平滑環繞運鏡，參考<<<video_2_2>>>交織。平滑行進感。鏡頭內實現晝夜交替與四季流轉。主角是歐洲女子<<<image_1_3>>>，置身充滿煙火氣的人海，凸顯極致的孤獨感與電影攝影質感。
分段運鏡與場景描述：
0-3 秒（平穩背跟）： 老舊木門<<<image_2_4>>>「吱呀」推開，鏡頭緊跟著歐洲女人穿著<<<image_3_5>>>的背影步出。他在門檻處微停，前方街巷光影斑駁，叫賣與人潮聲撲面而來。她神情疏離，緩緩邁步融入街頭。
3-6 秒（背側方跟拍）： 鏡頭保持平滑跟進，她步入擁擠的早市，氛圍參考<<<video_3_6>>>。兩側擠滿色澤濃鬱的水果攤與香料鋪，一隊街頭雜耍藝人正噴吐火龍，參考<<<image_4_7>>>，火光照亮人群，但她目不斜視，步伐勻速穿過。
6-9 秒（側邊平滑環繞）： 鏡頭開始向側前方平滑環繞，捕捉主角的側臉。她走過喧鬧的肉舖<<<image_5_8>>>，一位年輕母親抱著嬰兒<<<image_6_9>>>與他擦肩，嬰兒好奇地緊盯她，她卻只是微微垂下眼眸避開視線，沒有絲毫停留。
9-12 秒（正前方倒退跟拍）： 鏡頭繼續繞至主角正前方，進行倒退跟拍。前方人群突然如摩西分海般自然退至兩側，一隻披著華麗紅布的巨大大象<<<image_7_10>>>邁著沉穩的步伐，從畫面右側出現，佔據了大半個畫面。
12-15 秒（縫隙穿透與繞回）： 女人與大象即將相撞的瞬間，鏡頭巧妙地貼著大象與女人之間的狹窄縫隙滑過，重新繞回她的背影。大象龐大而安靜地掠過，頑童們歡呼追逐。象鈴聲、笑聲鼎沸，她卻連腳步都未曾放緩。
15-18 秒（環境光影漸變）： 伴隨她的行走，長鏡頭內的光影奇幻變幻－盛夏的刺眼陽光瞬間柔和，一陣微風捲起漫天金黃的落葉<<<video_2_2>>>0 ，季節在同一個長秋鏡頭中無縫過渡至深秋鏡頭。落葉拂過她的肩膀。
18-21 秒（360度沉浸環繞）： 前方驟然陷入一場盛大的街頭慶典<<<video_2_2>>>1 。空中噴吐出漫天彩帶與碎紙，攤販探出身子歡呼。鏡頭在此刻展開一段連貫的 360 度環繞運鏡，將安靜孤寂的主角與狂熱的周圍形成極其強烈的視覺撕裂。
21-24 秒（繞回側後方）： 當鏡頭環繞一週結束回到她側後方時，飄落的彩帶已悄悄化作漫天飛雪－瞬間入冬<<<video_2_2>>>2 。行人們紛紛撐起傘或戴上兜帽，女人微微瑟縮，豎起大衣衣領，服裝變成<<<video_2_2>>>3 ，在雪地中繼續孤身前行。
24-26 秒（慢推跟拍）： 隨著她走向長街盡頭，天色在行進中以肉眼可見的速度暗下，白晝無縫沉入黑夜。兩側昏黃的路燈與小攤的燈泡次第亮起<<<video_2_2>>>4 ，小販收拾貨物，喧鬧聲彷彿被大雪慢慢吸收、拉遠，她的腳步逐漸放緩。夜空驟然綻放盛大的煙火<<<video_2_2>>>5 ，煙火綻放聲音參考<<<video_2_2>>>6 五彩光斑在樓牆與她的眼眸中閃爍跳躍。世界熱鬧依舊，而她安靜仰望，鏡頭緩緩拉遠，在此溫柔收束。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 20: 突破敘事邊界-更多參考輸入-輸出-2

[![突破敘事邊界-更多參考輸入-輸出-2](assets/thumbnails/20-narrative-control-20-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 7

**Prompt:**

```text
明亮多彩的廣告片風格，果味餅乾為主角，包含草莓、蘋果、葡萄、橙子四種口味，草莓味參考<<<image_1_1>>>，餅乾與對應水果以強秩序感的幾何陣列排布，整體畫面乾淨、高級、節奏強。開場水果快速建立視覺聚焦，參考<<<video_1_2>>>的構圖，音樂重拍切入。隨後不同口味餅乾整齊排列，切特寫，參考<<<video_2_3>>>的動態和運鏡。高潮段一塊餅乾被折斷，瞬間進入慢動作，果味夾心爆開，碎屑飛濺，果汁感與顆粒衝擊被放大展示，參考<<<video_3_4>>>的衝擊感。橫向陣列，形成節奏拋物感，參考<<<video_4_5>>>的移動，突顯秩序美感與產品豐富度。隨後迅速回到快節奏剪輯。結尾英文文字 One bite of crispness, a heart full of delight 快速分詞切換入畫，配合強節奏文字運動與產品定格，參考<<<video_5_6>>>，最終品牌感收束，餅乾和水果向四周發散，參考<<<video_6_7>>>，畫面充滿年輕、活力、好吃、想分享的廣告氛圍好吃。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 21: 突破敘事邊界-更多參考輸入-參考影片-2-2

[![突破敘事邊界-更多參考輸入-參考影片-2-2](assets/thumbnails/21-reference-asset-21-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference2.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference2.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 7

**Prompt:**

```text
明亮多彩的廣告片風格，果味餅乾為主角，包含草莓、蘋果、葡萄、橙子四種口味，草莓味參考<<<image_1_1>>>，餅乾與對應水果以強秩序感的幾何陣列排布，整體畫面乾淨、高級、節奏強。開場水果快速建立視覺聚焦，參考<<<video_1_2>>>的構圖，音樂重拍切入。隨後不同口味餅乾整齊排列，切特寫，參考<<<video_2_3>>>的動態和運鏡。高潮段一塊餅乾被折斷，瞬間進入慢動作，果味夾心爆開，碎屑飛濺，果汁感與顆粒衝擊被放大展示，參考<<<video_3_4>>>的衝擊感。橫向陣列，形成節奏拋物感，參考<<<video_4_5>>>的移動，突顯秩序美感與產品豐富度。隨後迅速回到快節奏剪輯。結尾英文文字 One bite of crispness, a heart full of delight 快速分詞切換入畫，配合強節奏文字運動與產品定格，參考<<<video_5_6>>>，最終品牌感收束，餅乾和水果向四周發散，參考<<<video_6_7>>>，畫面充滿年輕、活力、好吃、想分享的廣告氛圍好吃。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 22: 突破敘事邊界-更多參考輸入-參考影片-2-3

[![突破敘事邊界-更多參考輸入-參考影片-2-3](assets/thumbnails/22-reference-asset-22-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference3.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference3.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 7

**Prompt:**

```text
明亮多彩的廣告片風格，果味餅乾為主角，包含草莓、蘋果、葡萄、橙子四種口味，草莓味參考<<<image_1_1>>>，餅乾與對應水果以強秩序感的幾何陣列排布，整體畫面乾淨、高級、節奏強。開場水果快速建立視覺聚焦，參考<<<video_1_2>>>的構圖，音樂重拍切入。隨後不同口味餅乾整齊排列，切特寫，參考<<<video_2_3>>>的動態和運鏡。高潮段一塊餅乾被折斷，瞬間進入慢動作，果味夾心爆開，碎屑飛濺，果汁感與顆粒衝擊被放大展示，參考<<<video_3_4>>>的衝擊感。橫向陣列，形成節奏拋物感，參考<<<video_4_5>>>的移動，突顯秩序美感與產品豐富度。隨後迅速回到快節奏剪輯。結尾英文文字 One bite of crispness, a heart full of delight 快速分詞切換入畫，配合強節奏文字運動與產品定格，參考<<<video_5_6>>>，最終品牌感收束，餅乾和水果向四周發散，參考<<<video_6_7>>>，畫面充滿年輕、活力、好吃、想分享的廣告氛圍好吃。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 23: 突破敘事邊界-更多參考輸入-參考影片-2-4

[![突破敘事邊界-更多參考輸入-參考影片-2-4](assets/thumbnails/23-reference-asset-23-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference4.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference4.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 7

**Prompt:**

```text
明亮多彩的廣告片風格，果味餅乾為主角，包含草莓、蘋果、葡萄、橙子四種口味，草莓味參考<<<image_1_1>>>，餅乾與對應水果以強秩序感的幾何陣列排布，整體畫面乾淨、高級、節奏強。開場水果快速建立視覺聚焦，參考<<<video_1_2>>>的構圖，音樂重拍切入。隨後不同口味餅乾整齊排列，切特寫，參考<<<video_2_3>>>的動態和運鏡。高潮段一塊餅乾被折斷，瞬間進入慢動作，果味夾心爆開，碎屑飛濺，果汁感與顆粒衝擊被放大展示，參考<<<video_3_4>>>的衝擊感。橫向陣列，形成節奏拋物感，參考<<<video_4_5>>>的移動，突顯秩序美感與產品豐富度。隨後迅速回到快節奏剪輯。結尾英文文字 One bite of crispness, a heart full of delight 快速分詞切換入畫，配合強節奏文字運動與產品定格，參考<<<video_5_6>>>，最終品牌感收束，餅乾和水果向四周發散，參考<<<video_6_7>>>，畫面充滿年輕、活力、好吃、想分享的廣告氛圍好吃。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 24: 突破敘事邊界-更多參考輸入-參考影片-2-5

[![突破敘事邊界-更多參考輸入-參考影片-2-5](assets/thumbnails/24-reference-asset-24-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference5.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference5.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 7

**Prompt:**

```text
明亮多彩的廣告片風格，果味餅乾為主角，包含草莓、蘋果、葡萄、橙子四種口味，草莓味參考<<<image_1_1>>>，餅乾與對應水果以強秩序感的幾何陣列排布，整體畫面乾淨、高級、節奏強。開場水果快速建立視覺聚焦，參考<<<video_1_2>>>的構圖，音樂重拍切入。隨後不同口味餅乾整齊排列，切特寫，參考<<<video_2_3>>>的動態和運鏡。高潮段一塊餅乾被折斷，瞬間進入慢動作，果味夾心爆開，碎屑飛濺，果汁感與顆粒衝擊被放大展示，參考<<<video_3_4>>>的衝擊感。橫向陣列，形成節奏拋物感，參考<<<video_4_5>>>的移動，突顯秩序美感與產品豐富度。隨後迅速回到快節奏剪輯。結尾英文文字 One bite of crispness, a heart full of delight 快速分詞切換入畫，配合強節奏文字運動與產品定格，參考<<<video_5_6>>>，最終品牌感收束，餅乾和水果向四周發散，參考<<<video_6_7>>>，畫面充滿年輕、活力、好吃、想分享的廣告氛圍好吃。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 25: 突破敘事邊界-更多參考輸入-參考影片-2-6

[![突破敘事邊界-更多參考輸入-參考影片-2-6](assets/thumbnails/25-reference-asset-25-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference6.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference6.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 7

**Prompt:**

```text
明亮多彩的廣告片風格，果味餅乾為主角，包含草莓、蘋果、葡萄、橙子四種口味，草莓味參考<<<image_1_1>>>，餅乾與對應水果以強秩序感的幾何陣列排布，整體畫面乾淨、高級、節奏強。開場水果快速建立視覺聚焦，參考<<<video_1_2>>>的構圖，音樂重拍切入。隨後不同口味餅乾整齊排列，切特寫，參考<<<video_2_3>>>的動態和運鏡。高潮段一塊餅乾被折斷，瞬間進入慢動作，果味夾心爆開，碎屑飛濺，果汁感與顆粒衝擊被放大展示，參考<<<video_3_4>>>的衝擊感。橫向陣列，形成節奏拋物感，參考<<<video_4_5>>>的移動，突顯秩序美感與產品豐富度。隨後迅速回到快節奏剪輯。結尾英文文字 One bite of crispness, a heart full of delight 快速分詞切換入畫，配合強節奏文字運動與產品定格，參考<<<video_5_6>>>，最終品牌感收束，餅乾和水果向四周發散，參考<<<video_6_7>>>，畫面充滿年輕、活力、好吃、想分享的廣告氛圍好吃。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 26: 突破敘事邊界-更多參考輸入-參考影片-2-7

[![突破敘事邊界-更多參考輸入-參考影片-2-7](assets/thumbnails/26-reference-asset-26-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference7.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference7.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 7

**Prompt:**

```text
明亮多彩的廣告片風格，果味餅乾為主角，包含草莓、蘋果、葡萄、橙子四種口味，草莓味參考<<<image_1_1>>>，餅乾與對應水果以強秩序感的幾何陣列排布，整體畫面乾淨、高級、節奏強。開場水果快速建立視覺聚焦，參考<<<video_1_2>>>的構圖，音樂重拍切入。隨後不同口味餅乾整齊排列，切特寫，參考<<<video_2_3>>>的動態和運鏡。高潮段一塊餅乾被折斷，瞬間進入慢動作，果味夾心爆開，碎屑飛濺，果汁感與顆粒衝擊被放大展示，參考<<<video_3_4>>>的衝擊感。橫向陣列，形成節奏拋物感，參考<<<video_4_5>>>的移動，突顯秩序美感與產品豐富度。隨後迅速回到快節奏剪輯。結尾英文文字 One bite of crispness, a heart full of delight 快速分詞切換入畫，配合強節奏文字運動與產品定格，參考<<<video_5_6>>>，最終品牌感收束，餅乾和水果向四周發散，參考<<<video_6_7>>>，畫面充滿年輕、活力、好吃、想分享的廣告氛圍好吃。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 27: 突破敘事邊界-秒畫面掌控-輸出-1

[![突破敘事邊界-秒畫面掌控-輸出-1](assets/thumbnails/27-narrative-control-27-second-level-frame-control-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group1/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group1/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 1

**Prompt:**

```text
3D 動畫廣告風，色彩明亮通透，果肉和汁水要有強烈的清爽感與衝擊力。整體氣質像高品質商業動畫短片，帶一點誇張幽默。沙漠角蜥角色可愛、靈動，表情豐富，參考<<<image_1_1>>>。畫面質感參考圖中那種柔和自然光、細膩絨毛 / 表皮質感、夢幻微距景深、真實中帶一點童趣 的感覺。
0-3 秒：畫面一片被烈日曝曬的沙漠。空氣熱得扭曲，沙地發燙，遠處像在冒煙。一隻沙漠角蜥 趴在滾燙的沙上，舌頭微微吐著，眼神渙散，快被曬乾了。它走兩步就晃一下，整隻沙漠角蜥像快要 “蒸發” 了。
音效熱浪呼呼聲，輕微誇張的乾裂聲。
3-6 秒：畫面沙漠角蜥突然停住，鼻子動了一下。它低頭一看，沙裡竟然埋著一顆 冰涼飽滿、帶著水珠的葡萄柚。葡萄柚在陽光下晶瑩發亮，表皮細膩，像沙漠裡突然出現的奇蹟。
表演蜥蜴眼睛瞬間瞪大，像看到救命稻草。
音效「叮」 一下的發現音效。
6-8 秒：畫面沙漠角蜥一個飛撲衝過去，雙手死死抱住葡萄柚，整張臉貼在果皮上。它露出 “終於活過來了” 的幸福表情。畫面定住 1 秒，形成一個誇張又好笑的廣告記憶點。
音效撲通一聲，隨後安靜半秒。
8-11 秒：畫面沙漠角蜥抓住葡萄柚。葡萄柚果皮裂開，裡面飽滿的果肉閃著透亮光澤。下一瞬間，汁水不是流出來，而是像海嘯一樣噴湧而出。
音效「喀嚓」 咬開聲，接一聲誇張的果汁爆開聲。
11-16 秒：畫面橙粉色、清透發亮的葡萄柚汁水瘋狂湧出，順著沙丘傾瀉，迅速淹沒整片沙漠。乾燥的黃沙瞬間變成一片 清涼、閃光、帶著果香感的夏日海洋。沙漠裡的仙人掌、石頭、小沙丘紛紛被果汁海浪吞沒，畫面誇張夢幻。
表演沙漠角蜥剛開始還很興奮，下一秒發現不對，表情從驚喜變成驚恐。
16-20 秒：畫面沙漠角蜥差點被 「葡萄柚海」 淹沒，慌忙死死抱住半顆葡萄柚，像抱著救生圈一樣漂浮在海面上。它濕漉漉地探出頭，表情一臉懵。海面波光粼粼，顏色像被陽光照亮的果汁。
音效誇張撲騰聲，海浪聲，帶一點喜劇感。
20-23 秒：畫面突然切白畫面。螢幕正中出現品牌字樣和 slogan：“Seedance 葡萄柚，咬開的是果肉，湧出來的是夏天。”
旁白念出整句：“Seedance 葡萄柚，咬開的是果肉，湧出來的是夏天。”
音效乾淨清爽的品牌提示音。
23-29 秒：畫面白螢幕切回。沙漠角蜥已經悠閒地坐在漂浮的葡萄柚上，戴著一副小墨鏡，抱著吸管杯，慢悠悠漂在 “果汁海面” 上度假。周圍漂著橘色果肉、小冰塊、清涼水花，天空變得湛藍，氣氛一下子從 「求生」 變成 「度假」。最後沙漠角蜥滿足地靠在葡萄柚上，鏡頭拉遠，定格在清爽、明亮、好玩的夏日畫面。
音效輕鬆夏日音樂，海浪輕拍聲。
字幕可只保留品牌名，不必加太多字。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 28: 突破敘事邊界-秒畫面掌控-輸出-2

[![突破敘事邊界-秒畫面掌控-輸出-2](assets/thumbnails/28-narrative-control-28-second-level-frame-control-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group2/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group2/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 1

**Prompt:**

```text
30 秒电影级青春竞速剧情短片，2d 动画风格。主角是少年車手，駕駛機車參加高規格比賽。整体风格热血、青春、情感强烈、电影感强，具有完整起承转合和清晰情绪弧线。全片僅使用兩種運鏡：高速跟拍、慢動作環繞。台词极少，自然像记忆碎片一样出现，语气真挚、温柔、克制，不喊口号，不过度煽情。不要災難感、不要負面表達、不要誇張科幻。重點突顯青春競速中的愛、支撐、反擊與成長。
0 秒到 5 秒
黄昏赛道，高速激烈竞速开场。鏡頭緊貼地面高速跟拍少年機車，輪胎掠過賽道邊線，機車轟鳴，風聲凌厲，氣氛緊張熾熱。少年全神貫注，夕陽在車身金屬外殼上拉出鋒利高光。
5 秒到 9 秒
進入關鍵彎道後，少年被對手突然超越。高速跟拍繼續推進，畫面表現出排名下滑和節奏被打亂的壓迫感。頭盔內近景出現短暫失神、呼吸發緊、輕微動搖。少年低声说：“Can I still catch up...”
9 秒到 14 秒
少年落在後方，呼吸加重，情緒跌入低谷。比赛没有停止，机车仍在高速前进。畫面開始在高速騎乘中閃回溫暖記憶碎片：童年學車時，有人從身後扶住他；父親替他整理頭盔，動作細緻而安靜；終點前，一個溫柔注視他的笑容；黃昏坡道上，並肩走過的背影。這些記憶都以金色逆光、柔和慢動作、片段化感受呈現。
14 秒到 18 秒
音乐从压抑逐渐转向昂扬。記憶中傳來克製而溫柔的聲音：「Don't be afraid — I'm always here.」「Stay steady.And look forward.」少年眼神重新聚焦，呼吸慢慢穩定，情緒從動搖轉為堅定。
18 秒到 23 秒
少年重新找回信念，全力提速，精準切線反擊。高速跟拍表現機車壓彎、出彎、逼近前車的力量感與控制力。少年低聲而堅定地說：“I won't stop here.”
23 秒到 27 秒
前方出現一段上揚賽道，少年迎著夕陽全速衝刺。畫面只保留呼吸聲、引擎聲和持續抬升的音樂，不再加入多餘台詞。機車借助慣性騰空而起，進入震撼慢動作。記憶深處最後傳來一句帶笑的溫柔聲音：“Go on.”
27 秒到 30 秒
攝影機圍繞著半空中的機車進行慢動作環繞特寫。將熱血、溫柔、自由、向上飛躍的情緒推向高潮。身後開出繁花特效，隨後出現seedance，參考<<<image_1_1>>>
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

## 拓展多語言呈現

### Case 29: 拓展多語種呈現-多語種表達-輸出-1

[![拓展多語種呈現-多語種表達-輸出-1](assets/thumbnails/29-multilingual-expression-29-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group1/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group1/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 11

**Prompt:**

```text
一镜到底 FPV 无人机第一视角视频，33 秒连续长镜头，无剪辑、无跳切、无转场。镜头从高空云端内部开始，沿云层、雾气、光影、山谷、瀑布、湖面、花田、城市建筑与近地广场形成一条连续下降飞行动线。全程依次出现 11 个清晰独立的语言展示区块，每个区块只显示对应单一语言文字，不混排、不叠加、不新增其他语言。
0–3 秒，<<<image_1_1>>>云团自然形成中文 “你好”；
3–6 秒，<<<image_2_2>>>薄雾和体积光形成英语 “Hello”；
6–9 秒，<<<image_3_3>>>高空水汽与阳光投影形成西班牙语（墨西哥）“Hola”；
9–12 秒，<<<image_4_4>>>空中丝带形成印度尼西亚语 “Halo”；
12–15 秒，<<<image_5_5>>>風箏編隊形成馬來語 “Hai”；
15–18 秒，<<<image_6_6>>>山谷晨雾形成泰语 “สวัสดี”；
18–21 秒，<<<image_7_7>>>瀑布水雾形成阿拉伯语مرحبا
21-24 秒，<<<image_8_8>>>湖面倒影和水波光纹形成葡萄牙语“Olá”；
24–27 秒，<<<image_9_9>>>花田与草地自然排列成越南语 “Xin chào”；
27–30 秒，<<<image_10_10>>>城市玻璃建筑反射光影形成日语 “こんにちは”；
30–33 秒，<<<image_2_2>>>0 近地广场喷泉水雾、地面铺装和灯带形成韩语 “안녕하세요”。
整体为清晨日出氛围，金色逆光、柔和体积光、真实云雾、自然运动模糊、电影级真实感。镜头速度从 3–5 m/s 慢速启动，逐渐加速到 14–16 m/s 穿越自然景观，再减速到 2–3 m/s 于近地广场稳定悬停。镜头参数：广角镜头，24fps，平滑 FPV drone movement，pitch 从 -5° 逐步过渡到 -18°，最后回到 0°；轻微 yaw ±10°，roll 控制在 0–10°，保证连续、稳定、真实的一镜到底飞行感。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 30: 拓展多語種呈現-多語種表達-輸出-2

[![拓展多語種呈現-多語種表達-輸出-2](assets/thumbnails/30-multilingual-expression-30-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group2/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group2/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 9

**Prompt:**

```text
真人實拍風格，快速剪輯，電影感，4K，24fps，溫暖自然光，真實人物表演，自然口型同步，無字幕。以一朵花的傳遞作為整支影片的核心視覺線索，花從一個國家快速傳到下一個國家，串聯全球不同地域與人群。每到一個場景，都有一個人物接過花、露出真誠微笑，並用當地語言說 “謝謝”。整體節奏輕快流暢，鏡頭富有動感，強調真實街頭 / 生活氣息、跨文化溫暖連結、人與人之間的善意傳遞。
轉場方式：以前一個人物把花遞出畫面，下一個鏡頭由另一個人物在新場景中接住花
或使用快速甩鏡、運動模糊、前景遮擋完成無縫轉場
保持花在畫面中的視覺連續性，形成 「一鏡傳全球」 的感覺
鏡頭風格：手持跟拍、輕微鏡頭晃動、快速推拉、近景與中景結合、真實環境音氛圍、電影級街拍質感。背景音樂溫馨、輕快、有世界旅行感，結尾溫柔淡出。
場景 1<<<image_1_1>>>中國花店內，真實生活化場景。女孩接過一枝玫瑰，看向鏡頭微笑，自然地說：「謝謝！」鏡頭跟隨花從畫面右側遞入，女孩接花後輕輕揚起花束。
場景 2<<<image_2_2>>>英格蘭街頭，微涼天氣，街景自然。男士接過一枝康乃馨，微笑點頭，說：「Thank you!」透過甩鏡轉場，花從上一場景甩入這一場景。
場景 3<<<image_3_3>>>墨西哥市場，色彩豐富，充滿煙火氣。阿姨接過一束萬壽菊，雙手合十，溫暖地說：「¡Gracias!」鏡頭快速掠過攤位與人群，定格在接花瞬間。
場景 4<<<image_4_4>>>印尼鄉村，自然陽光灑落。孩子接過一朵雞蛋花，開心微笑，微微鞠躬，說：「Terima kasih!」鏡頭帶一點奔跑感，氛圍純真自然。
場景 5<<<image_5_5>>>泰國街頭，熱鬧市井。攤販接過一串茉莉花環，雙手合十，親切地說：「ขอบคุณค่ะ!」鏡頭輕快推進，花環在陽光下微微擺動。
場景 6<<<image_6_6>>>阿拉伯庭院，光影柔和，環境優雅。女士接過一枝沙漠玫瑰，撫胸微笑，說：「شكراً!」畫面安靜而溫暖，人物神情真摯。
場景 7<<<image_7_7>>>巴西社區，氣氛熱情鮮活。男孩接過一朵非洲菊，十分開心，說：「Obrigado!」鏡頭富有節奏感，充滿生命力。
場景 8<<<image_8_8>>>日本街道，上班族接過便當上的一朵小花，禮貌鞠躬，說：「ありがとう！」鏡頭短促利落，保留都市節奏感。
場景 9<<<image_9_9>>>韓國街頭，現代都市感。女青年接過一枝杜鵑花，雙手自然合攏，微笑說：「감사합니다!」鏡頭在她微笑的瞬間稍作停留，隨後畫面柔和淡出。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

## 深化可控編輯

### Case 31: 可控編輯 1 輸出

[![可控編輯 1 輸出](assets/thumbnails/31-controllable-editing-31-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 2

**Prompt:**

```text
保持<<<video_1_1>>>中的人物、丛林环境、镜头运动、构图、动作节奏和时长不变。
人物手中緩緩出現藍白色能量弓與一支發光箭矢<<<image_1_2>>>，弓身由微弱電弧和粒子逐漸聚合成形，帶細膩流動的電流紋理、輕微體積光和穩定的能量輪廓。拉弓過程中，箭矢在弓弦中央凝聚成高亮能量箭，人物鬆手瞬間，箭矢高速射出，留下一道明亮細長、連續銳利的能量軌跡
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 32: 可控編輯 1 參考

[![可控編輯 1 參考](assets/thumbnails/32-controllable-editing-32-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/reference1.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/reference1.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 2

**Prompt:**

```text
保持<<<video_1_1>>>中的人物、叢林環境、鏡頭運動、構圖、動作節奏和時長不變。
人物手中緩緩出現藍白色能量弓與一支發光箭矢<<<image_1_2>>>，弓身由微弱電弧和粒子逐漸聚合成形，帶細膩流動的電流紋理、輕微體積光和穩定的能量輪廓。拉弓過程中，箭矢在弓弦中央凝聚成高亮能量箭，人物鬆手瞬間，箭矢高速射出，留下一道明亮細長、連續銳利的能量軌跡
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 33: 可控編輯 2 輸出

[![可控編輯 2 輸出](assets/thumbnails/33-controllable-editing-33-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 1

**Prompt:**

```text
刪除<<<video_1_1>>>畫面中的無人機以及左下角前景軌道 / 車體邊緣，對刪除區域進行自然補全。
保持長頸鹿群、樹木枝幹、遠處草原、金色夕陽逆光、空氣透視和鏡頭構圖完全不變。補全後的背景應與周圍環境一致，產生自然的天空、樹枝間隙和草地細節，不要出現塗抹感、閃爍、形變、重影或跳動。確保影片前後幀時序一致、運動連續，邊緣過渡自然，整體像原始實拍畫面。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 34: 可控編輯 2 參考

[![可控編輯 2 參考](assets/thumbnails/34-controllable-editing-34-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/reference1.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/reference1.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 1

**Prompt:**

```text
刪除<<<video_1_1>>>畫面中的無人機以及左下角前景軌道 / 車體邊緣，對刪除區域進行自然補全。
保持長頸鹿群、樹木枝幹、遠處草原、金色夕陽逆光、空氣透視和鏡頭構圖完全不變。補全後的背景應與周圍環境一致，產生自然的天空、樹枝間隙和草地細節，不要出現塗抹感、閃爍、形變、重影或跳動。確保影片前後幀時序一致、運動連續，邊緣過渡自然，整體像原始實拍畫面。
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 35: 可控編輯 3 輸出

[![可控編輯 3 輸出](assets/thumbnails/35-controllable-editing-35-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/output.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/output.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 4

**Prompt:**

```text
將兩人武打素版影片<<<video_1_1>>>替換為冷兵器對決前的空手試探風。
場景替換為中世紀石堡平台、古老庭院平地、山間堡壘外平台或簡潔石磚決鬥場，背景為古堡牆體、風、霧、遠處山線，地面平整石質<<<image_1_2>>>。
影片中深色衣服的男子的服飾替換為<<<image_2_3>>>，影片中淺色衣服的男子替換為<<<image_3_4>>>。動作仍然保持不變，不改變原始節奏。
AI 特效只做環境和質感強化：風吹衣擺、輕霧、接觸點少量塵土、金屬冷色反光質感、輕微顆粒和史詩感調色。整體風格為克制、真實、古典硬派決鬥氛圍。背景音樂卡點
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

### Case 36: 可控編輯 3 參考

[![可控編輯 3 參考](assets/thumbnails/36-controllable-editing-36-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/reference1.mp4)

[播放影片](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/reference1.mp4) · 點擊縮圖即可播放影片。

**參考素材:** 4

**Prompt:**

```text
將兩人武打素版影片<<<video_1_1>>>替換為冷兵器對決前的空手試探風。
場景替換為中世紀石堡平台、古老庭院平地、山間堡壘外平台或簡潔石磚決鬥場，背景為古堡牆體、風、霧、遠處山線，地面平整石質<<<image_1_2>>>。
影片中深色衣服的男子的服飾替換為<<<image_2_3>>>，影片中淺色衣服的男子替換為<<<image_3_4>>>。動作仍然保持不變，不改變原始節奏。
AI 特效只做環境和質感強化：風吹衣擺、輕霧、接觸點少量塵土、金屬冷色反光質感、輕微顆粒和史詩感調色。整體風格為克制、真實、古典硬派決鬥氛圍。背景音樂卡點
```

> [!NOTE]
> 這個官方案例還包含 manifest 中列出的參考素材。

---

## 📁 倉庫結構

```text
.
├── README.md
├── README.<lang>.md
├── assets/
│   ├── banner.png
│   └── thumbnails/
├── data/
│   ├── seedance-2-5-manifest.json
│   └── seedance-2-5-prompt-translations.json
└── use-cases/
    ├── README.md
    ├── en/
    │   ├── README.md
    │   ├── 01-consistency.md
    │   └── official-seedance-2-5-guide.md
    └── <lang>/
        ├── README.md
        └── official-seedance-2-5-guide.md
```

## 🙏 致謝

本倉庫由 EvoLink 維護，作為 Seedance 2.5 early access 的公開 guide。

- Official early access: [Get Seedance 2.5 Early Access](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide)
- Current API key path: [EvoLink signup](https://evolink.ai/signup?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide)
- Current API examples: [Seedance 2.5 Gateway Service](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)
