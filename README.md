# 🎮 Cat & Flower Greeting Card 猫爪花花互动卡片游戏

🌸 **粉色版 / Pink Edition** | 🔵 **蓝色版 / Blue Edition**  
一个点击猫爪会开出莫奈风格小花的互动祝福游戏，支持自定义祝福语与配色，适合节日惊喜、表白、生日祝福等场景！

---

## 🧩 使用方式 | How to Use

1. 打开 `cat&flower card-pink.html`（或蓝色版对应文件）  
2. 点击「开始游戏」，追踪场景中的猫爪（白色透明球体）  
3. 成功点中猫爪后，会触发祝福卡片和互动动画  
4. 可以点击空白区域手动生成莫奈风格花朵

---

## 🎨 如何更改配色和文字 | How to Customize Colors & Text

### 🌸 更改祝福文字 | Customize Blessing Text

在 HTML 文件中搜索：

```js
const randomPhrases = [
    "身体健康","工作顺利","步步高升"       
];
````

将内容替换为你想展示的祝福语：

```js
const randomPhrases = [
    "节日快乐", "你是最棒的", "每天都闪闪发光"
];
```

> 多条内容将随机弹出，支持中文或英文。

---

### 🎯 更改游戏标题文字 | Change Main Titles

在 `<body>` 部分查找：

```html
<h1 id="pageTitle">Surprise!</h1>
<h6 id="pageSubTitle">努力选中小猫爪吧</h6>
```

胜利后的提示：

```html
<h1>🎂 520节日快乐 🎉</h1>
<p class="win-message-body">
    祝xxx520节日快乐！<br>
    希望这个小小互动能给你带来一丝惊喜和快乐！
</p>
```

> 可替换为任意纪念日/节日祝福文案。

---

### 🧁 更改配色风格（花瓣颜色）| Modify Color Palette

查找以下代码：

```js
const monetFlowerColorPalettes = [
    { name: "糖粉", h_range: [0, 10], s_range: [10, 20], b_range: [97, 100] },
    ...
];
```

你可以修改或添加颜色组合，例如：

```js
{ name: "薄荷绿", h_range: [120, 130], s_range: [20, 40], b_range: [90, 100] }
```

**说明：**

* `h_range` 是色相（Hue）：0=红色，120=绿色，240=蓝色。
* `s_range` 是饱和度（Saturation）：控制颜色的鲜艳程度。
* `b_range` 是亮度（Brightness）：越高越亮。

---

### 🎀 切换主题色 | Switch Between Pink & Blue Theme

按钮颜色代码：

```css
#startButton, #restartButton {
    background-color: #ff69b4;
}
```

将 `#ff69b4` 修改为你想要的颜色，例如：

* 粉色（默认）：`#ff69b4`
* 浅蓝色：`#1e90ff`
* 薄荷绿：`#3cb371`

---

## 💡 适用场景 | Recommended Scenarios

* 🎂 生日祝福卡片
* 💌 表白互动小游戏
* 🌸 节日惊喜小彩蛋（如520、情人节）
* 🖼️ 个人网页作品或创意展示页

---

## 🛠 技术栈 | Tech Stack

* 🎨 前端：HTML + CSS + JS
* 🎮 动画与交互：p5.js
* 🎁 零依赖，可本地打开使用，无需服务器

---

## 🐾 作者 | Author

林霏开 · May 2025
欢迎自由使用和二创，转载请注明出处～❤️
