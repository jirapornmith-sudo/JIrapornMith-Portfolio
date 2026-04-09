# Project IS411 - StyleSwipe Community

โปรเจกต์วิชา IS411 พัฒนาโดยใช้ SvelteKit + FastAPI

---

### My Role:

- ออกแบบและพัฒนาหน้า **Community Feed** ทั้งหมด
  - แสดงโพสแฟชั่นของ Customer แบบ Social Feed
  - ระบบกรองโพสด้วย Tags (Woman, Men, Vintage, Y2K, Others)
  - Compact Card Layout แบบ Threads/Twitter
  - Horizontal Image Carousel ในแต่ละการ์ด

- ออกแบบและพัฒนาหน้า **Post Detail**
  - แสดงรายละเอียดโพสและคอมเมนต์
  - ระบบคอมเมนต์แบบ Dynamic (พิมพ์แล้วขึ้นทันที)
  - Dropdown เลือกเรียงคอมเมนต์ Recent / Popular
  - แสดงรูปโปรไฟล์และชื่อตาม User ที่ Login อยู่

- เชื่อมต่อ **FastAPI** ในส่วนของ Community
  - ดึงโพสทั้งหมดจาก `/posts/search`
  - กรองโพสด้วย Tag ผ่าน API
  - ใช้ SvelteKit `+page.server.js` ดึงข้อมูลฝั่ง Server

- พัฒนา **Svelte Store** (`shared.js`) สำหรับเก็บข้อมูล User ที่ Login
  - ใช้ `writable` store เพื่อ sync ข้อมูล User ข้ามหน้า
  - แสดงชื่อและรูปโปรไฟล์ของ User ที่ Login ในคอมเมนต์
  - Redirect ไปหน้า Signin ถ้ายังไม่ได้ Login

---

### Tech Stack ที่ใช้:
- **Frontend**: SvelteKit, Bulma CSS, Font Awesome
- **Backend**: FastAPI, SQLModel, SQLite
- **Key Concepts**: Dynamic Routing `[id]`, Svelte Store, `$state()`, `bind:value`, `{#each}`, `{#if}`, `fetch()`

---

### Credit:
Original Repository: [(https://github.com/prichladapha/ProjectIS411.git)]
