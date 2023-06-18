# laesson31
from uuid import uuid4


class Avto:
    """Avtomobil klassi"""

    __num_avto = 0
    def __init__(self,make,model,rang,yil,narh,km=0):

    def __init__(self, make, model, rang, yil, narh, km=0):
        """Avtomobilning xususiyatlari"""
        self.make = make
        self.model = model
@@ -12,26 +16,28 @@ def __init__(self,make,model,rang,yil,narh,km=0):
        self.__km = km
        self.__id = uuid4()
        Avto.__num_avto += 1
    

    @classmethod
    def get_num_avto(cls):
        return cls.__num_avto
    

    def get_km(self):
        return self.__km
    

    def get_id(self):
        return self.__id
    
    def add_km(self,km):

    def add_km(self, km):
        """Mashinaning km ga yana km qo'shish"""
        if km>=0:
        if km >= 0:
            self.__km += km
        else:
            print("Mashina km kamaytirib bo'lmaydi")


class Bus:
    pass


class Train:
    pass
    pass
from uuid import uuid4


class Avto:
    """Avtomobil klassi"""
    def __init__(self,make,model,rang,yil,narh,km=0):

    def __init__(self, make, model, rang, yil, narh, km=0):
        """Avtomobilning xususiyatlari"""
        self.make = make
        self.model = model
@@ -23,21 +26,22 @@ def __init__(self,make,model,rang,yil,narh,km=0):
        self.narh = narh
        self.__km = km
        self.__id = uuid4()
        

    def get_km(self):
        return self.__km
    

    def get_id(self):
        return self.__id
    
    def add_km(self,km):

    def add_km(self, km):
        """Mashinaning km ga yana km qo'shish"""
        if km>=0:
        if km >= 0:
            self.__km += km
        else:
            print("Mashina km kamaytirib bo'lmaydi")


# avto1 = Avto("GM","Malibu","Qora",2020,40000,100000)
# print(f"ID: {avto1.get_id()}")
# avto1.add_km(1500)
# print(avto1.get_km())
# print(avto1.get_km())
