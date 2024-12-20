## Exam-Pseudo- Robin olsson



 `` // G-Version Split the nota`` 

``` 
Instructions:

Split the nota räknar ut hur mycket varje vän ska betala på exempelvis en restaurang när notan kommer. Användaren matar in summan, antal vänner och sedan dricks (som skrivs i decimalform d.v.s 10% blir 0.10). Skisserna nedan är mest för att ge visuell bild av hur det ser ut, ni behöver inte ha med sådant som "byt vy" eller liknande i er pseudokod.

hur det funkar:
Utan_Dricks = summan utan dricks
Dricks= antal extra summa i procent (decimal)
antal_vänner = antal vänner som skall dela på notan

START


INPUT Utan_Dricks // Matar in summan av notan utan dricks
INPUT Dricks // Matar in dricks i decimalform (exempelvis 0.10 för 10%)
INPUT antal_vänner // Matar in antal vänner som ska dela på notan
    
CALCULATE Notan = Utan_Dricks + (Utan_Dricks * Dricks) // Beräknar totala summan + drics
CALCULATE Delad_summa = Notan / antal_vänner // Beräknar summan som varje vän skall betala
    
PRINT "Varje vän betalar: " + Delad_summa // Visar resultatet på skärmen



END
**


END



``` 

 `` // VG-Version`` 
 
``` 
 Instruktioner
Pusslet går ut på att du får ett startord och ett slutord och du ska genom att byta ut bokstäver i ditt startord få det till ditt slutord med så få byten som möjligt.

Regler

Du får enbart byta ut en bokstav åt gången.
Varje ord som bildas måste vara ett korrekt engelskt ord, dvs. det måste finnas i variabeln vid namn ordbok.
Exempel

I detta exempel så ska vi få FOUR att bli FIVE. Observera att själva spelet är på engelska.

FOUR (startord)
FOUL (Bytte ut R till L)
FOOL (Bytte ut U till O)
FOOT (Bytte ut L till T)
FORT (Bytte ut O till R)
FORE (Bytte ut T till E)
FIRE (Bytte ut O till I)
FIVE (Slutord)

R,L
U,O
L,T,
O,R,
T,e,
O,I








 SETUP
Set StartOrd = Four
SET SlutOrd = Five // Målet
SET OrdBok =  {FOUR, FOUL, FOOL, FOOT, FORT, FORE, FIRE, FIVE}
 
START

SET CurrentWord = StartOrd // startordet (Four) är nu start punkten

WHILE CurrentWord is not equal to SlutOrd:
    FOR i FROM 1 TO LENGTH(CurrentWord) - 1: // Iterera över bostaverna i ordet, börjar med position 1, baserat på längden av ordet, deta fall har alla 4 bokstäver.
        FOR Each Letter IN alfabetet FROM 'A' TO 'Z': // Testa varje bokstav igenom alfabetet
            SET New_Word = CurrentWord with Letter at position i replaced // Skapa nytt ord
            
            IF New_Word is in OrdBok AND New_Word is not equal to CurrentWord:
                SET CurrentWord = New_Word // Uppdatera CurrentWord till det nya ordet
                console.log("The word is: " + CurrentWord + " and it is in the OrdBok")
                Break // kanske inte behövs då end if finns,  lägger deb här ändå.
            ENDIF
        END FOR // Fortsätt till nästa bokstav i alfabetet, detta gör så att det blir en i taget.
    END FOR // Fortsätt till nästa position i ordet, en bokstav i taget.
ENDWHILE  // när Ordet är lika med Slut ordet.

// När slutordet har hittats
console.log("You did it Jesper, gratz! Sorry för svengelskan. GOD JUL och Gott Nytt År!")

END
      










``` 
# Figma Screens
# G ![alt text](image-1.png)
# VG![alt text](image.png)
# FigJam-FlowChart 
[FigJam-länk](https://www.figma.com/board/4XlI7H7LYmVJgLRe3YyqPS/Untitled?node-id=4-115&t=JZrQiQI2StqDKHVT-1) 
#

