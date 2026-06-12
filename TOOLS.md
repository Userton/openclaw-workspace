# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup.

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → 192.168.1.100, user: admin

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

## 🌐 瀏覽器自動化（Browser Relay）

Chrome Extension：OpenClaw Browser Relay

**使用流程：**
1. 安裝 OpenClaw Browser Relay 擴充功能
2. 開啟目標網頁，點擊擴展圖標，Badge 顯示 ON
3. 在聊天中直接讓夥計執行點擊、輸入、讀取等任務

**觸發關鍵字：**
- 「開啟網頁」、「點擊」、「輸入」、「讀取網頁」
- 「自動化這個頁面」、「幫我填表」

---

## 🎵 音樂播放器

- 指定使用 **PotPlayer** 播放本地音樂檔案
- 音樂資料夾：`D:\新歌2026`
- 路徑：`C:\Program Files\DAUM\PotPlayer\PotPlayerMini64.exe`

---

## 🔊 TTS 提示音

- 腳本：`C:\Users\user\.openclaw\workspace\scripts\say_done_edge.py`
- 每次完成程序/任務後**必須**立即播放
- 測試：`python say_done_edge.py "測試文字"`

---

Add whatever helps you do your job. This is your cheat sheet.

## Related

- [Agent workspace](/concepts/agent-workspace)
