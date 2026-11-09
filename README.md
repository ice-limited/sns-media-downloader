# IceLimited SNS Media Downloader

Source repository สำหรับเว็บแอปดาวน์โหลดและประมวลผลสื่อ ทำงานบนเครื่องผู้ใช้คนเดียว รองรับ macOS, Windows และ Linux

Repository นี้เป็นส่วน source code ของ workspace `sns-media-downloader-workspace` ซึ่งเก็บ CONTEXT.md, ข้อกำหนด agent, แผนฟีเจอร์ และบันทึกประชุมไว้ที่ระดับ workspace อ่านบริบทหลักก่อนเริ่มงานทุกครั้ง

เมื่อ checkout ผ่าน workspace อ่าน [CONTEXT.md](../../CONTEXT.md), [AGENTS.md](../../AGENTS.md) และ [MODEL-ROUTING.md](../../MODEL-ROUTING.md) ที่ workspace root หาก clone repository นี้แยกต่างหาก ให้เปิด workspace repository `git@github.com:ice-limited/sns-media-downloader-workspace.git` เพื่ออ่านเอกสารเหล่านี้

## สถานะ

อยู่ระยะวางแผน init ยังไม่มี implementation หรือผลการทดสอบแอป มี [plan stubs 001–018](../../plans/README.md) และ [roadmap init](../../docs/init-project-roadmap.md) ใน workspace แล้ว ซึ่งยังไม่อนุมัติ implement โครงสร้างที่เสนอคือ `apps/web` สำหรับ Next.js Web+API และ `apps/worker` สำหรับ background jobs ภายใต้ repository เดียว ยังไม่ได้สร้างโฟลเดอร์หรือเลือก dependency จริง

**ห้าม commit git ถ้าไม่มีการสั่ง** ก่อน commit ที่ผู้ใช้สั่งทุกครั้ง ต้องอัปเดต CHANGELOG.md ใน workspace และใน source repository ตามส่วนที่เปลี่ยนแปลง

ข้อกำหนดหลายภาษาเริ่ม UI/app-owned messages ด้วย EN/TH และเพิ่มภาษาได้ในอนาคต ดู [019](../../plans/019-multilingual-en-th.md) และ [architecture ภาษา](../../docs/internationalization.md) โดยทำ foundation ภาษาก่อน UI shell; ยังไม่ได้เลือก library หรือเริ่ม source implementation

เจ้าของเลือก [MIT License](LICENSE) สำหรับโครงการแล้ว License ของแอปไม่ให้สิทธิ์ใน media ที่ดาวน์โหลด; dependency, binary และ font มี license แยกที่ต้องตรวจสอบ
