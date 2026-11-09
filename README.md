# IceLimited SNS Media Downloader

Source repository สำหรับเว็บแอปดาวน์โหลดและประมวลผลสื่อ ทำงานบนเครื่องผู้ใช้คนเดียว รองรับ macOS, Windows และ Linux

Repository นี้เป็นส่วน source code ของ workspace `sns-media-downloader-workspace` ซึ่งเก็บ CONTEXT.md, ข้อกำหนด agent, แผนฟีเจอร์ และบันทึกประชุมไว้ที่ระดับ workspace อ่านบริบทหลักก่อนเริ่มงานทุกครั้ง

เมื่อ checkout ผ่าน workspace อ่าน [CONTEXT.md](../../CONTEXT.md), [AGENTS.md](../../AGENTS.md) และ [MODEL-ROUTING.md](../../MODEL-ROUTING.md) ที่ workspace root หาก clone repository นี้แยกต่างหาก ให้เปิด workspace repository `git@github.com:ice-limited/sns-media-downloader-workspace.git` เพื่ออ่านเอกสารเหล่านี้

## สถานะ

อยู่ระยะจัดทำ context ยังไม่มี implementation, feature plan หรือผลการทดสอบแอป โครงสร้างที่เสนอคือ `apps/web` สำหรับ Next.js Web+API และ `apps/worker` สำหรับ background jobs ภายใต้ repository เดียว ยังไม่ได้สร้างโฟลเดอร์หรือเลือก dependency จริง

**ห้าม commit git ถ้าไม่มีการสั่ง** ก่อน commit ที่ผู้ใช้สั่งทุกครั้ง ต้องอัปเดต CHANGELOG.md ใน workspace และใน source repository ตามส่วนที่เปลี่ยนแปลง

เจ้าของเลือก [MIT License](LICENSE) สำหรับโครงการแล้ว License ของแอปไม่ให้สิทธิ์ใน media ที่ดาวน์โหลด; dependency, binary และ font มี license แยกที่ต้องตรวจสอบ
