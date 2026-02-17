# 3A Bygg AS - Nettside

Dette er den komplette nettsiden for 3A Bygg AS, klar for opplasting til GitHub Pages.

## Filstruktur

```
/
├── index.html              # Hovedside (forside)
├── assets/                 # JS og CSS filer (generert av Vite)
├── images/                 # Alle bilder
│   ├── firmalogo3abygg.jpg # Firmalogo
│   ├── favicon.jpg         # Favicon (samme som logo)
│   ├── bad1.jpeg           # Hero-bilde
│   ├── best2-6.jpeg        # Prosjektbilder (bad1-prosjektet)
│   ├── nesten1-36.jpg      # Prosjektbilder (annet prosjekt)
│   └── ...
└── tjenester/              # SEO-sider for lokale søk
    ├── badrenovering-asker.html
    ├── badrenovering-baerum.html
    ├── badrenovering-drammen.html
    ├── flislegger-asker.html
    ├── flislegger-baerum.html
    ├── flislegger-drammen.html
    ├── membran-asker.html
    ├── membran-baerum.html
    ├── membran-drammen.html
    ├── totalrenovering-asker.html
    ├── totalrenovering-baerum.html
    └── totalrenovering-drammen.html
```

## Hvordan laste opp til GitHub

### Steg 1: Opprett et nytt repository
1. Gå til https://github.com
2. Klikk på "New repository"
3. Navn: `3abygg` (eller ønsket navn)
4. Velg "Public"
5. Klikk "Create repository"

### Steg 2: Last opp filene

**Alternativ A: Via GitHub web-grensesnitt**
1. Klikk på "uploading an existing file"
2. Dra alle filer fra `dist`-mappen til opplastingsfeltet
3. Klikk "Commit changes"

**Alternativ B: Via Git (kommandolinje)**
```bash
cd dist
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/DITT-BRUKERNAVN/3abygg.git
git push -u origin main
```

### Steg 3: Aktiver GitHub Pages
1. Gå til repository-innstillingene (Settings)
2. Scroll ned til "Pages" (i venstre meny)
3. Under "Source", velg "Deploy from a branch"
4. Velg "main" branch og "/ (root)"
5. Klikk "Save"
6. Vent noen minutter - nettsiden blir tilgjengelig på `https://ditt-brukernavn.github.io/3abygg`

## Koble til eget domene (3abygg.no)

### Steg 1: GitHub-innstillinger
1. I GitHub Pages-innstillingene, under "Custom domain", skriv: `3abygg.no`
2. Klikk "Save"
3. Huk av "Enforce HTTPS" (anbefalt)

### Steg 2: DNS-innstillinger hos domeneleverandør
Logg inn hos din domeneleverandør (f.eks. Domainnameshop, One.com, etc.) og legg til følgende DNS-records:

**For apex-domene (3abygg.no):**
```
Type: A
Name: @
Value: 185.199.108.153
Value: 185.199.109.153
Value: 185.199.110.153
Value: 185.199.111.153
```

**For www (valgfritt):**
```
Type: CNAME
Name: www
Value: ditt-brukernavn.github.io
```

### Steg 3: Vent på propagering
Det kan ta opptil 24-48 timer før DNS-endringene er aktive over hele verden.

## Viktig informasjon

### Kontaktskjema
Kontaktskjemaet er koblet til Formspree:
- URL: https://formspree.io/f/xbdayyoj
- E-post: post@3abygg.no

### Organisasjonsnummer
Org.nr: 936 92 1248 (ikke MVA-registrert)

### Telefon
477 59 456

### Områder
Asker og omegn, inkludert:
- Asker
- Heggedal
- Røyken
- Hurum
- Bærum (Sandvika, Lysaker, Stabekk)
- Drammen (Strømsø, Bragernes, Åssiden)
- Lier

## SEO-sider

Nettsiden har 12 SEO-optimaliserte landingssider for lokale søk:
- Badrenovering: Asker, Bærum, Drammen
- Flislegger: Asker, Bærum, Drammen
- Membran: Asker, Bærum, Drammen
- Totalrenovering: Asker, Bærum, Drammen

## Vedlikehold

### Oppdatere innhold
1. Gjør endringer i filene
2. Last opp oppdaterte filer til GitHub
3. Endringene er live umiddelbart

### Legge til nye prosjektbilder
1. Last opp bilder til `images/`-mappen
2. Oppdater referanser i HTML-filene

## Support

Ved spørsmål om nettsiden, kontakt utvikler eller se GitHub Pages dokumentasjon:
https://docs.github.com/en/pages
