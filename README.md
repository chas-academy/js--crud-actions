# 🤖 JavaScript i praktiken - CRUD actions

Denna uppgift bygger vidare på [js--fetch-intro](https://github.com/chas-academy/js--fetch-intro) och låter er utforska ytterligare möjligheter med Fetch API. Förutom att hämta data från en extern server kan ni använda det här verktyget för att skapa, uppdatera och radera data. **Rekommenderas att göras i grupp**.

- **C** reate
- **R** ead
- **U** pdate
- **D** elete

## 👩‍💻 Steg

1. Det finns redan en `BASE_URL` för ert API. För att det ska bli en fullständig endpoint behöver ni kedja på en route/path
   - Just nu finns `/users` och `/dawgs`. Meddela utbildaren om ni vill skapa er egen route. Det kan vara klokt för att undgå att ta bort någon annan grupps data. Så länge ni skapar mer än ni raderar bör det inte vara något större problem dock
   - Läs dokumentationen noga om ni väljer ett annat API. Den ska tillåta alla CRUD actions. Ibland kan det även krävas att ni skapar en token för att få använda API:t
2. Skriv logiken för att hämta, skapa, uppdatera och radera data från det API:et
   - Testa att skicka många olika slags key value pairs när ni skapar ny data - Arrayer, länkar till bilder etc.
3. Hantera eventuella errors och oväntad respons
4. Bekräfta att ni får tillbaka förväntad respons och att dina ändringar har effekt

### Jobba vidare på uppgiften (Valfritt)

1. Skapa ett UI för att visa upp hämtad data från API:et
   - Exempelvis en card layout för att visa upp datan i de olika objekten på ett snyggt sätt
   - Använd [dribble.com](https://dribbble.com/shots/26135934-UnifiedUI-Luxury-Stay-in-Paradise-Product-Section) eller liknande sida för att hitta designprototyper
2. Skapa ett formulär som kör PUT/PATCH-anropet när dess data skickas

### _Uppgiften är löst när datan från API:et har hämtats, skapats och delvis uppdaterats och raderats_
