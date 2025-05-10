# streambuilder_wildan

A new Flutter project.

## Praktikum 6
### Soal 12
![Capture soal 12](assets/streambuilder.gif)

1. Langkah 3
getNumber() mengembalikan sebuah stream dari angka acak (int) yang terus-menerus menghasilkan angka baru setiap 1 detik. yield* digunakan untuk meneruskan (delegate) semua nilai dari Stream.periodic. Random().nextInt(10) akan menghasilkan angka 0 sampai 9 secara acak.

2. Langkah 7
StreamBuilder digunakan untuk mendengarkan data yang dikirim oleh stream (dalam hal ini, angka acak dari getNumber()). Setiap kali ada data baru dari stream snapshot.hasData akan true, dan angka ditampilkan ke UI. Jika terjadi error, snapshot.hasError akan true, dan pesan 'Error' dicetak di konsol (namun tidak ditampilkan di UI). Jika belum ada data, UI akan merender SizedBox.shrink(), yaitu tampilan kosong.
