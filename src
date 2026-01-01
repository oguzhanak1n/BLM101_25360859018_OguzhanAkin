basekomutlar=["1","2","3","4","5","6","7","8","9","A","B","C","D","E","F"] #olabilen komutlar
global flag
flag=0
komut=[]
while(len(komut)!=4):
    print("Lütfen 4 hane girin")
    komut=(input("4 haneli bir HEX kodu girin(Örneğin:14A3 vb.): "))
else:
    bas=komut[0]
    for i in range(14):
        if(komut[0]==basekomutlar[i]):
            flag=1
            break
        
        """ for j in range(3):
            if(komut[j]==i):    
                flag=1
                break """
    if(flag==0):
        bas="error"      

if(bas=="4"):
    if(komut[1]!="0"):
        bas="error"
elif(bas=="A"):
    if(komut[2]!="0"):
        bas="error"
elif(bas=="C"):
    if((komut[1]=="0" and komut[2]=="0" and komut[3]=="0")==0):
        bas="error"
match(bas):
    case '1':
        print("{}{} adresindeki bellek hücresinin içeriğini, {} numaralı kaydediciye (Register) yükle.".format(komut[2],komut[3],komut[1]))
    case '2':
        print("{} Yazmacını {}{} hücresin içeriği ile yükle.".format(komut[1],komut[2],komut[3]))
    case '3':
        print("{} yazmacında bulunan içeriği {}{} adresli belleğe kaydet".format(komut[1],komut[2],komut[3]))
    case '4':
        print("{} yazmacında bulunan içeriği {} yazmacına taşı".format(komut[2],komut[3]))
    case '5':
        print("{} ve {} yazmaçlarının içeriklerini ikinin tümleyeni şeklinde topla ve sonucu {} yazmacına yaz".format(komut[2],komut[3],komut[1]))
    case '6':
        print("{} ve {} yazmaçlarının içeriklerini kayan nokta gösterimi şeklinde topla ve sonucu {} yazmacına yaz".format(komut[2],komut[3],komut[1]))
    case '7':
        print("{} ve {} yazmaçlarının içeriklerine OR(Veya) işlemi uygula,sonucu {} yazmacında tut".format(komut[2],komut[3],komut[1]))
    case '8':
        print("{} ve {} yazmaçlarının içeriklerine AND(VE) işlemi uygula,sonucu {} yazmacında tut".format(komut[2],komut[3],komut[1]))
    case '9':
        print("{} ve {} yazmaçlarının içeriklerine XOR(Ya da) işlemi uygula,sonucu {} yazmacında tut".format(komut[2],komut[3],komut[1]))
    case 'A':
        print("{} yazmacındaki veriyi {} kere döngüsel şekilde sağa doğru bit kaydırması yap(2 ye bölme işlemi)".format(komut[1],komut[3]))
    case 'B':
        print("Eğer {} yazmacının içeriği 0 numaralı yazmacın içeriğine eşit ise {}{} adresindeki komuta atla".format(komut[1],komut[2],komut[3]))
    case 'C':
        print("Çalışmayı Durdur")
    case "error":
        print("Hatalı komut")
    case _: #c deki default
        print("OVER")
