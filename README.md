# Tutorial Timer

## 1.2 Understanding how it works

![](assets/1.2.png)

Dari pengamatan outputnya, dapat dipahami bahwa fungsi async berjalan secara independen dari fungsi utama. Akibatnya, "hei hei" berpotensi menjadi keluaran sebelum "apa kabar!" dan "selesai!" karena "hei hei" berada di luar fungsi async. Program melanjutkan untuk mengeksekusi println!("hey hey"); sedangkan fungsi async masih menunggu hasil kedepannya.