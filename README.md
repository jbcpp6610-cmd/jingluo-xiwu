# 鲸落汐屋

一个短篇视觉小说。海边小镇、只卖汤的小店、一位蓝鲸鱼娘女仆，
三个晚上，四个结局。

**直接玩：** https://<你的用户名>.github.io/jingluo-xiwu/

## 玩法

- 点击画面 / 空格：推进对白
- 数字键 1–3：选择选项
- S / L：存档 / 读档
- 右上角：音乐、语音开关

## 实现

单页 HTML，无框架无构建。剧本写在页面里的 JSON 中，改剧情不用碰引擎。

- 配乐：Web Audio 实时合成（钟片 + 和声垫 + 鲸歌低频），七个场景各一套调式
- 人声：读取 `assets/voice/NN.wav`，文件不存在就静音跳过
- 存档：localStorage

## 文件

```
index.html          游戏本体
assets/B1..B8.webp  背景
assets/L1..L6.png   立绘
assets/voice/       人声（缺哪句就静音）
```
