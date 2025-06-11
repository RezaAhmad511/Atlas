Setelah mengekspor data dari file excel pada Realsa data, lakukan uji integritas, jika terbukti benar maka akan muncul 0 data validity error detected pada verify fields
Lalu lakukan "Analyze - Sequence" pada voucher number, hasilnya akan menunjukkan 0 data sequence errors. jika memang tidak terdapat data yang eror pada bagian sequence di voucher number
Langkah ketiga, lakukan analisis pada bagian "gaps" untuk melihat apakah ada yang kosong pada "voucher Number". Fungsinya untuk melihat pengeluaran pada voucher diluar pengeluaran pada kas kecil
pada bagian Analyze Gaps, hasilnya memang akan ada gap dikarenakan pencatatan yang terjadi adalah pencatatan awal tahun
Langkah empat lakukan analisis untuk melihat duplikasi pada voucher number. hasilonya akan berbentuk 0 duplicates. dan hal tersebut menutup pengujian test of control: Integrity test pada arbutus
Pada bagian test of control : Attribute Sampling, akan dilakukan vouching untuk melihat otorisasi. caranya klik pada extract kemudian pilih amount credit dan lihat between lalu cek pengeluaran yang telah dibagi menjadi 3 lapisan yaitu :
1. 20.000.000 - 50.000.000 memerlukan otorisassi kepala bagian
2. 50.000.000 - 100.000.000 otorisasi manajer keuangan
3. >100.000.000 otorisasi direktur utama 
Kemudian level otorisasi akan dibagi menjadi 3 sesuai lapisan-lapisan yg telah ditentukan. berikut hasil otorisasi lv 1
hasil otorisasi lv 2
hasil otorisasi lv 3
Menggunakan edit table layout, masukkan table yang telah dibuat pada "add column" pada voucher number kemudian hasilnya ada pada "status control" yang telah dibuat pada table tersebut
   berikut adalah hasil di command log setelah data control di classify. masing-masing akan tertera hasilnya. dan akan sesuai dengan hasil otorisasi
   Selanjutnya yaitu pengujian piutang, masukkan sheet AR di arbutus.
   >kemudian klik analyze - verify. hasilnya akan 0 eror
   >kemudian analyze sequence di cust number. hsilnya akan spti ini karna memang bawaan dri arbutus.
   >lalu analyze pada bagian duplicate. dan hasilnya akan ada sekitar 263 duplicate karna beberapa customer realsa melakukan beberapa transaksi, jadi wajar.
   selanjutnya masukkan pada ustomer credit limit untuk melihat transaksi yg berjumlah besar
   >selanjutnya kelompokkan piutang customer untuk melihat credit limit per customer
   >beikut adalah hasil, jika kita memilih untuk mengubah screen menjadi data. persentase merupakan yg paling penting
   >berikut adalah hasil ketika mengcompare credit limit dan piutang (AR) dan disini ditambahkan credit max nya
   >Kmeudian akan menambahkan tabel disebelahnya untuk melihat mana yang melebihi mana yg tidak dengan cara berikut:
   >berikut adalah alternatif lain
