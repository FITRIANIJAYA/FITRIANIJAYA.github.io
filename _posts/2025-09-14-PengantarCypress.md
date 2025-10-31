---
layout: post
date: 2025-09-14
author: "Kelompok 8 - Sistem Informasi 2023"
title: "Pengantar Cypress"
categories: [Software Development, Quality Assurance, Automation]
description: Pengantar Cypress, framework end-to-end testing modern untuk aplikasi web. Mencakup setup, perintah dasar, keunggulan, dan contoh test case.
tags: [Cypress, Automation Testing, E2E Testing, QA, JavaScript, Web Testing]
image: /assets/img/pengantar-cypress.png
---

# Pengantar Cypress

Cypress adalah framework modern untuk end-to-end testing aplikasi web dengan pengalaman developer yang interaktif. Karena berjalan di dalam browser, Cypress memberikan hasil yang stabil dan tooling visual untuk debugging.

## Keunggulan utama
- Test runner interaktif dan visual (“time travel” snapshots).  
- Automatic waits sehingga mengurangi kebutuhan sleep/manual waits.  
- Mudah dipasang lewat npm dan mendukung headless runs untuk CI.  
- Cocok untuk testing E2E, integration, dan component testing.

## Instalasi singkat
1. npm init -y  
2. npm install cypress --save-dev  
3. npx cypress open (membuka Test Runner)  
4. npx cypress run (menjalankan tes headless)

## Perintah dasar (intuitif)
- cy.visit(url) — buka halaman  
- cy.get(selector) — pilih elemen  
- cy.contains(text) — cari elemen berdasar teks  
- cy.click(), cy.type(text) — aksi pada elemen  
- cy.url().should('include', '/path') — assertion

## Contoh test (Login)
```javascript
describe('Login Test', () => {
  it('logs in with valid credentials', () => {
    cy.visit('https://saucedemo.com');
    cy.get('input[name="user-name"]').type('standard_user');
    cy.get('input[name="password"]').type('secret_sauce');
    cy.get('input[type="submit"]').click();
    cy.url().should('include', '/inventory.html');
  });
});
```

## Tips penggunaan
- Gunakan fixtures dan environment variables untuk data sensitif.  
- Manfaatkan Test Runner saat debugging.  
- Kombinasikan dengan CI untuk menjalankan tes otomatis setiap commit.

## Kesimpulan
Cypress mempercepat pembuatan dan debugging tes E2E untuk aplikasi modern. Fitur interaktif dan automatic waits membuat tes lebih mudah dibuat dan lebih stabil dibanding beberapa pendekatan tradisional.