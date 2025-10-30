Super! Zacznijmy od pierwszego problemu z macierzami.

Masz dane macierze:

$$
A=\begin{pmatrix}1 & 2\\ 3 & 4\end{pmatrix} \quad \text{i} \quad B=\begin{pmatrix}0 & -1\\ 2 & 1\end{pmatrix}
$$

Obliczymy teraz poszczególne działania krok po kroku.

---

## 1. Dodawanie macierzy ($A+B$)

Aby dodać macierze, dodajemy **odpowiadające sobie elementy** (na tych samych pozycjach).

$$
A+B = \begin{pmatrix}1 & 2\\ 3 & 4\end{pmatrix} + \begin{pmatrix}0 & -1\\ 2 & 1\end{pmatrix} = \begin{pmatrix}1+0 & 2+(-1)\\ 3+2 & 4+1\end{pmatrix} = \begin{pmatrix}1 & 1\\ 5 & 5\end{pmatrix}
$$

---

## 2. Odejmowanie macierzy ($A-B$)

Aby odjąć macierze, odejmujemy **odpowiadające sobie elementy**.

$$
A-B = \begin{pmatrix}1 & 2\\ 3 & 4\end{pmatrix} - \begin{pmatrix}0 & -1\\ 2 & 1\end{pmatrix} = \begin{pmatrix}1-0 & 2-(-1)\\ 3-2 & 4-1\end{pmatrix} = \begin{pmatrix}1 & 3\\ 1 & 3\end{pmatrix}
$$

---

## 3. Mnożenie macierzy przez skalar ($2A$)

Aby pomnożyć macierz przez skalar (liczbę), **każdy element** macierzy mnożymy przez ten skalar.

$$
2A = 2 \cdot \begin{pmatrix}1 & 2\\ 3 & 4\end{pmatrix} = \begin{pmatrix}2\cdot 1 & 2\cdot 2\\ 2\cdot 3 & 2\cdot 4\end{pmatrix} = \begin{pmatrix}2 & 4\\ 6 & 8\end{pmatrix}
$$

---

## 4. Kombinacja liniowa macierzy ($3B-2A$)

Najpierw obliczamy $3B$ i $2A$ (to $2A$ już znamy), a następnie odejmujemy macierze.

$$
3B = 3 \cdot \begin{pmatrix}0 & -1\\ 2 & 1\end{pmatrix} = \begin{pmatrix}3\cdot 0 & 3\cdot (-1)\\ 3\cdot 2 & 3\cdot 1\end{pmatrix} = \begin{pmatrix}0 & -3\\ 6 & 3\end{pmatrix}
$$

Teraz odejmujemy:
$$
3B-2A = \begin{pmatrix}0 & -3\\ 6 & 3\end{pmatrix} - \begin{pmatrix}2 & 4\\ 6 & 8\end{pmatrix} = \begin{pmatrix}0-2 & -3-4\\ 6-6 & 3-8\end{pmatrix} = \begin{pmatrix}-2 & -7\\ 0 & -5\end{pmatrix}
$$

---

## 5. Mnożenie macierzy ($A\cdot B$)

Mnożenie macierzy wykonujemy, mnożąc **wiersze** pierwszej macierzy przez **kolumny** drugiej macierzy. Element w *i*-tym wierszu i *j*-tej kolumnie macierzy wynikowej jest iloczynem skalarnym *i*-tego wiersza $A$ i *j*-tej kolumny $B$.

$$
A\cdot B = \begin{pmatrix}1 & 2\\ 3 & 4\end{pmatrix} \cdot \begin{pmatrix}0 & -1\\ 2 & 1\end{pmatrix}
$$

1.  **Element (1, 1)** (wiersz 1 z $A$, kolumna 1 z $B$):
    $$(1)\cdot (0) + (2)\cdot (2) = 0 + 4 = 4$$
2.  **Element (1, 2)** (wiersz 1 z $A$, kolumna 2 z $B$):
    $$(1)\cdot (-1) + (2)\cdot (1) = -1 + 2 = 1$$
3.  **Element (2, 1)** (wiersz 2 z $A$, kolumna 1 z $B$):
    $$(3)\cdot (0) + (4)\cdot (2) = 0 + 8 = 8$$
4.  **Element (2, 2)** (wiersz 2 z $A$, kolumna 2 z $B$):
    $$(3)\cdot (-1) + (4)\cdot (1) = -3 + 4 = 1$$

Zatem:
$$
A\cdot B = \begin{pmatrix}4 & 1\\ 8 & 1\end{pmatrix}
$$

---

## 6. Sprawdzenie, czy $A\cdot B = B\cdot A$

Musimy obliczyć $B\cdot A$ i porównać z $A\cdot B$.

$$
B\cdot A = \begin{pmatrix}0 & -1\\ 2 & 1\end{pmatrix} \cdot \begin{pmatrix}1 & 2\\ 3 & 4\end{pmatrix}
$$

1.  **Element (1, 1)** (wiersz 1 z $B$, kolumna 1 z $A$):
    $$(0)\cdot (1) + (-1)\cdot (3) = 0 - 3 = -3$$
2.  **Element (1, 2)** (wiersz 1 z $B$, kolumna 2 z $A$):
    $$(0)\cdot (2) + (-1)\cdot (4) = 0 - 4 = -4$$
3.  **Element (2, 1)** (wiersz 2 z $B$, kolumna 1 z $A$):
    $$(2)\cdot (1) + (1)\cdot (3) = 2 + 3 = 5$$
4.  **Element (2, 2)** (wiersz 2 z $B$, kolumna 2 z $A$):
    $$(2)\cdot (2) + (1)\cdot (4) = 4 + 4 = 8$$

Zatem:
$$
B\cdot A = \begin{pmatrix}-3 & -4\\ 5 & 8\end{pmatrix}
$$

Porównujemy:
$$
A\cdot B = \begin{pmatrix}4 & 1\\ 8 & 1\end{pmatrix} \quad \text{oraz} \quad B\cdot A = \begin{pmatrix}-3 & -4\\ 5 & 8\end{pmatrix}
$$

Ponieważ macierze nie są identyczne, możemy stwierdzić, że **$A\cdot B \ne B\cdot A$**. Mnożenie macierzy **nie jest przemienne** w ogólnym przypadku.

---
**Podsumowanie wyników:**

* $A+B = \begin{pmatrix}1 & 1\\ 5 & 5\end{pmatrix}$
* $A-B = \begin{pmatrix}1 & 3\\ 1 & 3\end{pmatrix}$
* $2A = \begin{pmatrix}2 & 4\\ 6 & 8\end{pmatrix}$
* $3B-2A = \begin{pmatrix}-2 & -7\\ 0 & -5\end{pmatrix}$
* $A\cdot B = \begin{pmatrix}4 & 1\\ 8 & 1\end{pmatrix}$
* $A\cdot B \ne B\cdot A$

Gotowe! Czy masz już kolejny problem do rozwiązania?