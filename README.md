# A1 German Anki Deck

876 flashcards for German A1 vocabulary (Goethe wordlist).

Available in two languages:
- 🇷🇴 **German → Romanian**
- 🇬🇧 **German → English**

## Download

📥 **[Download from Releases](https://github.com/oprobiu/DataDAF1/releases)** — import directly into [Anki](https://apps.ankiweb.net/)

Each release includes both language variants as separate .apkg files.

## What's in the deck

- 876 cards (1752 with reverse), covering Goethe A1 wordlist
- German word + example sentence on front, translation on back
- TTS audio for every word and sentence (gTTS, de-DE)
- Color-coded by word type: nouns (by gender), verbs (by form), adjectives, adverbs, etc.
- Tags: NOUN, VERB, ADJ, ADV, PREP, CONJ, PRON, PHRASE, QWORD, NUM, OTHER

## Build from source

```bash
bash bootstrap.sh        # fetch AFAS tools
make validate            # check both languages
make build               # build both .apkg files
make build-ro            # build Romanian only
make build-en            # build English only
```

## Structure

```
data/
├── ro/                  # German → Romanian
│   ├── notes.csv
│   └── deck.json
├── en/                  # German → English
│   ├── notes.csv
│   └── deck.json
├── note_meta.csv        # shared Anki IDs
└── card_meta.csv        # shared card IDs
media_files/             # shared TTS audio
```

## License

See [LICENSE](LICENSE).
