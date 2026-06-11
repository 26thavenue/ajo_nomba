# ajo_nomba

Here's the PRD as a visual document you can reference and share:That's your basic PRD. A few things worth flagging:

**Why this combo wins at the hackathon:** Ajo alone is too social, offline-first alone is too technical — together they tell a complete story: a real Nigerian problem, solved with real Nomba infrastructure, that works where internet doesn't.

**The strongest demo moment** will be showing a contribution logged with airplane mode on, then toggling network back on and watching it sync + trigger a Nomba payout automatically. Judges will feel that.

Use the buttons at the bottom of the PRD to keep building — user stories, DB schema, or a timeline are good next steps.

Great question — let me break it down simply.

**The core problem it solves:**

Most of Nigeria's markets — Balogun, Onitsha, Aba, Ariaria — have terrible or inconsistent internet. If you build a normal app and the network drops, the app just... stops working. A trader trying to record that Mama Titi paid her ₦5,000 contribution gets an error. She walks away. Nothing is saved.

**Offline-first means the app works first, syncs later.**

Here's the mental model:

> Think of it like how your phone's camera works. You take photos whether you have data or not. The photos sit on your phone. The moment you get WiFi, they upload to iCloud. You never lose a photo because of bad network.

AjoChain works the same way:

1. Organiser collects ₦5,000 from a member at the market
2. They tap "Record payment" — it saves **instantly on the device** (no internet needed)
3. The member gets a receipt on the spot
4. Later, when the organiser's phone catches network — even briefly — it silently syncs everything to the server and triggers the Nomba payout

**Without offline-first, you have this problem:**

- Network drops mid-market day → app freezes
- Organiser not sure if payment was recorded → records it again → duplicate entry
- Member disputes the record → no receipt → drama in the group

**With offline-first:**

- Network is irrelevant to the organiser's daily workflow
- Every payment is timestamped and receipted immediately
- Sync happens in the background, invisible to the user

The technical piece (IndexedDB, Service Workers, sync queues) is just the machinery that makes this happen — but the *product value* is simply: **your ajo group runs smoothly even in Ladipo market with one bar of network.**

Want me to show what the actual user flow looks like screen by screen?
