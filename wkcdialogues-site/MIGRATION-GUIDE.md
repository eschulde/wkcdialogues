# How to Move This Site to Google Sites

## What's Built

A complete standalone HTML site at `/Users/es/Desktop/es/openclaw/wkcdialogues-site/` with:
- ✅ All 15 pages (Home, Overview, Participants, 6 Video Dialogue categories, Journal, Design Proposals, Contribute, About AoD, Volunteer, Acknowledgement)
- ✅ 49 YouTube videos embedded (6 pending upload)
- ✅ Bilingual EN/ZH toggle
- ✅ Design proposal images (Foster, OMA, Rocco) + PDFs
- ✅ Event photos (Oct workshop sessions)
- ✅ Pre-workshop photos (6 images)
- ✅ Participant portrait photos (60+ portraits next to videos and in participant list)
- ✅ Original WordPress title images for each section
- ✅ Home page index image collage (16 images from original site)
- ✅ Original WKCDialogues logo
- ✅ Drawings (Li Chi Ching, Jeffrey Lau Wan Kit)
- ✅ Group/collaboration photos (Marisa Yiu + Ai Weiwei, Eric Schuldenfrei + Leo Lee Ou Fan, etc.)
- ✅ Journal entries with highlighted quotes (using original WKC color coding)
- ✅ Full participant list (~65 people)

## Moving to Google Sites

The new Google Sites (sites.google.com) has **no API** for programmatic page creation. This must be done manually in the browser. Here's the fastest path:

### Step 1: Open Your Google Site
Go to: https://sites.google.com/eskyiu.com/wkcdialogues/home?authuser=1

### Step 2: Create the Page Structure

In Google Sites, click **Pages** (left sidebar) → **+** → **New page**. Create these pages in order:

1. **Home** (already exists)
2. **Overview** (sub-page of Home)
3. **The Participants** (sub-page of Home)
4. **Video Dialogues** (sub-page of Home) — this will be a parent for the 6 categories:
   - On Nature
   - On Building Codes
   - On Ideas
   - On Networks
   - On Demographics
   - On Education
5. **Journal** (sub-page of Home)
6. **Design Proposals** (sub-page of Home)
   - Foster + Partners
   - OMA
   - Rocco Design Architects
7. **Contribute Your Dialogue** (sub-page of Home)
8. **About AoD** (sub-page of Home)
9. **Volunteer** (sub-page of Home)
10. **Acknowledgement** (sub-page of Home)

### Step 3: Add Content to Each Page

For each page, use the content from the matching file in `google-sites-content/`:

| Google Sites Page | Content File |
|-------------------|-------------|
| Home | `00-home-en.md` (type the intro text, add navigation links) |
| Overview | `01-overview-en.md` + `01-overview-zh.md` |
| The Participants | `02-participants-en.md` (copy the participant list) |
| On Nature | `04-on-nature-en.md` — paste YouTube URLs, Google Sites auto-embeds them |
| On Building Codes | `05-on-building-codes-en.md` |
| On Ideas | `06-on-ideas-en.md` |
| On Networks | `07-on-networks-en.md` |
| On Demographics | `08-on-demographics-en.md` |
| On Education | `09-on-education-en.md` |
| Journal | `03-journal-en.md` |
| Design Proposals | `14-design-proposals-en.md` + upload PDFs/images |
| Contribute | `10-contribute-en.md` |
| About AoD | `11-about-aod-en.md` (content needed) |
| Volunteer | `12-volunteer-en.md` (content needed) |
| Acknowledgement | `13-acknowledgement-en.md` (content needed) |

### Step 4: Embed Videos

For each video dialogue page:
1. In Google Sites edit mode, click **Insert** → **YouTube**
2. Paste the YouTube URL from the content file
3. Google Sites auto-embeds the video player
4. Add the person's name and topic as text above each video

**6 videos not yet on YouTube** (show as "not uploaded"):
- Lucien Gamborotta — tidal energy (Nature)
- Wallace Chang — green art mobilizations (Building Codes)
- Yung Ho Chang — stacking and density as city culture (Building Codes)
- Graphic Airlines — show us the artist incentives (Ideas)
- Yana Peel + Nick Simunovic + Joanne Ooi — much more on M+ (Ideas)
- Zhu Tao (Ideas) + Jay Forster (Networks)

