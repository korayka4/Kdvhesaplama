

def kdv_hesapla():
    gida_urunleri = ["ekmek", "peynir", "zeytin", "cikolata"]
    beyaz_esya = ["bilgisayar", "televizyon", "buzdolabi"]

    urun = input("Aldığınız eşyanın adını girin: ").lower()
    fiyat = int(input("Aldığınız eşyanın fiyatı: "))

    if urun in gida_urunleri:
        kdvli_fiyat = fiyat + (fiyat * 0.10)  
    elif urun in beyaz_esya:
        kdvli_fiyat = fiyat + (fiyat * 0.20)  
    else:
        kdvli_fiyat = fiyat + (fiyat * 0.18)  

    print("KDV'li fiyat:", kdvli_fiyat)

kdv_hesapla()