# RiffBoard
Overview of my journey with claude code developed app for musicians. Note: This repo does not contain the app code, and is only for sharing my experience, product thoughts and journey.

## Overview ##
StickyNotes started as a personal frustration: as a hobbyist musician and songwriter, I kept losing track of ideas buried in an ever-growing, disorganized Voice Memos library, so I set out to build the tool I actually wanted — one built specifically for songwriters, not musicians broadly, with organization and retrieval as the core differentiator rather than just recording. 

The project began with a GTM strategy session, identifying the key user (ICP) and a 12-month cost/revenue model before a single line of code. I ran through many trade - off analyses on development methods such as:
- Base44/Loveable vs Claude Code - I wanted to learn claude code, fullstack development and the utilities that are necessary. 
- Native vs PWA - Wider Coverage and multi-platform was a differentiator
- Cloud Storage vs Local
- GTM, including target market segments (TAM/SAM/SOM)
- Pricing/Paywall timing - Subscription or one-off, feature or usage limits.

Furthermore, competitive research identified few similar apps in the space of Voice Memos for musicians, such as: Tape It, Dubnote, and I was able to refine my concept further through structured feedback from early testers.

Once I was in a position to understand my product's core value, proposition and market differentiation, moved into using Claude Design as my UX/UI designer, the UX and flow, then designing the infrastructure. (See an example design exploration html file).

## Development ##
The first real version had to be highly stripped, but functional for the large chunk of the user journey.
The development used Claude Code only. Using claude skills to hone and refine prompts to develop in 2 phases, infrastructure, then frontend. The app is React.js based PWA with a Supabase backend (auth, storage, and database). I wanted analytics from the start, and integrated Posthog as part of the infrastructure phase. This was to ensure I can understand users from the very beginning, and support bugs fixes with usage and recordings. It's now a freemium product with Stripe monetization shortly being rolled out, and remains very much a living, evolving project.

The v1 is live with an ever growing user base [StickyNotes](audiostickynotes.netlify.app) 
