# Versioning & GitHub Safety

## Current version
`v0.2.0`

## สิ่งที่เพิ่มใน v0.2.0
- เพิ่ม UI แบบ Playbook + Sidebar navigation
- เพิ่มเมนูต้นทุนทีมเต็ม / SME / Agency / ต้นทุนเพิ่มเติม
- เพิ่ม 17 AI Specialist cards + search + filter + profile dialog
- เพิ่ม workflow และ Human-in-the-loop governance
- เพิ่ม salary-cost comparison เป็น illustrative benchmark

## กติกาการอัปเดต
1. ห้ามลบ `agents/`, `data/`, `docs/` เดิมเพียงเพื่ออัปเดต UI
2. ก่อนแก้ไขให้สร้าง branch เช่น `ui/v0.2.0`
3. ตรวจ `git status` และ `git diff` ก่อน commit
4. Commit แยกตามงาน เช่น `feat(ui): add playbook sidebar`
5. ห้าม commit `.env`, API key, token หรือข้อมูลพนักงานจริง
6. Tag release เมื่อทดสอบแล้ว เช่น `v0.2.0`
7. หากต้องการย้อนกลับ ให้ใช้ tag/commit ก่อนหน้า ไม่ใช้ `git reset --hard` แบบไม่ตรวจสอบ

## Suggested Git flow
```bash
git checkout -b ui/v0.2.0
git status
git diff --check
git add index.html styles.css app.js docs/VERSIONING.md docs/CHANGELOG.md VERSION
git commit -m "feat(ui): add complete HR team playbook navigation"
git push -u origin ui/v0.2.0
```

จากนั้นตรวจบน GitHub และ merge เข้า `main` เมื่อผ่านการทดสอบเท่านั้น
