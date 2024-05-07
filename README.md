> Fari Hafizh Ramadhan - 2206083691

# Modul 10: Asynchronous Programming

### 1.2 Understanding how it works
![Image 1.2](img/1.2.png)

Dalam gambar di atas, terlihat bahwa 'bonjour!' diprint terlebih dahulu sebelum 'howdy!' dan 'done!'. Hal ini disebabkan oleh perbedaan dalam penjadwalan eksekusi. 'howdy' dan 'done' dicetak dalam sebuah task yang dipicu oleh spawner.spawn(async { ... }), yang berjalan secara asinkronus setelah executor.run(). Sementara itu, 'bonjour!' dicetak langsung di dalam thread utama tanpa menunggu executor.run(). Inilah yang menyebabkan urutan output seperti yang terlihat.

