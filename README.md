# Pizasiparis
# Pizza Sipariş Sayfası

print("Hoşgeldiniz! Lütfen aşağıdaki seçeneklerden birini seçin:")

# Pizza Boyutu Seçimi
print("\nLütfen pizza boyutunu seçin:")
print("1 - Klasik")
print("2 - Margarita")
print("3 - TürkPizza")
pizza_boyutu = input("Seçiminiz (1/2/3): ")

# Pizza Sos Seçimi
print("\nLütfen pizza sosunu seçin:")
print("1 - Domates sosu")
print("2 - Barbecue sosu")
print("3 - Ranch sosu")
pizza_sosu = input("Seçiminiz (1/2/3): ")

# Pizza Toppings Seçimi
print("\nLütfen pizzanıza eklemek istediğiniz malzemeleri seçin:")
print("1 - Mantar")
print("2 - Zeytin")
print("3 - Keçi Peyniri")
print("4 - Et")
print("5 - Soğan")
print("6 - Mısır")
pizza_malzemeleri = input("Seçiminiz (1-6 arası rakamlar arasında virgülle ayırarak): ")

# Sipariş Özeti
print("\nSiparişiniz aşağıdaki gibi olacak:")
if pizza_boyutu == "1":
  print(" - Klasik pizza")
elif pizza_boyutu == "2":
  print(" - Margarita pizza")
else:
  print(" - TürkPizza pizza")
if pizza_sosu == "1":
  print(" - Domates sosu")
elif pizza_sosu == "2":
  print(" - Barbecue sosu")
else:
  print(" - Ranch sosu")
if pizza_malzemeleri:
  pizza_malzemeleri = pizza_malzemeleri.split(",")
  print(" - İçerikler:", end=" ")
  for malzeme in pizza_malzemeleri:
    if malzeme == "1":
      print("Mantar", end=", ")
    elif malzeme == "2":
      print("Zeytin", end=", ")
    elif malzeme == "3":
      print("Keçi Peyniri", end=", ")
    elif malzeme == "4":
      print("Et", end=", ")
    elif malzeme == "5":
      print("Soğan", end=", ")
    elif malzeme == "6":
      print("Mısır", end=", ")
else:
  print(" - İçerikler: Sade pizza")
