---
layout: post
date: 2025-09-14
author: "Kelompok 7 - Sistem Informasi 2023"
title: "Pengantar Selenium WebDriver"
categories: [Software Development, Quality Assurance, Automation]
description: Panduan pengantar Selenium WebDriver, alat automasi browser open-source, keunggulannya, dan contoh test case untuk automasi web.
tags: [Selenium, WebDriver, Automation Testing, QA, Python, Java, Web Testing]
image: /assets/img/pengantar-selenium-webdriver.png
---

# Pengantar Selenium WebDriver

Selenium adalah rangka kerja open-source untuk mengotomatiskan interaksi pada browser. WebDriver adalah API inti yang mengontrol browser dan memungkinkan skrip test berinteraksi seperti pengguna nyata.

## Kapan dan untuk apa gunakan Selenium
Selenium cocok untuk mengautomasi pengujian fungsional aplikasi web di berbagai browser dan platform, terutama untuk regression test dan skenario end-to-end yang melibatkan UI.

Keunggulan utama:
- Gratis dan open-source
- Multi-bahasa (Python, Java, JavaScript, C#, dll.)
- Mendukung banyak browser dan platform
- Mudah diintegrasikan ke framework testing dan pipeline CI

## Langkah dasar penggunaan
1. Pasang library Selenium untuk bahasa Anda (mis. pip install selenium).  
2. Inisialisasi WebDriver (mis. ChromeDriver/GeckoDriver).  
3. Temukan elemen di halaman (by id/name/css/xpath) dan lakukan aksi (click, type, submit).  
4. Validasi hasil (assert URL, presence of element, text, dll.).  
5. Tutup browser.

## Contoh skenario test (ringkas)
- TC-001: Login berhasil dengan kredensial valid.  
- TC-002: Login gagal dengan username/password salah.  
- TC-003: Setelah login, menambahkan item ke cart.

## Contoh kode sederhana (Python)
```python
from selenium import webdriver

driver = webdriver.Chrome()
driver.get("https://saucedemo.com")
driver.find_element("name", "user-name").send_keys("standard_user")
driver.find_element("name", "password").send_keys("secret_sauce")
driver.find_element("css selector", "input[type='submit']").click()
assert "inventory.html" in driver.current_url
driver.quit()
```

## Praktik dan sumber belajar
- Integrasikan Selenium dengan framework (pytest, JUnit) untuk laporan hasil.  
- Gunakan page object pattern untuk pemeliharaan skrip.  
Sumber: dokumentasi Selenium, tutorial online, repo contoh.

## Kesimpulan
Selenium WebDriver adalah alat penting bagi penguji yang ingin mengotomatisasi alur pengguna di browser. Dengan praktik yang baik (struktur test, isolation, CI integration) Selenium meningkatkan kecepatan dan konsistensi pengujian.