### Step 5: Upload Design Proposal PDFs & Images

1. Upload all PDFs from `assets/design-proposals/` to Google Drive
2. In Google Sites, use **Insert** → **Drive** to embed the PDFs
3. For panel images, use **Insert** → **Images** and upload the JPG files

### Step 6: Bilingual Approach

**Recommended**: Put EN and ZH on the same page, separated by a horizontal line:
1. Paste English content first
2. Add a divider (Insert → Divider)
3. Paste Chinese content below

Or create EN/ZH sub-pages with a language toggle link at the top of each page.

### Step 7: Upload Title Images

The original WordPress title images are in `assets/images/`:
- `title_aims.png` / `title_aims_zh.png` — for Overview page
- `title_participants.png` / `title_participants_zh.png` — for Participants page
- `title_nature.png`, `title_building.png`, `title_ideas.png`, `title_network.png`, `title_demographic.png`, `title_eduction.png` — for each video category
- `title_about.png`, `title_volunteer.png`, `title_acknowledgement.png`
- `title_-journal.png`, `title_dialogue.png`, `title_diagrams.png`, `title_films.png`, `title_photos.png`, `title_audio.png`

### Step 8: Set Custom Domain

1. In Google Sites, click **Settings** (gear icon)
2. **Custom domain** → enter `www.eskyiu.com`
3. Follow Google's domain verification steps (add CNAME record to your DNS)

### Step 9: Event Photos

Upload event photos from `assets/event-photos/` to the Design Proposals page or a separate Photos page:
- 2010_OCT01 — Ben L, DY, Ag Lin
- 2010_OCT24 — Eric and DEX group
- 2010_OCT26 — Ai Weiwei and Marisa Yiu
- 2010_OCT28 — Ire Tsui Architecture Session
- 2010_OCT31 — BCM YES

## What Still Needs Content

- **About AoD** page — not in WordPress DB, need Eric to provide
- **Volunteer** page — not in WordPress DB, need Eric to provide
- **Acknowledgement** page — not in WordPress DB, need Eric to provide
- **6 videos** still need uploading to YouTube (@ESKYIUhk channel)

## Quick Reference: File Locations

```
wkcdialogues-site/
├── index.html              ← Complete working site (open in browser)
├── MIGRATION-GUIDE.md      ← This file
├── assets/
│   ├── images/             ← 74 title images from WordPress (section headers)
│   ├── uploads/            ← 252 original WordPress images:
│   │                         - Participant portraits (60+)
│   │                         - Home page index collage (16 images)
│   │                         - Category navigation graphics
│   │                         - Logos (6 color variants)
│   │                         - Background images
│   │                         - Pre-workshop photos (6)
│   │                         - Group/collaboration photos
│   │                         - Drawings (Li Chi Ching, Lau Wan Kit)
│   ├── design-proposals/   ← 24 files (PDFs + JPGs from plans.zip)
│   └── event-photos/       ← 5 event photos + 2 AI files
```

## What to Upload to Google Drive for Google Sites

When building the Google Site, upload these to Google Drive first:
1. **All PDFs** from `assets/design-proposals/` (Foster, OMA, Rocco)
2. **All design panel JPGs** from `assets/design-proposals/` (OMA + Rocco panels)
3. **Participant portraits** from `assets/uploads/` — needed for each video page and the participants page
4. **Title images** from `assets/images/` — for each section header
5. **Home page collage images** from `assets/uploads/WKCDialogue_index_*.jpg`
6. **Event photos** from `assets/event-photos/`
7. **Pre-workshop photos** from `assets/uploads/PreWorkshop_*.jpg`
8. **Drawings** from `assets/uploads/li_chi_ching_drawing.jpg` and `jeffrey_lau_wan_kit_drawing.jpg`
9. **Logo** from `assets/uploads/logo_index.png`

## Time Estimate

- Manual Google Sites build: ~2-3 hours (copy-paste for 15 pages)
- PDF/image uploads: ~30 min
- Video embeds: ~45 min (49 videos)
- Domain setup: ~15 min (if DNS access ready)
- **Total: ~3-4 hours**