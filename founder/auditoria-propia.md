# Auditoria pròpia de WoFa (9 de novembre de 2026)

Feta per Claude directament sobre l'app real de WoFa a Base44 (codi i base de dades), **sense fer servir cap document del Drive**. Només s'han llegit xifres agregades; cap dada personal. wofa.cat no és accessible des d'aquesta sessió, així que no s'ha pogut revisar la web publicada des de fora.

## Les xifres reals

| Què | Xifra | Comentari |
| --- | ---: | --- |
| Usuaris registrats | ~95 | Inclou el compte d'administrador i el de social manager |
| Registres per mes | abr 3 · maig 2 · juny 13 · jul 12 · ago 0 · set ~46 · oct 13 · nov 1 | Pic al setembre i caiguda forta després |
| Feines publicades per clients (total) | **5** | 3 completades (jardí ×2, neteja), 1 assignada, 1 oberta a Barcelona des del juliol |
| Ofertes de serveis actives (wofers) | **25** | Gossos 8, classes 6, cangur 5, jardí 4, mudances 1, música 1 |
| Wofers amb alguna feina feta | 1 de 25 | 24 ofertes no han fet mai cap feina |
| Contractacions d'ofertes | 6 | 3 "completades" a 1-3 € (semblen proves), 1 acceptada a 15 €, 1 pendent des del setembre, 1 rebutjada |
| Valoracions | 13, totes de 5 estrelles | Corresponen a ~6 transaccions, algunes de l'abril i el juny |
| Comerços a WoFa Deals | 4 aprovats | |
| Configuració de llançament | Fase 0, comissió 0%, 12 mesos gratis | La fase 0 acaba el 19/08/2027 |

## El que diuen les xifres

1. **Hi ha oferta però no hi ha demanda.** 25 veïns s'han ofert per fer feines i només 5 clients n'han publicat cap en tota la vida de l'app. El coll d'ampolla és el client, no el wofer.
2. **El creixement s'ha aturat.** Després del pic del setembre (~46 registres), l'octubre en fa 13 i el novembre 1. Sense una campanya activa, no entra gent.
3. **Encara no hi ha cap prova de negoci.** El valor total que ha passat per WoFa és de l'ordre de desenes d'euros. Les valoracions de 5 estrelles són reals però molt poques.
4. **El codi ha millorat respecte a l'auditoria anterior.** La valoració falsa "4,8 (120)" ja no està escrita al codi: ara la valoració només surt de les ressenyes reals dels wofers. No he trobat cap NIF ni domicili al codi, així que probablement encara falta la identificació legal del titular (cal revisar-ho a la web publicada).

## Panell de 100 compradors simulats

Detall a `founder/panel/results.md`. Perfil i missatge a `founder/customer.json` i `founder/pitch.md` (categories i preus reals de l'app; les proporcions de segments són estimacions de Claude).

- **5 compren, 95 no (5%).** És un sostre: els compradors simulats tendeixen a dir que sí més que la gent real.
- **Qui compra:** persones amb gos que treballen fora tot el dia (12%) i gent que prova apps noves (50%). Ningú dels que cuiden un pare o una mare gran, ni estudiants, ni els que funcionen pel boca-orella o busquen el més barat.
- **Per què no:** confiança (42) i costum (37): "ho pregunto al grup de WhatsApp de l'escola i en dues hores tinc tres noms". Després, preu i pagament amb targeta (9) i no tenir la necessitat (5).
- **Què els faria canviar:** una recomanació personal d'algú que coneixen, verificació real (DNI i, per a cangurs, el certificat de delictes sexuals), una persona de WoFa que respongui per telèfon i poder conèixer el wofer abans.
- **Una necessitat que l'app no cobreix:** diversos compradors que cuiden un pare o una mare gran busquen companyia o ajuda puntual per a gent gran, i no la troben a les categories.

## Recomanacions

1. **Atacar la demanda, no l'oferta.** No cal captar més wofers ara; cal que els 25 que hi ha facin feines.
2. **Entrar pels grups de WhatsApp, no competir-hi.** La gent ja busca ajuda allà. Cada wofer hauria de tenir un enllaç al seu perfil fàcil de compartir als grups de l'escola i del barri, i cada feina feta hauria de generar una recomanació que circuli per aquests grups.
3. **Verificació visible.** DNI comprovat i, per a cangurs i classes amb menors, el certificat de delictes sexuals (obligatori a Espanya per treballar amb menors), amb una insígnia al perfil. Un telèfon o WhatsApp de WoFa on respon una persona.
4. **Començar per la categoria que ja té tracció:** passejar gossos per a gent que treballa fora tot el dia. Té la millor taxa del panell i la més oferta de wofers.
5. **Afegir "companyia i ajuda a gent gran"** com a categoria, amb verificació reforçada.
6. **Comprovar-ho amb gent real** abans d'invertir: 10 trucades o missatges a clients potencials de la categoria triada, i una prova de 2 setmanes en un sol barri.
