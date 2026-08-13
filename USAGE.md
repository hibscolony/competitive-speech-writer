# Panduan Pakai — Skill Competitive Speech Writer

Skill ini bikin AI agent (Antigravity, Claude Code, dll) bisa nulis naskah pidato/orasi kompetisi gaya Indonesia — islami, kebangsaan, atau akademik — lengkap dengan rima strategis, greeting multibahasa, humor natural, dan argumen yang berbasis sumber valid (bukan ngarang).

---

## 1. Instalasi (dari repo GitHub)

### Clone repo

```bash
git clone https://github.com/<username>/competitive-speech-writer.git
cd competitive-speech-writer
```

### Global di Antigravity (kepake di semua project)

Cara paling gampang, copy foldernya:

```bash
mkdir -p ~/.gemini/config/skills
cp -R . ~/.gemini/config/skills/competitive-speech-writer
```

Atau, kalau mau tiap `git pull` di repo langsung ke-apply tanpa copy ulang, pakai symlink:

```bash
mkdir -p ~/.gemini/config/skills
ln -s "$(pwd)" ~/.gemini/config/skills/competitive-speech-writer
```

Setelah itu, restart Antigravity (tutup, buka ulang), lalu cek: tanya ke agent — *"skill apa aja yang terinstall?"* — `competitive-speech-writer` harus muncul di daftar.

> Folder `~/.gemini/config/skills/` itu ada di **home directory** kamu, bukan di dalam project mana pun. Sekali taruh di situ, otomatis aktif di **semua** project yang kamu buka di Antigravity — gak perlu diinstall ulang tiap ganti project/folder kerja.

Kalau gak kebaca di path itu (beda versi Antigravity), coba juga:
- `~/.gemini/antigravity/skills/`
- `~/.gemini/antigravity-cli/skills/` (khusus Antigravity CLI)

### Workspace (cuma 1 project tertentu)

Clone langsung ke dalam folder project:

```bash
mkdir -p <root-project-kamu>/.agents/skills
git clone https://github.com/<username>/competitive-speech-writer.git <root-project-kamu>/.agents/skills/competitive-speech-writer
```

### Update ke versi terbaru

Kalau pakai symlink (global) atau clone langsung (workspace):

```bash
cd ~/.gemini/config/skills/competitive-speech-writer   # atau path workspace-nya
git pull
```

Kalau pakai `cp -R` (bukan symlink), ulangi `cp -R` setelah `git pull` di repo aslinya — copy-nya gak otomatis ke-update.

### Tool lain di luar Antigravity

Format `SKILL.md` ini open standard, portable ke tool lain — clone atau symlink ke folder skills masing-masing:
- Claude Code → `~/.claude/skills/`
- Cursor → `~/.cursor/skills/`
- Gemini CLI → `~/.gemini/skills/`

---

## 2. Cara Manggil

Gak perlu sebut nama skill-nya. Cukup minta pidato secara natural dalam satu pesan, brief + sumber sekaligus:

> "Bikinin pidato tema kemandirian energi, 5 menit. Sumbernya UU No. 30/2007 tentang Energi, data BPS rasio elektrifikasi, QS Al-A'raf ayat 56."

---

## 3. Aturan Sumber (wajib, gak ada jalan pintas)

- Tiap naskah kompetisi butuh **3–5 sumber** (ayat/hadits, UU/data resmi, jurnal/laporan, dsb).
- Sumbernya **harus dari kamu** — boleh lengkap (teks penuh) atau setengah jadi:
  - link
  - potongan referensi: *"QS Al-Hujurat soal tabayyun"*, *"hadits tentang menjaga lisan"*, *"UU ITE"*
- Kalau setengah jadi, agent boleh cari & lengkapin detail persisnya sendiri (nomor ayat, wording, nomor pasal) — ini tetap dihitung *kamu yang kasih sumber*, cuma agent yang ngerjain detailnya.
- Kalau kamu **sama sekali gak kasih arah sumber**, agent akan berhenti dan nanya balik dulu — nyaranin tipe sumber yang cocok buat tema itu — bukan asal nulis atau asal cari sendiri.
- Kalau kamu eksplisit minta *"carikan ayat yang cocok"* tanpa kasih topik, hasil carian agent jadi **proposal** yang perlu kamu setujui dulu, bukan otomatis masuk naskah.

---

## 4. Bahasa & Nada

Default Bahasa Indonesia, formal-kompetitif. Tinggal sebut di kalimat permintaan kalau mau beda, misal: *"bahasa Inggris"*, *"tone-nya youthful dan ada humor"*, *"buat lomba orasi islami"*.

---

## 5. Yang Kamu Terima di Output

- Judul pidato
- Naskah lengkap siap dibacakan (bukan outline)
- Daftar **Sumber** yang dipakai + catatan cara pakainya — buat dicek ulang sebelum dipakai lomba beneran
- Estimasi durasi baca

---

## 6. Fitur Gaya yang Sudah Ter-encode

- **Rima strategis** — dipakai kuat di opening/transisi/klimaks/closing, bukan dipaksa di semua kalimat (biar gak kedengaran "maksa nyanyi")
- **Greeting multibahasa/kedaerahan** kalau relevan sama tema atau konteks lomba
- **Humor natural** 1–2 titik, sebagai jeda napas, gak motong momentum argumen
- **Solusi 3 langkah** yang gampang diinget (nama pendek + makna jelas + aksi konkret)
- **Anti-klise** — skill ini otomatis ngindarin frasa AI generik kayak "di era yang serba digital" atau "tidak dapat dipungkiri"

---

## 7. Mode Kontrol Penuh (opsional)

Kalau mau kunci semua detail dari awal (nama lomba, subtema, audiens, tone, requirement khusus), isi `templates/REQUEST_TEMPLATE.md` dan `templates/SOURCE_PACK_TEMPLATE.md`. Ini opsional — buat pemakaian sehari-hari, satu kalimat natural di atas sudah cukup.

---

## 8. Troubleshooting

| Masalah | Coba ini |
|---|---|
| Skill gak muncul di daftar | Cek nama folder tujuan persis `competitive-speech-writer` dan ada `SKILL.md` langsung di dalamnya (bukan kesimpen di satu folder lagi di dalamnya, misal `.../competitive-speech-writer/competitive-speech-writer/SKILL.md`). Restart session Antigravity. |
| Skill gak keupdate padahal udah `git pull` | Kalau instalasinya pakai `cp -R` (bukan symlink), `git pull` di repo asli gak otomatis ke-apply — copy ulang manual, atau ganti ke symlink biar auto-update. |
| Agent tetap nulis walau sumber kurang, atau tetap nanya walau sumber udah lengkap | Kemungkinan versi `SKILL.md` yang terinstall belum yang terbaru — `git pull` lalu copy ulang/pastikan symlink-nya nunjuk ke commit terbaru, restart. |
| Rima kerasa kurang/kebanyakan | Gak perlu edit skill, tinggal bilang di chat: *"rima-nya diperbanyak di bagian solusi"* atau *"kurangin rima-nya"*. |
| Mau ganti bahasa/tone tengah jalan | Sebut langsung di pesan berikutnya, gak perlu ulang dari awal. |
