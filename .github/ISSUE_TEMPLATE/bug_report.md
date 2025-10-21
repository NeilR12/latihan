---
name: Bug report
about: Create a report to help us improve
title: "[bug]"
labels: bug, documentation, enhancement
assignees: NeilR12

---

name: "🐞 Bug Report"
description: Laporkan bug atau error yang kamu temukan di project ini
title: "[Bug]: "
labels: ["bug"]
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        Terima kasih sudah bantu ngecek project ini 🙏  
        Tolong isi laporan bug di bawah dengan detail biar bisa cepat ditangani.

  - type: input
    id: bug_summary
    attributes:
      label: "Ringkasan Bug"
      description: Jelaskan singkat apa masalahnya
      placeholder: Contoh: Tombol login gak bisa diklik

  - type: textarea
    id: steps
    attributes:
      label: "Langkah untuk Mereproduksi"
      description: Tulis urutan langkah supaya bug ini bisa direproduksi
      placeholder: |
        1. Buka halaman login
        2. Isi username dan password
        3. Klik tombol login
        4. Gak ada respon

  - type: textarea
    id: expected
    attributes:
      label: "Perilaku yang Diharapkan"
      description: Apa yang seharusnya terjadi?
      placeholder: Setelah klik tombol login, user diarahkan ke dashboard

  - type: dropdown
    id: severity
    attributes:
      label: "Tingkat Keparahan"
      options:
        - Rendah
        - Sedang
        - Tinggi
        - Kritis

  - type: input
    id: environment
    attributes:
      label: "Lingkungan Sistem"
      description: Tuliskan detail sistem saat bug muncul
      placeholder: Windows 11 / Chrome 120 / App v1.2.3

  - type: textarea
    id: evidence
    attributes:
      label: "Bukti / Screenshot"
      description: Upload screenshot atau log error kalau ada
      placeholder: Seret & lepaskan file di sini

  - type: textarea
    id: notes
    attributes:
      label: "Catatan Tambahan"
      description: Info lain yang bisa bantu tim memahami bug ini
      placeholder: Misal: bug cuma muncul kalau user belum login
