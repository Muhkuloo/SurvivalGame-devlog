# Hiisi – devlog

Moi! Tämä on kehityspäiväkirja pelistä, jota teen työnimellä **Project Hiisi**.

Hiisi on PC:lle tuleva selviytymispeli 1–4 pelaajalle. Etenemisen malli on otettu Valheimista ja kauhun tunnelma Sons of the Forestista, mutta kaikki muu on suomalaista: metsät, suot, kansanusko ja Kalevala. Pelissä rakennetaan kylä, puolustetaan sitä ja edetään kohti Pohjolaa ja lopulta Tuonelaa.

Lähdekoodi on yksityinen, mutta kirjaan tänne, mitä kulloinkin teen, mikä onnistui ja mikä meni pieleen.

## Merkinnät

| Päivä | Mitä tein |
|---|---|
| [9.11.2026](devlog/2026-11-09.md) | Iso päivä: maailma, päivä ja yö, metsät, puunkaato, työkalut, hahmo ja rakentaminen |
| [8.11.2026](devlog/2026-11-08.md) | Projekti käyntiin ja ensimmäinen moninpeli toimii |

---

## Millaista peliä teen?

### Tunnelma

Tavoittelen maalauksellista realismia: mittasuhteet ovat realistiset, mutta pinnat näyttävät käsin maalatuilta. Värit tulevat suomalaisesta luonnosta: sammal, jäkälä, suo, ruska ja kaamos. Valo on pelin tunnusmerkki, sillä vuorossa ovat yötön yö, kaamoksen pimeys ja revontulet.

Kauhu ei tule verestä vaan kansanuskosta. Metsänpeittoon voi joutua, ja jokin liikkuu puiden välissä. Mitä pidemmälle pääsee, sitä synkemmäksi maailma muuttuu.

### Biomit ja niiden haltijat

| Biomi | Bossi |
|---|---|
| Kangasmetsä | Hiiden hirvi |
| Korpi | Ajattara |
| Aapasuo | Lempo |
| Järviylänkö | Iku-Turso |
| Tunturi ja Pohjola | Louhi |
| Tuonela | Hiisi |

Päämanner on yhtenäinen. Pohjolaan pääsee vain veneellä meren yli, ja Tuonela odottaa joen toisella puolella.

### Eteneminen synnyillä

Kun bossi kaatuu, siltä jää esine, joka uhrataan kotileirin kalliolle. Kallioon piirtyy kalliomaalaus, ja pelaajat oppivat **synnyn** eli tiedon siitä, mistä jokin on saanut alkunsa. Synty on yhteinen koko maailmalle, joten co-opissa kukaan ei jää jälkeen.

Jokainen synty avaa seuraavan biomin rajan. Ensin vastassa on metsänpeitto, sitten suo, vesi ja pakkanen ja lopuksi Tuonelan joki. Rajat eivät ole näkymättömiä seiniä: ensimmäinen vain eksyttää, myöhemmät ovat oikeasti vaarallisia.

Mukana kulkee **kantele**. Jokainen synty lisää siihen kielen, ja loppupään rajoista pääsee yli vain soittamalla.

### Mitä pelissä tehdään?

- **Rakennetaan ja puolustetaan kylää.** Avattujen biomien olennot hyökkäävät kylään, joten puolustuksen rakentaminen on oma osa peliä. Vaikeus kasvaa loivasti pelaajamäärän mukaan.
- **Kehitetään varusteita.** Jokainen biomi tuo parempaa varustusta kaikille rooleille: soturille, metsästäjälle ja tietäjälle. Tärkeitä virstanpylväitä ovat suomalmista sulatettu rauta, hauenluukantele ja Ilmarisen paja.
- **Tutkitaan maailmaa.** Hiidenkirnuista löytyy luolia, maailma luodaan proseduraalisesti, ja kokkaamalla saa hyödyllisiä buffeja.
- **Pelataan pitkään.** Yksi läpipeluu kestää yli 80 tuntia. Ensimmäisissä biomeissa viihtyy 6–8 tuntia, Tuonelassa yli 20.

---

<sub>Tehty Unity 6:lla (URP). Moninpeli toimii Netcode for GameObjectsilla. Nimi ja kaikki muukin voi vielä muuttua.</sub>
