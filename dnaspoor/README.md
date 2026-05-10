# DNASpoor Assistent — Installatiegids

## Stap 1 — Download de projectbestanden
Download de map `dnaspoor` met daarin:
- `api/chat.js` — de backend die de Anthropic API aanroept
- `public/index.html` — de volledige website
- `vercel.json` — Vercel configuratie
- `package.json` — projectinfo

## Stap 2 — Maak een GitHub account (gratis)
1. Ga naar https://github.com
2. Klik op "Sign up" en maak een account
3. Klik op "New repository" (groene knop)
4. Naam: `dnaspoor-assistent`
5. Kies "Public"
6. Klik "Create repository"

## Stap 3 — Upload de bestanden naar GitHub
1. Klik op "uploading an existing file" op je lege repository-pagina
2. Sleep de volledige `dnaspoor` map hiernaartoe
3. Klik "Commit changes"

## Stap 4 — Maak een Vercel account (gratis)
1. Ga naar https://vercel.com
2. Klik "Sign Up" → kies "Continue with GitHub"
3. Geef Vercel toegang tot je GitHub account

## Stap 5 — Deploy op Vercel
1. Klik op "Add New Project"
2. Kies je `dnaspoor-assistent` repository
3. Klik "Deploy" (Vercel detecteert alles automatisch)

## Stap 6 — Voeg je API-sleutel toe
1. Ga naar https://console.anthropic.com
2. Klik op "API Keys" → "Create Key"
3. Kopieer de sleutel (begint met `sk-ant-...`)
4. In Vercel: ga naar je project → "Settings" → "Environment Variables"
5. Voeg toe:
   - Name: `ANTHROPIC_API_KEY`
   - Value: jouw sleutel
6. Klik "Save" en dan "Redeploy"

## Klaar! 🎉
Je assistent draait nu op een URL zoals:
`https://dnaspoor-assistent.vercel.app`

## Hulp nodig?
- Vercel docs: https://vercel.com/docs
- Anthropic API: https://console.anthropic.com
