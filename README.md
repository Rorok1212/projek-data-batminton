def cerita_interaktif():
    print("Selamat datang di cerita interaktif!")
    print("Kamu adalah seorang petualang yang sedang menjelajahi hutan ajaib.")
    print("Di depanmu ada dua jalan yang bisa kamu pilih.")
    print("1. Jalan ke kiri")
    print("2. Jalan ke kanan")
    
    pilihan = input("Pilih jalan (1 atau 2): ")
    
    if pilihan == "1":
        jalan_kiri()
    elif pilihan == "2":
        jalan_kanan()
    else:
        print("Pilihan tidak valid. Silakan coba lagi.")
        cerita_interaktif()

def jalan_kiri():
    print("Kamu memilih jalan ke kiri.")
    print("Setelah berjalan beberapa langkah, kamu menemukan sebuah danau yang indah.")
    print("Di tepi danau, ada seorang penyihir yang menawarkanmu dua pilihan.")
    print("1. Minta kekuatan sihir")
    print("2. Minta petunjuk untuk menemukan harta karun")
    
    pilihan = input("Apa yang kamu pilih? (1 atau 2): ")
    
    if pilihan == "1":
        print("Kamu mendapatkan kekuatan sihir! Sekarang kamu bisa melakukan hal-hal luar biasa.")
    elif pilihan == "2":
        print("Penyihir memberikan peta menuju harta karun. Kamu pun berpetualang menemukannya!")
    else:
        print("Pilihan tidak valid. Silakan coba lagi.")
        jalan_kiri()

def jalan_kanan():
    print("Kamu memilih jalan ke kanan.")
    print("Setelah berjalan, kamu bertemu dengan seekor naga yang sedang tidur.")
    print("Kamu bisa:")
    print("1. Berusaha membangunkan naga")
    print("2. Menghindari naga dan melanjutkan perjalanan")
    
    pilihan = input("Apa yang kamu pilih? (1 atau 2): ")
    
    if pilihan == "1":
        print("Naga terbangun dan marah! Tapi, kamu berhasil menjalin persahabatan dengannya.")
    elif pilihan == "2":
        print("Kamu berhasil melewati naga dan menemukan jalan menuju desa yang aman.")
    else:
        print("Pilihan tidak valid. Silakan coba lagi.")
        jalan_kanan()

cerita_interaktif()
