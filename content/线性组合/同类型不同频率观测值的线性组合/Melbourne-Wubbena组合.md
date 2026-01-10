- MW 组合由[[载波相位测量|相位]]的[[宽巷组合]]和[[伪距测量|伪距]]的[[窄巷组合]]相减得到
# $L_{6}=\frac{1}{f_{1}-f_{2}}(f_{1}L_{1}-f_{2}L_{2})-\frac{1}{f_{1}+f_{2}}(f_{1}P_{1}+f_{2}P_{2})=\lambda_{\text{MW}}(N_{L_{1}}-N_{L_{2}})$

^6126dd

- $\lambda_{\text{MW}}=\frac{c}{(f_{L_{1}}-f_{L_{2}})}=0.86\text{m}$


## 作用
- 消除了[[电离层误差]]，[[对流层误差]]
- 消除了[[卫星钟差]]
- 消除了[[接收机钟差]]
- 与卫地几何距离无关
- 该组合观测值的计算结果只包含[[宽巷组合|宽巷]][[整周模糊度|模糊度]]参数
- 具有较长的波长（约为$86cm$），容易确定[[整周模糊度]]
	- 适用于静态、动态数据的[[周跳]]探测，能够探测出2周左右的小[[周跳]]
		- **当两个频率上发生数值相等或相近的[[周跳]]时，该方法失效**
		- 不受观测值采样间隔的影响

## 推导过程
- 首先写出双频$f_{1},f_{2}$下的$L_{1},L_{2},P_{1},P_{2}$：
	- $L_{1}=\rho+c\delta t_{r}-c\delta t_{s}-I_{1}+T+\lambda_{1}N_{1}$
	- $L_{2}=\rho+c\delta t_{r}-c\delta t_{s}-I_{2}+T+\lambda_{2}N_{2}$
	- $P_1 = \rho + c\delta t_r - c\delta t_s + I_1 + T$
	- $P_2 = \rho + c\delta t_r - c\delta t_s + I_2 + T$
- $f_{1}L_{1}-f_{2}L_{2}=f_{1}\left(\rho+c\delta t_{r}-c\delta t_{s}+I_{1}+T+\lambda_{1}N_{1}\right)-f_{2}\left(\rho+c\delta t_{r}-c\delta t_{s}+I_{2}+T+\lambda_{2}N_{2}\right)$
		$=\left(f_{1}-f_{2}\right)\left(\rho+c\delta t_{r}-c\delta t_{s}+T\right)-\left(f_{1}I_{1}-f_{2}I_{2}\right)+f_{1}\lambda_{1}N_{1}-f_{2}\lambda_{2}N_{2}$
	- $f_1 \lambda_1 = f_2 \lambda_2 = c$, $f_1 \lambda_1 N_1 - f_2 \lambda_2 N_2 = c(N_1 - N_2)$
- $f_1 P_1 + f_2 P_2 = f_1 (\rho + c\delta t_r - c\delta t_s - I_1 + T) + f_2 (\rho + c\delta t_r - c\delta t_s - I_2 + T) \tag{2}$
		$= (f_1 + f_2)(\rho + c\delta t_r - c\delta t_s + T) + (f_1 I_1 + f_2 I_2)$
- 由$L_{MW} = \frac{1}{f_{1}-f_{2}}(f_{1}L_{1}-f_{2}L_{2})-\frac{1}{f_{1}+f_{2}}(f_{1}P_{1}+f_{2}P_{2})$得
	- $L_{MW} = \frac{1}{f_{1}-f_{2}}[(f_{1}-f_{2})(\rho+c\delta t_{r}-c\delta t_{s}+T)-(f_{1}I_{1}-f_{2}I_{2})+c(N_{1}-N_{2})]-\frac{1}{f_{1}+f_{2}}[(f_{1}+f_{2})(\rho+c\delta t_{r}-c\delta t_{s}+T)+(f_{1}I_{1}+f_{2}I_{2})]$
- 逐项化简：
	 - $\frac{1}{f_1-f_2}\cdot(f_1-f_2)(\rho+c\delta t_r-c\delta t_s)-\frac{1}{f_1+f_2}\cdot(f_1+f_2)(\rho+c\delta t_r-c\delta t_s)=0$
	 - $\frac{1}{f_{1}-f_{2}}\cdot T(f_{1}-f_{2})-\frac{1}{f_{1}+f_{2}}\cdot T(f_{1}+f_{2}) = T-T=0$
	 - 由于[[电离层误差|电离层延迟]]满足$I_{1}=\frac{A}{f_{1}^{2}},I_{2}=\frac{A}{f_{2}^{2}}$，得
		 - $- \frac{1}{f_1-f_2}(f_1I_1-f_2I_2) - \frac{1}{f_1+f_2}(f_1I_1+f_2I_2) = 0$
 - 最后得$L_{MW}=\frac{1}{f_{1}-f_{2}} \cdot c(N_{1}-N_{2})=\lambda_{MW}(N_{1}-N_{2})$
 