<img width="739" height="239" alt="image" src="https://github.com/user-attachments/assets/6f1bdf72-444f-4258-be99-f36918cdd224" />

$$x_n = a \cdot x_{n-1} - b \cdot c \cdot x_{n-2}$$

$$x_1 = -6$$

$$x_2 = \begin{vmatrix} -6 & 2 \\ -8 & -6 \end{vmatrix} = 36 + 16 = 52$$

$$x_n = -6x_{n-1} + 16x_{n-2}$$

$$x_n \to \lambda^n$$

$$\lambda^n = -6\lambda^{n-1} + 16\lambda^{n-2} \quad \big| : \lambda^{n-2}$$

$$\lambda^2 = -6\lambda + 16$$

$$\lambda^2 + 6\lambda - 16 = 0$$

$$\lambda_1 = -8; \; \lambda_2 = 2$$

$$x_n = A_1 \lambda_1^n + A_2 \lambda_2^n; \; x_n = (-8)^n A_1 + 2^n A_2$$

$$\begin{cases} -6 = A_1 \cdot (-8) + A_2 \cdot 2 \\ 52 = A_1 \cdot (-8)^2 + A_2 \cdot 2^2 \end{cases}$$

$$\begin{cases} -8A_1 + 2A_2 = -6 \quad | \cdot 2 \\ 64A_1 + 4A_2 = 52 \end{cases}$$

$$\begin{cases} -16A_1 + 4A_2 = -12 \\ 64A_1 + 4A_2 = 52 \end{cases}$$

$$80A_1 = 64$$

$$A_1 = \frac{64}{80} = 0{,}8$$

$$0{,}8 \cdot (-8) + A_2 \cdot 2 = -6$$

$$2A_2 = 0{,}4$$

$$A_2 = 0{,}2$$

$$x_n = 0{,}8 \cdot (-8)^n + 0{,}2 \cdot 2^n$$

$$x_{11} = 0{,}8 \cdot (-8)^{11} + 0{,}2 \cdot 2^{11} = -6871947264$$
