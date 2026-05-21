# โจทย์เวกเตอร์หนึ่งหน่วยและมุมระหว่างเวกเตอร์

## โจทย์

ให้ $\vec{u}$ และ $\vec{v}$ เป็นเวกเตอร์หนึ่งหน่วย และ $\theta$ เป็นขนาดของมุมระหว่าง $\vec{u}$ และ $\vec{v}$

ถ้า

$$\vec{u}-2\vec{v} \perp 4\vec{u}+\vec{v}$$

แล้ว $\sec\theta$ มีค่าเท่าใด

ตัวเลือก:

1. $\dfrac{7}{2}$
2. $\dfrac{2}{7}$
3. $\dfrac{\sqrt{85}}{2}$
4. $\dfrac{2}{\sqrt{85}}$
5. หาค่าไม่ได้

---

## วิธีทำอย่างละเอียด

## 1) ใช้เงื่อนไข "ตั้งฉาก" แปลงเป็นดอทโปรดักต์

เมื่อเวกเตอร์สองตัวตั้งฉากกัน จะมีดอทโปรดักต์เป็นศูนย์:

$$\left(\vec{u}-2\vec{v}\right)\cdot\left(4\vec{u}+\vec{v}\right)=0$$

ขยายดอทโปรดักต์ทีละพจน์:

$$\vec{u}\cdot4\vec{u}+\vec{u}\cdot\vec{v}-2\vec{v}\cdot4\vec{u}-2\vec{v}\cdot\vec{v}=0$$

$$4(\vec{u}\cdot\vec{u})+(\vec{u}\cdot\vec{v})-8(\vec{v}\cdot\vec{u})-2(\vec{v}\cdot\vec{v})=0$$

เพราะ $\vec{u}\cdot\vec{v}=\vec{v}\cdot\vec{u}$:

$$4\|\vec{u}\|^2-7(\vec{u}\cdot\vec{v})-2\|\vec{v}\|^2=0$$

## 2) ใช้ข้อมูลว่าเป็นเวกเตอร์หนึ่งหน่วย

เวกเตอร์หนึ่งหน่วยมีความยาว 1:

$$\|\vec{u}\|=\|\vec{v}\|=1 \Rightarrow \|\vec{u}\|^2=\|\vec{v}\|^2=1$$

แทนค่า:

$$4(1)-7(\vec{u}\cdot\vec{v})-2(1)=0$$

$$2-7(\vec{u}\cdot\vec{v})=0$$

$$\vec{u}\cdot\vec{v}=\frac{2}{7}$$

## 3) เชื่อมกับมุมระหว่างเวกเตอร์

สูตรดอทโปรดักต์:

$$\vec{u}\cdot\vec{v}=\|\vec{u}\|\|\vec{v}\|\cos\theta$$

เมื่อทั้งสองเป็นเวกเตอร์หนึ่งหน่วย:

$$\vec{u}\cdot\vec{v}=\cos\theta$$

ดังนั้น

$$\cos\theta=\frac{2}{7}$$

จึงได้

$$\sec\theta=\frac{1}{\cos\theta}=\frac{7}{2}$$

---

## คำตอบ

**ข้อ 1.** $\dfrac{7}{2}$

---

# เนื้อหาเพื่อศึกษาเพิ่มเติม

## 1) ดอทโปรดักต์ (Dot Product)

สำหรับเวกเตอร์ $\vec{a},\vec{b}$

$$\vec{a}\cdot\vec{b}=\|\vec{a}\|\,\|\vec{b}\|\cos\phi$$

โดย $\phi$ คือมุมระหว่างเวกเตอร์

## 2) คุณสมบัติที่ใช้บ่อยมาก

1. สลับที่ได้: $\vec{a}\cdot\vec{b}=\vec{b}\cdot\vec{a}$
2. แจกแจงได้: $\vec{a}\cdot(\vec{b}+\vec{c})=\vec{a}\cdot\vec{b}+\vec{a}\cdot\vec{c}$
3. คูณสเกลาร์: $(k\vec{a})\cdot\vec{b}=k(\vec{a}\cdot\vec{b})$
4. $\vec{a}\cdot\vec{a}=\|\vec{a}\|^2$
5. ตั้งฉากกันก็ต่อเมื่อ $\vec{a}\cdot\vec{b}=0$

## 3) เวกเตอร์หนึ่งหน่วย (Unit Vector)

เวกเตอร์หนึ่งหน่วยคือเวกเตอร์ที่มีความยาวเท่ากับ 1

$$\|\vec{u}\|=1$$

เมื่อ $\vec{u},\vec{v}$ เป็นหนึ่งหน่วย จะได้

$$\vec{u}\cdot\vec{v}=\cos\theta$$

จึงใช้หามุมหรือหาค่า $\cos\theta$ ได้เร็วมาก

## 4) แนวคิดทำโจทย์แนวนี้ให้ไว

1. เห็นคำว่า "ตั้งฉาก" ให้ตั้งสมการดอทโปรดักต์เท่ากับ 0 ทันที
2. ขยายพจน์โดยจัดกลุ่ม $\vec{u}\cdot\vec{u},\vec{v}\cdot\vec{v},\vec{u}\cdot\vec{v}$
3. ใช้ข้อมูล one-unit เพื่อลดรูปให้เหลือ $\cos\theta$
4. โจทย์ถาม $\sec\theta$ หรือ $\tan\theta$ ค่อยแปลงจาก $\cos\theta$

## 5) โจทย์ฝึกเพิ่มเติม

### ข้อฝึก 1

ให้ $\vec{u},\vec{v}$ เป็นเวกเตอร์หนึ่งหน่วย และ $(\vec{u}+\vec{v})\perp(\vec{u}-3\vec{v})$ จงหา $\cos\theta$

เฉลยย่อ:
$$ (\vec{u}+\vec{v})\cdot(\vec{u}-3\vec{v})=0 $$
$$ \|\vec{u}\|^2-2\vec{u}\cdot\vec{v}-3\|\vec{v}\|^2=0 $$
$$ 1-2\cos\theta-3=0 \Rightarrow \cos\theta=-1 $$

### ข้อฝึก 2

ให้ $\vec{u},\vec{v}$ เป็นเวกเตอร์หนึ่งหน่วย และ $\|\vec{u}-\vec{v}\|=1$ จงหา $\cos\theta$

เฉลยย่อ:
$$\|\vec{u}-\vec{v}\|^2=(\vec{u}-\vec{v})\cdot(\vec{u}-\vec{v})=2-2\cos\theta$$
$$1=2-2\cos\theta \Rightarrow \cos\theta=\frac{1}{2}$$

### ข้อฝึก 3

ให้ $\vec{u},\vec{v}$ เป็นเวกเตอร์หนึ่งหน่วย และ $\vec{u}\cdot\vec{v}=\frac{3}{5}$ จงหา $\sec\theta$

เฉลยย่อ:
$$\cos\theta=\frac{3}{5} \Rightarrow \sec\theta=\frac{5}{3}$$
