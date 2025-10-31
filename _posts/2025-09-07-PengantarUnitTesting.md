---
layout: post
date: 2025-09-07
author: "Kelompok 5 - Sistem Informasi 2023"
title: "Pengantar Unit Testing"
categories: [Software Development, Quality Assurance]
description: Panduan pengantar unit testing, dari konsep dasar, pentingnya, pola AAA (Arrange, Act, Assert), hingga framework populer seperti JUnit, Jest, dan Pytest.
tags: [Unit Testing, SDLC, Testing, QA, JUnit, Jest, Pytest, AAA]
image: /assets/img/pengantar-unit-testing.png
---

# Pengantar Unit Testing

Unit testing memeriksa unit terkecil program (fungsi/metode/kelas) secara terisolasi untuk memastikan setiap bagian bekerja sesuai harapan. Biasanya ditulis dan dijalankan oleh developer sebagai lapisan pertama pertahanan terhadap bug.

## Manfaat utama
- Menemukan bug lebih awal.  
- Membantu refactoring aman.  
- Menjadi dokumentasi penggunaan fungsi.  
- Mempercepat feedback loop development.

## Pola AAA (Arrange, Act, Assert)
1. Arrange: Siapkan objek/data dan kondisi awal.  
2. Act: Panggil fungsi/metode yang diuji.  
3. Assert: Verifikasi hasil sesuai ekspektasi.

## Framework populer
- JUnit (Java) — ekosistem matang untuk JVM.  
- Jest (JavaScript) — zero-config untuk Node/React.  
- Pytest (Python) — sederhana dengan fixtures kuat.

## Contoh singkat (Java/JUnit)
```java
@Test
void testAdd() {
    Calculator calc = new Calculator();
    assertEquals(5, calc.add(2,3));
}
```

## Praktik terbaik singkat
- Buat test yang cepat dan independen.  
- Mock dependency eksternal.  
- Integrasikan test ke CI untuk memastikan regresi terdeteksi cepat.

## Kesimpulan
Unit testing adalah investasi penting untuk kualitas jangka panjang. Menulis test yang jelas dan dapat dipelihara meningkatkan kepercayaan saat melakukan perubahan kode.