
def türe() :
     print("  ")
     print("  ")
     print("  ")
     print("Wilkommen, zu meinem kleinen adventure Game!")
     print("Du wachst in einer heruntergekommenen Hütte in einem Zauberwald auf.")
     print("Deine Erinnerungen sind verblasst.")
     print("Du stehst auf und läufst zur Türe.")
     print("Hinter der Türe hörst du ein merkwürdiges Rascheln.")
     print("Möchtest du die Türe öffnen?")
     
     türe_öffnen = input("> ")
     if(türe_öffnen == "öffnen"):

        print("Du öffnest die Türe.")
        print("Du kommst in ein Zimmer. In diesem Zimmer steht eine verschlossene Truhe.")
        print("Die Geräusche kommen aus der Truhe.")
        print("Möchtest du die Truhe öffnen?")

     elif(türe_öffnen == "nicht öffnen"):
        print("Du entdeckst ein Fenster.")
        print("Doch das Fenster öffnet sich nicht.")
        print("Du musst die Türe öffnen.")
        türe()

     else:
         print("Ungültige Auswahl, bitte wähle öffnen oder nicht öffnen.")
         türe()

def truhe() :

    truhe_öffnen = input("> ")
    if(truhe_öffnen == "öffnen"):
        print("Du öffnest die Truhe.Ein kleiner Elf fliegt heraus.")
        print("Er bedankt sich und verpufft.")
        print("Dir fällt ein Regal mit verstaubten Büchern auf.")
        print("In diesem Regal entdeckst du ein Buch,das schon etwas vorgeschoben ist.")
        print("Möchtest du das Buch herausnehmen?")

    elif(truhe_öffnen == "nicht öffnen"):
        print("Du lässt die Truhe geschlossen.")
        print("Dann rennst du ängstlich zur Eingangstüre.") 
        print("Du verlässt die Hütte und versuchst dem Zauberwald zu entkommen.")
        print("Doch du schaffst es nicht.")
        print("ENDE")
        türe()
        truhe()
        buch()
        gang()
        elf()

    else:
        print("Ungültige Auswahl, bitte wähle öffnen oder nicht öffnen.")
        truhe()
       


def buch() :    
        
        buch_herausnehmen = input("> ")
        if(buch_herausnehmen == "nehmen"):
            print("Du nimmst das Buch heraus.")
            print("Das Regal gleitet zur Seite und es öffnet sich ein dunkler Gang.")
            print("Du gehst den dunklen Gang entlang und kommst an eine Wegspaltung.")
            print("Wählst du den linken oder den rechten Gang?")

        elif(buch_herausnehmen == "nicht nehmen"):
            print("Das Buch Fesselt deinen Blick.")
            print("Du entscheidest dich ungewollt das Buch herraus zu nehmen.")
            buch()  

        else:
            print("Ungültige Auswahl, bitte wähle nehmen oder nicht nehmen.")
            buch()

        


def gang() :  
                     
            linker_gang = input("> ")
            if(linker_gang == "links"):
                print("Du kommst in ein kleines Schloss.")
                print("Auf einem kleinen Thron sitz ein weiterer Elf.")
                print("Er winkt dich zu ihm.")
                print("Gehst du zu ihm? oder rennst du weg?")

            elif(linker_gang == "rechts"):
                print("Du kommst zu einer Hexe.")
                print("Die Hexe lacht.")
                print("Du versuchst wegzurennen.")
                print("Doch die Hexe verwandelt dich in einen verzauberten Baum.")
                print("Du stehst bis ans Ende aller Tage im Zauberwald.")
                print("ENDE")
                türe()
                truhe()
                buch()
                gang()
                elf()

            else:
                print("Ungültige Auswahl, bitte wähle links oder rechts.")
                gang()

             
def elf():   
                         
               gehst_zuihm = input("> ")
               if(gehst_zuihm == "hingehen"):
                    print("Der Elf freut sich das du seinen Freund gerettet hast.")
                    print("Als Dank dafür erhälst du ein Zauberbuch.")
                    print("Dieses Zauberbuch erfüllt dir jeden Wunsch.")
                    print("Du bedankst dich herzlich und wünschst dich nach Hause.")
                    print("ENDE")
                    print(" ")
                    print(" ")

               elif(gehst_zuihm == "wegrennen"):
                    print("Du rennst aus der Türe neben seinem Thron.")
                    print("Dort gelangst du in einem Raum mit einer weiteren Truhe.")
                    print("Du öffnest sie. Plötzlich bildet sich Rauch um dich.")
                    print("Du schläfst langsam in dem Rauch ein.")
                    print("Als du aufwachst, befindest du dich in deinme Bett Zuhause.")
                    print("ENDE")
                    türe()
                    truhe()
                    buch()
                    gang()
                    elf()
                    
               else:
                    print("Wungültige Auswahl, bitte wähle hingehen oder wegrennen.")
                    elf()

türe()
truhe()
buch()
gang()
elf()
