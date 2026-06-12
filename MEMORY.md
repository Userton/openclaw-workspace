# MEMORY.md - 夥計的長期記憶

> 這裡是我的腦袋——重要的事情、決定、喜好、以後要記住的東西。

---

## 👤 關於鴻哥

- 名字：鴻哥
- 時區：Asia/Taipei (GMT+8)
- 2026-05-19 首次對話

---

## 📌 重要記事

### 2026-06-09 Agnes AI 接入 OpenClaw
- Agnes AI 已設為輔助模型（`agnes/agnes-2.0-flash`、`agnes/agnes-1.5-flash`）
- Base URL: `https://apihub.agnes-ai.com/v1`，Provider ID: `agnes`
- API Key: `sk-bxw…DfOr`（寫入 `openclaw.json`）
- 注意：`input` 必須是 `["text"]` 陣列格式，否則 validation 失敗

### 2026-06-09 Docker 擴充功能
- Portainer `:9000`（Docker 管理介面）
- n8n `:5678`（工作流自動化）
- SearXNG `:8888`（私人搜尋引擎）
- OpenWebUI `:3000`（Ollama Web UI）
- Anything-LLM `:3001`（文件問答）
- Anything-LLM 安裝需加 `--user root:root`，環境變數 `STORAGE_DIR=/app/anything-llm`
- Watchtower 安裝失敗（Docker API 版本不相容）

### 備份位置（2026-06-10 更新）
- 備份全部改到 `D:\openclaw-backups`
- 涵蓋：增量備份、災難復原、驗證

### 2026-06-10 四大模組強化（已完成）
- 📱 快捷指令學習自動化（command_learn + auto_learn + intent_detector）
- 📋 待辦系統強化（四象限 + 截止提醒）
- 🧠 錯誤學習記錄（預防引擎 + 教訓庫）
- 🌐 統一控制中心（unified_home.html，61KB）

### 2026-06-10 遠端存取安全化（已完成）
- WireGuard VPN + 反向代理 + DDNS
- 全部 PowerShell 編碼修復完成

### 2026-06-10 自動化報告系統（已完成）
- LINE 每日/每週報告（排程已就緒）
- 知識庫成長追蹤報告

### 2026-06-10 語音強化（已完成）
- Edge TTS 柔美女性音色（預設）
- 🌸 甜美少女：zh-CN-XiaoxiaoNeural
- 🎙️ 專業主播：zh-CN-YunyangNeural
- PyTorch CUDA 版安裝成功（2.7.1+cu118）

### 2026-06-02 先知知識庫 架設完成
- Docker Desktop + Ollama (nomic-embed-text) + qdrant 已就緒
- 知識庫：「先知」，collection: zhi_xian
- 腳本：knowledge_base_watcher.py（監控）、knowledge_search.py（搜尋）
- 路徑：C:\Users\user\Documents\知識庫
- OpenClaw RAG 已設定，問相關問題會自動搜尋

### 2026-05-22 《築基》第一集 完成
- Windows TTS（HuHan Desktop）修復成功，生成 6 段中文配音（win_cn_1~6.wav）
- 桌面 `C:\Users\user\Desktop\築基\`：場景圖 × 6、配音 × 6、樂曲、劇本、影片
- 影片 `築基_對話版.mp4`（30秒，6場景，配音精準對位）
- 待鴻哥確認第1集效果後再繼續

---

## 🎯 重要原則（鴻哥的要求）

### 🚨 完成程序後發出提示音（不可違背）
- **每次完成任何程序/任務後，必須立即播放提示音**
- 使用 Windows SAPI（Microsoft Hanhan Desktop）
- 腳本：`python C:\Users\user\.openclaw\workspace\scripts\say_done_edge.py`

### 🎵 音樂播放器原則
- **指定使用 PotPlayer 播放本地音樂檔案**
- 音樂資料夾：`D:\新歌2026`
- 路徑：`C:\Program Files\DAUM\PotPlayer\PotPlayerMini64.exe`

### 🌐 Gateway 安全原則
- **Gateway 必須綁定在 127.0.0.1（loopback），禁止暴露到外部網路**

---

_更新於 2026-06-02_
