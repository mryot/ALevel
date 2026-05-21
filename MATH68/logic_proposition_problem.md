# โจทย์ตรรกศาสตร์: หาประพจน์ที่เป็น Contingency

## โจทย์

ให้ $p, q, r$ เป็นประพจน์ ประพจน์ใดต่อไปนี้มีค่าความจริง**เป็นจริงในบางกรณี และเป็นเท็จในบางกรณี**

1. $(p \vee \sim p) \to (r \wedge \sim r)$
2. $(\sim p \wedge q) \wedge (p \wedge r)$
3. $(q \to r) \leftrightarrow (q \wedge \sim r)$
4. $(p \vee r) \wedge (q \vee \sim r)$
5. $(p \wedge q) \wedge (\sim p \vee \sim q)$

---

## แนวคิด

ประพจน์ที่มีค่าความจริง "เป็นจริงในบางกรณี และเป็นเท็จในบางกรณี" เรียกว่า **Contingency**

ดังนั้นเราต้องตัดประพจน์ที่เป็น:
- **สัจนิรันดร์ (Tautology)** — เป็นจริงเสมอ
- **ข้อขัดแย้ง (Contradiction)** — เป็นเท็จเสมอ

ออกไป แล้วเหลือข้อที่เป็น Contingency

---

## วิเคราะห์แต่ละข้อ

### ข้อ 1: $(p \vee \sim p) \to (r \wedge \sim r)$

- $p \vee \sim p \equiv \mathbf{T}$ (สัจนิรันดร์)
- $r \wedge \sim r \equiv \mathbf{F}$ (ข้อขัดแย้ง)
- ดังนั้น $\mathbf{T} \to \mathbf{F} \equiv \mathbf{F}$ เสมอ

→ **เป็นเท็จเสมอ (Contradiction)** ✗

---

### ข้อ 2: $(\sim p \wedge q) \wedge (p \wedge r)$

จัดรูปใหม่โดยใช้สมบัติการสลับที่และการเปลี่ยนกลุ่ม:

$$(\sim p \wedge q) \wedge (p \wedge r) \equiv (\sim p \wedge p) \wedge (q \wedge r)$$

- $\sim p \wedge p \equiv \mathbf{F}$
- ดังนั้นทั้งประพจน์ $\equiv \mathbf{F} \wedge (q \wedge r) \equiv \mathbf{F}$

→ **เป็นเท็จเสมอ (Contradiction)** ✗

---

### ข้อ 3: $(q \to r) \leftrightarrow (q \wedge \sim r)$

ใช้สมบัติ: $q \to r \equiv \sim(q \wedge \sim r)$

ให้ $X = q \wedge \sim r$ ประพจน์กลายเป็น

$$\sim X \leftrightarrow X$$

ซึ่งเป็นเท็จเสมอ (เพราะ $\sim X$ และ $X$ มีค่าตรงข้ามกันเสมอ)

→ **เป็นเท็จเสมอ (Contradiction)** ✗

---

### ข้อ 4: $(p \vee r) \wedge (q \vee \sim r)$ ✓

ทดลองหาค่าความจริงบางกรณี:

| $p$ | $q$ | $r$ | $p \vee r$ | $\sim r$ | $q \vee \sim r$ | ผลรวม |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| T | T | T | T | F | T | **T** |
| F | F | F | F | T | T | **F** |
| T | F | F | T | T | T | **T** |
| F | F | T | T | F | F | **F** |

- พบทั้งกรณีที่เป็นจริงและเป็นเท็จ

→ **เป็น Contingency** ✓

---

### ข้อ 5: $(p \wedge q) \wedge (\sim p \vee \sim q)$

