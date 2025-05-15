# Tutorial 9
**Nama:**   Malvin Scafi<br>
**NPM:**    2306152430<br>
**Kelas:**  Adpro A<br>

## Modul 9
### Reflection 1

1. How much data your publisher program will send to the message broker in one run?  
   Program publisher akan mengirimkan 5 pesan ke message broker dalam satu kali eksekusi. Pesan-pesan tersebut adalah event `user_created` dengan data `user_id` dan `user_name` yang berbeda-beda, seperti yang terlihat pada implementasi di file `main.rs`.

2. The url of: `amqp://guest:guest@localhost:5672` is the same as in the subscriber program, what does it mean?  
   URL tersebut menunjukkan bahwa program publisher dan subscriber menggunakan message broker yang sama, yaitu RabbitMQ yang berjalan di `localhost` (komputer lokal) pada port `5672`. Kredensial `guest:guest` adalah username dan password default untuk mengakses RabbitMQ. Dengan menggunakan URL yang sama, publisher dan subscriber dapat berkomunikasi melalui message broker yang sama.