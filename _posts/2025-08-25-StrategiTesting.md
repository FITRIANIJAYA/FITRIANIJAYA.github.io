---
layout: post
date: 2025-08-25
author: "Kelompok 1 - Sistem Informasi 2023"
title: "Strategi Testing"
categories: [Software Development, Quality Assurance]
description: Panduan komprehensif mengenai strategi software testing, mencakup siklus hidup (STLC), berbagai level klasifikasi (Abstraction, Function, Domain, Structure), dan pentingnya testing dalam SDLC.
tags: [Software Testing, STLC, SDLC, Unit Testing, Integration Testing, System Testing, Black Box, White Box, Quality Assurance]
image: /assets/img/strategi-testing.png
---

# Strategi Pengujian Perangkat Lunak

## Pengertian singkat
Software testing adalah kegiatan terstruktur untuk mengevaluasi perangkat lunak dengan tujuan menemukan cacat dan memastikan aplikasi memenuhi kebutuhan fungsional serta non-fungsional sebelum dirilis.

## Mengapa testing krusial?
Testing mengurangi risiko, meningkatkan keandalan, memperbaiki pengalaman pengguna, dan menghemat biaya perbaikan jika bug ditemukan lebih awal. Selain itu testing membangun kepercayaan stakeholder.

Ringkasan manfaat:
- Verifikasi & validasi spesifikasi
- Mengurangi risiko kegagalan sistem
- Hemat biaya perbaikan
- Meningkatkan keamanan dan UX
- Bukti kualitas bagi stakeholder

## Peran testing di SDLC
Testing harus menjadi aktivitas berkelanjutan sepanjang SDLC — bukan hanya fase akhir. Pendekatan modern mendorong "shift-left" (uji lebih awal) dan integrasi testing dalam CI/CD.

Contoh integrasi:
- Unit tests di development
- Integration tests saat penggabungan modul
- System & Acceptance tests sebelum release

## STLC — Siklus Pengujian
STLC adalah rangka kerja untuk melaksanakan pengujian secara sistematis. Fase umum:
1. Test Planning — strategi, ruang lingkup, sumber daya.
2. Test Design — pembuatan test case, data, RTM.
3. Test Execution — menjalankan test, logging bug, regression.
4. Reporting & Closure — analisis hasil, metrik, rekomendasi.

## Aktivitas tiap fase (intinya)
- Perencanaan: dokumen Test Plan, estimasi effort.
- Desain: test cases, skenario end-to-end, expected results.
- Eksekusi: jalankan test, catat hasil, retest setelah perbaikan.
- Pelaporan: test summary, bug metrics, rekomendasi technical/business.

## Level pengujian (Testing Pyramid)
- Unit Testing — pengujian fungsi/kelas terkecil (developer).
- Integration Testing — verifikasi antar-modul atau layanan.
- System Testing — pengujian end-to-end pada sistem utuh.
- Acceptance Testing (UAT) — validasi oleh pengguna atau klien.

## Klasifikasi pengujian
Pengujian dapat diklasifikasikan menurut beberapa dimensi:

1. Berdasarkan level abstraksi: Unit, Integration, System, UAT.  
2. Berdasarkan fungsi: Functional (apa yang dilakukan) vs Non-functional (bagaimana sistem bekerja — performa, keamanan, usability).  
3. Berdasarkan domain: perfomance testing, security testing, usability testing, compatibility, dll.  
4. Berdasarkan struktur: Black-box (tanpa pengetahuan kode), White-box (berdasarkan kode), Gray-box (pengetahuan sebagian).

## Contoh singkat tiap tipe testing
- Unit: test logika fungsi dengan framework (JUnit/Jest/pytest).
- Integration: tes API end-to-end antara service A dan B.
- System: alur beli produk sampai konfirmasi email.
- UAT: klien melakukan uji operasional sebelum go-live.
- Performance: load test dengan JMeter atau k6.
- Security: penetration test & scanning (OWASP ZAP, Burp).
- Usability: usability testing, heatmap, A/B test.

## Teknik pengujian black-box
Equivalence partitioning, boundary value analysis, decision tables, state transition — dipakai untuk mendesain test case dari perspektif pengguna.

## Teknik white-box
Statement/branch/path coverage, loop testing — bertujuan memastikan alur kode teruji.

## Pelaporan dan metrik penting
- Test coverage, pass rate, bug count, defect density, severity/priority breakdown.  
Gunakan metrik untuk memutuskan rilis dan prioritas perbaikan.

## Praktik terbaik singkat
- Mulai testing lebih awal (shift-left).
- Otomatiskan pengujian repetitif.
- Tulis test case yang jelas dan dapat direproduksi.
- Gunakan data nyata saat mungkin.
- Dokumentasikan dan kolaborasi erat antara dev & QA.

## Kesimpulan
Testing adalah bagian tak terpisahkan dari kualitas perangkat lunak. Strategi yang terstruktur dan kombinasi metode (manual + automated, black-box + white-box) memastikan produk lebih andal, aman, dan memuaskan pengguna.

## Referensi
Materi disusun dari presentasi kelompok dan sumber umum (ISTQB, OWASP, tool docs). Lihat bahan presentasi untuk detail dan contoh penuh.