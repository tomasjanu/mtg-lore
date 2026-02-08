# MTG Lore Translator

A web app for reading Magic: The Gathering lore stories translated to Czech.

## Features

- **Fetch stories from URL** – paste a link from `magic.wizards.com` and the app extracts the article text
- **Manual paste** – if URL fetching fails (CORS), you can copy-paste the story text directly
- **Automatic translation** – translates English text to Czech using MyMemory API (free)
- **Story library** – all stories are saved in your browser's localStorage
- **Reading view** – comfortable reading layout with English/Czech toggle
- **Google Translate fallback** – link to open untranslated articles in Google Translate

## How to host (GitHub Pages)

1. Go to your repository **Settings** → **Pages**
2. Under "Source", select the branch (e.g. `main`) and folder `/ (root)`
3. Click **Save**
4. Your page will be available at `https://<username>.github.io/mtg-lore/`

## Translation limits

The app uses [MyMemory API](https://mymemory.translated.net/) for translation:

- **Without email**: ~5,000 characters/day
- **With email** (enter in the form): ~50,000 characters/day (enough for 1-2 full stories)
- Alternatively, save without translation and use the Google Translate link

## Usage

1. Click **+ Přidat příběh** (Add story)
2. Paste a URL like `https://magic.wizards.com/en/news/magic-story/lorwyn-eclipsed-episode-1-out-of-this-wood` and click **Načíst** (Fetch)
3. If fetching fails, copy the story text from the browser and paste it in the text area
4. Click **Přeložit a uložit** (Translate & save)
5. Read the translated story from the library