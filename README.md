# TANG BOT · Física 1

Chatbot de Física 1 (Gemini) + simulador de circuitos. Hosting gratuito en Vercel.

## API Key de Gemini
1. Crea la clave en https://aistudio.google.com/apikey (sin vincular facturación).
2. Nunca la pegues en el código. Va solo como variable de entorno `GEMINI_API_KEY`.

## Desplegar en Vercel
1. Sube la carpeta a un repositorio de GitHub (incluye `api/`, `index.html`, `sim.js`, `vercel.json`, `package.json`).
2. En https://vercel.com → **Add New → Project** → elige el repositorio.
3. En **Environment Variables** agrega `GEMINI_API_KEY` con tu clave.
4. Pulsa **Deploy**. Si cambias la clave después: *Settings → Environment Variables* y **Redeploy**.

## Ejecutar en local
```bash
npm i -g vercel
echo "GEMINI_API_KEY=tu_clave" > .env
vercel dev
```
Abre http://localhost:3000

Opcional: `GEMINI_MODEL=modelo1,modelo2` define el orden de modelos de respaldo.
