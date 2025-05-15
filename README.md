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

### Reflection 2 (Running RabbitMQ)
![Screenshot of running RabbitMQ on local machine](RabbitMQ.png)

### Reflection 3 (Sending and processing events)
![Screenshot of sending events with publisher and consuming events with subscriber](SendingProcessingEvent.png)

### Reflection 4 (RabbitMQ chart)
![Screenshot of spikes in RabbitMQ dashboard chart](Spike.png)
- Gambar menunjukkan bahwa adanya lonjakkan setiap kali RabbitMQ menerima pesan baru. Spike yang terjadi berasal dari setiap kali publisher mengirim pesan baru ke broker RabbitMQ, Semakin banyak message yang dikirim dalam suatu waktu atau interval per pesannya maka akan semakin tajam dan banyak pula spike nya.


## Modul 9 Bonus
### Reflection 5 (Running RabbitMQ - Cloud)
![Running RabbitMQ on cloud](RabbitMQ_Cloud.png)

### Reflection 6 (Sending and processing events - Cloud)
![Sending and processing events - Cloud](SendingProcessingEvent_Cloud.png)
- Sama seperti yang sebelumnya akan tetapi ada perbedaan pada instance yang digunakan yakni menggunakan *cloud* dan bukan *localhost*.

### Reflection 7 (RabbitMQ chart - Cloud)
![Spikes in graph on cloud](Spike_Cloud.png)
- Sama seperti yang sebelumnya akan tetapi ada perbedaan pada instance yang digunakan yakni menggunakan *cloud* dan bukan *localhost*.