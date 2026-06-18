# almara-waitlist

Fake-door A/B demand test for **Almara**. Two landing pages, same app, opposite
positioning. Run ~$150 of TikTok/Reddit traffic to each and compare waitlist conversion.

- **`/a/`** — *control:* chores & rewards that stick ("the sticker chart is dead").
- **`/b/`** — *the bet:* a calm daily contemplative ritual ("the two minutes...").

Both pages are built on the **almara-pitch design system** (Cormorant Garamond + Inter
Tight, the landscape hero art, the real skill/equipment art, shared `/assets`), trimmed
to a focused conversion page and differing only in **positioning** (hero + thesis +
steps + proof section) so the A/B cleanly tests the message, not the polish.

Signups POST to a Supabase `waitlist` table tagged by `variant` (`A` / `B`), so the
split is measurable. Read results with the service_role key or the Supabase dashboard;
the anon key in these pages can only INSERT (see `0024_waitlist.sql` in the app repo).

Copy + judging rationale: `almara` repo → `docs/marketing/landing-page-tournament.md`.

Live (GitHub Pages):
- https://ttsatsos.github.io/almara-waitlist/a/
- https://ttsatsos.github.io/almara-waitlist/b/
