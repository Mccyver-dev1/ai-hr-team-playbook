# Architecture

```text
                HR DIRECTOR / HR MANAGER
                         │
                  [AI HR ORCHESTRATOR]
                         │
 ┌───────────────┬───────┼────────┬───────────────┐
 Strategy     Lifecycle Compliance  Performance/Data  Knowledge/AI
                         │
              Feishu / HRIS / Payroll / Documents
```

## Workflow
1. User หรือระบบสร้างงาน
2. Orchestrator จัดประเภทงาน
3. เรียก Specialist Agent
4. QA / Compliance ตรวจ
5. Human Approval
6. ส่งผลกลับระบบต้นทาง
7. เก็บบทเรียนลง Knowledge Base

## ระดับสิทธิ
- Read only
- Draft
- Recommend
- Execute with approval
- Human only

งาน High-risk เช่น เงินเดือน วินัย เลิกจ้าง และการเปลี่ยนสภาพการจ้าง ต้องเป็น Human Approval
