# 🧬 BioForge-Antigravity-Workshop
### AI 時代的生物資訊與新藥研發：從蛋白質語言模型到 Agentic 生物計算防線

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vvchung/BioForge-Antigravity-Workshop/blob/main/BioForge_Antigravity_Workshop_2.ipynb)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![ESM-2](https://img.shields.io/badge/Model-Meta_ESM--2_8M-red.svg)](https://huggingface.co/facebook/esm2_t6_8M_UR50D)
[![DeepMind Antigravity](https://img.shields.io/badge/Workflow-DeepMind_Antigravity_Lead-orange.svg)](https://deepmind.google/blog/accelerating-antimicrobial-discovery/)
[![Clean Science](https://img.shields.io/badge/Scientific_Integrity-Zero_Paper_Mill-green.svg)](#-科學良心與極客守門員理念)

---

> **「在生醫領域，造假與洗經費往往靠著冗長的臨床週期當掩護；誠實申報實驗失敗反而成了博士們的自殺行為。但當 AI 成為超級放大器時，真實的陰性數據能化腐朽為神奇地引導模型決策邊界，而浮誇的膨風與洗論文，在數學張量面前將無所遁形。」**

本專案是一個面向大專院校生命科學、醫學工程與資訊科學跨領域研究者的 **開源 AI 藥物開發教學與實戰工作坊（Workshop POC）**。我們徹底揚棄古典生統中「為了應付考試而死背微積分公式」的陳舊範式，帶領學習者親手運用 **蛋白質語言模型（pLM, ESM-2）** 將自然界未標註的胺基酸序列投影為高維幾何向量，親眼見證功能性分子（抗菌肽, AMP）在潛在空間中的自發聚類，並串聯 Google DeepMind 於 2026 年 10 月發布的 **[Antigravity Agentic 工作流](https://deepmind.google/blog/accelerating-antimicrobial-discovery/)**，構築一套跨越資料庫、結構拓撲、操縱子（Operon）基因體上下文與成藥性評估的嚴謹乾實驗驗證體系。

---

## ⚡ 為什麼需要這場「範式轉移」？（Paradigm Shift）

### 1. 拒絕象牙塔的論文洗產線（Anti-Paper-Mill）
傳統生醫研究常受困於「陽性結果至上」的扭曲激勵，導致特定學術團隊靠美化條帶、竄改顯微圖獲取高額補助，把無法重現實驗的後續學弟妹視為代罪羔羊。**真正的計算生物學不是為了炮製更多不可重現的垃圾論文，而是透過高維數學嚴謹探索未知的生命化學邊界。**

### 2. 數學直覺的重塑：從「變化率微積分」到「高維幾何距離」
生科系學生學的傳統微積分多用於一維連續曲線分析（如生長曲線、酵素動理學擬合）；但現代分子 AI（如 ProtNLM、AlphaFold、ESM 系列）的通用語言是：
* **線性代數與張量分解（Tensor Decomposition）**
* **高維潛在空間的餘弦相似度與歐幾里得幾何距離**
* **空間旋轉與平移的等變性（SE(3) Equivariance）**

---

## 🏗️ 三層核心技術架構（The 3-Tier Architecture）

本專案規劃三層漸進式架構，打破學界與業界的鴻溝：

```
+-----------------------------------------------------------------------------------+
|  Tier 3: 結構拓撲、成藥性 (Developability) 與 Antigravity Agentic 流程驗證        |
|  - 3D 結構對齊 (AlphaFold DB / RMSD) | 染色體操縱子上下文 (Operon Context)         |
|  - 成藥性過濾 (溶血毒性、不穩定指數、pI、疏水力矩) | 輸出真正可落地的濕實驗 SOP    |
+-----------------------------------------------------------------------------------+
                                        ▲
                                        │ (特徵傳遞 / 假設驗證)
+-----------------------------------------------------------------------------------+
|  Tier 2: 序列語意與表徵學習 (Sequence Representation Learning)                    |
|  - 載入 Meta ESM-2 (800萬參數輕量級 pLM)                                          |
|  - 提取 320 維全局幾何特徵向量 (CLS Token Embeddings)                             |
|  - UMAP / t-SNE 潛在空間降維視覺化 (AMP vs. Non-AMP 聚類)                         |
+-----------------------------------------------------------------------------------+
                                        ▲
                                        │ (張量幾何投影)
+-----------------------------------------------------------------------------------+
|  Tier 1: 幾何數學直覺重塑 (Geometric Foundations for Drug AI)                    |
|  - 揚棄繁瑣微積分，擁抱高維線性代數與解析幾何                                     |
|  - 潛在空間流形（Latent Manifolds）、特徵分解與距離度量                            |
+-----------------------------------------------------------------------------------+
```

---

## 🚀 快速上手：一鍵在 Google Colab 運行

點擊上方徽章或使用專屬連結直接載入最新版 Workshop Notebook：

👉 [**啟動 BioForge_Antigravity_Workshop_2.ipynb**](https://colab.research.google.com/github/vvchung/BioForge-Antigravity-Workshop/blob/main/BioForge_Antigravity_Workshop_2.ipynb)

### 本地環境建置（可選）

```bash
# 複製本專案
git clone https://github.com/vvchung/BioForge-Antigravity-Workshop.git
cd BioForge-Antigravity-Workshop

# 安裝依賴套件
pip install -r requirements.txt
```

---

## 📊 核心成果展示：ESM-2 潛在幾何空間聚類

在完全**不提供任何人工標籤（Label-free）**、模型也未經過抗菌下游任務監督微調的前提下，ESM-2 單憑蛋白質語言模型預訓練學到的演化語法，即可在 320 維張量空間中準確捕捉生物學物理特徵：

```
      Geometric Dimension 2 (UMAP 2)
              ▲
              │   [AMP: 抗菌肽 (紅點)]
              │      🔴 Cecropin (38aa)
              │   🔴 Magainin (13aa)
              │      🔴 Defensin (18aa)
              │
              │
              │                               [Non-AMP: 胞內蛋白 (藍點)]
              │                                  🔵 GFP (36aa)
              │                                  🔵 Ubiquitin (36aa)
              │                               🔵 Myoglobin (36aa)
              └───────────────────────────────────────────────► Geometric Dimension 1 (UMAP 1)
```

> **關鍵觀察**：
> 1. **長度無關性**：13 個胺基酸的蛙皮素（Magainin）與 38 個胺基酸的天蠶素（Cecropin）緊密群聚在同一側，證明 AI 並不是依照粗淺的「序列長度」分類。
> 2. **深層特徵提取**：紅點自發形成的簇群，精確反映了陽離子分佈與兩親性 $\alpha$-螺旋（Amphipathic Helix）在三維膜穿刺反應中的共通拓撲特徵。

---

## 🛡️ 業界級成藥性防線（Developability & Wet-lab Reality Check）

產業界不需要「只會畫漂亮散佈圖、但拿到培養皿裡根本無法合成或毒死正常細胞」的空氣分子。本架構導入以下工程防線：

1. **成藥性指標過濾（ADMET & Physicochemical Filter）**
   * **疏水性力矩（Hydrophobic Moment, $\mu H$）**：量化兩親性強度，篩選出真正能瓦解細菌外膜的活性候選。
   * **溶血性風險評估（Hemolytic Toxicity Risk）**：剔除對人體紅血球膜具無差別破壞性的高毒性分子。
   * **固相胜肽合成性（SPPS Synthesizability）**：過濾易聚合沉澱、高氧化敏感（過多半胱胺酸未成鍵）的死靶。
2. **基因體鄰域與轉運幫浦驗證（DeepMind Antigravity 策略）**
   * 不單獨看胜肽，而是使用生信 Agent 檢查上游操縱子（Operon）：確認是否偶聯 **ABC 轉運蛋白（ABC Transporter Permease）** 或專屬自保抗性基因，確立細菌素分泌與自我防衛的生化合理性。
3. **終端可執行濕實驗方案（Actionable Wet-lab SOP）**
   * 計算管線輸出包含：微量稀釋法（Broth Microdilution）MIC 測定規劃、重組蛋白表現載體建構建議與質譜檢測標準。

---

## 💡 科學良心與極客守門員理念

> *「那些為了應付考核、騙取經費而拼湊出來的漂亮作假數據，在時間和數學模型的沖刷下終究會被無情揭露；而親手驗證、哪怕帶著瑕疵卻絕對真實的每一次陰性實驗與除錯紀錄，才是真正推動臨床轉譯最堅硬的底氣。」*

本專案獻給所有頂住體制壓力、堅持不造假、拒絕同流合污的真實科學家與工程師。

---

## 📜 授權協議

本專案採用 [MIT License](LICENSE) 條款開放共享。歡迎所有學術機構、實驗室、產學研討會 Fork、引用與衍生改進。
