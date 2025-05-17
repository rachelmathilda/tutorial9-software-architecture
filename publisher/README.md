## Publisher
1. banyak data yang program publisher kirim ke pesan broker dalam satu kali eksekusi sebanyak 5 kali. hal ini dikarenakan terdapat 5 panggilan ke metode publish_event. masing-masing mengirim satu instance dari UserCreatedEventMessage. pesan pertama memiliki user_id = "1" dan user_name: "129500004y-Amir" dan seterusnya hingga 5 pesan. setiap panggilan mengirim satu pesan ke queue/exchange bernama "user_created" di message broker. 

2. amqp://guest:guest@localhost:5672 merupakan URL koneksi yang digunakan untuk menghubungkan program ke message broker berbasis amqp seperti RabbitMQ. amqp:// merupakan protokolnya. guest pertama merupakan nama pengguna untuk autentikasi ke RabbitMQ. guest kedua merupakan password untuk autentikasi juga. localhost menunjuk pada server lokal untuk menjalankan message broker. terakhir, 5672 merupakan port yang digunakan. 

## Running RabbitMQ
![alt text](image.png)
![alt text](image.png)