ENERGY DRINK RATINGS - THREADS POST BATCHES (read me first)

YOUR JOB
Write a batch of draft posts for the Threads account @edratingshq (Energy Drink Ratings). You do NOT post to Threads. You write one CSV file into this repo; a local job on Tom's PC loads it into a queue, Tom approves each post, and only approved posts are published at the time you set.

WHERE
  Public GitHub repo Tom62g/social-images
  Write your file to:  edr/threads/incoming/batch-YYYY-MM-DD.csv   (YYYY-MM-DD = the day you write it, Eastern)
  Commit and push it to the main branch. Never edit or delete a batch after pushing it. If a row needs fixing, push a NEW file (batch-YYYY-MM-DD-b.csv) with NEW ids.
  Do not touch any other folder. Do not edit queue files or other bots' files.

WHEN TO WRITE
  Once a week, on Sunday at 14:00 Eastern or later (the weekly new-drinks job finishes by 13:00). Cover the 7 days that start tomorrow.

THE CSV (UTF-8, first row is the header, exactly these columns in this order)
  id,post_at_et,text,image,notes
  id          grok-YYYY-MM-DD-NN  (date you wrote the batch, NN = 01, 02, ...). Letters, digits, dot, dash, underscore only. Never reuse an id.
  post_at_et  Eastern time, written 2026-11-10 12:30 (24-hour, no seconds, no time zone label)
  text        the post. Put the whole value in double quotes; write a double quote inside it as two double quotes. Line breaks inside the quotes are fine.
  image       leave EMPTY for a text-only post, or a path inside this repo, for example edr/weekly-new-drinks/archive/2026-11-08/images/<slug>.jpg
  notes       REQUIRED for every row: the source of every number or claim in the post (a page URL or manifest field) and one short line on why this post. Tom reads this to approve.
  Do NOT add an "approved" column. Every row arrives unapproved.

SCHEDULING
  - 1 or 2 posts per day, 7 days at most, so 7 to 14 rows per batch.
  - Times between 07:30 and 21:00 Eastern, at least 3 hours apart on the same day, and not always the same minute.
  - Every post_at_et must be at least 24 hours after you push, so Tom can approve it first. Rows in the past, or invalid ones, are rejected.

IMAGES
  - Only use an image that already exists in this repo (push it first if it is yours; put new images in edr/threads/images/).
  - Do NOT use edr/weekly-new-drinks/latest/... for an image: that folder is overwritten every Sunday. Use edr/weekly-new-drinks/archive/<runDate>/images/<slug>.jpg (the archive is permanent).
  - JPEG or PNG, under 8 MB, at least 320 px wide. A text-only post is fine and often better.
  - Only use pictures of a drink for the drink named in the post. Check the picture matches the caption.

WHAT TO POST ABOUT (mix across the week)
  1. New drinks: the manifest at edr/weekly-new-drinks/latest/new-drinks.json (see README-for-bot.txt in that folder). One drink per post, or a roundup that links to https://energydrinkratings.com/new.
  2. Caffeine and label facts from drink pages, brand pages (https://energydrinkratings.com/brands/<brand>) or the State of Energy Drinks report (https://energydrinkratings.com/state-of-energy-drinks).
  3. "Rate it" invitations for drinks with few or zero ratings (zero ratings means unrated, not bad).
  4. Occasional plain questions for readers ("What is your go-to ... ?"), no more than 1 in 5 posts.

NUMBERS MUST BE FRESH
  Open the live page the same day you write the batch and copy the figures from it. Never reuse a number from an older post, an earlier batch or memory: catalog counts and percentages change every week. Put the page URL and the "as of" date in notes. A wrong number is worse than no post.

WRITING RULES
  - Maximum 500 characters including the link. Aim for 150 to 350.
  - Voice: plain, factual, a little dry. No hype words, no all caps, at most one emoji, no hashtags (at most one topic word if it reads naturally).
  - Facts are label values from EnergyDrinkRatings.com. Name EnergyDrinkRatings as the source when you quote a figure.
  - Never call any amount of caffeine safe, healthy or recommended for a person, and make no health claims or medical advice.
  - Ratings always come with their count. Never call a drink "the best" from a handful of ratings.
  - Do not invent scores, reviews, quotes, sales claims or rankings. Do not name or tag individual people.
  - One link per post, as a bare URL, with tracking on the end: ?utm_source=threads&utm_medium=social&utm_campaign=<short-topic-slug>  (if the URL already has "?", join with "&"). Link to the site, not to a retailer.
  - No engagement bait ("like if...", "tag a friend"), no politics, no comparisons that put down a named competitor.
  - Do not repeat a topic, drink or wording used in your earlier batches (read the files already in edr/threads/incoming/ before writing).

CHECK BEFORE YOU PUSH
  Header row exact; every id new; every post_at_et valid and at least 24 hours ahead; every text 500 characters or fewer; every image path exists; every row has notes; every number matches the live page.
