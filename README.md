# Bevezetés a bioinformatikába

félév menete:
1. zh
2. féléves feladat; lehet:
   - bioinfo adatok feldolgozása
   - 2D vizualizáció
3. pótzh/elővizsga

---------------------------

## 1. EA
- **bioinformatika**: számítógépes módszerek kifejlesztése alkalmazása a biológiai információ kezelésére és értelmezésére; (https://bioinformatika.szialab.org/ea01/ea01.htm)
  - [MIT biological engineering division](https://be.mit.edu/)
- biokémia alapok 
  - [fehérjék](https://szerves.chem.elte.hu/oktatas/ea/biologiaikemia_aminosavak_korabbi.pdf)
  - gének
  - [makromolekulák](https://hu.khanacademy.org/science/biology/macromolecules)
- matematika, [stat](https://github.com/gabboraron/biostatisztika_es_alkalmazasai)
- informtika: [Bioperl](https://bioperl.org), [BioPython](https://biopython.org/), [R](https://datacarpentry.org/genomics-r-intro/)

next generation sequencing, mutációk vizualizálása, lokális mutációs adatbázis építés

bioinformatikai versenyek: https://predictioncenter.org/casp15/index.cgi

- **PROTEOMICS** fehérjékkel foglalkozik
- **genomics** - génstruktúrákkal

**élőlények**: 
- fehérjék => sejtmaggal vagy a nélkül létező lények <= prokarióták és eukkarióták
- nukleinsavak
- lipidek
- poliszaharidok

főbb részeik: sejtmag, golgi apparátus, mitokondruium, sejthártya, csilló, sejtburok

***Fehérjék** azok amikből lehet építeni gépeket

**fehérjék szerep az élőlényekben:**
- [enzimek](https://hu.wikipedia.org/wiki/Enzim)
- transzportfehérjék - feladatuk a szervek közti szállító feladatok ellátása
- védőfehérjék - lehetővé teszik, hogy a szervezet fertőzéssel vagy sérüléssel szemben védekezzen
- toxinok - például kígyómérgek
- hormonok - pl inzulin
- kontraktilis fehérjék
- struktúra fehérjék - a mozgáshoz szilárd vázat biztosítanak, és a külső védelmet szolgálják.

[![The inner life of a cell](https://i.ytimg.com/an_webp/yKW4F0Nu-UY/mqdefault_6s.webp?du=3000&sqp=CIzY_JgG&rs=AOn4CLCiFz6uYq2F7WBI-ZGGnvIV2pohQw)](https://www.youtube.com/watch?v=yKW4F0Nu-UY)

**fehérjék**: 
```
H2N - CH - COOH
       |    
       R
-COOH - karboxil csoport
-NH2 - amino csoport
-szénatom - alfahelyzetű
-R valamilyen gyök
```

**Aminosavak:**
- szerkezetük az `R` csoportban különbözik
- az, hogy mit tudunk feldolgozni az faj függő
- 20 természetes aminosavból építkezünk
- az egyes R-el jelzett gyökök kiemelkednek mint oldalláncok, és ezek lesznek a biológiailag aktív hatócsoportok

**fehérjék:**
- elsődleges: amonosav sorerndje a fehérjén
- másodlagos: szkaszokat különböztetünk meg
  - hélix
  - béta redő
  - harmadlagos szerkezet
- harmadlagos: hol kapcoslódnak egmyáshoz a fehérjék
- negyedleges: a több fehérje ami egmyás mellé állt egyben alkot egy negyedleges szerkezetet

![A kép az OpenStax Biology ábrájának módosított változata, mely a National Human Genome Research Institute munkája alapján készült. https://hu.khanacademy.org/science/biology/macromolecules/proteins-and-amino-acids/a/orders-of-protein-structure ](https://cdn.kastatic.org/ka-perseus-images/3833fbc75d3e54cde6b94ab1863e8ded1cd4c844.png)

pl: hemoglobin 

**fehérjének van:**
- mérete: centrifuga, szűrő
- oldékonysága: függ attól, hogy mi az aminosav sorrendje a fehérjének, mi szerkezetr
- töltése
- kötődési affintás
- mennyiségi meghatározása: izolálni kell, hogy mennyi van benne
- alakja:
  - hosszúkás - fibrilláris
  - gömbszerű - globuláris
- szerkezete: 100 aminosavból álló fehérje esetén 2^100 egymástól eltérő lehet
- másodlagos szerkezet:
  - periodikus, aperiodikus, kanyarok 

**nukleinsavak:**
- fehérjékben van
- az osztódások folyamatosak
- mitózis: számtartó osztódás 
- amitózis: csak egysejteknél
- meiózis: számfelezős

Minden fehérje tartlamazza a DNS-t így minden fehéreje minden fehérjét előllíhat a szervezetben

**Teloméra:**
- minden egyes osztódáskor rövidül

**mutáció:** 64 aminosavat tudnánk kódoolni de csak 20-as nagságrendet kell, és akkor vagy értelmetlen vagy valami túlzottan erősen lesz kódolva.
- szomatikus
- pontmutáció
- gén vagy kromoszómaát érintő

**Mutagén hatások**:  környezeti hatások miatt nem mind kijavítható!
- ionizáló
- antibiotikumok
- kemikáliák
- azbeszt
- tartósítószerek

Genom rpojektek:
- [HUGO](https://www.hugo-international.org)
- EMBL
- DDBJ - DNA bank of Japan

https://www.internationalgenome.org/

Szekvenálás költsége: [genome.gov/sequeninge](https://www.genome.gov/)

eszközök:
- [Gén chip](https://www.youtube.com/watch?v=V8uNJCO7Qqo)
- [next generation sequencing](https://www.illumina.com/science/technology/next-generation-sequencing.html)
- [single cell genomics](https://www.youtube.com/watch?v=yTl1Q0D7aZ0)

# EA2
# EA3
# EA4 - [proteomika](https://hu.wikipedia.org/wiki/Proteomika) (fehérjék)
Aminosavak - peptidkötés kialakulásánál víz kilépés van.

áll:
- karboxil csoport
- amino csoport

# EA5 - genomika
Van sejtmag (eukarióta); nincs sejtmagja (prokarióta) -> az eukarióták bekebelezhetnek másokat

Az eukaritóáknál a sejmaghártyán belül van a sejtmag main belül tárolódik az örökítőanyag. Az egysejtűek és többsejtűek között nagy különbség nincs e téren.

![eukarióta](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b8/Endomembrane_system_diagram_en.svg/500px-Endomembrane_system_diagram_en.svg.png)

Testi sejtek (diploid): 2N elemmel, 1 apai és egy anyai kromszómaszerelvénnyel; képesek osztódni, önmagukat duplikálni, 1 sejtből 4 sejt lesz

Ivarsejtek (haploid): 1N 1 kromoszómaszerelvény; felezik magukat 1 sejtből két sejt lesz

![kromoszómák](https://cms.sulinet.hu/get/d/5fa650cf-8fc8-4619-80bb-65b50b264410/1/7/b/Normal/8gen03.jpg)

tudásbázison az mberi szaporodás: https://tudasbazis.sulinet.hu/hu/termeszettudomanyok/biologia/biologia-8-evfolyam/az-ember-szaporodasa/az-emberi-oroklodes

olvasnivaló: [Dawnkins - önző gén](https://www.libri.hu/konyv/richard_dawkins.az-onzo-gen--1.html)

osztódás típusok:
- mitózis: számtartó osztódás (identikus másolat)
- amitózis: egysejtűeknél
- mejózis: számfelező osztódás: mitózis + felezés

![mitózis vs mejózis](https://slideplayer.hu/slide/2214695/8/images/12/Mei%C3%B3zis+Mit%C3%B3zis+1n+1n+1n+1n+DNS+megkett%C5%91z%C5%91d%C3%A9s+DNS+megkett%C5%91z%C5%91d%C3%A9s.jpg)

sejthalál típusok:
- [apoptózis](https://hu.wikipedia.org/wiki/Programozott_sejthal%C3%A1l) programozott sejthalál - egy jel hazására *pl égési sérülés* történik.
- [nekrózis](https://hu.wikipedia.org/wiki/Apopt%C3%B3zis) 


[Hiszton](https://hu.wikipedia.org/wiki/Hiszton)ok:

![hiszton](https://www.termvil.hu/archiv/szamok/tv2017/tv1706/szabad1.jpg)

- http://physiology.elte.hu/eloadas/kornyezet_egeszsegtan/KornyEgeszseg_6.pdf
- https://www.termvil.hu/archiv/szamok/tv2017/tv1706/szabad.html

A hisztonok nagy mennyiségben ugyanolyanok. Ezek tartják a DNSt feltekerve.

kb 30.000 fehérjét ismerünk

centrális dogma:
- replikáció: DNS -> DNS
- transzkripció: DNS -> RNS
- transzláció: mRNS -> fehérje

ennek ellentéte:
- retrovírusok: RNS -> DNS
- RNS vírusok: RNS -> RNS
- Prionok: fehérje -> DNS felező részecske

genetikai kód:
- 3 db nukleinsav = 1 aminosav
- 20 aminosavunk van de 4^3 = 64 aminosavat tudunk kódolni
- de az értelmes kodonokból csak 61-et
- 3 db nem értlemezhető kodon van : *stop kodon* 

**DNS -> RNS**
A->T -> U
T->A 
G->C
C->G
