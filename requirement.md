# Project: Smart IT Helpdesk Portal

## 1. Objective
ระบบบริหารจัดการแจ้งปัญหาไอทีภายในองค์กร สำหรับพนักงานและทีม IT Support

## 2. Core Features (MVP)
1. **Ticket Dashboard:** แสดงรายการปัญหา แบ่งตามสถานะ (New, In Progress, Resolved)
2. **Real-time Search:** ค้นหาปัญหาตามชื่อหรือแผนก
3. **Status Transition:** ปุ่มอัปเดตสถานะปัญหาตามลำดับ: New -> In Progress -> Resolved
4. **Create Ticket Modal:** ฟอร์มแจ้งปัญหาใหม่ (หัวข้อ, แผนก, ความเร่งด่วน: Low, Medium, High)
5. **Metric Cards:** สรุปตัวเลขสถิติตั๋วทั้งหมด และตั๋วแต่ละสถานะ

## 3. Data Specification
- id (INTEGER PRIMARY KEY AUTOINCREMENT)
- title (TEXT NOT NULL)
- department (TEXT NOT NULL: HR, Sales, Marketing, Dev)
- priority (TEXT NOT NULL: Low, Medium, High)
- status (TEXT NOT NULL: New, In Progress, Resolved)
- created_at (TIMESTAMP DEFAULT CURRENT_TIMESTAMP)