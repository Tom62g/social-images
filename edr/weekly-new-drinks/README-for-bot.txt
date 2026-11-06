ENERGY DRINK RATINGS - WEEKLY NEW DRINKS FOLDER (read me first)

An automated job refreshes this folder every Sunday at 12:00 noon Eastern. Read it at 13:00 ET the same day. Do not edit or delete anything here.

LOCATION: public GitHub repo Tom62g/social-images, folder edr/weekly-new-drinks/
  manifest: https://raw.githubusercontent.com/Tom62g/social-images/main/edr/weekly-new-drinks/latest/new-drinks.json
  poster:   https://raw.githubusercontent.com/Tom62g/social-images/main/edr/weekly-new-drinks/latest/poster.png
  (the manifest also gives posterUrl and a raw GitHub imageRawUrl for each drink)

WHERE TO LOOK
  latest/new-drinks.json   the manifest. It is written LAST, so if it exists and is dated today, the rest of the folder is complete.
  latest/poster.png        1080x1350 poster for this week's drinks (not created when nothing is new)
  latest/images/<slug>.jpg one image per drink (1000 px max side)
  latest/new-drinks.csv    the same list as a spreadsheet
  archive/<YYYY-MM-DD>/    a copy of every past run

HOW TO DECIDE WHETHER TO POST
  1. Open latest/new-drinks.json. Only post if runDate equals today's date (Eastern) AND status is "new-drinks" AND count is greater than 0.
  2. If status is "none", count is 0, or runDate is an older date, there is nothing new this week. Do not post, and do not reuse last week's content.

FIELDS PER DRINK (drinks[])
  name, brand, slug
  datePublished   the day it went live on the site (approximate to the day)
  pageUrl         the clean link to the drink's page
  trackedUrl      same page with tracking tags (utm_source=grok). Prefer this link in posts. You may change utm_source to the platform name (for example pinterest or x); leave the other tags as they are.
  imageFile       path inside latest/ (images/<slug>.jpg); imageUrl is the same picture on the live site
  whatsNew        one or two plain sentences on what is new about the drink
  tags            short facts you can use as hashtags or labels
  facts           caffeineMg, sugarG, calories, servingSizeFlOz, sugarFree, carbonated (label values; null means not known)
  ratingCount     how many ratings it has (0 means unrated, not bad)

CONTENT RULES
  - Facts are label values from EnergyDrinkRatings.com. Quote caffeine and sugar as labeled and name EnergyDrinkRatings as the source.
  - Do not call any caffeine amount safe or healthy for a particular person, and make no health claims.
  - A drink with 0 ratings is unrated, not poorly rated. Invite people to rate it; do not invent scores, reviews or quotes.
  - Use only what is in the manifest. If a detail is missing (for example no image), skip that detail instead of guessing.
  - For a week with many drinks, lead with the poster and link to newPageUrl (the site's /new page) and feature a few drinks individually.
