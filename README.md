import random
print("""********************
      1 den 100 adar sayı belirtemeniz gerekiyor.
      7 hakkınız vardır.
      **********************""")
rastgele_sayı=random.randint(1,100)
tahmin_hakkı=7
while True:
    try:
        tahmin= int(input("LÜTFEN SAYI GİRİNİZ:"))
    except ValueError :
        print("lütfen Harf Girmeyiniz Sayı Olarak giriniz...")
        continue
    if tahmin < rastgele_sayı:
        print("lütfen Büyük Sayı Giriniz..",tahmin_hakkı)
        tahmin_hakkı -=1
    elif tahmin > rastgele_sayı:
        print("Lütfen Küçük Sayı Giriniz..",tahmin_hakkı)
        tahmin_hakkı -=1
    else:
        print("Tebrikler Doğru Bildiniz...")
        break
