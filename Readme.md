# 自動化數據處理及晶格繞射點預測程式

本專案包含兩個 Python 程式。第一個程式用於自動化讀取數據文件並繪製 XRD、XRR 和 Rocking Curve 圖表。第二個程式用於預測晶格繞射點。

## 目錄

- 安裝
- 自動化數據處理程式
- 晶格繞射點預測程式

## 安裝

使用這些程式需要在您的計算機上安裝 Python。此外，您還需要以下 Python 庫：

- `numpy`
- `matplotlib`

您可以使用 pip 來安裝這些庫：

```sh
pip install numpy matplotlib
```

## 自動化數據處理程式

YCMOSTO100_5%.ipynb 和 YCMOSTO110_5%.ipynb 中的程式是用來讀取數據文件並繪製 XRD、XRR、Rocking Curve 和 Phi scan 圖表。

### 使用說明

1. 在使用之前確保您的數據文件格式正確，並位於與程式相同的目錄中。
2. 修改程式中的文件名以匹配您的數據文件。
3. 從 GitHub 倉庫`clone`此項目：

   ```sh
   git clone https://github.com/Rae-C429/experiment.git
   ```

4. 輸入檔案即可出圖

## 晶格繞射點預測程式

XRD.ipynb 中的程式利用提供的參數預測晶格繞射點。

### 使用說明

1. 從 GitHub 倉庫`clone`此項目：

   ```sh
   git clone https://github.com/Rae-C429/experiment.git
   ```

2. 從程式中匯入函數。
3. 使用適當的參數調用 xRD 函數來計算繞射點。
4. 使用 similar_axis 函數查找相似軸點。

參數說明
`meterial`: 晶格材料的名稱或標識。
`hkl`: 晶格平面指數，例如 `[h, k, l]`。
`mno`: 主軸向量，例如 `[m, n, o]`。
`pqr`: 次軸向量，例如 `[p, q, r]`。
`a, b, c`: 晶格常數，分別對應三個坐標軸。
