Del 2
=====
elektrisk transistor modell
OBLIG 1 !!!!
uttrykk for strøm gjennom transistor
PN overgang (learn this shit !!!!)
 - sperrer strøm
 - revers blokkerende?
sterkt dopet vs svakt dopet

ikke helt rent dopet: frie ladningsbærere av begge typer
majoritetsbærer vs minoritetsbærer

prosess (diode)
-------
skal lage masker i cadence?
fototeknisk og kjemiske prosesser
UV på følsomt materiale

intrinsikk Si som grunnlag
legger på Silisium di oksid: leder ikke?
 - tynnoksid
 - tykkoksid: god isolator
fjerner oksiden på spesifikk område
gasser på for p-type
mer oksid
maske
gass for n-type

leder polysilisium strøm?

PN overgang
-----------
revers forspent: minimalt strøm ~ 0 strøm
deplesjon

transistor tverrsnitt
---------------------
nMOS:
p-substrat er base
n+ er sterkt dopet
tynnoksid? under gaten
g eller d < src ?
substrate spenning > gnd?

lage ntype mellom s og d, kanal, leder strøm
1 på gate dytter vekk hull fra gaten
  og tiltrekker elektroner fra n+ terminalene

substrattilkobling
p+ ved n+ terminalen
jord skal til p-substratet
Kontakter rundt hele brønnen? Ellers er du fucked

pMOS:
tilsvarende, men motsatt
substratets spenning er Vdd

koblet gnd til Vdd -> kretsen er fucked

designprosedyre
---------------
blir lett for komplisert
hvordan velge riktig løsning?

Akkumulasjon
------------
minus 1 på gate
VELDIG skrudd av
brukes i praksis ikke

alt:
1 på src og 1 på drn?

deplesjon
---------
hverken p eller n under gate
i overgangen fra den ene til den andre
går ikke strøm
på vei inn til inversjon

inversjon????
---------
Vg = 0
blir condensator (SiO2 mellom gate og substrat)
ha kontroll på denne kapasitansen
C = eA/d
d = avstand mellom plater = tox tykkelse? til tynndioksid
A = areal til plate (tykk ~1 nm)
e = permittivitet vakuum

0 < Vg < Vt
elektr går vekk fra gate
samler seg ved substrat
og lager deplesjons layer uten overskudd av n eller p

inversjon:
Vg > Vt
Flere elektroner under gatens oksid
deplesjon under
og så substrat

akkumulasjon:
Vg < 0
under gate blir ENDA mer sperret av hull
Litt elektroner på gate

beskrivelse av MOS transistor
-----------------------------
en modell for AV og to for PÅ avhengig av drain spenning

AV:
strømmen er 0?
enkel modell
(realistisk modifikasjon om noen uker)

PÅ:
Vgd = Vgs
strøm fremdeles 0
trenger E-felt

litt drain spenning
=> litt strøm

øker drain
dårlig kanal?

øker mer?
kanal når ikke frem?
metning!
strøm uavhengig av Vds
strøm går fremdeles, men øker ikke
ønsker å ha transistoren i metning

inverter
--------
if (strøm uavhengig spenning)
nesten ideell strømkilde
forsterkning!
inngang kan være shit? utgang blir fin?

Vt = terskelspenning?

lineært område
strøm avhengig av Vds
PÅ og lik d og s
motsetning til metning
Vgt > Vt
Vds < Vgs - Vt

Del 2 fortsatt
==============
MOS transistor modell
---------------------
gate capasitans?
er den statisk?
uten kanal (deplesjon): mer cap?

2-3 ganger forskjell i output
gjør matematiske modeller mindre betydningsfull

AV: cutoff
Vgs < Vt
Ids = 0

PÅ lineært
Vgs > Vt
0 < Vds < Vgs - Vt
kanal hele veien
Vds bestemmer kanal

pÅ metning
kanal ikke hele veien (kanalforkortning)
Vgs > Vt
Vds > Vgs - Vt

pMOS
omvendt av nMOS

parametre for strøm
-------------------
avstand, cap, spenning, bredde
I ~ width/length = bredde/avstand
C ~ w*l/tox = bredde*avstand/tox
liten nanometer: reversfaktorer gjør fysikken komplisert
legg lengden til minimum?

tradeoffs:
forsterkning?  øker l
hastighet?  minker l
pMOS har dårligere ladningsbærere
 - dobler bredde gir lik strøm?
 - kunne økt lengde til nMOS? nei: I ~ W/L og blir svak strøm
 - L endrer hastighet

Transistormodell
----------------
Q = CV

kanal:
V over Cg er

Vgc = Vgs - Vds/2

tox = tykkelse til dioksid

Cg = eox*W*L/tox = Cox*W*L

mobilitet = mu

mu_n ~ 2*mu_p

hastighet = mu * E
E = efelt
  = Vds/L

tid:
t = L/v

strøm
I = Q/t
  = CV/t
  = ...
gjør utledningen!!!!
"Lineær" strømmodell?
skitten forenkling, fordi Vds er liten og ignorerer addisjon med den.

Vt = terskelspenning!!!!

som motstand (lineært)
------------
I lineært område fungerer strømmen *som* ved motstand
Idt = Vds/Rds

konduktans = G = R^-1 = B(Vgs-Vt)

men lineært område suger: uklart output

I metning
---------
Vdsat = Vgs - Vt

transkonduktans stor => stor amp
A = gm / go
for god karakter!!!!

