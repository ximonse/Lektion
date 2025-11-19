# Lärargenomgång - Inspelningsapp

En app för att spela in, transkribera och rensa lärargenomgångar.

## Funktioner
- 🎤 Spela in ljudgenomgångar
- 📝 Transkribera med OpenAI Whisper (billigt!)
- 🧹 Rensa bort irrelevanta kommentarer med Claude
- 💾 Ladda ner som textfil

## Deployment till Vercel

### Alternativ 1: Via Vercel Web Interface (Enklast!)

1. Gå till [vercel.com](https://vercel.com) och logga in
2. Klicka på "Add New" → "Project"
3. Dra och släpp hela projektmappen i upload-området
4. Klicka på "Deploy"
5. Klar! Du får en URL typ `larar-inspelning.vercel.app`

### Alternativ 2: Via Vercel CLI

```bash
# Installera Vercel CLI
npm install -g vercel

# Gå till projektmappen
cd larar-inspelning

# Deploya
vercel deploy --prod
```

### Alternativ 3: Via GitHub

1. Skapa ett GitHub-repo
2. Pusha detta projekt till repot
3. Gå till [vercel.com](https://vercel.com)
4. Importera repot från GitHub
5. Klicka på "Deploy"

## Vad du behöver

- En **OpenAI API-nyckel** från [platform.openai.com/api-keys](https://platform.openai.com/api-keys)
- Första gången du använder appen matar du in nyckeln

## Kostnad

- Whisper: ~$0.006 per minut inspelning
- Claude: ~200-500 tokens för rensning (några ören per genomgång)

**Totalt:** En 10-minuters genomgång kostar cirka 10-15 ören!

## Support

Appen fungerar på:
- ✅ Desktop (Chrome, Firefox, Edge, Safari)
- ✅ Android (Chrome)
- ✅ iOS/iPad (Safari 14.3+)
