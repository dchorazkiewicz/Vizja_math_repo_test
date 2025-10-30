## 📝 Macierze i podstawowe operacje: Rozwiązanie

Dla macierzy $A=\begin{pmatrix}1 & 2\\ 3 & 4\end{pmatrix}$ i $B=\begin{pmatrix}0 & -1\\ 2 & 1\end{pmatrix}$

---

### 1. Dodawanie macierzy ($A+B$)

**Krok:** Dodajemy odpowiadające sobie elementy.

$A+B = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} + \begin{pmatrix} 0 & -1 \\ 2 & 1 \end{pmatrix} = \begin{pmatrix} 1+0 & 2-1 \\ 3+2 & 4+1 \end{pmatrix} = \begin{pmatrix} 1 & 1 \\ 5 & 5 \end{pmatrix}$

---

### 2. Odejmowanie macierzy ($A-B$)

**Krok:** Odejmujemy odpowiadające sobie elementy.

$A-B = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} - \begin{pmatrix} 0 & -1 \\ 2 & 1 \end{pmatrix} = \begin{pmatrix} 1-0 & 2-(-1) \\ 3-2 & 4-1 \end{pmatrix} = \begin{pmatrix} 1 & 3 \\ 1 & 3 \end{pmatrix}$

---

### 3. Mnożenie przez skalar ($2A$)

**Krok:** Mnożymy każdy element macierzy $A$ przez 2.

$2A = 2 \cdot \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} = \begin{pmatrix} 2 & 4 \\ 6 & 8 \end{pmatrix}$

---

### 4. Kombinacja liniowa ($3B-2A$)

**Krok:** Obliczamy $3B - 2A$.

$3B-2A = 3 \begin{pmatrix} 0 & -1 \\ 2 & 1 \end{pmatrix} - 2 \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} = \begin{pmatrix} 0 & -3 \\ 6 & 3 \end{pmatrix} - \begin{pmatrix} 2 & 4 \\ 6 & 8 \end{pmatrix} = \begin{pmatrix} -2 & -7 \\ 0 & -5 \end{pmatrix}$

---

### 5. Mnożenie macierzy ($A\cdot B$)

**Krok:** Mnożymy wiersze $A$ przez kolumny $B$.

$A\cdot B = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} \cdot \begin{pmatrix} 0 & -1 \\ 2 & 1 \end{pmatrix} = \begin{pmatrix} 1\cdot 0 + 2\cdot 2 & 1\cdot (-1) + 2\cdot 1 \\ 3\cdot 0 + 4\cdot 2 & 3\cdot (-1) + 4\cdot 1 \end{pmatrix} = \begin{pmatrix} 4 & 1 \\ 8 & 1 \end{pmatrix}$

---

### 6. Sprawdzenie przemienności ($A\cdot B = B\cdot A$)

**Krok:** Obliczamy $B\cdot A$.

$B\cdot A = \begin{pmatrix} 0 & -1 \\ 2 & 1 \end{pmatrix} \cdot \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} = \begin{pmatrix} 0\cdot 1 + (-1)\cdot 3 & 0\cdot 2 + (-1)\cdot 4 \\ 2\cdot 1 + 1\cdot 3 & 2\cdot 2 + 1\cdot 4 \end{pmatrix} = \begin{pmatrix} -3 & -4 \\ 5 & 8 \end{pmatrix}$

**Wniosek:** Ponieważ $A\cdot B = \begin{pmatrix} 4 & 1 \\ 8 & 1 \end{pmatrix} \ne \begin{pmatrix} -3 & -4 \\ 5 & 8 \end{pmatrix} = B\cdot A$, mnożenie macierzy **nie jest przemienne**.