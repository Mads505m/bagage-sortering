# Bagagesorteringssystem i Rust - README
Introduktion
Dette projekt simulerer et bagagesorteringssystem, der håndterer bagage fra check-in skranker til terminaler (gates), hvor bagagen lastes på fly. Systemet omfatter en række komponenter som skranker, et automatiseret sorteringsanlæg og terminaler, der er forbundet med transportbånd og stregkodelæsere. En central server overvåger og synkroniserer alle disse enheder. Dette system implementeres i Rust, og benytter tråde og synkronisering til at simulere de forskellige processer.

## Problemområde
Bagagesorteringssystemet består af følgende hovedkomponenter:

Skranker (Check-in): Til modtagelse og registrering af bagage.
Sorteringsanlæg: Automatiseret system til at sortere bagage.
Terminaler (Gates): Hvor bagagen samles og lastes på fly.
Transportbånd og stregkodelæsere: Bruges til at spore bagagen gennem systemet.

## Systemets Informationer
Systemet skal kunne håndtere følgende informationer:

Reservationssystem: Passagernummer, navn, flyafgang.
Flyveplan: Flyafgang, terminalnummer (Gate-nummer).
Skranker (Check-in): Skranke åbnes/lukkes, passagernummer, bagagenummer, tidsstempel.
Sorteringsanlæg: Bagagenummer, tidsstempel (ind), tidsstempel (ud/sorteret).
Terminaler (Gates): Gate åbnes/lukkes, bagagenummer, tidsstempel
