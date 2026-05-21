# โจทย์ตรีโกณมิติ: $\cot - \tan$

## โจทย์

ค่าของ

$$\cot\!\left(\dfrac{\pi}{12}\right) - \tan\!\left(\dfrac{\pi}{12}\right)$$

ตรงกับข้อใดต่อไปนี้

1. $\sqrt{3}$
2. $2\sqrt{3}$
3. $4\sqrt{3}$
4. $\dfrac{9}{2}$
5. $\dfrac{15}{2}$

---

## วิธีทำ (วิธีที่ 1: ใช้เอกลักษณ์ $\cot\theta - \tan\theta = 2\cot 2\theta$)

### พิสูจน์เอกลักษณ์

$$\cot\theta - \tan\theta = \frac{\cos\theta}{\sin\theta} - \frac{\sin\theta}{\cos\theta} = \frac{\cos^2\theta - \sin^2\theta}{\sin\theta\cos\theta}$$

ใช้สูตร double angle:
- $\cos^2\theta - \sin^2\theta = \cos 2\theta$
- $\sin\theta\cos\theta = \tfrac{1}{2}\sin 2\theta$

$$= \frac{\cos 2\theta}{\tfrac{1}{2}\sin 2\theta} = 2 \cdot \frac{\cos 2\theta}{\sin 2\theta} = 2\cot 2\theta$$

### แทนค่า $\theta = \dfrac{\pi}{12}$

$$\cot\!\left(\tfrac{\pi}{12}\right) - \tan\!\left(\tfrac{\pi}{12}\right) = 2\cot\!\left(2 \cdot \tfrac{\pi}{12}\right) = 2\cot\!\left(\tfrac{\pi}{6}\right)$$

ทราบว่า $\cot\!\left(\tfrac{\pi}{6}\right) = \cot 30° = \sqrt{3}$

$$= 2\sqrt{3}$$

---

## วิธีทำ (วิธีที่ 2: หา $\tan(\pi/12)$ และ $\cot(\pi/12)$ โดยตรง)

ใช้สูตรลบมุม: $\dfrac{\pi}{12} = \dfrac{\pi}{4} - \dfrac{\pi}{6}$ (45° − 30° = 15°)

$$\tan 15° = \tan(45° - 30°) = \frac{\tan 45° - \tan 30°}{1 + \tan 45°\tan 30°} = \frac{1 - \tfrac{1}{\sqrt{3}}}{1 + \tfrac{1}{\sqrt{3}}}$$

คูณบนล่างด้วย $\sqrt{3}$:

$$= \frac{\sqrt{3} - 1}{\sqrt{3} + 1}$$

ทำส่วนเป็นจำนวนตรรกยะ (คูณด้วยคอนจูเกต):

$$= \frac{(\sqrt{3} - 1)^2}{(\sqrt{3})^2 - 1^2} = \frac{3 - 2\sqrt{3} + 1}{2} = \frac{4 - 2\sqrt{3}}{2} = 2 - \sqrt{3}$$

ดังนั้น

$$\cot 15° = \frac{1}{\tan 15°} = \frac{1}{2 - \sqrt{3}} = \frac{2 + \sqrt{3}}{(2 - \sqrt{3})(2 + \sqrt{3})} = \frac{2 + \sqrt{3}}{4 - 3} = 2 + \sqrt{3}$$

ลบกัน:

$$\cot 15° - \tan 15° = (2 + \sqrt{3}) - (2 - \sqrt{3}) = 2\sqrt{3}$$

---

## คำตอบ

**ข้อ 2.** $2\sqrt{3}$

---

# เนื้อหาที่ควรทบทวนเพิ่มเติม

## 1. นิยามของฟังก์ชันตรีโกณมิติ 6 ตัว

| ฟังก์ชัน | นิยาม |
|---|---|
| $\sin\theta$ | $y/r$ |
| $\cos\theta$ | $x/r$ |
| $\tan\theta$ | $\sin\theta/\cos\theta = y/x$ |
| $\csc\theta$ | $1/\sin\theta = r/y$ |
| $\sec\theta$ | $1/\cos\theta = r/x$ |
| $\cot\theta$ | $\cos\theta/\sin\theta = 1/\tan\theta = x/y$ |

