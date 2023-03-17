# belah-ketupat1
DEKLARASI
    a, b, kpk, fpb : INTEGER

BACA
    a <- INPUT("Masukkan bilangan pertama: ")
    b <- INPUT("Masukkan bilangan kedua: ")

PROSES
    # mencari fpb dengan algoritma Euclidean
    x <- a
    y <- b
    WHILE y != 0 DO
        r <- x % y
        x <- y
        y <- r
    END WHILE
    fpb <- x
    
    # mencari kpk menggunakan fpb yang sudah ditemukan
    kpk <- (a * b) / fpb

TULIS
    WRITE("Bilangan pertama adalah ", a)
    WRITE("Bilangan kedua adalah ", b)
    WRITE("FPB dari ", a, " dan ", b, " adalah ", fpb)
    WRITE("KPK dari ", a, " dan ", b, " adalah ", kpk)
