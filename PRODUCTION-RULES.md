# 中國神話故事 - 製作規則（VideoExpress 專業版 v2.1）

基於 VideoExpress + CloneVoice Stickman Story Workflow 最佳實踐，並依實際製作（帝江集）更新。

最後更新：2026-10-09

---

## 0. 系列固定風格（優先於下文任何舊敘述）

- 角色：一律 3D 皮克斯風格
- 背景：一律水彩畫風格
- 旁白：中文繁體，結尾固定台詞見第 1 節
- 主片與 Shorts 風格必須一致；Shorts 從主片擷取，不重新生成

## 1. 選題與故事規劃

- 來源：《山海經》或其他古籍
- 主片長度：約 1 分鐘（可依故事自然完整，實際帝江集約 4 分鐘）
- 避免重複：女媧補天、牛郎織女已做過
- 教育意義優先於娛樂性

故事架構：
1. 開場：固定格式「中國神話故事」＋集數標題卡
2. 故事發展：beginning → development → memorable turn → ending
3. 結尾：「中國神話故事 END」＋男性旁白：「小朋友喜歡這樣的中國神話故事嗎？我們下次再一起冒險！」

製作前必建「故事 Ledger」：場景 ID、旁白文稿、必需角色/道具及數量、來場狀態、主要動作、離場狀態、下一場連接、備註。

## 2. 主角設計（Master Character）

1. 任何場景之前，先獨立製作一張主角 Master Character 圖（純白中性背景、放鬆三角站姿、雙手雙腳可見）。
2. 風格：3D 皮克斯角色。
3. 每個故事選新的主角名稱，故事內保持一致。
4. 保存為「故事標題 — Master Character」，啟用 Use Consistent Character，設為 Reference Photo 1，全程不變。

## 3. 場景環境設計

- 每個新位置做一張獨立環境參考圖（不含主角），作為 Reference Photo 2。
- 重複出現的位置寫下固定佈局（左/中/右/上/地面）與固定攝影機視角。
- 每場景重複相同佈局描述；拒絕鏡像、移動地標、無故改變視角。

## 4. 場景動作連貫性

- 先把整支影片設計為一個有序動作序列，建立 Continuity Table。
- Scene N 的離場狀態 = Scene N+1 的來場狀態。
- 追蹤角色位置、姿勢、面向、視線、持物；故事關鍵物件數量與身份穩定。
- 禁止無故重置姿勢、重複動作迴圈、意外視角跳躍。

## 5. 場景圖像生成

VideoExpress 設定（每個故事一次）：寬高比 16:9（或 9:16，需一致）、Creative Mode OFF、自動增強提示 OFF、Advanced Mode OFF、Choose my Audio ON、Lipsync HD OFF、公開分享 OFF。

每個圖像提示必須包含：Scene ID、寬高比、風格（3D 皮克斯＋水彩背景）、精確敘述時刻、角色身份與數量/服裝/表情/姿勢、螢幕位置與面向、道具數量與位置、前中後景、場景地理與地標、鏡頭與構圖、光線與時間、與相鄰鏡頭的連貫性。

圖像審查（動畫前）：身份、解剖、道具計數、連貫性、地標、視線。不接受未來完成的動作、重置狀態、移動或翻轉的地標。

快速製作：一圖通過審查 → 生成一支視頻 → 下一場景；每場景最多重試 3 次。

## 6. 配音（CloneVoice）

- Voice：Beau Whitaker（已授權）；語言：中文繁體；每場景 3–5 秒自然語速。
- TTS 文本框只放該場景旁白，不含場景標籤或時間戳。
- 流程：輸入提示 → Choose my Audio → Create Video → CloneVoice → 輸入旁白 → 生成 → 記錄 Job ID → 準備下一場景（可同時最多 5 支渲染）。

## 7. 組合與導出

- Media Library → My AI Videos → Add to Timeline，依序、每場景一次，確認軌道正確。
- Auto Align Clips 後驗證無間隙/重疊，保存專案。
- 導出：MP4、1080p、High。

## 8. YouTube 上傳設定

- 標題：中英雙語，格式「中國神話故事 - [故事名稱] | [English title]」
- 描述：中文一段＋英文一段；英文段落註明 Shan Hai Jing 出處、「Chinese narration with subtitles」、AI 生成內容聲明
- 英文標籤：#ChineseMythology #ShanHaiJing #KidsStories #BedtimeStory #MythologyForKids＋該集神獸英文名
- 分類：教育；為兒童打造：是（YouTube 會因此停用留言與通知）
- AI 內容聲明：是
- 主片發布：每週六 20:00（GMT+8）
- 縮圖：1280×720，與影片風格一致，含故事名稱

## 9. YouTube Shorts 策略（已依帝江集實作更新）

- 規格：每集 3 支，15–20 秒，9:16（1080x1920，30fps）
- 製作方式：從已完成的主片擷取，ffmpeg 轉直式（boxblur 背景補滿）、保留原字幕與音軌、淡入 0.3 秒/淡出 0.4 秒；不在 VideoExpress 重新生成（省點數、風格一致）
- 選段：該集最有視覺記憶點、核心設定揭示、情感收尾各一支
- 中英雙語標題與描述，描述附主片連結
- 排程：主片先公開，Shorts 一律晚於主片，一天最多一支。帝江集範例：主片週六 20:00，Short 1 週六 20:30，Short 2 週日 10:00，Short 3 週一 19:30

## 10. 重要約束

- 不刪除已發布專案或庫存媒體
- 發布前確認所有設定；排程前再核對一次時間與連結
- 保持 Ledger 完整記錄

參考：VideoExpress + CloneVoice Stickman Story Workflow（https://community.dualup.com/@videoexpress/workflows/videoexpress-clonevoice-stickman-story-workflow）、https://app.videoexpress.ai/
