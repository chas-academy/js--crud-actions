# 🤖 JavaScript i praktiken - CRUD actions

Denna uppgift bygger vidare på [js--fetch-intro](https://github.com/chas-academy/js--fetch-intro) och låter er utforska ytterligare möjligheter med Fetch API. Förutom att hämta data från en extern server kan ni använda det här verktyget för att skapa, uppdatera och radera data. **Rekommenderas att göras i grupp**.

- **C** reate
- **R** ead
- **U** pdate
- **D** elete

## 👩‍💻 Steg

1. Det finns redan en `BASE_URL` för ett mock API. För att det ska bli en fullständig endpoint behöver ni kedja på en route/path
   - Just nu finns `/users` och `/dawgs`. Utöka `db.json` om ni önskar fler routes. Namnet på keyn blir namnet på routen.
   - Läs dokumentationen noga om ni väljer ett annat API. Den ska tillåta alla CRUD actions. Ibland kan det även krävas att ni skapar en token för att få använda API:t
2. Följ guiden för att sätta upp JSON Server om ni inte valt ett eget API.
3. Skriv logiken för att hämta, skapa, uppdatera och radera data från det API:et
   - Testa att skicka många olika slags key value pairs när ni skapar ny data - Arrayer, länkar till bilder etc.
4. Hantera eventuella errors och oväntad respons
5. Bekräfta att ni får tillbaka förväntad respons och att dina ändringar har effekt

### Mocka API via JSON Server

Med hjälp av NPM-paketet `json-server` kan vi skapa ett mock REST API utan att behöva bry oss om rate limiting, access tokens och liknande hinder. Detta kräver en mindre set-up. Följ guiden nedan:

1. Installera paketet globalt på din dator med `npm install -g json-server` (Eller lokalt för denna repo. Isåfall måste du först initiera en `package.json`-fil med `npm init`)
2. Starta upp en lokal JSON-server med `json-server --watch db.json`. Den kommer automatiskt att välja port 3000 på local host. Du kan använde `--port` flaggan om du vill specifikt använda en annan port - Exempelvis `json-server --watch db.json --port 8000`
   - Notera `db.json` i andra halvan av kommandot. Det betyder att `db.json` är din mock-databas som JSON Server håller koll på.
3. Du har nu en lokal REST API att hämta, skapa, uppdatera och radera data från.

### Jobba vidare på uppgiften (Valfritt)

1. Skapa ett UI för att visa upp hämtad data från API:et
   - Exempelvis en card layout för att visa upp datan i de olika objekten på ett snyggt sätt
   - Använd [dribble.com](https://dribbble.com/shots/26135934-UnifiedUI-Luxury-Stay-in-Paradise-Product-Section) eller liknande sida för att hitta designprototyper
2. Skapa ett formulär som kör PUT/PATCH-anropet när dess data skickas

### _Uppgiften är löst när datan från API:et har hämtats, skapats och delvis uppdaterats och raderats_