## 2. ค่าของฟังก์ชันตรีโกณมิติของมุมพิเศษ

| มุม | $0°$ | $30°$ | $45°$ | $60°$ | $90°$ |
|:---:|:---:|:---:|:---:|:---:|:---:|
| $\sin$ | $0$ | $\tfrac{1}{2}$ | $\tfrac{\sqrt{2}}{2}$ | $\tfrac{\sqrt{3}}{2}$ | $1$ |
| $\cos$ | $1$ | $\tfrac{\sqrt{3}}{2}$ | $\tfrac{\sqrt{2}}{2}$ | $\tfrac{1}{2}$ | $0$ |
| $\tan$ | $0$ | $\tfrac{1}{\sqrt{3}}$ | $1$ | $\sqrt{3}$ | – |
| $\cot$ | – | $\sqrt{3}$ | $1$ | $\tfrac{1}{\sqrt{3}}$ | $0$ |

## 3. สูตรมุมคู่ (Double Angle Formulas)

$$\sin 2\theta = 2\sin\theta\cos\theta$$
$$\cos 2\theta = \cos^2\theta - \sin^2\theta = 2\cos^2\theta - 1 = 1 - 2\sin^2\theta$$
$$\tan 2\theta = \frac{2\tan\theta}{1 - \tan^2\theta}$$

## 4. สูตรผลบวก-ผลต่างของมุม

$$\sin(A \pm B) = \sin A\cos B \pm \cos A\sin B$$
$$\cos(A \pm B) = \cos A\cos B \mp \sin A\sin B$$
$$\tan(A \pm B) = \frac{\tan A \pm \tan B}{1 \mp \tan A\tan B}$$

## 5. เอกลักษณ์ที่มีประโยชน์ในการรวบ $\tan + \cot$ และ $\cot - \tan$

$$\tan\theta + \cot\theta = \frac{\sin^2\theta + \cos^2\theta}{\sin\theta\cos\theta} = \frac{1}{\sin\theta\cos\theta} = \frac{2}{\sin 2\theta} = 2\csc 2\theta$$

$$\cot\theta - \tan\theta = \frac{\cos^2\theta - \sin^2\theta}{\sin\theta\cos\theta} = \frac{2\cos 2\theta}{\sin 2\theta} = 2\cot 2\theta$$

$$\tan\theta - \cot\theta = -2\cot 2\theta$$

## 6. ค่าของ $\sin, \cos, \tan$ ที่ $15°$ (อาจถามตรง ๆ ในข้อสอบ)

$$\sin 15° = \frac{\sqrt{6} - \sqrt{2}}{4}, \quad \cos 15° = \frac{\sqrt{6} + \sqrt{2}}{4}$$
$$\tan 15° = 2 - \sqrt{3}, \quad \cot 15° = 2 + \sqrt{3}$$

## 7. โจทย์ฝึกเพิ่มเติม พร้อมเฉลย

### ข้อ 1: หาค่า $\tan\!\left(\dfrac{\pi}{12}\right) + \cot\!\left(\dfrac{\pi}{12}\right)$

**เฉลย:** $= 2\csc\!\left(\dfrac{\pi}{6}\right) = 2 \cdot 2 = 4$

### ข้อ 2: หาค่า $\cot\!\left(\dfrac{\pi}{8}\right) - \tan\!\left(\dfrac{\pi}{8}\right)$

**เฉลย:** $= 2\cot\!\left(\dfrac{\pi}{4}\right) = 2 \cdot 1 = 2$

### ข้อ 3: หาค่า $\sin 15° \cdot \cos 15°$

**เฉลย:** $= \tfrac{1}{2}\sin 30° = \tfrac{1}{2} \cdot \tfrac{1}{2} = \tfrac{1}{4}$

### ข้อ 4: หาค่า $(\cot 15° + \tan 15°)^2$

**เฉลย:** $\cot 15° + \tan 15° = 2\csc 30° = 4$ → ยกกำลังสอง $= 16$
