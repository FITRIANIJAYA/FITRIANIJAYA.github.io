---
layout: post
date: 2025-09-07
author: "Kelompok 6 - Sistem Informasi 2023"
title: "API Testing"
categories: [Software Development, Quality Assurance, API]
description: Pengantar API Testing, mengapa ini penting, anatomi request & response, serta tools populer seperti Postman dan SoapUI.
tags: [API Testing, API, QA, Quality Assurance, Postman, SoapUI, REST, SOAP]
image: /assets/img/api-testing.png
---

# API Testing

API testing fokus pada pengujian lapisan backend (business logic) aplikasi melalui endpoint API. Tujuannya memastikan request diproses benar dan response sesuai kontrak.

## Mengapa penting?
- Mendeteksi bug di tingkat layanan lebih cepat daripada menunggu di UI.  
- Mempermudah otomasi dan mempercepat siklus rilis.  
- Menjamin integritas data dan keamanan antar layanan.

## Komponen dasar request & response
- Request: HTTP method (GET, POST, PUT, DELETE), URL/endpoint, headers, body (JSON/XML).  
- Response: status code (200, 201, 400, 401, 404, 500), headers, body (payload), dan response time.

## Tools populer
- Postman: user-friendly untuk eksplorasi API, collection, test scripts, environment.  
- SoapUI: kuat untuk SOAP dan REST pada skenario enterprise, mendukung data-driven tests dan security testing.

## Praktik testing
- Validasi status code dan struktur response.  
- Uji kasus edge (invalid input, missing fields).  
- Performance test pada endpoint kritis.  
- Keamanan: otentikasi, otorisasi, injection tests.

## Kesimpulan
API testing adalah bagian krusial untuk memastikan layanan backend berfungsi dan terintegrasi dengan benar. Menggunakan tooling yang tepat (Postman/SoapUI) serta otomasi meningkatkan kecepatan dan keandalan pengujian.