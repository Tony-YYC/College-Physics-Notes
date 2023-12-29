# Chapter13 电流与电源

## 13.1 电流与电源

### 13.1.2 电流强度与电流密度矢量

电流强度
$$I=\dfrac{dq}{dt}$$

载流导体中任一点的**电流密度矢量** \
**大小**：单位时间内流过该点所在的、且与该点正电荷定向移动方向垂直的单位面积截面的电量。
$$\left| \vec{j} \right| = \dfrac{dq}{dtdS_⊥} = \dfrac{dI}{dS_⊥}$$
**方向**：该点正电荷定向移动的方向
$$\vec{j} = \dfrac{dI}{dS_⊥} \vec{e_n}$$

**电流场**：导体内每一点都有对应的 $\vec{j}(x,y,z)$

### 13.1.3 电流连续性方程

1. **电流连续性方程** \
由电荷守恒定律，单位时间内由S流出的净电量应等于S内电量的减少

<p align="center">
<img src="image-4.png" alt="Image" style="width:30%; height:auto;">
</p>

$$\oiint_{S}\vec{j}\cdot d\vec{S} = -\dfrac{dq_{S内}}{dt}$$


2. **稳恒电流** \
导体中各处的电流密度矢量不随时间变化
$$\dfrac{dq_{S内}}{dt} = 0 \quad \oiint_{S}\vec{j}\cdot d\vec{S} = 0$$
* 区分概念：**均匀电流**：导体中各处的电流密度矢量相同

### 13.1.4 金属导体中的电流密度矢量与载流子的平均漂移速度

设每个载流子电量为$q$，载流子数密度为$n$，平均漂移速度的大小$v_d$ \
在时间$\Delta t$内，柱体元内的自由电子将穿过截面$\Delta S$，易得以下结论：
<p align="center">
<img src="image-5.png" alt="Image" style="width:25%; height:auto;">
</p>

$$\Delta I = qnv_d\Delta S$$
$$j=\dfrac{\Delta I}{\Delta S} = nqv_d$$
（$\rho_e=nq$ 电荷体密度）
$$\vec{j} = nq\vec{v_d} = \rho_e\vec{v_d}$$

### 13.1.5 欧姆定律：德鲁德模型

$$\vec{j} = \dfrac{ne^2\tau}{2m}\vec{E} = \gamma \vec{E}$$
(令$\gamma = \dfrac{ne^2\tau}{2m}$为电导率)

## 13.2 磁场及其基本描述量

### 13.2.1 磁场力
运动电荷在磁场中受力：
$$\vec{F} = q\vec{v} \times \vec{B}$$
<p align="center">
<img src="image-6.png" alt="Image" style="width:30%; height:auto;">
</p>
## 13.3 毕奥-萨伐尔定律：电流的磁效应

### 毕奥-萨伐尔定律

取电流元$I d\vec{l} = \vec{v_d}dq$
$$d\vec{B} = \dfrac{\mu_0}{4 \pi} \dfrac{Id\vec{l} \times \vec{r}}{r^3}$$（向量形式） 
$$dB = \dfrac{\mu_0}{4 \pi} \dfrac{Idl sin \theta}{r^2}$$（标量形式）
任意导线：
$$\vec{B} = \int d\vec{B} = \int \dfrac{\mu_0}{4 \pi} \dfrac{Id\vec{l} \times \vec{r}}{r^3}$$
载流回路：
$$\vec{B} = \oint_{l} d\vec{B} = \oint_{l} \dfrac{\mu_0}{4 \pi} \dfrac{Id\vec{l} \times \vec{r}}{r^3}$$

### 电流产生的磁感应强度的计算

解题基本逻辑：

1. 取电流元$I d\vec{l} $ ，套公式，计算由电流元产生的磁感应强度$d \vec{B}$
2. 判断$d \vec{B}$的方向，把它进行分解 $d\vec{B} \to dB_x,dB_y,dB_z$
3. 看一眼对称性，由对称性可以判断一些方向的分量积分以后显然为0，就不必算了
4. 对剩下的分量分部积分 $B_x=\int dB_x,B_y = \int dB_y,B_z = \int dB_z$

一些技巧：

- 对整体也善用对称性判断，有些对称性很好的电流，在其对称中心产生的$\vec{B}$显然为0，例如

  - 下面这个正方体电路在其中心产生的磁感应强度

  <img src="assets/image-20231229203948006.png" alt="image-20231229203948006" style="zoom:50%;" />

  - 无限长均匀圆柱面在其对称轴上产生的磁感应强度

    <img src="assets/image-20231229211026530.png" alt="image-20231229211026530" style="zoom:50%;" />

### 常见的电流产生的磁感应强度的模型

注：下面的磁感应强度都没指出方向，用的时候记得自己看一下方向！

- 直线段电流产生的磁场（模型如图所示，所计算点与直线距离为$a$，起终点$\vec{r}$与电流方向夹角分别为$\theta_1$，$\theta_2$）：

  <img src="assets/image-20231229182115571.png" alt="image-20231229182115571" style="zoom:50%;" />
  $$
  B= \dfrac{\mu_0 I}{4\pi a}(cos \theta_1 - cos\theta_2)
  $$

- 特别地，无限长直线电流产生的磁场（所计算点与直线距离为$a$）：
  $$
  B = \dfrac{\mu_0 I}{2 \pi a}
  $$

- 显然，半无限长直线：
  $$
  B = \dfrac{\mu_0 I}{4 \pi a}
  $$

- 宽度为a的无限长平面，单位宽度电流为$\alpha$，求平面上方任一点（与平面距离$y$）的磁感应强度
  $$
  B = \dfrac{\mu_0 \alpha}{\pi} arctan \dfrac{a}{2y}
  $$

- 特别地（上式取$a \to \infty$），无限大均匀平面电流（电流线密度为$\alpha$）：
  $$
  B = \dfrac{\mu_0 \alpha}{2}
  $$

- 无限长均匀圆柱面电流的磁场（设与中轴距离为$r$）（算起来贼烦，记一下结论吧）：
  $$
  B =
  \begin{cases}
  \ 0 & r<R \\
  \ \dfrac{\mu_0 I}{2 \pi r} & r>R \\
  \end{cases}
  $$

- 圆电流轴线上的磁场分布
  $$
  B = \dfrac{\mu_0 I R^2}{2(R^2+z^2)^{\frac{3}{2}}}
  $$
  <img src="assets/image-20231229214825519.png" alt="image-20231229214825519" style="zoom:50%;" />

- 圆弧电流在圆心处产生的磁感应强度
  $$
  B = \dfrac{\mu_0}{4\pi}\dfrac{IL}{R^2} = \dfrac{\mu_0}{4\pi}\dfrac{I}{R}\theta
  $$
  <img src="assets/image-20231229220027555.png" alt="image-20231229220027555" style="zoom: 67%;" />

  

## 13.4 磁场的基本规律

## 13.5 磁场对电流的作用

## 13.6 带电粒子的运动与磁场
