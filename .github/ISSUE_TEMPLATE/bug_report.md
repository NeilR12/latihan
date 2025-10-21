name: "🐞 Bug Report"
description: Laporkan bug atau error yang kamu temukan di project ini.
title: "[Bug]: "
labels: ["bug"]
assignees: [NeilR12]

body:
  - type: markdown
    attributes:
      value: |
        Terima kasih sudah bantu ngecek project ini 🙏  
        Tolong isi laporan bug di bawah dengan detail biar bisa cepat ditangani.

  - type: input
    id: bug_summary
    attributes:
      label: "🧩 Ringkasan Bug"
      description: Jelaskan singkat apa masalahnya.
      placeholder: "Contoh: Tombol login gak bisa diklik"

  - type: textarea
    id: steps
    attributes:
      label: "🪜 Langkah untuk Mereproduksi"
      description: Urutan langkah agar bug ini bisa direproduksi.
      placeholder: |
        1. Buka halaman login  
        2. Isi username dan password  
        3. Klik tombol login  
        4. Tidak ada respon

  - type: textarea
    id: expected
    attributes:
      label: "✅ Perilaku yang Diharapkan"
      description: Apa yang seharusnya terjadi?
      placeholder: "Setelah klik tombol login, user diarahkan ke dashboard"

  - type: dropdown
    id: severity
    attributes:
      label: "🔥 Tingkat Keparahan"
      options:
        - Rendah
        - Sedang
        - Tinggi
        - Kritis

  - type: input
    id: environment
    attributes:
      label: "💻 Lingkungan Sistem"
      description: Detail sistem tempat bug muncul.
      placeholder: "Windows 11 / Chrome 120 / App v1.2.3"

  - type: textarea
    id: evidence
    attributes:
      label: "📸 Bukti / Screenshot"
      description: Upload screenshot atau log error (jika ada).
      placeholder: "Seret & lepaskan file di sini"

  - type: textarea
    id: notes
    attributes:
      label: "📝 Catatan Tambahan"
      description: Info lain yang bisa bantu tim memahami bug.
      placeholder: "Misal: bug hanya muncul kalau user belum login"
