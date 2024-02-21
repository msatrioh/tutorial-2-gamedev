Scene BlueShip dan StonePlatform sama-sama memiliki sebuah child node bertipe Sprite. Apa fungsi dari node bertipe Sprite?
> Fungsi sprite adalah menjadi tempat memberikan texture untuk object kita. Texture adalah bagaimana art dari objek kita terlihat.

Root node dari scene BlueShip dan StonePlatform menggunakan tipe yang berbeda. BlueShip menggunakan tipe RigidBody2D, sedangkan StonePlatform menggunakan tipe StaticBody2D. Apa perbedaan dari masing-masing tipe node?
> Perbedaan antara RigidBody2D dan StaticBody2D adalah: StaticBody2D umumnya digunakan untuk object yang tidak perlu digerakkan oleh physics engine. Tetap berperan dalam collision detection, tetapi tidak bergerak karena collision tersebut. Sedangkan, RigidBody2D adalah node yang mengimplementasikan physics 2D yang disimulasikan. Kita tidak mengontrol RigidBody2D secara langsung, tetapi benda memberikan gaya pada benda tersebut dan gerakkan dikalkulasikan oleh physics engine.

Ubah nilai atribut Mass dan Weight pada tipe RigidBody2D secara bebas di scene BlueShip, lalu coba jalankan scene MainLevel. Apa yang terjadi?
> tidak terjadi apa-apa(?) ulang lagi nanti

Ubah nilai atribut Disabled pada tipe CollisionShape2D di scene StonePlatform, lalu coba jalankan scene MainLevel. Apa yang terjadi?
> Pesawat tembus melalui stone platform dan jatuh ke bawah

Pada scene MainLevel, coba manipulasi atribut Position, Rotation, dan Scale milik node BlueShip secara bebas. Apa yang terjadi pada visualisasi BlueShip di Viewport?
> Posisi, orientasi, dan ukuran blue ship menjadi berubah-uba

Pada scene MainLevel, perhatikan nilai atribut Position node PlatformBlue, StonePlatform, dan StonePlatform2. Mengapa nilai Position node StonePlatform dan StonePlatform2 tidak sesuai dengan posisinya di dalam scene (menurut Inspector) namun visualisasinya berada di posisi yang tepat?
> Posisi node stonePlatform dan stonePlatform2 adalah y=0. Hal ini dikarenakan posisi kedua node tersebut adalah relatif terhadap posisi node platform blue, karena merupakan child dari node tersebut. Sedangkan, node platform blue merupakan child dari main scene, sama seperti blue ship, sehingga posisinya absolut.

