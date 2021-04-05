# PR21 - Projektna naloga
### Člani:
- Luka Gregorn
- Luka Nikolič
- Andraž Štemberger

### PREDSTAVITEV MNOŽICE PODATKOV 
-----

Naša množica podatkov, nad katero bomo izvajali raziskave je podatkovna baza sporočil iz Discord strežnika, ki smo ga študentje ustvarili za medsebojno pomoč. Trenutno je na serverju več kot 1500 študentov vključenih v enega od programov FRI, ki dnevno sodeluje v pogovorih na različnih temah. Prvo sporočilo sega vse do leta 2017. 

Za to množico podatkov smo se odločili, saj se nam je zdelo, da bi bila ta tema zanimiva za nas ter ostale študente, ki sodelujejo pri predmetu Podatkovno rudarjenje. 

Podatkovna množica je sestavljena iz več .JSON datotek (za vsak predmet svoja). Vsaka datoteka vsebuje sporočila, ki imajo sledeče atribute:

Atribut | Opis      | Tip  |
--------|-----------|-------
id | zaporedna številka sporočila | Int
type | tip sporočila | String
timestamp | časovna značka, kdaj je bilo sporočilo poslano | Time stamp 
timestampEdited | časovna značka, kdaj je bilo sporočilo popravljeno | Time stamp 
callEndedTimestamp | časovna značka, kdaj je bil končan klic  | Time stamp 
isPinned | indikator ali je sporočilo pripeto | Boolean
content | vsebina sporočila | String
author | avtor sporočila (id, ime) | Dictionary
attachments | priponke sporočilu (id, url) | Dictionary
embeds | vpeta sporočila (id, url) | Dictionary
reactions | reakcije na sporočilo | Dictionary
mentions | kdo vse je omenjen v sporočilu | Dictionary
reference | referenca na drugo sporočilo | Dictionary


### UGOTOVITVE 
----- 

Pri pregledovanju sporočil, smo ugotovili, da število sporočil je v povprečju močno prevladovalo v prvem letu uporabe serverja (študijsko leto 2017/18), že naslednje leto pa je padlo skoraj na polovico. V študijskem letu 2019/20 se je število sporočil povečalo pri predmetih iz drugega semestra, kar lahko pripisujemo pojavu koronavirusa. Študentje so morali poiskati drug vir komunikacije in očitno je bil Discord eden izmed njih.

https://github.com/lukagregorn/PR21LGLNAS/blob/eae7759299e733c6cd1873edfa47c20eca0e069d/Grafi/prva.png


Število pripetih sporočil, ki ponavadi predstavljajo snov, se je z leti precej zmanjšalo. To ponazarja, da veliko študentov še vedno uporablja snov preteklih let. Pri nekaterih predmetih se je z leti prenehalo dodajanje snovi. Iz tega lahko razberemo, da se tudi snov pri posameznih predmetih ne spreminja veliko.



Pri analizi reakcij na sporočila smo ugotovil, da se v drugem semestru reakcije oz. emjoi-ji pogosteje in večkrat uporabljajo. Če primerjamo uporabo največkrat uporabljenega emojia v prvem semestru, je ta 157 uporab, v drugem semestru pa kar 500 uporab. V obeh semestrih, se najpogosteje uporablja emoji :lekosalute:.
Po našem mnenju, se v drugem semestru bolj uporabljajo emoji-ji, zato ker ima Discord takrat več uporabnikov kot v prvem semestru. Na začetku prvega semestra marsi kdo sploh ne ve za ta Discord server, ki ga imamo, zato ga tudi ne uporablja, medtem ko v drugem semestru, Discord server večina študentov že pozna in ga tudi uporablja.
