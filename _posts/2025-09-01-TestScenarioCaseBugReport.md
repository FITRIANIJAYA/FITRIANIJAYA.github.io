---
layout: post
date: 2025-09-01
author: "Kelompok 4 - Sistem Informasi 2023"
title: "Test Scenario, Test Case, dan Bug Report"
categories: [Software Development, Quality Assurance]
description: Panduan praktis untuk memahami Test Scenario (Apa yang diuji), Test Case (Bagaimana menguji), dan Bug Report (Pelaporan kesalahan).
tags: [Test Scenario, Test Case, Bug Report, QA, Quality Assurance, Testing]
image: /assets/img/test-scenario-test-case-and-bug-report.png
---

# Test Scenario, Test Case, dan Bug Report

## Perbedaan singkat
- Test Scenario: ringkasan fitur atau alur yang perlu diuji (Apa).  
- Test Case: langkah rinci untuk menguji scenario tersebut (Bagaimana).  
- Bug Report: catatan formal ketika actual result berbeda dari expected result.

## Komponen penting Test Case
- ID, judul, precondition, langkah, data uji, expected result, actual result, status (Pass/Fail), catatan.

## Menulis Bug Report yang efektif
Isi minimal:
1. Judul singkat & jelas.  
2. Langkah reproduksi terperinci.  
3. Hasil yang diharapkan vs hasil aktual.  
4. Screenshot/logs/recording bila ada.  
5. Severity & Priority.  
6. Lingkungan pengujian (build, OS, browser).  
7. Assignee & reporter.

## Severity vs Priority
- Severity: dampak teknis bug (Critical → Low).  
- Priority: urgensi perbaikan dari sisi bisnis (P1 → P4).

## Praktik untuk mengurangi bug
- Pahami requirement dengan jelas.  
- Lakukan unit tests dan code reviews.  
- Siapkan test plan & otomasi untuk regresi.  
- Kolaborasi aktif antara developer & QA.

## Kesimpulan
Test scenario dan test case adalah dasar kegiatan QA; bug report adalah mekanisme komunikasi untuk memperbaiki masalah. Dokumentasi yang baik dan proses yang teratur membantu mempercepat perbaikan dan meningkatkan kualitas produk.