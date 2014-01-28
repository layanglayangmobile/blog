---
layout: post
title: Mencoba Ghost
---

Ghost memang masih baru, seperti yang saya sudah bahas [sebelumnya](http://praw.me/kesan-awal-ghost/). Beberapa fitur masih belum ada, salah satu yang terpenting adalah analytics. 

Namun setelah mencari tahu, kita sudah bisa menyematkan script Google Analytics ke dalam Ghost kita, sehingga kita bisa melacak statistik dan menganalisis traffic dari blog kita yang menggunakan Ghost.

Caranya pun memang belum praktis, namun cukup mudah. Intinya adalah menambahkan script Google Analytics ke dalam file default.hbs.

Akses filenya menggunakan FTP atau SSH, lalu locate file default.hbs
{<1>}![alt](https://dl.dropboxusercontent.com/u/27354932/buatghost/default.hbsss.png)

Setelah itu masukkan script Google Analytics tepat di atas `</head>`
{<2>}![alt](https://dl.dropboxusercontent.com/u/27354932/buatghost/nano.png)

Setelah itu restart service Ghost
`service ghost restart`

Niscaya setelah restart, blogmu sudah terlacak oleh Google Analytics. Mudah bukan?
