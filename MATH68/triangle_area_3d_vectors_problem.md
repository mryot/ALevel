# โจทย์เวกเตอร์สามมิติ: พื้นที่สามเหลี่ยม OAB

## โจทย์

ให้ $O$ เป็นจุดกำเนิดในระบบพิกัดฉากสามมิติ และให้ $A, B$ เป็นจุดที่มีพิกัดเป็น

$$A(-3,1,0), \quad B(t,-4,4)$$

ตามลำดับ โดยที่ $t$ เป็นจำนวนจริงบวก

ถ้า

$$|\overrightarrow{AB}| = 3|\overrightarrow{OA}|$$

แล้วรูปสามเหลี่ยม $OAB$ มีพื้นที่กี่ตารางหน่วย

ตัวเลือก:
1. $4\sqrt{7}$
2. $2\sqrt{10}$
3. $4\sqrt{10}$
4. $2\sqrt{14}$
5. $4\sqrt{14}$

---

## วิธีทำอย่างละเอียด

## 1) เขียนเวกเตอร์ที่ต้องใช้

$$\overrightarrow{OA} = A - O = (-3,1,0)$$

$$\overrightarrow{AB} = B - A = (t-(-3),\,-4-1,\,4-0) = (t+3,-5,4)$$

## 2) ใช้เงื่อนไขความยาว $|\overrightarrow{AB}| = 3|\overrightarrow{OA}|$

### หา $|\overrightarrow{OA}|$

$$|\overrightarrow{OA}| = \sqrt{(-3)^2 + 1^2 + 0^2} = \sqrt{10}$$

จึงได้

$$|\overrightarrow{AB}| = 3\sqrt{10}$$

### เขียนสมการจากความยาวของ $\overrightarrow{AB}$

$$|\overrightarrow{AB}|^2 = (t+3)^2 + (-5)^2 + 4^2 = (t+3)^2 + 41$$

และ

$$|\overrightarrow{AB}|^2 = (3\sqrt{10})^2 = 90$$

เท่ากันจึงได้

$$ (t+3)^2 + 41 = 90 $$
$$ (t+3)^2 = 49 $$
$$ t+3 = \pm 7 $$
$$ t = 4 \;\text{หรือ}\; -10 $$

แต่โจทย์กำหนดว่า $t$ เป็นจำนวนจริงบวก จึงได้

$$\boxed{t=4}$$

ดังนั้น

$$B=(4,-4,4)$$

## 3) หาเวกเตอร์ $\overrightarrow{OB}$

$$\overrightarrow{OB}=B-O=(4,-4,4)$$

## 4) ใช้สูตรพื้นที่สามเหลี่ยมจากครอสโปรดักต์

พื้นที่สามเหลี่ยมที่เกิดจากเวกเตอร์ด้าน $\overrightarrow{OA}$ และ $\overrightarrow{OB}$ คือ

$$\text{Area}(\triangle OAB)=\frac{1}{2}\left|\overrightarrow{OA}\times\overrightarrow{OB}\right|$$

คำนวณครอสโปรดักต์:

$$\overrightarrow{OA}\times\overrightarrow{OB}
=\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
-3 & 1 & 0 \\
4 & -4 & 4
\end{vmatrix}
=(4,12,8)$$

ขนาดของเวกเตอร์นี้:

$$\left|(4,12,8)\right|=\sqrt{4^2+12^2+8^2}=
\sqrt{16+144+64}=\sqrt{224}=4\sqrt{14}$$

ดังนั้นพื้นที่สามเหลี่ยมคือ

$$\text{Area}=\frac{1}{2}(4\sqrt{14})=2\sqrt{14}$$

---

## คำตอบ

**ข้อ 4. $2\sqrt{14}$**

---

# เนื้อหาเพื่อศึกษาเพิ่มเติม

## 1) สูตรความยาวเวกเตอร์ใน 3 มิติ

ถ้า $\vec{v}=(x,y,z)$ แล้ว

$$|\vec{v}|=\sqrt{x^2+y^2+z^2}$$

## 2) เวกเตอร์ระหว่างสองจุด

ถ้า $P(x_1,y_1,z_1), Q(x_2,y_2,z_2)$

$$\overrightarrow{PQ}=Q-P=(x_2-x_1,\,y_2-y_1,\,z_2-z_1)$$

## 3) ครอสโปรดักต์และพื้นที่

สำหรับเวกเตอร์ $\vec{u},\vec{v}$

$$|\vec{u}\times\vec{v}|=|\vec{u}|\,|\vec{v}|\sin\theta$$

โดยค่า $|\vec{u}\times\vec{v}|$ คือพื้นที่รูปสี่เหลี่ยมด้านขนานที่มีด้านเป็น $\vec{u},\vec{v}$

ดังนั้นพื้นที่สามเหลี่ยมคือครึ่งหนึ่ง:

$$\text{Area}_{\triangle}=\frac{1}{2}|\vec{u}\times\vec{v}|$$

## 4) ข้อควรระวังที่เจอบ่อย

1. สับสนระหว่าง $\overrightarrow{AB}$ กับ $\overrightarrow{BA}$ (ทิศตรงข้าม)
2. ลืมเงื่อนไขโจทย์ เช่น ในข้อนี้กำหนด $t>0$
3. ได้พื้นที่สี่เหลี่ยมด้านขนานแล้วลืมหาร 2 เพื่อเป็นพื้นที่สามเหลี่ยม

## 5) โจทย์ฝึกเพิ่มเติม

### ข้อฝึก 1

ให้ $O=(0,0,0), A=(1,2,2), B=(3,0,1)$ จงหาพื้นที่สามเหลี่ยม $OAB$

เฉลยย่อ:
- $\overrightarrow{OA}=(1,2,2), \overrightarrow{OB}=(3,0,1)$
- $\overrightarrow{OA}\times\overrightarrow{OB}=(2,5,-6)$
- ขนาด $=\sqrt{65}$
- พื้นที่ $=\dfrac{\sqrt{65}}{2}$

### ข้อฝึก 2

ให้ $A=(2,-1,0), B=(5,3,4), C=(1,2,2)$ จงหาพื้นที่สามเหลี่ยม $ABC$

เฉลยย่อ:
- ใช้ $\overrightarrow{AB}=B-A, \overrightarrow{AC}=C-A$
- พื้นที่ $=\dfrac{1}{2}|\overrightarrow{AB}\times\overrightarrow{AC}|$

### ข้อฝึก 3

ถ้า $|\vec{u}|=4, |\vec{v}|=5$ และมุมระหว่างเวกเตอร์เป็น $30^\circ$ จงหาพื้นที่สามเหลี่ยมที่เกิดจาก $\vec{u},\vec{v}$

เฉลยย่อ:
$$\text{Area}=\frac{1}{2}|\vec{u}|\,|\vec{v}|\sin30^\circ
=\frac{1}{2}\cdot4\cdot5\cdot\frac{1}{2}=5$$
