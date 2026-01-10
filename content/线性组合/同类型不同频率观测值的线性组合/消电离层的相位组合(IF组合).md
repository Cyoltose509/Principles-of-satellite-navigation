# $\varphi_{iono-free} = \frac{f_{L1}^2}{f_{L1}^2 - f_{L2}^2} \varphi_{L1} - \frac{f_{L1} \cdot f_{L2}}{f_{L1}^2 - f_{L2}^2} \varphi_{L2}$

^df1f0b

# $L_{3}=\frac{1}{f_{1}^{2}-f_{2}^{2}}\left(f_{1}^{2} L_{1}-f_{2}^{2} L_{2}\right)$
## 作用
- 消除了[[电离层误差|电离层]]的一阶项的影响
- [[整周模糊度|模糊度]]不具有整数特性；常用于长距离[[相对定位]]或精密[[单点定位]]
- 观测噪声为$L_{1}$的3倍，不适合于短[[基线]]

## 推导过程
- 核心是**消除[[电离层误差|电离层延迟]]项**$I_{L_{1}},I_{L_{2}}$，构造线性组合：
	- $\varphi_{\text{iono-free}} = \alpha \cdot \varphi_{L1} + \beta \cdot \varphi_{L2}$
- $\lambda_{L1}\varphi_{L1} = \rho + c\delta t_r - c\delta t_s - I_{L1} + T + \lambda_{L1}N_{L1}$
- $\lambda_{L2}\varphi_{L2} = \rho + c\delta t_r - c\delta t_s - I_{L2} + T + \lambda_{L2}N_{L2}$
- 将[[电离层误差|电离层]]项代入组合式，要求[[电离层误差|电离层]]项的系数和为 0：
	- $\alpha \cdot I_{L1} + \beta \cdot I_{L2} = 0$
	- $I_{L1} = \frac{f_{L2}^2}{f_{L1}^2} I_{L2}$
	- $\alpha \cdot \frac{f_{L2}^2}{f_{L1}^2} I_{L2} + \beta \cdot I_{L2} = 0 \implies \alpha \cdot \frac{f_{L2}^2}{f_{L1}^2} + \beta = 0$
- 同时，为保留几何距离、钟差等公共项，要求几何项的系数相等：
	- $\alpha \cdot \frac{1}{\lambda_{L1}} = \beta \cdot \frac{1}{\lambda_{L2}}$
- 得出$\alpha = \frac{f_{L1}^{2}}{f_{L1}^{2}-f_{L2}^{2}}$, $\beta = -\frac{f_{L1}f_{L2}}{f_{L1}^{2}-f_{L2}^{2}}$