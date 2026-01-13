# $L_{iono-free}=\frac{1}{f_{1}^{2}-f_{2}^{2}}\left(f_{1}^{2} L_{1}-f_{2}^{2} L_{2}\right)$

^df1f0b

# $\varphi_{iono-free} = \frac{f_{L1}^2}{f_{L1}^2 - f_{L2}^2} \varphi_{L1} - \frac{f_{L1} \cdot f_{L2}}{f_{L1}^2 - f_{L2}^2} \varphi_{L2}$
## 作用
- 消除了[[电离层误差|电离层]]的一阶项的影响
- [[整周模糊度|模糊度]]不具有整数特性；常用于**长距离[[相对定位]]或精密[[单点定位]]
- 观测噪声为$L_{1}$的3倍，不适合于短[[基线]]

## 推导过程
- 核心是**消除[[电离层误差|电离层延迟]]项**$I_{L_{1}},I_{L_{2}}$，构造线性组合：
	- $L_{\text{iono-free}} = \alpha \cdot L_{1} + \beta \cdot L_{2}$
- $L_{1} = \rho + c\delta t_r - c\delta t_s - I_{L_{1}} + T+\lambda  \cdot N_1$
- ${L_{2}} = \rho + c\delta t_r - c\delta t_s - I_{L_{2}} + T + \lambda \cdot N_{2}$
- 将[[电离层误差|电离层]]项代入组合式，要求[[电离层误差|电离层]]项的系数和为 0：
	- $\alpha \cdot {I_2} + \beta \cdot {I_2} = 0$
	- $I_1 = \frac{f_2^2}{f_1^2} I_2$
	- $\implies \alpha \cdot \frac{f_2^2}{f_1^2} + \beta = 0$
- 同时，为保留几何距离、钟差等公共项，要求：
	- $\alpha +\beta=1$
- 得出$\alpha = \frac{f_1^{2}}{f_1^{2}-f_2^{2}}$, $\beta = -\frac{f_2^2}{f_1^{2}-f_2^{2}}$
- 即$L_{iono-free}=\frac{1}{f_{1}^{2}-f_{2}^{2}}\left(f_{1}^{2} L_{1}-f_{2}^{2} L_{2}\right)$
- 
- 同理可得$\varphi_{iono-free} = \frac{f_{L1}^2}{f_{L1}^2 - f_{L2}^2} \varphi_{L1} - \frac{f_{L1} \cdot f_{L2}}{f_{L1}^2 - f_{L2}^2} \varphi_{L2}$