# AI HR TEAM PLAYBOOK

ระบบต้นแบบ “ทีม HR ที่ทำงานร่วมกับ AI” สำหรับองค์กร E-Commerce / Warehouse

> **AI ทำงาน · คุณตัดสินใจ**

## v0.2.0 — Complete Playbook UI

เวอร์ชันนี้เพิ่ม UI แบบ Playbook ให้ใกล้กับแนวคิดต้นแบบที่แบ่งเนื้อหาเป็นทีม, คนที่ควรใช้ก่อน, ต้นทุนทีมเต็ม, ต้นทุนแบบ SME, เทียบเอเจนซี, ต้นทุนเพิ่มเติม และหลัก Human-in-the-loop

### เมนูหลัก
- Dashboard
- รู้จัก 17 AI Specialists
- 3 คนที่ควรใช้ก่อน
- ต้นทุนทีมเต็ม
- ต้นทุนแบบ SME
- เทียบกับเอเจนซี
- ต้นทุนเพิ่มเติม
- Workflows
- AI ทำงาน · คุณตัดสินใจ

## Repository structure
```text
.
├── index.html              # Playbook UI entry
├── styles.css              # UI styles
├── app.js                  # UI data + interactions
├── agents/                 # 17 specialist role playbooks
├── data/                   # Agent catalog
├── docs/                   # Architecture, workflows, roadmap, versioning
├── VERSION
└── LICENSE
```

## Safe update policy
อัปเดต UI โดยไม่ทับ/ลบ knowledge files ใน `agents/`, `data/`, `docs/` โดยไม่จำเป็น ดู `docs/VERSIONING.md`

## Cost disclaimer
ตัวเลขต้นทุนใน UI เป็น illustrative benchmark สำหรับการคิดเชิงระบบ ไม่ใช่ quotation หรือคำแนะนำด้านงบประมาณจริง โดย reference ตลาดแรงงานไทยปี 2026 ใช้ Adecco Thailand Salary Guide 2026 และแหล่งประกาศงานที่ระบุในเอกสารประกอบ

## Principle
AI ช่วยวิเคราะห์ ร่าง ตรวจ และจัดระบบได้ แต่การอนุมัติวินัย การเลิกจ้าง การเปลี่ยนสภาพการจ้าง การจ่ายเงิน และการตัดสินใจที่มีผลทางกฎหมายต้องมีผู้มีอำนาจเป็นผู้ตัดสินใจ
