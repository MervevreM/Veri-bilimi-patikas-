# 1. Fonksiyon
 Bir listeyi düzleştiren (flatten) fonksiyon yazın. 
 Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir. 

        liste = [[1, 'a', ['cat'], 2], [[[3]], 'dog'], 4, 5]
        flatten_list = []
        def flatten(liste):
            for i in liste:
                if isinstance(i,list):
                    flatten(i)
                else:
                    flatten_list.append(i)

        flatten(liste)
        print(flatten_list)


# 2. Fonksiyon
Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün.


        liste = [[1, 2], [3, 4], [5, 6, 7]]
        def reverser(liste):
            for i in liste:
                i.reverse()
            liste.reverse()
            return liste

        reverser(liste)
        print(liste)
