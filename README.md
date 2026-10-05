# MIVA · B2B Partner Portal Demo

Kompletan statički demo za prezentaciju Lani / MIVA, prilagođen hrvatskom jeziku i njihovom asortimanu. Radi na GitHub Pagesu bez instalacije i bez build koraka.

## Postavljanje na GitHub Pages

1. Raspakirajte ZIP na računalu.
2. U GitHub repozitorij prenesite **sadržaj ZIP-a**, tako da je `index.html` izravno u korijenu repozitorija. Prenesite i cijele mape `assets`, `vendor` i `primjeri`.
3. Otvorite **Settings → Pages → Deploy from a branch**.
4. Odaberite granu **main** i mapu **/ (root)**, pa kliknite **Save**.
5. Nakon završetka objave otvorite poveznicu koju GitHub prikaže. Ako vidite staru verziju, osvježite stranicu s Ctrl+F5.

Sve putanje do datoteka su relativne, pa demo radi i u podmapi GitHub Pages repozitorija. Nije potrebno mijenjati `app.js` ni instalirati pakete. `index.html` se može otvoriti i izravno u pregledniku; za dosljedno pamćenje demo promjena preporučena je GitHub Pages poveznica.

## Demo pristup

Najlakše je na početnom ekranu kliknuti jedan od gotovih profila.

| Uloga | E-mail | Lozinka |
| --- | --- | --- |
| Restoran / HoReCa | restoran@demo.miva.hr | Demo2026! |
| Hotel | hotel@demo.miva.hr | Demo2026! |
| Trgovina s blokiranim kreditom | trgovina@demo.miva.hr | Demo2026! |
| Lana / administracija | lana@demo.miva.hr | Demo2026! |

## Uključene funkcionalnosti

- Kupac i administrator, odvojeni izbornici, brzi ulazak i **Odjavi se**.
- 116 stvarnih proizvoda iz MIVA javnog asortimana, lokalne originalne fotografije, proizvođači i dostupne specifikacije.
- Vina, pjenušci i šampanjci, žestoka pića, Riedel čaše, delikatese i dodaci.
- Katalog u mrežnom i tabličnom prikazu, pretraživanje, filtri po kategoriji, proizvođaču i dostupnosti, sortiranje i favoriti.
- Detalji svakog proizvoda: volumen / format, proizvođač, godište i alkohol kada su dostupni, oznake regije/sorte, demo pakiranje, zalihe po skladištima i količinski uvjeti. Poveznica na izvorni MIVA proizvod s punim opisom.
- Cjenici po partneru, rabati 10–20% po profilu i količinska pravila 10 / 20 / 30%. Primjenjuje se povoljniji rabat; rabati se ne zbrajaju.
- Košarica, izmjena količine, automatski obračun, spremanje i učitavanje košarice, adresa / poslovnica, način dostave, skladište, željeni datum, referenca i napomena.
- Provjera zalihe izabranog skladišta i kreditnog limita. Slanje narudžbe, rezerviranje raspoložive robe i kreditnog iznosa, ručno ili automatsko odobravanje.
- Brza narudžba po šifri ili nazivu, više redaka odjednom, provjera nepoznatih artikala i količina.
- Stvarno čitanje CSV, TXT, XLSX i XML datoteka, pregled redaka i dodavanje samo valjanih artikala. Mapa `primjeri` sadrži datoteke spremne za isprobavanje.
- Fotografija / PDF: jasno označeni pripremljeni primjer prepoznavanja, s nepoznatim artiklom za provjeru. **OCR nije implementiran.**
- 15 početnih narudžbi i novi lokalno spremljeni unosi. Statusi: u obradi, čeka odobrenje, blokirana, potvrđena, u pripremi, otpremljena, isporučena, otkazana. Povijest promjena, detalji i ponavljanje narudžbe po aktualnim cijenama.
- PDF potvrde, demo računi / otpremnice, ponuda iz košarice, cjenici CSV / XLSX / PDF, izvoz narudžbi, zaliha i izvještaja.
- Kreditni profil, rok plaćanja, ugovoreni rabat, dugovanje i rezervirani iznos.
- MIVA Partner klub kao B2B koncept: Silver / Gold / Platinum, bodovi i iskorištavanje demo nagrada.
- Upiti i reklamacije: kupac kreira upit, administrator prati i mijenja status.
- Administracija partnera, rabata, limita, dugovanja, bodova i blokade računa. Pogled pojedinog kupca.
- Administracija zaliha u tri demo skladišta, količinskih pravila, minimalne narudžbe i automatskog odobravanja.
- Zahtijeva pažnju: blokirane narudžbe i zahtjevi za pregled; izvještaji i dnevnik aktivnosti.
- Simulacija toka katalog/cjenici → portal, narudžbe → ERP, zalihe/statusi → portal.
- Prilagodljiv prikaz za mobitel i računalo, dijalozi, tipkovnica i obavijesti.

## Predloženi redoslijed prezentacije

1. Prijavite se kao restoran. Otvorite katalog i detalje jednog vina; pokažite zalihe i ugovorenu cijenu.
2. Dodajte dostupan artikl i promijenite količinu na 60 ili 120. Pokažite promjenu rabata i ukupnog iznosa.
3. Pošaljite narudžbu iz skladišta koje ima dovoljnu zalihu. Otvorite detalje i preuzmite demo PDF.
4. Uvezite `primjeri/narudzba.xlsx`; zatim isprobajte primjer fotografije s nepoznatim artiklom.
5. Otvorite trgovački profil da pokažete kreditnu blokadu, ili povećajte količinu kako biste prešli raspoloživi kredit.
6. Odjavite se i otvorite administraciju. Pokažite zahtjeve za pažnju, uvjete partnera, provjeru kreditnog limita, odobravanje i promjenu statusa.
7. Pokažite zalihe, cjenike, Partner klub i označeni demo integracija.
8. Prije nove prezentacije otvorite **Administracija → Postavke → Vrati početne podatke**.

## Izvori i granice demonstracije

Nazivi, fotografije, javne cijene i dostupne specifikacije preuzeti su s https://www.miva.com.hr/ 5. listopada 2026. Ovo je reprezentativan izbor od 116 proizvoda, **nije cijeli MIVA katalog**. Točni izvori za svaki proizvod nalaze se u `izvori.csv` i detaljima proizvoda.

Poslovni kupci i kontakti su izmišljeni. B2B cijene, pakiranja, skladišta, zalihe, limiti, dugovanja, narudžbe i B2B program vjernosti su demonstracijski podaci. B2B cijena izvedena je iz javne cijene uz ilustrativno skidanje 25% PDV-a i primjenu demo rabata. Time se ne tvrdi da MIVA koristi ove poslovne uvjete ili porezni obračun za svaki stvarni artikl.

Nema stvarne prijave, slanja e-mailova, plaćanja, ERP/WMS veze ni izdavanja stvarnih računa. Ne upisujte stvarne lozinke ili osjetljive podatke. Demo podatke preglednik čuva lokalno; različiti uređaji nemaju zajedničku bazu. Odjava čuva promjene za nastavak prezentacije. Proizvodne narudžbe zahtijevaju zaseban backend i stvarnu integraciju.

Fotografije i logo pripadaju njihovim nositeljima prava i ovdje se koriste za prezentacijski koncept za MIVA. Uključene biblioteke: SheetJS CE 0.18.5 (Apache 2.0), jsPDF 2.5.2 (MIT); licence su u `vendor/LICENSES.txt`.
