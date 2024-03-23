# Sehirler-odevi
import random


kelimeler = ["Ankara", "İstanbul", "Aksaray", "Kütahya", "İzmir"]


harf = input("Bir harf giriniz: ")


secilen_kelime = random.choice(kelimeler)


if harf in secilen_kelime:
    # Harf kelimenin içinde ise
    sifrelenmis_kelime = ''.join([c if c == harf else '!' for c in secilen_kelime])#W3 School sağ olsun.
    print(f"Seçilen kelime: {sifrelenmis_kelime}")
else:
    # Harf kelimenin içinde değilse
    print(f"Seçilen kelime içinde '{harf}' harfi yok.")
