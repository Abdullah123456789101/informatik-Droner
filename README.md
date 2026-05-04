# Logbog
# informatik-Droner
afsnit 1 tello drone
   3-lags modellen er en metode til at undersøge/analysere et produkt:
       Præsentation her er en person som logger ind, på en app og laver noget input
       logik her er at dens kode oversætter det input til noget drone kan forstå og så udføre
       dat er om hvordan den kan bevæge frem ad, osv

    I dag den 16-08-2024, har vi lært hvordan man kan kontrolere en drone via python. Vi har lært hvordan en drone virker.

    26-08-2024 
    Vi har lært noget om audrino, og hvordan man kan bruge det til sine drone.
    Vi har fået et projekt, hvor vi skal komme med en idee for hvad vi kan bruge vores drone til. Her er vores ideer:

    mind control, hvor du styrer hastigheden på dronene, og en kontroller til hvor den skal flyver hen.

    Normal kontroller, vi kontrollere dronen med en ps4 kontroller.

    motion censor, den ser hvor du går hen, også følger efter dig.
    
    Vi valgte så  ideen, at dronen vil følge efter dig, via et kamera. Et slags motion censor. 

    ![image](https://github.com/user-attachments/assets/aa4fc45e-ef59-4e9d-b961-c1c589794bd8)

# opsumering af Drone forløb 16/08/2024 til 22/11/2024
I dette forløb blev vi introduceret til tello droner. Vi lærte hvordan man kan programmer dem via libraries såsom djitellopy. Derefter begyndte vi så et projekt omkring disse tello droner. kravet for opgaven var at finde en smart/sjov måde at styre tello dronen. Vi valgte så at bruge kamearet på dronen for at lave et program som kan genkende brugerens ansgit, og følge efter dem. Vores program består hovedsagligt af to dele. Et ansigt genkendelse program og et program som genkende den øverste den af menneske kroppen, fra mave til og med hovedet. Dermed kan dronen var foran eller bagved brugeren. 
Her er et blokdiagram og flowchart af programmet:
<img width="789" height="554" alt="image" src="https://github.com/user-attachments/assets/c7c29b5b-e73b-4dc9-a398-b85e1f0dc320" />

<img width="902" height="321" alt="image" src="https://github.com/user-attachments/assets/2bcd7c76-2934-4f82-8aeb-4b996f30b682" />

Under dette forløb blev vi introduceret til nyt teori såsom de fire p'er. Det vi skrev for de fire p'er var:

Produkt: Iden med at dronen flyver efter dig, baseret på din position er i midten, men læner sig lidt mere til radikal.
Proces: Processen er lidt mere til inkrementel, da vi ikke kommer med en ny proces.
Position: Læner sig lidt mere til radikal. Målgruppen er mere for folk der vil bruge det nyeste nye.
Paradigme: Læner sig lidt mere til inkrementel.

Vi blev jo også introduceret til brugertest. Vores brugertest bestod af nogle række spørgsmål som brugeren skulle besvarer efter de havde testet den nuværende iteration. Vi havde også brugt flere metoder som usability teori, iterationsprocess, osv.



Her er et billede af ansigt genkednelse prgrammet når det genkender et ansigt:
<img width="819" height="541" alt="image" src="https://github.com/user-attachments/assets/a262d6ee-c898-4b9f-93ec-190bcb551b13" />

Her er et link til vores repository: https://github.com/Tobias-Henriksen/TelloDroneSamarbejde


# Databaser 05/12/2024 til 13/12/2024
Her blev vi introduceret til falsk og websever, dog gik vi ikke i gang med noget rigtigt. Det var bare mark der yappede om masser af ting. Han talte om forskellige http kald, såsom get,post,put, osv. Han talte også om endpoint og hvordan det giver client mulighed for at læse og tilføj data på serveren.

# Kryptering 10/01/2025 til 21/02/2025
Her blev vi introduceret til kryptering. Vi lærte de forskellige former af kryptering, såsom asymetriske og symetriske krypteringsalgoritmer, private og offtenlig nøgler, osv. Efter det skulle vi så prøve at kode noget RSA. Hvor vi skulle prøve at kryptere en besked og derefter dekryptere. Her er noget simpelt kode som viser det:

import rsa

Generér nøgler (1024 bit)
public_key, private_key = rsa.newkeys(1024)

Besked
message = "Hello RSA!"

Krypter med PUBLIC KEY
cipher = rsa.encrypt(message.encode(), public_key)

Dekrypter med PRIVATE KEY
plaintext = rsa.decrypt(cipher, private_key).decode()

print("Cipher:", cipher)
print("Decoded:", plaintext)

output:
Cipher: b'.\xb8\x1d\x89\xa1\xb9\x98:W\x19\x95\xff\xe2\x9c\xb4v\x894\xffkD\xeb\xf2\x112$;\xd8\xc2N\x0bu\xe2\xf1\xcb\xed\x05Fu\xa1\xe8mbr\x9c\xd9\x02E\xd4o`~\xe5-\xec\x82\xbd#1\xe4O\xb2\xfa\xdd]\xaeScM\x84\x1aS#?[BhaG\x159\x05\xf6\xd1xv\xce\xa5\xect*\xb8\xa2G\xb7\x83e\xe99\x01\xd5\x91\xf9\xd4Z\x8b\xbe\xd2}\x11\x8b\xd1\x865\x0c\xbf\x07*3\x00\xe2\xd2\xb4p?h\x81('
Decoded: Hello RSA!

Vi havde også et projekt i dette forløb, hvor vi skulle prøve at komme op med et program som skulle kryptere bedskeder. Mig og min gruppe valgte i starten med at prøve at kryptere beskeder over lyd, dog viste det sig at det var for svært. Så vi valgte at prøve stenografi. Her brugte vi LSB metoden, hvor vi ændre RGB farveværdiner for en bit, hvis ændring ikke kunne ses via øje, men computere kan så nemt se og dekryptere beskeden. Her er et link til vores repository: https://github.com/Ag-chr/SIGINT-projekt. 



# linux command eller SSH 13-03-2025 til 27/03/2025
Her prøvet vi at bruge SSH til at skrive krypterede beskeder til hinanden. Jeg skrev for eksempel til mark. 

# Teachablemachine 05/05/2025 til 16/05/2025
Vi blev introduceret til machine learning. Hvor vi skulle bruge google teachable machine til at gøre noget. Mig og min gruppe valgte at lære den hvornår brugeren laver forhand eller backhand i bordtennis. Det gjorde ved at give den masser af billede af den røde del af bordtennis battet da det er tradionelt den man bruge som forhand. Og sort til backhand. Vi prøvde med bevægelser i starten, men det kunne den ikke da bevægelserne var alt for hurtigt for den. Her er et billede af det:
<img width="639" height="704" alt="image" src="https://github.com/user-attachments/assets/2f999e0b-2431-4e3e-877e-838b312be057" />

# API 21/08/2025 til 5/11/2025
I dette projekt begyndte vi igen på flask. Denne gang skulle lave en api, altså et program som er en interface mellem brugeren og data. Vi skulle få data fra arduino. Vi valgte at lave en api som viser støjniveuaet i forskellige lokaler. Her brugte vi arduino til at måle støjnivueaet og skabe en database og Flask for hjemmesiden. Vi lærte at sætte vores viden ind i noget større. For eksempel 3-lags-modellen. Vi lærte også hvordan en database og programmet brude være strukturetet. Vi lærte også hvordan vi kunne sætte vores api på python.anywhere så folk havde adgang til vores side.

Vi endte med en api som så sådan ud her:
<img width="363" height="1060" alt="image" src="https://github.com/user-attachments/assets/25db92f7-aad1-4005-bc20-e239462e5ea6" />

Og når brugeren havde valgt tid, lokale, osv vil de få data ud som en graf, for eksempel:
<img width="901" height="894" alt="image" src="https://github.com/user-attachments/assets/6dc68a12-3c1b-4554-bea2-a64c295af935" />

link til repository: https://github.com/Abdullah123456789101/Larm 

# Gates 
Vi blev introduceret til gates. Gates er dem som opbygger cpuerne i vores computer i dag. Vir lærte simple gates, såsom not,or,and,xor,nand, osv. Vi skulle så bruge vores viden om gates til at bygge en lommeregner eller adder 4 bit. Derefter en 8 bit adder, også 16 bit adder, osv. Jeg havde valgt at bruge det program som sebastian lauge havde vist i hans video " how do computers work". Vi lærte også om sandhedstabler som skal vise hvad outputtet vil være basert på input, for eksempel: 
<img width="699" height="217" alt="image" src="https://github.com/user-attachments/assets/3291e778-9d43-4062-b2a4-197e18dea385" />

Sandhedstabbeller viser hvordan outputet vil se ud i basert på inputet. Så for eksempel en not gate. Så står der hvis inputet er 0 så er output 1, hvis input er 1 så er output 0. Det betyder hvis output var en lampe og inputet var en lyskontakt Så når lyskontakten er ikke slået til, vil der være lys, hvis den er så er der ikke lys.

Her er et screenshot a min 4 bit adder:
<img width="1903" height="718" alt="image" src="https://github.com/user-attachments/assets/b9aaa10b-5ff2-4157-b451-b81c2724356c" />

# Robotmæssigt samfundsperspektiv
I dette forløb arbejdede vi med robotter i et samfundsmæssigt perspektiv. Vi skulle udvikle en ide til, hvordan robotter kan bruges i smafundet.

Vi havde besøg fra Aarhus kommune og var også på besøg hos Capra Robotics. Her blev vi introduceret til, hvordan robotter allerede bliver brugt i det offentlige rum, og hvilke muligheder der er i fremtiden.

Vi lærte især om aktører, altså hvilke personer og grupper der er relevante i et projekt. I vores projekt (robot skolepatrulje) var aktørene:
- skolen
- kommunen
- Elever
- Fodgængere
- Billister
- osv
Vi arbejde også med ideer til, hvordan robotter kan løse samfundsproblemer, og hvordan man skal tage hensyn til brugere og omgivelser, og at man ikke bare kunne udvikle teknologi uden at tænke over de relevante grupper, personer eller orginasationer ens ide vil påvirke.

Vi valgte at lave en robot skolepatrulje, som skal hjælpe-børn sikkert over vejen og samtidig vænne mennekser til, at robotter bliver en del af hverdagen.

Vores ide var at lave en robot, som kan stå ved et fodgængerfelt og reagere på trafik og mennesker. Problemfomuleringen var: "Hvordan kan robotter bruges til at gøre det tydeligere, at børn krydser vejen, og samtidig vænne folk til robotter i det offentlige rum?"

Projektet bestod af to dele. Robotten, altså alt hardware, som ESP32 mikrocontroller, Grove vision ai kamera, micro bit bil, arduino modul som kan registrere personer og estimere afstand.
Og hjemmsiden software. Her er et billede af hjemmesiden
<img width="361" height="370" alt="image" src="https://github.com/user-attachments/assets/6d6e5210-0bd6-4c32-afff-0adb9e83ccaa" />

# Privacy og databrokering
I dette forløb arbejdede vi med privacy og hvordan vores data bliver indsamlet og brugt på internettet. Vi så en video, der forklarede, hvordan virksomheder registrrerer vores adfærd online, for eksempel hvad vi klikker på, hvad vi søger efter, og hvor vi befinder os. Disse data bliver derefter brugt til blandt andet reklamer, anbefalinger og profilering.

Vi lærte også om databrokere, som er virksomheder, der indsamler store mængder data om mennesker og sælger det videre til andre-virksomheder. Det betyder, at vores information kan blive delt og brugt, uden at vi nødvendigvis er klar over det.

Videoen viste også nogle af de problemer, der kan være ved dette, såsom manglende privatliv, usikkerhed om hvem der har ens data, og risikoen for at data bliver misbrugt. Det kan også føre til, at man bliver påvirkert eller manipuleret gennem målrettede reklamer.

Det fik mig til at tænke over, hvor meget data jeg selv deler på nettet, og hvor lidt kontrol man egentlig har over sine egne oplysninger. 

# Eksamensprojekt - Smart drivhus
I eksamensprojektet udvikelede vi et system for at drive et drivhus, ved at automatisere vanding og samtidig give brugeren mulighed for at overvåge og styre systemet. Vi byggede et system bestående af sensorer, en ESP32, relæ og en hjemmeside, som var forbundet gennem en backend.

Sensorerne målte jordfugtighed, temperatur og luftfugtighed, og disse data blev sendt til vores server. På hjemmesiden kunne brugeren se mållingerne og enten lade systemet vande automatisk eller selv styre det manuelt. Systemet fungerede derfor som en kombination af hardware og software, hvor de forskellige dele arbejde sammen.

Vi arbejdede iterativt gennem hele projektet, hvor vi startede med en simpel version og derefter løbende forbedrede systemet. Undervejs testede vi systemet og brugte feedback til at gøre det mere brugervenligt. 

Her er billleder og videoer fra projektet:
<img width="1920" height="1029" alt="image" src="https://github.com/user-attachments/assets/5d049c10-0e88-4284-af51-888970069562" />

<img width="1913" height="1030" alt="image" src="https://github.com/user-attachments/assets/2cbe9a27-5db7-4552-af1b-81017a0f5a94" />

https://www.youtube.com/watch?v=W4GXyA66lKs 








