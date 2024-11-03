> 以下內容及程式實現不是由我本人原創，而是基於以下專案的 fork 版本：
> - https://github.com/joshpocock/agent.exe 
> - https://github.com/corbt/agent.exe

---

# Agent.exe
提供 **Agent.exe**：讓 Claude 的新[電腦使用](https://www.anthropic.com/news/3-5-models-and-computer-use)功能最簡單地控制您的電腦！

### 動機
我想測試 Claude 的新[電腦使用](https://www.anthropic.com/news/3-5-models-and-computer-use) API 的效果如何，而他們提供的預設專案感覺太過笨重。這是一個簡單的 Electron 應用程式，可讓 Claude 3.5 Sonnet 直接控制您的本地電腦。我原本計劃添加一個「半自動」模式，讓用戶在每個動作執行前都需要確認，但由於每個步驟都很慢，我發現這並非必要，而且如果模型出現混亂，您可以輕鬆地按下「停止」按鈕來結束運行。

### 開始使用
1. `git clone https://github.com/corbt/agent.exe`
2. `cd agent.exe`
3. `npm install`
4. 將 `.env.example` 重新命名為 `.env` 並添加您的 Anthropic API 密鑰
5. `npm start`
6. 提示模型在您的電腦上做一些有趣的事情！

### 支援的系統
- MacOS
- 理論上支援 Windows 和 Linux，因為所有依賴包都是跨平台的

### 已知限制
- 僅適用於主要顯示器
- 讓 AI 完全控制您的電腦
- 噢天啊，可能還有很多其他限制

### 使用技巧
- Claude *非常*喜歡 Firefox。如果必要的話它會使用其他瀏覽器，但如果您安裝 Firefox 並讓它進入它的快樂天地，它的表現會好得多。

### 發展規劃
- 我實際上只花了 6 小時寫這個，可能不會有太多後續發展。但我會審查 PR 並在覺得不錯的情況下合併它們。

---

Presenting **Agent.exe**: the easiest way to let Claude's new [computer use](https://www.anthropic.com/news/3-5-models-and-computer-use) capabilities take over your computer!

### Motivation
I wanted to see how good Claude's new [computer use](https://www.anthropic.com/news/3-5-models-and-computer-use) APIs were, and the default project they provided felt too heavyweight. This is a simple Electron app that lets Claude 3.5 Sonnet control your local computer directly. I was planning on adding a "semi-auto" mode where the user has to confirm each action before it executes, but each step is so slow I found that wasn't necessary and if the model is getting confused you can easily just hit the "stop" button to end the run.

### Getting started
1. `git clone https://github.com/corbt/agent.exe`
2. `cd agent.exe`
3. `npm install`
4. Rename `.env.example` --> `.env` and add your Anthropic API Key
5. `npm start`
6. Prompt the model to do something interesting on your computer!

### Supported systems
- MacOS
- Theoretically Windows and Linux since all the deps are cross-platform

### Known limitations
- Only works on the primary display
- Lets an AI completely take over your computer
- Oh jeez, probably lots of other stuff too

### Tips
- Claude *really* likes Firefox. It will use other browsers if it absolutely has to, but will behave so much better if you just install Firefox and let it go to its happy place.

### Roadmap
- I literally wrote this in 6 hours, probably isn't going anywhere. But I will review PRs and merge them if they seem cool.
