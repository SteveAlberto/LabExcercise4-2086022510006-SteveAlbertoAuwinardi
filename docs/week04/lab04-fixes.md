# Catatan Perbaikan
1. StoreHeader : untuk bagian header saya menambahkan expanded pada columnnya dan memberikan flex, maxlines dan textoverflow, dan saya juga menggunakan flexible untuk bagian ratingnya dengan flex, maxlines dan textoverflow.
2. CategoryBar : untuk bagian categorybar saya menggunakan singlechildscrollview ke arah horizontal dan memindahkan padding kedalamnya.
3. PromoStrip : untuk bagian promostrip juga saya menggunakan singlechildscrollview ke arah horizontal dan memindahkan padding kedalamnya.
4. PromoCard : untuk bagian menuitem saya menggunakan flexible untuk bagian text item.name nya.
5. MenuTile : untuk bagian menutile saya menambahkan expanded dan memasukkan column kedalamnya, lalu spacer saya hilangkan.
6. MenuCard : pada menucard saya menambahkan expanded pada container, menghilangkan heightnya, dan menambahkan maxlines dan textoverflow untuk item.name nya.
7. CartBar : untuk bagian cartbar saya menambahkan flexible dan juga maxlines dan textoverflow pada text pesanan.
8. MenuScreen (landscape) : untuk bagian scaffold saya mengganti isinya dengan layoutbuilder dan customscrollview menggunakan SliverToBoxAdapter, sedangkan daftar menunya memakai sliver builder supaya tetap lazy.
9. MenuScreen (tablet) : saya mengganti breakpoint dengan layoutbuilder pada lebar 600 dp ke atas, dan memakai SliverGrid.builder dengan maxCrossAxisExtent, sedangkan di bawah 600 dp memakai SliverList.builder.
10. MenuScreen (notch dan gesture bar) : saya juga menambahkan safearea kedalam bodynya scaffold untuk notchnya, dan juga pada bottomnavigationbar untuk gesture bar.
11. MenuScreen (zero items) : saya menambahkan pengecekan promos.length >= 2 sebelum promostrip, lalu membuat widget emptystate (ikon, pesan, dan tombol) dengan key empty-state yang ditampilkan lewat SliverFillRemaining, dan searchcontroller supaya tombol reset bisa mengosongkan kolom pencarian.