ใช้กฎเดอมอร์แกน (De Morgan's law):

$$\sim p \vee \sim q \equiv \sim(p \wedge q)$$

ให้ $Y = p \wedge q$ ประพจน์กลายเป็น

$$Y \wedge \sim Y \equiv \mathbf{F}$$

→ **เป็นเท็จเสมอ (Contradiction)** ✗

---

## คำตอบ

**ข้อ 4.** $(p \vee r) \wedge (q \vee \sim r)$

---

# เนื้อหาที่ต้องศึกษาเพิ่มเติม

## 1. ประพจน์ (Proposition)

**ประพจน์** คือ ประโยคหรือข้อความที่บอกค่าความจริงได้แน่นอนว่าเป็น **จริง (T)** หรือ **เท็จ (F)** อย่างใดอย่างหนึ่ง

---

## 2. ตัวเชื่อมประพจน์ (Logical Connectives)

| ตัวเชื่อม | สัญลักษณ์ | ชื่อ | อ่านว่า |
|---|:---:|---|---|
| นิเสธ | $\sim p$ | Negation | "ไม่ $p$" |
| และ | $p \wedge q$ | Conjunction | "$p$ และ $q$" |
| หรือ | $p \vee q$ | Disjunction | "$p$ หรือ $q$" |
| ถ้า...แล้ว | $p \to q$ | Conditional | "ถ้า $p$ แล้ว $q$" |
| ก็ต่อเมื่อ | $p \leftrightarrow q$ | Biconditional | "$p$ ก็ต่อเมื่อ $q$" |

### ตารางค่าความจริง

| $p$ | $q$ | $\sim p$ | $p \wedge q$ | $p \vee q$ | $p \to q$ | $p \leftrightarrow q$ |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| T | T | F | T | T | T | T |
| T | F | F | F | T | F | F |
| F | T | T | F | T | T | F |
| F | F | T | F | F | T | T |

**ข้อควรจำ:**
- $p \to q$ เป็นเท็จเมื่อ $p$ จริง และ $q$ เท็จ เท่านั้น
- $p \leftrightarrow q$ เป็นจริงเมื่อ $p$ และ $q$ มีค่าความจริงเหมือนกัน

---

## 3. ประเภทของประพจน์ผสม

### สัจนิรันดร์ (Tautology)
ประพจน์ที่มีค่าความจริง **เป็นจริงเสมอ** ทุกกรณี

ตัวอย่าง: $p \vee \sim p$, $p \to p$

### ข้อขัดแย้ง (Contradiction)
ประพจน์ที่มีค่าความจริง **เป็นเท็จเสมอ** ทุกกรณี

ตัวอย่าง: $p \wedge \sim p$

### Contingency
ประพจน์ที่มีค่าความจริง **บางกรณีเป็นจริง บางกรณีเป็นเท็จ**

ตัวอย่าง: $p \to q$, $p \wedge q$

---

## 4. สมบัติและกฎที่สำคัญ

### กฎเดอมอร์แกน (De Morgan's Laws)
$$\sim(p \wedge q) \equiv \sim p \vee \sim q$$
$$\sim(p \vee q) \equiv \sim p \wedge \sim q$$

### กฎการกระจาย (Distributive Laws)
$$p \wedge (q \vee r) \equiv (p \wedge q) \vee (p \wedge r)$$
$$p \vee (q \wedge r) \equiv (p \vee q) \wedge (p \vee r)$$

### กฎที่ใช้บ่อยกับ $\to$ และ $\leftrightarrow$
$$p \to q \equiv \sim p \vee q$$
$$p \to q \equiv \sim(p \wedge \sim q)$$
$$\sim(p \to q) \equiv p \wedge \sim q$$
$$p \leftrightarrow q \equiv (p \to q) \wedge (q \to p)$$
$$p \leftrightarrow q \equiv (p \wedge q) \vee (\sim p \wedge \sim q)$$

### กฎ Identity และ Domination
$$p \wedge \mathbf{T} \equiv p, \quad p \vee \mathbf{F} \equiv p$$
$$p \wedge \mathbf{F} \equiv \mathbf{F}, \quad p \vee \mathbf{T} \equiv \mathbf{T}$$

### กฎ Complement
$$p \vee \sim p \equiv \mathbf{T} \quad \text{(สัจนิรันดร์)}$$
$$p \wedge \sim p \equiv \mathbf{F} \quad \text{(ข้อขัดแย้ง)}$$

### กฎ Idempotent
$$p \wedge p \equiv p, \quad p \vee p \equiv p$$

### กฎ Double Negation
$$\sim(\sim p) \equiv p$$

---

## 5. เทคนิคการตรวจสอบประเภทประพจน์

### วิธีที่ 1: สร้างตารางค่าความจริง
- ถ้าคอลัมน์สุดท้ายเป็น **T ทั้งหมด** → สัจนิรันดร์
- ถ้าคอลัมน์สุดท้ายเป็น **F ทั้งหมด** → ข้อขัดแย้ง
- ถ้ามีทั้ง **T และ F** → Contingency

### วิธีที่ 2: จัดรูปโดยใช้สมบัติ
- มองหารูปแบบ $X \wedge \sim X$ → ข้อขัดแย้ง
- มองหารูปแบบ $X \vee \sim X$ → สัจนิรันดร์
- มองหา $X \leftrightarrow \sim X$ → ข้อขัดแย้ง
- มองหา $X \to \sim X$ ที่บังคับให้ $X$ ต้องเป็นเท็จเสมอ

### วิธีที่ 3: ลองแทนค่า
- ถ้าหาค่า T ได้ 1 กรณี และ F ได้ 1 กรณี → Contingency (ตอบได้ทันที)

---

## 6. โจทย์ฝึกเพิ่มเติม พร้อมเฉลย

### ข้อ 1: ตรวจสอบว่า $(p \to q) \vee (q \to p)$ เป็นประเภทใด

**วิธีทำ:**

สร้างตารางค่าความจริง:

| $p$ | $q$ | $p \to q$ | $q \to p$ | $(p \to q) \vee (q \to p)$ |
|:---:|:---:|:---:|:---:|:---:|
| T | T | T | T | **T** |
| T | F | F | T | **T** |
| F | T | T | F | **T** |
| F | F | T | T | **T** |

**สังเกต:** เมื่อ $p \to q$ เป็นเท็จ (กรณี $p$=T, $q$=F) จะทำให้ $q \to p$ เป็นจริงทันที (เพราะ $q$=F) และในทางกลับกันก็เช่นกัน ดังนั้นจึงเป็นไปไม่ได้ที่ทั้งสองจะเป็นเท็จพร้อมกัน

→ **เป็นสัจนิรันดร์ (Tautology)**

---

### ข้อ 2: ตรวจสอบว่า $[(p \to q) \wedge p] \to q$ เป็นสัจนิรันดร์หรือไม่ (Modus Ponens)

**วิธีทำ:**

ใช้วิธีสมมติให้ประพจน์เป็นเท็จ แล้วหาข้อขัดแย้ง

สมมติ $[(p \to q) \wedge p] \to q \equiv \mathbf{F}$

จะได้:
- $(p \to q) \wedge p \equiv \mathbf{T}$ ... (1)
- $q \equiv \mathbf{F}$ ... (2)

จาก (1): $p \to q \equiv \mathbf{T}$ และ $p \equiv \mathbf{T}$

แต่ $p \equiv \mathbf{T}$ และ $q \equiv \mathbf{F}$ ทำให้ $p \to q \equiv \mathbf{F}$ — **ขัดแย้ง!**

→ **เป็นสัจนิรันดร์ (Tautology)** ✓

ตารางค่าความจริงยืนยัน:

| $p$ | $q$ | $p \to q$ | $(p \to q) \wedge p$ | ผลรวม |
|:---:|:---:|:---:|:---:|:---:|
| T | T | T | T | **T** |
| T | F | F | F | **T** |
| F | T | T | F | **T** |
| F | F | T | F | **T** |

---

### ข้อ 3: ตรวจสอบว่า $(p \leftrightarrow q) \leftrightarrow [(p \to q) \wedge (q \to p)]$ เป็นสัจนิรันดร์หรือไม่

**วิธีทำ:**

ใช้สมบัติ: $p \leftrightarrow q \equiv (p \to q) \wedge (q \to p)$ (นิยามของ biconditional)

ให้ $X = p \leftrightarrow q$ และ $Y = (p \to q) \wedge (q \to p)$

เนื่องจาก $X \equiv Y$ ดังนั้น $X \leftrightarrow Y \equiv \mathbf{T}$ เสมอ

→ **เป็นสัจนิรันดร์ (Tautology)** ✓

ยืนยันด้วยตารางค่าความจริง:

| $p$ | $q$ | $p \leftrightarrow q$ | $p \to q$ | $q \to p$ | $(p \to q) \wedge (q \to p)$ | ผลรวม |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| T | T | T | T | T | T | **T** |
| T | F | F | F | T | F | **T** |
| F | T | F | T | F | F | **T** |
| F | F | T | T | T | T | **T** |

---

### ข้อ 4: หาประพจน์ที่สมมูลกับ $\sim(p \to q)$

**วิธีทำ:**

**วิธีที่ 1:** ใช้สมบัติ $p \to q \equiv \sim p \vee q$

$$\sim(p \to q) \equiv \sim(\sim p \vee q)$$

ใช้กฎเดอมอร์แกน:

$$\equiv \sim(\sim p) \wedge \sim q$$

ใช้กฎ Double Negation:

$$\equiv p \wedge \sim q$$

**วิธีที่ 2:** คิดเชิงตรรกะ

$p \to q$ เป็นเท็จเพียงกรณีเดียวคือ $p$=T และ $q$=F

ดังนั้น $\sim(p \to q)$ จะเป็นจริงเมื่อ $p$=T และ $q$=F นั่นคือ $p \wedge \sim q$

**ยืนยันด้วยตารางค่าความจริง:**

| $p$ | $q$ | $p \to q$ | $\sim(p \to q)$ | $\sim q$ | $p \wedge \sim q$ |
|:---:|:---:|:---:|:---:|:---:|:---:|
| T | T | T | F | F | F |
| T | F | F | **T** | T | **T** |
| F | T | T | F | F | F |
| F | F | T | F | T | F |

ค่าคอลัมน์ที่ 4 และ 6 ตรงกันทุกแถว

→ $\boxed{\sim(p \to q) \equiv p \wedge \sim q}$
