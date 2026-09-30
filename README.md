# Sprout

Sprout is a small, beginner friendly AI-style chat app that needs no API key and no build tools. It searches Wikipedia's public API when you ask a question, makes a short answer from the retrieved passages, and links to the pages it used. You can also save notes for Sprout; those notes and your chat history live in this browser's local storage.

## Run it

1. Open `index.html` in a modern browser.
2. Ask a question while connected to the internet (Wikipedia lookup needs a connection).
3. Choose **Teach Sprout** to add personal notes. Use the same browser profile to see them again.

You can also serve this folder with any static web server. There are no packages to install, no account, and no API credentials.

## What it does and does not do

This is retrieval, not model training. Sprout searches Wikipedia and assembles relevant sentences; it does not learn new language skills or update model weights. The saved notes provide simple keyword based context and do not leave the device. Wikipedia content is available under its own licensing terms; this app links back to source pages. To train a capable general purpose model from scratch takes a large curated dataset, substantial compute, and a much bigger training pipeline. This project is a workable first step for learning how an AI chat app can retrieve open information and cite it.

The app uses the MediaWiki API at `https://en.wikipedia.org/w/api.php` and requires internet access for answers. It has no server component and does not send chat or notes to a backend.
