# Will you be my Valentine?

一個情人節趣味小網頁：問「Will you be my Valentine?」，Yes 可點、No 會逃跑，點 Yes 後顯示「I knew you'd say yes」。粉色泡泡風格，純 HTML / CSS / JS，無需後端。

## 內容

- **第一頁**（`index.html`）：標題、Yes / No 按鈕；滑鼠靠近 No 時按鈕會隨機移動，難以點到。
- **第二頁**（`yes.html`）：點 Yes 後跳轉，顯示「I knew you'd say yes」。

## 本地執行

直接開啟 `index.html`，或用任意靜態伺服器：

```bash
# 例如用 Python
python3 -m http.server 8000
# 瀏覽器開啟 http://localhost:8000
```

## 部署到 GitHub Pages（取得公開網址）

1. 把此專案 push 到 GitHub 的某個 repo（例如 `valentine`）。
2. 到該 repo：**Settings → Pages**。
3. **Source** 選 **Deploy from a branch**。
4. **Branch** 選 `main`（或你使用的預設分支），資料夾選 **/ (root)**，儲存。
5. 幾分鐘後網址會是：`https://<你的帳號>.github.io/valentine/`（repo 名為 `valentine` 時）。

用這個 URL 就能在網路上分享，不需在本地執行。

## 檔案說明

| 檔案 | 說明 |
|------|------|
| `index.html` | 首頁：問句與 Yes / No 按鈕，No 有逃跑效果 |
| `yes.html` | 點 Yes 後的感謝頁 |
| `README.md` | 本說明檔 |

## 技術

- 純前端：HTML、CSS、JavaScript，無框架。
- 泡泡動畫為 CSS `@keyframes`，No 按鈕移動為 `position: fixed` + 隨機座標。
