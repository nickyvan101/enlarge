# ENLARGE

**ENLARGE** 是一套 Windows 桌面 AI 圖片放大工具，使用 SeedVR2 3B 模型與 TTP 分塊處理，在 NVIDIA GPU 上把圖片高保真放大到你指定的像素尺寸。

- 官方網站：https://www.101worlds.com
- 免費使用；可自由轉發完整且未修改的官方版本；**禁止轉售、付費散布與修改**
- 著作權：© 2026 Nic
- 完整授權：[EULA.txt](EULA.txt)

## 下載

請從 **Releases** 下載最新版安裝檔：

- `ENLARGE-Setup-x.y.z.exe`
- 官方模型透過 Hugging Face 模型頁下載（由 App 首次使用時一鍵處理，不放在 GitHub）
- 種子檔案與 SHA256 校驗值會附在 Release assets

> 本儲存庫只提供官方文件與發行檔，**不公開主程式原始碼**。請勿從非官方來源下載可執行檔。

## 系統需求

- Windows 10 / 11 x64
- NVIDIA RTX 顯示卡（建議 8GB VRAM 以上）
- 16GB RAM 以上
- 約 10GB 以上可用磁碟空間（首次下載元件與模型）
- 可連線至 GitHub、Hugging Face、PyTorch 與 Python 官方下載平台

## 首次使用

1. 安裝並啟動 ENLARGE。
2. 閱讀並同意 EULA。
3. 載入圖片、設定像素尺寸，按「開始放大」。
4. 首次使用會跳出元件下載視窗，一鍵下載：
   - SeedVR2 引擎（Apache-2.0；GitHub Releases）
   - Python 3.12 + PyTorch 2.10 CUDA 執行環境（官方平台）
   - SeedVR2 3B Q8 模型與 VAE（Hugging Face 官方模型頁）
5. 下載完成後會自動開始放大；之後啟動不再重複下載，除非元件有新版本。

元件與模型儲存在 `%LOCALAPPDATA%\ENLARGE`，程式更新不會刪除；移除程式時會詢問是否保留。

## 更新

- App 啟動時會檢查 GitHub Releases 最新版本，有新版會顯示通知。
- 可一鍵下載並執行新版安裝檔，直接覆蓋安裝，不需要先移除舊版。
- 若自動更新失敗，會提示開啟 GitHub Releases 下載頁。
- 引擎／模型更新由元件管理器處理，只下載變更部分。

## 模型與第三方元件

- SeedVR2 3B / ByteDance Seed：Apache-2.0
- AInVFX Q8 量化權重／numz 節點與 VAE：Apache-2.0
- Electron / Chromium / FFmpeg；PyTorch、Python、NumPy、Pillow、uv、adm-zip 等
- 完整授權與 attribution：[THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt) 與 [licenses](licenses/)

ENLARGE 與 ByteDance、AInVFX、numz、ComfyUI 無隸屬或背書關係。SeedVR2 屬生成式細節重建，非位元級無損；輸出 PNG 為無損格式，但生成內容可能與原圖有細微差異。

## 支持

如果這個工具對你有幫助，可以請我喝咖啡：https://www.101worlds.com/sponsor.html
