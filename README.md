# รายงานสรุปผลการเรียนรู้รายสัปดาห์ (Week 01 – Week 04)

![course](https://img.shields.io/badge/course-KMUTT%20ND69-1a2f5a?style=flat-square)
![track](https://img.shields.io/badge/track-ND01-0e7490?style=flat-square)
![weeks](https://img.shields.io/badge/weeks-01--04-334155?style=flat-square)
![lang](https://img.shields.io/badge/lang-TH-2563eb?style=flat-square)

## โครงการบัณฑิตพันธุ์ใหม่ (Non-Degree) รุ่นที่ 2 ประจำปี 2569 — มหาวิทยาลัยเทคโนโลยีพระจอมเกล้าธนบุรี (KMUTT)
### หลักสูตร ND01: นักพัฒนาอุปกรณ์ Edge AI และ IoT ที่มีความปลอดภัย (Edge AI and Secure IoT Device Developer)
- **ผู้สอน:** ผศ. ดร. สันติ นุราช (Asst. Prof. Dr. Santi Nuratch) | ภาควิชาวิศวกรรมระบบควบคุมและเครื่องมือวัด (INC-KMUTT)
- **รวบรวมและจัดทำโดย:** ผู้เข้าอบรมหลักสูตร ND01

---

## สารบัญแยกตามรายสัปดาห์ (Weekly Modules: Week 01 – Week 04)

เอกสารสรุปผลการเรียนรู้ถูกแยกออกเป็นรายสัปดาห์เพื่อให้สะดวกต่อการศึกษารายหัวข้อและการส่งมอบงาน สามารถคลิกเลือกอ่านแต่ละสัปดาห์ได้จากตารางด้านล่าง:

| สัปดาห์ | หัวข้อการเรียนรู้หลัก | ลิงก์เอกสารสรุป |
| :---: | --- | :---: |
| **Week 01** | **ปฐมนิเทศ พื้นฐาน Edge AI & IoT และสภาพแวดล้อมการจำลอง**<br>• วัตถุประสงค์โครงการและเกณฑ์การประเมินผล<br>• แนวคิด Edge AI vs Cloud AI ในระบบสมองกลฝังตัว<br>• กระบวนการคิดแบบ Simulation-First Paradigm | [📄 เปิดอ่าน Week 01](week01/README.md) |
| **Week 02** | **สถาปัตยกรรมชิป ESP32-S3R8 ฮาร์ดแวร์ ES3C28P และวงจรเชื่อมต่อ**<br>• ซีพียู Xtensa Dual-Core LX7 & Vector Instructions<br>• ลำดับชั้นหน่วยความจำ (ROM, SRAM, Octal PSRAM, Flash, eFuse)<br>• การจองหน่วยความจำ `heap_caps_malloc` & Partition Table<br>• กับดัก Native USB-Serial, วงจรจ่ายไฟ และอุปกรณ์ต่อพ่วงบนบอร์ด ES3C28P | [📄 เปิดอ่าน Week 02](week02/README.md) |
| **Week 03** | **การติดตั้ง ESP-IDF v6.1 และแกนกลาง FreeRTOS บนเครื่องคอมพิวเตอร์**<br>• สถาปัตยกรรมทูลเชน ESP-IDF (CMake, Ninja, Python Venv)<br>• การคอมไพล์ แฟลช และมอนิเตอร์โปรเจกต์ Hello World บน ESP32-S3<br>• ทฤษฎี Preemptive Multitasking & FreeRTOS Task States<br>• กลไกสื่อสารระหว่างทาสก์ (Queue, Mutex, Semaphore, Event Group, Task Notify) | [📄 เปิดอ่าน Week 03](week03/README.md) |
| **Week 04** | **ปฏิบัติการ Onsite Workshop @ อาคาร KX มจธ. (Firmware Engineering Labs)**<br>• การใช้งานเครื่องมือ `rbdev` CLI และสถาปัตยกรรม Thin-App<br>• เจาะลึก Device Labs (ex00 – ex06): แก้ปัญหาฮาร์ดแวร์บล็อกด้วย FreeRTOS<br>• ปฏิบัติการ Special Labs (ex01 – ex06), UI Demos และ RTOS Game Capstones | [📄 เปิดอ่าน Week 04](week04/README.md) |

---

## ภาพรวมเส้นทางการเรียนรู้ (Learning Roadmap)

การเรียนรู้ตลอดระยะเวลา 4 สัปดาห์แรกของหลักสูตร **ND01: นักพัฒนาอุปกรณ์ Edge AI และ IoT ที่มีความปลอดภัย** ได้วางรากฐานทางวิศวกรรมสมองกลฝังตัว (Embedded Systems Engineering) อย่างเข้มข้น โดยเน้นการผสมผสานระหว่างภาคทฤษฎีฮาร์ดแวร์ระดับซิลิคอน, การบริหารจัดการหน่วยความจำ, สถาปัตยกรรมระบบปฏิบัติการเวลาจริง (Real-Time Operating System: FreeRTOS) ตลอดจนการพัฒนาเฟิร์มแวร์เชิงโครงสร้างบนบอร์ดไมโครคอนโทรลเลอร์สมรรถนะสูง **ESP32-S3**

```mermaid
flowchart TD
    subgraph W1["สัปดาห์ที่ 1: Foundation & Simulation"]
        A1["ปฐมนิเทศและเป้าหมาย Edge AI & IoT"] --> A2["Edge AI vs Cloud AI Paradigms"]
        A2 --> A3["Simulation-First Mindset (PC/Wokwi)"]
    end

    subgraph W2["สัปดาห์ที่ 2: Hardware & Embedded Fundamentals"]
        B1["ชิป ESP32-S3R8 Architecture"] --> B2["ลำดับชั้นหน่วยความจำ SRAM/PSRAM/Flash/eFuse"]
        B2 --> B3["Peripherals บอร์ด ES3C28P (LCD, Touch, Audio, RMT)"]
        B3 --> B4["Embedded C & Memory Layout (Heap/Stack/NVS)"]
    end

    subgraph W3["สัปดาห์ที่ 3: ESP-IDF Toolchain & FreeRTOS Core"]
        C1["ติดตั้งและเซ็ตอัป ESP-IDF v6.1"] --> C2["Hello World Bring-up & idf.py Workflow"]
        C2 --> C3["แกนกลาง FreeRTOS บน PC (Tasks, Scheduler, Ticks)"]
        C3 --> C4["กลไก IPC: Queue, Semaphore, Mutex, Notifications"]
    end

    subgraph W4["สัปดาห์ที่ 4: Onsite Workshop @ KX"]
        D1["เครื่องมือ Workshop: rbdev CLI & Thin-App Architecture"] --> D2["Device Labs ex00-ex06 (แก้ปัญหา I/O บล็อกด้วย RTOS)"]
        D2 --> D3["Special Labs ex01-ex06 (Mutex, ISR, Priority, Events)"]
        D3 --> D4["UI Widget Demos & FreeRTOS Game Capstones"]
    end

    W1 --> W2 --> W3 --> W4
```

---

## บทสรุปทักษะทางวิศวกรรมที่ได้รับ (Key Engineering Competencies)

1. **Hardware-Software Co-Design:** สามารถอ่านและทำความเข้าใจวงจรเชื่อมต่อ การเลือกชนิดหน่วยความจำ (SRAM vs PSRAM) การหลีกเลี่ยงข้อจำกัดของขา Strapping Pin และเข้าใจโครงสร้างภายในของ ESP32-S3 อย่างถ่องแท้ ([อ่านเพิ่มเติมใน Week 02](week02/README.md))
2. **Determinism & Real-Time Performance:** เปลี่ยนวิธีคิดจากการเขียนโปรแกรมวนลูปที่ไม่มีความแน่นอน (Super-loop) มาเป็นการจัดสรรสถาปัตยกรรมแบบมัลติทาสก์ที่มีการรับประกันเวลาตอบสนองผ่าน FreeRTOS Preemptive Scheduler ([อ่านเพิ่มเติมใน Week 03](week03/README.md))
3. **Concurrent Data Safety:** สามารถนำเครื่องมือ Inter-Task Communication (Queue, Mutex, Semaphore, Event Group, Task Notification) มาใช้แก้ปัญหาความขัดแย้งของข้อมูลและสภาวะการแย่งชิงทรัพยากรได้อย่างถูกต้อง ([อ่านเพิ่มเติมใน Week 03](week03/README.md) และ [Week 04](week04/README.md))
4. **Toolchain & Industrial Workflow:** เชี่ยวชาญการใช้งานเครื่องมือ ESP-IDF มาตรฐาน ควบคู่กับระบบคำสั่งอัตโนมัติ `rbdev` เพื่อรองรับการพัฒนาซอฟต์แวร์สมองกลฝังตัวที่มีความซับซ้อนสูง ([อ่านเพิ่มเติมใน Week 04](week04/README.md))

---
*เอกสารฉบับนี้จัดทำขึ้นเพื่อเป็นรายงานสรุปผลการเรียนรู้อย่างเป็นทางการ รายวิชา ND01 โครงการบัณฑิตพันธุ์ใหม่ (Non-Degree) มหาวิทยาลัยเทคโนโลยีพระจอมเกล้าธนบุรี (KMUTT)*
