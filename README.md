import os
os.system("cls")

class card:
    def __init__(self, egasi, balans):
        self.egasi = egasi
        self.balans = balans
    def pul_yuklash (self,summa):
        self.balans += summa
        print(f"{summa} so'm yuklandi. Balans:{self.balans}")

    def pul_yechish(self, summa):
        if summa <= self.balans:
            self.balans -= summa
            print(f"{summa} so'm yechildi. Balans: {self.balans}")
        else:
            print("Balans yetarli emas!")

k = card("Dom Cobb ", 100000)
k.pul_yuklash(50000) 
k.pul_yechish(70000)
