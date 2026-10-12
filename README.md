# 折射震測探究實驗室

可直接部署到 GitHub Pages 的純靜態互動式教學網站。

## 主要功能
- 自由指定敲擊位置：滑桿、預設位置、直接點地表
- 受波器數量：5 / 8 / 12 / 16 / 24
- 受波器間距：2 / 3 / 4 / 5 m
- 調整兩層地下模型：V1、V2、界面深度、環境雜訊
- 震波傳遞動畫：直達波與折射首波代表性路徑
- 多通道合成震波紀錄（wiggle plot）
- 單通道波形、direct / refracted arrival 與 first arrival
- 5 次重複敲擊疊加，觀察 SNR 改善
- distance–time travel-time curve 與 crossover distance
- 正向 / 反向敲擊
- 未知地下模型挑戰
- POE + CER 探究流程

## 物理模型
採水平兩層介質、V2 > V1 的簡化折射震測模型。

直達波：`t_direct = x / V1`

臨界角：`ic = asin(V1 / V2)`

截距時間：`t_i = 2 h cos(ic) / V1`

折射首波：`t_refracted = t_i + x / V2`

網站只有在 offset 足以形成臨界折射路徑時，才把折射波當成可用的實際 ray path，避免把截距直線外插區誤解為真實傳播路徑。

## GitHub Pages
此專案的靜態網站檔案位於 repository 根目錄：`index.html`、`style.css`、`script.js`。

若尚未啟用 Pages：Settings → Pages → Deploy from a branch → `main` → `/(root)`。
