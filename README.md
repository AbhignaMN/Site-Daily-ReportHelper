# Site Daily Report Helper

A simple one-page web app for construction supervisors in India. Type rough notes in **Hindi, English or Hinglish**, tap one button, and get a clean daily site report that you can copy or send on WhatsApp.

It works on a phone, uses large buttons, and needs no install, no login and no server.

**Live app:** https://abhignamn.github.io/Site-Daily-ReportHelper/

## Screenshots

![Output 1](Screenshot%202026-11-19%20102243.png)

![Output 2](Screenshot%202026-11-19%20102259.png)

![Output 3](Screenshot%202026-11-19%20102315.png)

## What it does

You write messy notes the way you would normally say them, for example:

```
aaj 3rd floor slab ka shuttering complete hua
12 mistri, 20 helper, 4 carpenter aaye
cement 50 bag kal tak chahiye
sand ka truck late aaya, 2 ghante kaam ruka
kal slab ki dhalai shuru karenge
```

The app sorts them into five sections:

| Section | What goes in it |
| --- | --- |
| Work Done | Work finished or in progress today |
| Manpower | Each trade with its count, plus a total |
| Material Needed | Material to order, with quantity and date |
| Problems | Delays, breakdowns, weather, shortages |
| Plan for Tomorrow | What is planned next |

## How to use

1. Type or paste your notes into the box.
2. Choose the report language, **English** or **हिन्दी**.
3. Tap **Make Report**.
4. Tap **Copy Report** to copy it, or **Send on WhatsApp** to share it.

The **Example** button loads sample notes. **Clear** empties the box. Your notes are saved on your own phone so they are still there if you reopen the page.

## How it works

The app is a single file, `index.html`, with no libraries to install. It sorts each line of the notes using keyword matching for Hindi (Devanagari), English and Hinglish words. It looks at worker names with numbers (mistri, helper, mason, labour and similar), words for needing something (chahiye, lagega, required), problem words (late, kharab, delay, barish) and future words (kal, karenge, tomorrow).

Because it is keyword based, it can sometimes put a line in the wrong section. **Read the report once before you send it.**

## Run it on your own computer

Download `index.html` and open it in any browser. Nothing else is needed.

## Put it online with GitHub Pages

1. Upload `index.html` to a GitHub repository.
2. Go to **Settings → Pages**.
3. Set the source to **Deploy from a branch**, choose `main` and `/ (root)`, then save.
4. Your link will be `https://<username>.github.io/<repository>/`.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app |
| `README.md` | This file |
| `Screenshot *.png` | Pictures of the output |
