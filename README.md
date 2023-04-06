<!--    ConsoleApp40      -->
# 精銳矩陣計算求解器(Sharp Matrix Solver, SMS)驗證  

## 測試實例採用 : William E. Boyce and Richard C. DiPrima, "Elementary Differential Equations and Boundary Value Problems 10th Edition" 第413頁 至 416頁，作爲SMS實作驗證  

### $$\dot{y} = A * y $$  

$$
A =
\begin{bmatrix}
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
-2 & 1.5 & 0 & 0 \\
1.333 & -3 & 0 & 0
\end{bmatrix} 系統矩陣  
$$  

$$
y(t = 0) =
\begin{bmatrix}
-1 \\ 4 \\ 1 \\ 1  
\end{bmatrix} 初始值@t = 0  
$$

### 空間維度【Space Dimension】有四個自由度Degree of Freedom(m = 4)，狀態維度【State Dimension】僅有一個自由度，即一階微分(r = 1)，時間維度【Time Dimension】是時間的函數，可以任意選取，故整個【系統矩陣】為4X4的實數矩陣，C#程式碼是引用Matrix_0類別庫，即程式碼的開頭是引用 ```using Matrix_0；```  

# 雖然系統矩陣是實數，但系統特徵值和特徵向量，其預設值(Default Value)都是複數矩陣(Complex Matrix)，請參考程式碼的輸出結果  
