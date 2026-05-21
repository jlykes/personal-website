---
title: Dushu
subtitle: A Kindle-like app for Chinese language learners
kicker: Agentic Software Development / Chinese Learning
description: "Dushu is my personal Chinese reading app. It gives me a way to read Chinese more easily, and provides a number of features to help in my language learning journey. "
meta:
  - Cursor
  - Codex
  - React
  - Desktop and Mobile
heroImage: /images/dushu.png
heroImageAlt: Tablet showing a dark-mode Chinese reading interface with vocabulary annotations
videoOverviewUrl: https://youtu.be/bvZcCDngIQw?si=mfpLM4OGVZgkz5kV
videoOverviewLabel: Dushu video overview
problem:
  - Most tools pull Chinese reading in two opposite directions. E-readers are comfortable for long-form reading, but they assume I already know the language. Language-learning apps offer more support, but they often break reading into exercises or something else that feels more academic and less fun.
  - Dushu sits in the middle. It is designed for reading real Chinese text while still giving me enough help to keep going when I hit unknown words, confusing sentences, or text that is just slightly above my current level.
functionality:
  - title: Library View
    image: /images/dushu-library.png
    imageAlt: Dushu library view showing Chinese books and reading progress
    placeholder: Dushu library view with books, texts, and notes
    body: The library is the starting point for books and notes. It gives me a place to browse what I am reading, track progress, and manage different kinds of Chinese content in one place.
  - title: Books Reader
    image: /images/dushu-booksview.png
    imageAlt: Dushu books reader showing Chinese text with learning annotations
    placeholder: Main reader view for books
    body: The books reader is the core of the app. It is built to feel closer to a normal long-form reading experience than a lesson screen. It supports paginated reading, chapter navigation, saving of reading position, sentence-level progress tracking, pinyin, tone colors, and different underline style to keep track of how well I know a given word.
  - title: Notes Reader
    image: /images/dushu-notesview.png
    imageAlt: Dushu notes reader showing a shorter Chinese note with Markdown formatting
    placeholder: Main reader view for notes with Markdown formatting
    body: My other main reader view is for notes - selections of text that are much smaller than a typical book. The notes reader supports Markdown formatting, so that Chinese notes from any Markdown file will render cleanly.
  - title: Word and Sentence Popups
    placeholder: Word popup and sentence popup
    body: "When I click a word, Dushu shows the information I usually need in the moment: pinyin, a definition of that word in context, a star rating for how frequently the word appears, and the ability to score each word from 0 to 5 based on how well I know it. When I click a sentence, I can see a translation, as well as an explanation for any tougher elements that would trip up a language learner."
  - title: Flashcards
    placeholder: Sentence mining or Anki card creation drawer
    body: From the reading interface, I can create Anki flashcards both for learning new characters as well as new words. This makes flashcard creation super easy without having to leave the app, reducing friction.
howBuilt:
  - "I started building Dushu in the summer of 2025 using agentic software development tools - primarily Cursor. The first push took a few months and got the app to roughly 80% percent of what I wanted: a working Chinese reader with enough features to be useful in my daily study routine."
  - After that first push, I spent the next six months or so making smaller updates whenever a new piece of functionality became useful. I never had a full plan or roadmap - it just evolved to fit my needs in the moment.
  - For the first four or five months, AI was generating 90%+ of the code, but I was still reading and understanding almost all of it. As the AI tools improved, I got to the point where I was comfortable not looking at the code at all anymore, beause the AI rarely made major mistakes. And whenever it did make mistakes or introduce bugs, the AI was almost always able to fix them without me looking at the code. 
  - Technically, Dushu is a React progressive web app, running on Node.js. I use AI to pre-process all books and notes. I created a customized book/note JSON format that includes additional information such as definitions for each word, pinyin, translations, etc. Because everything is pre-processed in advance, pulling up things like word definitions in the app is almost instant. 
  - See below for a diagram of all of the moving parts and how this all fits together. 
technicalDiagramPlaceholder: "Technical diagram: reader -> vocabulary -> Anki / Notion / LingQ"
currentState:
  - I use Dushu almost every day and it has become a core part of my language learning routine. I expect to keep making small tweaks here and there as I think of other features that would be useful. The next major piece on my mind is adding audio support so that I can also have an "Audible-like" audiobook experience. 
  - Right now there are only two people who have access to Dushu - me and one other friend. If you are interested in trying it, you can reach out to me directly and I can most likely give you access for free.
---

This Markdown file powers the Dushu project page. Edit the frontmatter above to change the page copy, links, metadata chips, image paths, feature sections, and placeholder labels.
