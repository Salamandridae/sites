MOS transistor og komplementær logikk.
Litt Del 1 først.

Ha not-strek over uttrykket?
Er det essensielt? Bedre?

Komplementær logikk:
Sørg for at utgangen er drevet?
Tristate driver buss?
Opptrekk/nedtrekk på samtidig -> shit
Starte med nedtrekk er EZ?

passtransistor
nMOS god på 0, dårlig på 1
pMOS motsatt
To slike sammen = transmisjonsport

tristate:
Buffer med enable?
Hvordan brukes til buss?
logisk sett: færre er bedre
elektrisk sett: må ta hensyn

shit mux:
udefinert for last?

inverterende mux:
Se hvordan den er LIK shit-mux
hva om D0 og D1 begge er 0?

forenklet mux:
fjerner en ledning -> mindre last
capasitans ved alle noder (e.g. transistor)?
 - pga PN overganger

hastighet
---------
t = RC
U = RI
R = U/R

opplading av capasitor:
I = C*dV/dt
dt = C*dV/I
Finn C og I så kan du si noe om hastighet

switch speed til transistor:
C ~ 1e-16 F
Vdd ~ 1V?
I = 1e-4
=>
dt = 1e-12
=>
1 THz er mulig i dag, men brenner opp

komplementær fortsatt
---------------------
latch:
veldig komplisert å forstå
fra 2:1 mux
forskyvning av klokkesignal :S
kommer senere?
