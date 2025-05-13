# Advanced Programming - Tutorial 09
## Daniel Ferdiansyah, 2306275052

**a. How much data your publisher program will send to the message broker in one
run?**

Publisher akan mengirim 5 pesan (event) ke message broker dalam sekali jalan, masing-masing untuk event `user_created`. Tiap pesan isinya data dengan type `UserCreatedEventMessage` yang terdiri dari 2 property:

- `user_id`: String (integer) dari ID pengguna

- `user_name`: String yang berisi nama pengguna, diawali dengan NPM saya. Misalnya `"2306275052-Amir"`. 

**b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean?**

Artinya, baik publisher maupun subscriber terhubung ke broker message yang sama dengan URL `amqp://guest:guest@localhost:5672`. Publisher mengirim pesan ke broker, subscriber menerima pesan dari broker yang sama. Sehingga, publisher dan subscriber bisa saling berinteraksi dalam satu sistem distribusi pesan yang sama.


