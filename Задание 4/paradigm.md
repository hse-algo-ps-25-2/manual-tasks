# Задание №4

## Вычисление ленточного определителя (трёхдиагональной матрицы)

### Вариант 2. Команда Paradigm.

$$    
A =     
  \begin{pmatrix}    
  4 & 1 & 0 & \cdots & 0 & 0 \\    
  4 & 4 & 1 & \cdots & 0 & 0 \\    
  0 & 4 & 4 & \cdots & 0 & 0 \\    
  \vdots  & \vdots & \vdots & \ddots & \vdots & \vdots  \\    
  0 & 0 & 0 & \cdots & 4 & 1 \\    
  0 & 0 & 0 & \cdots & 4 & 4     
  \end{pmatrix}     
$$


Порядок матрицы n = 12.

### Решение

1) Рекуррентное соотношение.

$x_n = 4 \cdot x_{n-1} + 1 \cdot (-1) \cdot 4 \cdot x_{n-2}$

$x_n = 4x_{n-1} - 4x_{n-2}$

2) Характеристическое уравнение.

$x_n \to \lambda^n$

$\lambda^n = 4\lambda^{n-1} - 4\lambda^{n-2}$ &nbsp;&nbsp; $| : \lambda^{n-2}$

$\lambda^2 = 4\lambda - 4$

$\lambda^2 - 4\lambda + 4 = 0$

$\lambda_1 + \lambda_2 = 4$, $\lambda_1 \cdot \lambda_2 = 4$, откуда $\lambda_1 = \lambda_2 = 2$.

3) Общее решение.

Корни совпадают, поэтому:

$x_n = A_1 \cdot n \cdot 2^n + A_2 \cdot 2^n$

$x_1 = 4$, $x_2 = 12$

$$
\begin{cases}
4 = A_1 \cdot 2 + A_2 \cdot 2 & | \cdot 2 \\
12 = A_1 \cdot 8 + A_2 \cdot 4
\end{cases}
$$

Вычитаем из второго уравнения первое, умноженное на 2: $4A_1 = 4$, откуда $A_1 = 1$, $A_2 = 1$.

$x_n = n \cdot 2^n + 2^n = 2^n (n + 1)$

4) Определитель порядка 12.

$x_{12} = 2^{12} \cdot 13 = 53248$

### Ответ

Определитель матрицы порядка 12 равен 53248.
