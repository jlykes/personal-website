# Dushu

## Page Intent

This is the working copy for the Dushu project page. The page should read like a project case study for a personal tool, not like a SaaS landing page. It should explain what Dushu is, why I built it, what the interface includes, how it was built, and where the project stands now.

## Hero

**Title:** Dushu

**Subtitle:** A Kindle-like app for Chinese language learners

**Image placeholder:**
`[hero image: Dushu tablet/e-reader image from homepage]`

**Short description:**
Dushu is my personal Chinese reading app. It gives me a calm long-form reading surface while adding the language-learning layer I need: pop-up definitions, pinyin, color representation for tones, vocabulary status, flashcard creation, and progress tracking across books, imported texts, and generated notes.


## The Problem

Most tools pull Chinese reading in two opposite directions. E-readers are comfortable for long-form reading, but they assume I already know the language. Language-learning apps offer more support, but they often break reading into exercises or something else that feels more "academic" and less fun. 

Dushu sits in the middle. It is designed for reading real Chinese text while still giving me enough help to keep going when I hit unknown words, confusing sentences, or text that is just slightly above my current level.

You can see a video describing the app and its functionality here: https://youtu.be/bvZcCDngIQw?si=mfpLM4OGVZgkz5kV


## What It Does

### Library View

`[image placeholder: Dushu library view with books/texts/notes]`

The library is the starting point for books, imported texts, and notes. It gives me a place to browse what I am reading, track progress, and manage different kinds of Chinese content in one place.



### Reading View


The reader is the core of the app. It is built to feel closer to a normal long-form reading experience than a lesson screen.

It supports paginated Chinese reading, saved reading position, chapter navigation, sentence-level progress tracking, display of pinyin and/or colors for tones, and different colored underlines to keep track of how well I know a given word.

`[image placeholder: main reader view for books]`
`[image placeholder: main reader view for notes]`

I have one interface for books, and one interface for other general notes/texts (supports Markdown formatting).


### Word and Sentence Popups

`[image placeholder: word popup with definition, pinyin, learning status, and controls]`

When I click a word, Dushu shows a popup with the information I usually need in the moment: 

- Pinyin
- Definition of that word in context (pre-generated using AI)
- Score for how frequently the word appears
- Ability to score each word from 0 to 5 based on how well I know it


`[image placeholder: sentence popup with translation and grammar explanation]`

When I click a sentence, I can also see a translation (pre-generated using AI), as well as an explanation for any tough grammar or anything else that would trip up a language learner


### Flashcards

`[image placeholder: sentence mining or Anki card creation drawer]`

From the reading interface, I can create Anki flashcards both for learning new characters as well as new words. This makes flashcard creation feel like a byproduct of reading rather than a separate workflow that I have to remember to do later.


## How I Built It

I started building Dushu in the summer of 2025 using Cursor. The first push took a few months and got the app to roughly an 80 percent version of what I wanted: a working Chinese reader with enough vocabulary support and progress tracking to become useful in my actual study routine.

After that first push, I spent the next six months or so making smaller updates whenever a new piece of functionality became useful. The app grew less like a finished product with a fixed roadmap and more like a personal tool that grew to fit my exact preferences.

`[image placeholder: technical diagram or workflow image showing reader -> vocabulary -> Anki/Notion/LingQ]`

Technically, Dushu is a React 18, TypeScript, Vite, and Tailwind PWA with a Node/Express proxy and Supabase-backed persistence. Books / notes are pre-processed using AI to generate key information surfaced in the app such as word definitions (defined in the context of the passage). 


## Current State And Next Steps

Dushu is active and I use it almost every day. It is probably around 90 percent of what I currently want it to be. I expect to keep making small tweaks here and there. Next major thing might be adding support for audio so that I can have a full audiobook experience. 

Right now, Dushu is mainly for my own individual use. I have also given access to one friend. If you are interested in trying it, you can reach out to me directly and I can most likely give you access for free. 
