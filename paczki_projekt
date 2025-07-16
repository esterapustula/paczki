nr_paczki = 1
ilosc_elementow = int(input ("Ile elementow chcesz wysłać?: "))
suma_wag = 0
puste_kg = 0
max_puste_kg = 0
nr_paczki_max_puste_kg = 1

for i in range(1, ilosc_elementow + 1):
    waga = int(input(f"Podaj wagę elementu nr {i} (1-10 kg): "))
    if 1 <= waga <= 10:
        print("Prawidłowa waga paczki.")
    else:
        print("Nieprawidłowa waga! Paczka musi ważyć od 1 do 10 kg.")
        break
    if suma_wag + waga <= 20:
        suma_wag += waga

    else:
        print(f"Spakowano {nr_paczki} paczkę")
        puste_kg = 20 - suma_wag
        if puste_kg > max_puste_kg:
            max_puste_kg = puste_kg
            nr_paczki_max_puste_kg = nr_paczki
        nr_paczki += 1
        suma_wag = waga

if suma_wag > 0:
    print(f"Spakowano {nr_paczki} paczkę")
    puste_kg = 20 - suma_wag
    if puste_kg > max_puste_kg:
        max_puste_kg = puste_kg
        nr_paczki_max_puste_kg = nr_paczki

print (f"Wyslano {nr_paczki} paczki")
print (f"Max pustych kg jest w paczce {nr_paczki_max_puste_kg} i wynosi {max_puste_kg}")
