# 🎁 Peraduan Gempak Component (CMS-Safe)

Repository ini mengandungi kod sumber dan pengurusan data untuk komponen **Peraduan Gempak** yang dipasang pada CMS Astro Gempak. Komponen ini memaparkan senarai aktif dan arkib bagi **GMW Giveaways** serta **Gempak Movie Night Out** secara dinamik menggunakan API Fetch daripada fail `data.json`.

---

## 🚀 Ciri-Ciri Utama Komponen

- **CMS-Safe & Isolation:** Semua class CSS menggunakan prefix `pgx-` untuk mengelakkan pertembungan gaya (_style collision_) dengan design global pada CMS atau website utama.
- **Dinamik & Ringan:** Dibina menggunakan Pure HTML, CSS, dan Vanilla JS (ES5) tanpa memerlukan external library tambahan (seperti jQuery atau Tailwind).
- **Susunan Status Automatik:** Komponen akan menapis dan menyusun item secara automatik—item berstatus `open` diletakkan di bahagian atas, manakala item berstatus `closed` dipindahkan ke bahagian bawah di bawah penanda **"Sudah Tamat"**.
- **Integrasi Kalendar (.ics):** Fungsi JavaScript akan menjana fail `.ics` secara _on-the-fly_ untuk peraduan aktif yang mempunyai parameter tarikh kalendar.
- **Fully Responsive:** Reka bentuk kad dilaraskan mengikut peranti desktop, tablet, dan peranti mudah alih melalui _media queries_.

---

## 📂 Struktur Fail GitHub

```bash
├── data.json          # Fail pangkalan data (JSON) utama
└── README.md          # Dokumentasi teknikal & fail kod sumber (Fail ini)

data.json
{
  "giveaway": [
    {
      "title": "Giveaway Tiket Konsert LOKALOKO 2026",
      "status": "open",
      "badge": "Sertai Sekarang",
      "day": "28",
      "month": "MEI",
      "dow": "KHA",
      "thumb": "[https://gempak.com/images/poster-lokaloko.jpg](https://gempak.com/images/poster-lokaloko.jpg)",
      "venue": "Stadium Malawati, Shah Alam",
      "link": "[https://gempak.com/gmwgiveaways/lokaloko](https://gempak.com/gmwgiveaways/lokaloko)",
      "cal_date": "20260528",
      "cal_title": "Konsert LOKALOKO 2026"
    }
  ],
  "movie": [
    {
      "title": "Gempak Movie Night Out: Telemovie Astro Raya",
      "status": "closed",
      "badge": "Tamat",
      "day": "15",
      "month": "APR",
      "dow": "RAB",
      "thumb": "[https://gempak.com/images/poster-rayamovie.jpg](https://gempak.com/images/poster-rayamovie.jpg)",
      "venue": "GSC Mid Valley",
      "link": "[https://gempak.com/gempakmovienightout/raya-special](https://gempak.com/gempakmovienightout/raya-special)"
    }
  ]
}{
  "giveaway": [
    {
      "title": "Giveaway Tiket Konsert LOKALOKO 2026",
      "status": "open",
      "badge": "Sertai Sekarang",
      "day": "28",
      "month": "MEI",
      "dow": "KHA",
      "thumb": "[https://gempak.com/images/poster-lokaloko.jpg](https://gempak.com/images/poster-lokaloko.jpg)",
      "venue": "Stadium Malawati, Shah Alam",
      "link": "[https://gempak.com/gmwgiveaways/lokaloko](https://gempak.com/gmwgiveaways/lokaloko)",
      "cal_date": "20260528",
      "cal_title": "Konsert LOKALOKO 2026"
    }
  ],
  "movie": [
    {
      "title": "Gempak Movie Night Out: Telemovie Astro Raya",
      "status": "closed",
      "badge": "Tamat",
      "day": "15",
      "month": "APR",
      "dow": "RAB",
      "thumb": "[https://gempak.com/images/poster-rayamovie.jpg](https://gempak.com/images/poster-rayamovie.jpg)",
      "venue": "GSC Mid Valley",
      "link": "[https://gempak.com/gempakmovienightout/raya-special](https://gempak.com/gempakmovienightout/raya-special)"
    }
  ]
}
JavaScript
var DATA = '[https://raw.githubusercontent.com/NAMA_USER_BARU/REPO_BARU/main/data.json](https://raw.githubusercontent.com/NAMA_USER_BARU/REPO_BARU/main/data.json)';
```
