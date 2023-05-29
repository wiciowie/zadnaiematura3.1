liczbadzietna = ""
with open("pi.txt") as plik:
    for wiersz in plik:
        liczbadzietna = liczbadzietna + wiersz

ciag = liczbadzietna.split()
count = 0

for i in range(len(ciag)-1):
    liczba = int(ciag[i] + ciag[i+1])
    if 90 < liczba:
        count = count + 1
print(count)
