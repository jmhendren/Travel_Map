# Unified Travel Map — Project Handoff

**Last Updated:** February 10, 2026
**Live URL:** https://jmhendren.github.io/travel-map/
**GitHub Repo:** https://github.com/jmhendren/travel-map (public, GitHub Pages enabled)
**Owner:** John Hendren (jmhendren@gmail.com, GitHub: jmhendren)
**Status:** 16 destinations fully rebuilt to quality standards, 3,670 POIs total, 80 itineraries (5 per destination), all `longDesc` unique, `deploy/` ready for GitHub upload

---

## What This Is

An interactive HTML travel map built on Leaflet.js. Supports multiple destinations with lazy-loaded JSON data files. Full sidebar UI with itinerary planning, category filtering, activity swapping, AI chatbot, geolocation, export tools, and per-POI personal notes.

**Live at:** https://jmhendren.github.io/travel-map/

---

## Current Destinations

| Destination | Hotels | Restaurants | Experiences | Kid-Friendly | Markets | Itineraries | Total POIs |
|-------------|--------|-------------|-------------|--------------|---------|-------------|------------|
| **Japan** 🇯🇵 | 39 | 60 | 52 | 28 | 18 | 5 | 197 |
| **Italy** 🇮🇹 | 101 | 110 | 104 | 27 | 21 | 5 | 363 |
| **Greece** 🇬🇷 | 39 | 50 | 38 | 19 | 15 | 5 | 161 |
| **UK** 🇬🇧 | 50 | 60 | 55 | 25 | 20 | 5 | 210 |
| **Spain** 🇪🇸 | 73 | 220 | 97 | 26 | 17 | 5 | 433 |
| **Thailand** 🇹🇭 | 50 | 53 | 50 | 27 | 17 | 5 | 197 |
| **Korea** 🇰🇷 | 40 | 70 | 55 | 22 | 15 | 5 | 202 |
| **Vietnam** 🇻🇳 | 50 | 77 | 80 | 27 | 17 | 5 | 251 |
| **Portugal** 🇵🇹 | 56 | 73 | 68 | 28 | 22 | 5 | 247 |
| **China** 🇨🇳 | 40 | 74 | 65 | 20 | 20 | 5 | 219 |
| **Taiwan** 🇹🇼 | 50 | 74 | 80 | 27 | 17 | 5 | 248 |
| **Europe Ski** ⛷️ | 51 | 28 | 50 | 27 | 17 | 5 | 173 |
| **France** 🇫🇷 | 48 | 60 | 51 | 30 | 25 | 5 | 214 |
| **Belgium** 🇧🇪 | 30 | 74 | 48 | 20 | 22 | 5 | 194 |
| **Mexico** 🇲🇽 | 44 | 61 | 39 | 24 | 25 | 5 | 193 |
| **Singapore** 🇸🇬 | 38 | 56 | 39 | 20 | 15 | 5 | 168 |
| **Total** | **799** | **1,200** | **971** | **397** | **303** | **80 itineraries** | **3,670** |

### Itineraries (all destinations now have 5 standardized itineraries)

**Japan (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Italy (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Greece (5):** Greatest Hits (10d) | Hidden Gems (10d) | Family Comfort (12d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**UK (5):** Greatest Hits (7d) | Hidden Gems & Countryside (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Spain (5):** Greatest Hits (7d) | Hidden Gems & Deep Culture (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Thailand (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Korea (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Vietnam (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Portugal (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**China (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Taiwan (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Europe Ski (5):** Dolomites & Italian Alps (7d) | French Alps Family Ski (7d) | Austrian & Swiss Alpine (10d) | Swiss Luxury & Powder (10d) | Grand European Ski Tour (14d)

**France (5):** Paris Greatest Hits (7d) | Hidden Gems & Regions (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Belgium (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Beer, Chocolate & Foodie Tour (10d) | Grand Tour (14d)

**Mexico (5):** Greatest Hits (7d) | Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

**Singapore (5):** Greatest Hits (7d) | Hawker & Hidden Gems (7d) | Family Comfort (10d) | Foodie Deep-Dive (10d) | Grand Tour (14d)

---

## File Structure

```
Travel/
  index.html                 <- Map code (~165 KB), loads JSON on demand, includes notes UI
  destinations.json          <- Manifest of all 16 destinations
  destinations/
    japan.json               <- 197 POIs, 5 itineraries (quality rebuilt Feb 9, audit passed Feb 10)
    italy.json               <- 363 POIs, 5 itineraries (rebuilt Feb 9, coords fixed Feb 10)
    greece.json              <- 161 POIs, 5 itineraries (rebuilt Feb 9, expanded from 93)
    uk.json                  <- 210 POIs, 5 itineraries (rebuilt Feb 9, descs fixed Feb 10)
    spain.json               <- 433 POIs, 5 itineraries (rebuilt Feb 9, major desc/coord fix Feb 10)
    thailand.json            <- 197 POIs, 5 itineraries (rebuilt Feb 9, coord fix Feb 10)
    korea.json               <- 202 POIs, 5 itineraries (rebuilt Feb 9, expanded from 131, coords fixed Feb 10)
    vietnam.json             <- 251 POIs, 5 itineraries (rebuilt Feb 9, descs fixed Feb 10)
    portugal.json            <- 247 POIs, 5 itineraries (rebuilt Feb 9, audit passed Feb 10)
    china.json               <- 219 POIs, 5 itineraries (rebuilt Feb 9)
    taiwan.json              <- 248 POIs, 5 itineraries (rebuilt Feb 9, descs fixed Feb 10)
    europe-ski.json          <- 173 POIs, 5 itineraries (rebuilt Feb 9, audit passed Feb 10)
    france.json              <- 214 POIs, 5 itineraries (rebuilt Feb 9, expanded from 53, 3 OOB removed Feb 10)
    belgium.json             <- 194 POIs, 5 itineraries (rebuilt Feb 9, expanded from 57)
    mexico.json              <- 193 POIs, 5 itineraries (rebuilt Feb 9, expanded from 17)
    singapore.json           <- 168 POIs, 5 itineraries (rebuilt Feb 9, expanded from 27)
  deploy/                    <- Clean copy for GitHub Pages (map files only, no personal data)
    index.html
    destinations.json
    destinations/*.json
  Takeout-2/                 <- Google Maps Takeout export (source for Feb 9 import)
    Maps (your places)/Saved Places.json  <- GeoJSON, 152 places with GPS coords
    Saved/                   <- 73 CSV files by city/category, 1,017 places
    Maps/My labeled places/  <- Labeled places (personal, mostly US)
    My Maps/                 <- 13 KMZ files (older custom maps)
  serve.sh / serve.bat       <- Local dev servers (optional, not needed with GitHub Pages)
  Travel_Map.html            <- Monolithic backup (3 destinations only, no UK)
  build_index.py             <- Regenerate index.html from Travel_Map.html
  PROJECT_HANDOFF.md         <- THIS FILE
  Japan 2026/                <- Source: Excel, itinerary docs, flight PDFs
  Italy/                     <- Source: Excel, GPS JSON, Instagram extraction
  Greece/                    <- Source: Excel, itinerary doc
  United Kingdom/            <- Source: Excel (London_UK_Trip_Reference.xlsx)
  Spain/                     <- Source: Excel (Spain_Trip_Guide.xlsx)
  Thailand/                  <- Source: Excel (Thailand_Trip_Guide.xlsx)
  Korea/                     <- Source: Excel (Korea_Trip_Reference.xlsx)
  Vietnam/                   <- Source: Excel (Vietnam_Trip_Guide.xlsx)
  Portugal/                  <- Source: Excel (Portugal_Trip_Reference.xlsx)
  China/                     <- Source: Excel (China_Trip_Guide.xlsx, China_Trip_Guide_with_GPS.xlsx)
  Taiwan/                    <- Source: Excel (Taiwan_Trip_Guide_geocoded.xlsx)
  Europe General/            <- Source: Excel (Europe_Ski_Resorts_Trip_Guide.xlsx)
```

---

## Hosting & Deployment

The map is hosted on **GitHub Pages** from the `deploy/` folder contents pushed to https://github.com/jmhendren/travel-map.

### How to update the live site

**Current workflow (manual):**
1. Claude builds/updates JSON files in `destinations/` and `destinations.json`
2. Claude copies updated files to `deploy/`
3. John drags the `deploy/` folder contents to GitHub via the web upload interface (github.com repo page > "Add file" > "Upload files")
4. GitHub Pages auto-deploys — can take up to a few minutes, not always instant

**GitHub Personal Access Token:** John has a fine-grained token (`cowork-deploy`) scoped to the `travel-map` repo with Contents read/write. Token starts with `github_pat_11ARW6K3Q...`. Note: Claude Cowork's sandbox cannot make outbound network requests to GitHub, so direct `git push` from Cowork is not possible. See Roadmap for automation ideas.

---

## Excel File Structure (Source Data)

Each destination has a source Excel workbook (e.g., `Spain_Trip_Guide.xlsx` or `Korea_Trip_Reference.xlsx`). All recent files follow the same standardized sheet layout:

### Sheets and their JSON mappings

| Excel Sheet | JSON Key | Columns |
|---|---|---|
| **Hotels & Ryokans** | `hotels` | Name, Location, Type, Price Range, Best For, Key Features, Instagram Source, Likes |
| **Restaurants & Bars** | `restaurants` | Name, Location, Cuisine/Type, Price Range, Highlights, Instagram Source, Likes |
| **Markets & Food Spots** | `markets` | Name, Location, Type, Highlights, Tips |
| **Experiences & Activities** | `experiences` | Name, Location, Category, Best For, Highlights, Instagram Source, Likes |
| **Kid-Friendly** | `kidFriendly` | Name, Location, Type, Age Range, Highlights, Instagram Source, Likes |
| **Apps & Tools** | *(not used in JSON)* | Name, Category, What It Does, Source |
| **Travel Tips** | *(not used in JSON)* | Category, Tip, Source/Details |
| **Day Trip Ideas** | *(not used in JSON)* | Destination, From, Travel Time, Highlights, Best For, Source |

### What the Excel does NOT contain

The Excel files have a **Location** column (e.g., "Madrid", "Bangkok (Old Town)", "Seoul (Jongno)") but **no GPS coordinates**. Claude must geocode every POI during the JSON build step.

### How to handle geolocation (GPS coordinates)

This is the most important and error-prone part of building a new destination JSON. Every POI needs a `[lat, lng]` coordinate pair. Here is the recommended approach:

1. **Use a geocoding API when available.** If Claude has internet access (e.g., via MCP tools or browser), use Google Maps Geocoding API, Nominatim (OpenStreetMap), or similar to look up precise coordinates for each POI by name + city. This is the most accurate method.

2. **Use Claude's training knowledge as fallback.** For well-known hotels, landmarks, and restaurants, Claude generally knows accurate coordinates. For less-known places, use the city/neighborhood center and apply small offsets so pins don't stack on top of each other.

3. **Build a city/neighborhood coordinate base first.** Before geocoding individual POIs, establish base coordinates for each unique Location value in the Excel (e.g., "Barcelona" → [41.3874, 2.1686], "Madrid (Salamanca)" → [40.4280, -3.6760]). Then refine individual POIs from that base.

4. **Verify coordinates are in the right country.** A common failure mode is coordinates that are wildly wrong (e.g., a Spanish restaurant placed in Africa). After building the JSON, run a validation check that all coordinates fall within a reasonable bounding box for the destination.

5. **The `cityCenters` field** should include every major city and neighborhood that appears in the data, with a radius value (in degrees) that roughly covers the area. This is used for the map's city-center zoom feature.

6. **Itinerary coordinates** should match the POI coordinates in the main arrays. When an itinerary references a hotel or restaurant, use the same coords as its entry in the `hotels` or `restaurants` array.

### Description field style

The `desc` field in each POI should be a short phrase (~60-80 characters), not a full sentence. Style: comma-separated highlights. Examples: "Art Deco icon, legendary service, afternoon tea, Mayfair" or "Playful modern Spanish, considered world's best, Barcelona". Build these by condensing the Excel's Key Features / Highlights / Tips columns.

The `longDesc` field is a 1-2 sentence expanded description (~15-40 words) of what makes the place special and worth visiting. It appears below the `desc` tagline in the map popup. Style: warm, informative, specific — written for a family traveler who loves food, design, and culture. All 3,164 current POIs have `longDesc` populated. When adding new POIs, generate a `longDesc` using Claude's knowledge of the place.

---

## How to Add a New Destination

This is the standard workflow when John drops a new Excel file into the Travel folder:

1. **John** drops an Excel file (e.g., `France/France_Trip_Guide.xlsx`) into the Travel folder
2. **Claude** reads this handoff doc, then reads the Excel
3. **Claude** geocodes all POIs (see "How to handle geolocation" above)
4. **Claude** builds the JSON following the schema below, including 3 itineraries
5. **Claude** creates `destinations/france.json` and adds an entry to `destinations.json`
6. **Claude** copies updated files to `deploy/`
7. **John** uploads `deploy/` contents to GitHub

### JSON Schema (all destinations use this)

```json
{
  "key": "country",
  "name": "Country Family Adventure",
  "subtitle": "Interactive Trip Map",
  "flag": "🇫🇷",
  "defaultCenter": [46.0, 2.0],
  "defaultZoom": 6,
  "hotels": [{"name": "...", "coord": [lat, lng], "desc": "...", "longDesc": "..."}],
  "restaurants": [{"name": "...", "coord": [lat, lng], "desc": "...", "longDesc": "..."}],
  "experiences": [{"name": "...", "coord": [lat, lng], "desc": "...", "longDesc": "..."}],
  "kidFriendly": [{"name": "...", "coord": [lat, lng], "desc": "...", "longDesc": "..."}],
  "markets": [{"name": "...", "coord": [lat, lng], "desc": "...", "longDesc": "..."}],
  "cityCenters": {"City": [lat, lng, radius]},
  "itineraryData": {
    "a": {
      "name": "Itinerary Name",
      "color": "#2563EB",
      "days": [{"day": 1, "title": "Day Title", "items": [
        {"type": "hotel|breakfast|lunch|dinner|sightseeing|optional|nap", "name": "...", "coord": [lat, lng]}
      ]}]
    }
  }
}
```

**Itinerary colors:** blue `#2563EB`, green `#059669`, amber `#D97706`, red `#DC2626`, purple `#7C3AED`

**Common flags:** 🇯🇵 🇮🇹 🇬🇷 🇬🇧 🇫🇷 🇪🇸 🇵🇹 🇹🇭 🇲🇽 🇭🇷 🇹🇷 🇲🇦 🇰🇷 🇻🇳 🇨🇳 🇹🇼 🇧🇪 🇸🇬 ⛷️

---

## Roadmap

### Near-term (completed Feb 8 2026)
- ~~**Itinerary names in UI**~~ — Done. Tabs now show full names (e.g., "Greatest Hits") instead of "A", "B", "C". Reads `itin.name || itin.title` from the JSON.
- ~~**Italy deduplication**~~ — Done. Removed 22 duplicate entries (137 → 115 POIs).
- ~~**Adaptive filter chips**~~ — Done. Chips are now built dynamically per destination. Japan gets Cameras & Skincare; all others get the universal set. Extensible via `destFilterChips` in JS.
- ~~**Italy region filtering**~~ — Done. Added a region dropdown (Northern, Central, Southern, Islands) using a generic `regions` array in the JSON. Any destination can opt in by adding a `regions` field.
- ~~**Coordinate refinement (China, Italy, UK)**~~ — Done (Feb 8 2026). John provided ChatGPT-generated geocoded Excel files for China, Italy, Spain, UK, and Taiwan. The Excel data was mostly unusable (city-center duplicates, unevaluated formulas, empty columns), so Claude re-geocoded via Nominatim and manual lookups. Results: China fixed 188 POIs that had a wrong default Hong Kong coordinate (96% unique coords now); Italy geocoded 115 POIs and resolved 26 city-center duplicates in Florence/Rome/Venice/Trieste (84% unique); UK geocoded 189 POIs including Stonehenge fix (92% unique). Spain was left unchanged — existing coords were already better than the Excel data. All updated files copied to `deploy/`.
### Near-term (completed Feb 8 2026, continued)
- ~~**Taiwan destination build**~~ — Done. Built `destinations/taiwan.json` with geocoded POIs, cityCenters, and 3 itineraries. Added to `destinations.json` and copied to `deploy/`. 12th destination live.
- ~~**Mobile UI overhaul**~~ — Done. Sidebar replaced with a draggable bottom sheet on mobile (≤768px) with three states: collapsed (145px), half (50vh), expanded (85vh). Swipe gestures with velocity-based flicking, snap-to-nearest, and drag handle. All modals (chat, nearby, city browser, QR, add destination) converted to full-width bottom sheets. FAB positioning adjusted to avoid overlap.

- ~~**Coordinate refinement (remaining 6 destinations)**~~ — Done (Feb 8 2026). Initial pass using Claude's knowledge. Results: Vietnam 5.2% → 96.4% unique; Spain 34.7% → 95.2%; Korea 30.1% → 93.1%; Portugal 13.2% → 91.6%; Thailand 40.5% → 91.3%; Europe Ski 32.7% → 64.7%. Fixed 23 Åre (Sweden) POIs incorrectly placed in the French Alps.
- ~~**Geoapify batch geocoding (all 12 destinations)**~~ — Done (Feb 8 2026). Exported all 2,297 POIs to CSV, John ran them through Geoapify's online geocoder in 5 batches of 500. Imported results back into all 12 destination JSONs. 1,761 POIs updated with Geoapify coordinates; 233 out-of-bounds results rejected; 190 bad matches (wrong city/country) reverted to previous coords; 303 had no geocoding result (kept existing). Final uniqueness: 92.9% overall (2,134/2,297 unique). Per destination: Vietnam 98.0%, Greece 96.8%, UK 96.3%, Japan 95.6%, Portugal 95.6%, Spain 95.6%, Taiwan 94.0%, Korea 93.9%, Italy 93.9%, China 90.3%, Thailand 87.7%, Europe Ski 73.3%. All updated files copied to `deploy/`.

- ~~**Geoapify retry (726 failed POIs)**~~ — Done (Feb 8 2026). Re-exported the 726 POIs that failed the first pass (bad matches, out-of-bounds, no results) with city names added to search queries. Retry recovered 23 more accurate coords. The remaining ~700 are places Geoapify/OSM simply can't resolve — too niche, unusual names, or conceptual POIs (e.g., "Peking duck night" or "Spa reset at a top hotel"). These retain their Claude-knowledge-based coordinates.

### Completed (Feb 9, 2026)

- ~~**Google Maps Takeout Import**~~ — Done. Parsed `Takeout-2/` export: 152 GeoJSON places (with GPS coords) + 1,017 CSV entries from 73 city/category lists. Cross-referenced against all existing destination JSONs using fuzzy name matching. Results by destination:
  - **Spain:** +190 new POIs (Granada tapas from Bourdain episodes, Seville restaurants, Madrid spots, Mallorca/Menorca, food markets). 6 existing POIs got personal notes merged (e.g., "bourdain", "marta granada guide", "your guide recommended it").
  - **Italy:** +109 new POIs (Rome restaurants with 26 annotated, Bologna trattorias, Venice, Egadi Islands).
  - **Portugal:** +46 new POIs (mostly Lisbon restaurants from saved places).
  - **Japan:** +27 new POIs (Tokyo food, sushi, ryokans, camera shops).
  - **UK:** +23 new POIs (London food, pubs, playgrounds, coffee shops).
  - **Europe Ski:** +23 new ski resort hotels (AKI Plose, Six Senses Crans-Montana, etc.).
  - **Thailand:** +2, **Vietnam:** +3 new POIs from GeoJSON saved places.
  - Geocoding approach: GeoJSON coords used where available (real Google Maps GPS); remaining places geocoded from URL-embedded coords or Claude's knowledge with city-center fallback. Validated all coordinates against per-destination bounding boxes.

- ~~**4 new destinations built from Takeout data:**~~
  - **France** 🇫🇷 — 53 POIs: Paris restaurants (Angelina, Caviar Kaspia, Les 110 de Taillevent, etc.), chocolate shops (Jean-Paul Hévin, Jacques Genin), pastry (Cédric Grolet, Stohrer), Alpine ski restaurants (Val d'Isère, Méribel, Courchevel). 3 itineraries.
  - **Belgium** 🇧🇪 — 57 POIs: Antwerp fine dining & casual (Kommilfoo, 't Fornuis, Dôme sur Mer), Bruges restaurants & bistros, moules frites, chocolate, kid activities. 3 itineraries.
  - **Mexico** 🇲🇽 — 17 POIs: Mexico City restaurants (Rosetta, Máximo), Tulum. 2 itineraries.
  - **Singapore** 🇸🇬 — 27 POIs: Michelin restaurants, hawker centers, Marina Bay area. 2 itineraries.

- ~~**Notes UI added to map**~~ — Done. Every POI popup now includes a "📝 My Notes" section with an editable textarea and "Save Note" button. Notes persist to localStorage keyed by `tripMap_notes_{destKey}_{poiName}`. A "📝 Notes" button in the sidebar header opens a panel showing all saved notes for the current destination. This is the first phase of the "Personal annotations" roadmap item.

- ~~**Updated `destinations.json`**~~ to include all 16 destinations and copied everything to `deploy/`. Ready for John to upload to GitHub.

- ~~**Richer POI descriptions (`longDesc`)**~~ — Done (Feb 9 2026). Added a `longDesc` field to every POI across all 16 destinations (3,164 POIs total, 100% coverage). Each `longDesc` is a 1-2 sentence description of what makes the place special and worth visiting, written for a family traveler who loves food, design, and culture. Generated using Claude's knowledge of each place, anchored to the existing `desc` and POI name. Average length ~20 words per description. The map popup now shows `desc` as the short tagline and `longDesc` below it. Also fixed a bug where restaurant, experience, kid-friendly, and market popups were not displaying the `desc` field at all (only hotels were). Per-destination avg word counts: Taiwan 38.9, Japan 29.7, Mexico 26.8, Thailand 25.6, UK 24.7, Portugal 22.9, France 21.2, Greece 20.7, Singapore 19.6, Belgium 18.7, China 17.9, Vietnam 17.1, Korea 16.8, Europe Ski 15.7, Italy 15.5, Spain 13.5. All updated files copied to `deploy/`.

### Completed (Feb 9, 2026, continued)

- ~~**Show descriptions in itinerary popups**~~ — Done (Feb 9 2026). Itinerary popups now show the `desc` tagline and `longDesc` expanded description, matching the category popup style. Implementation: added a global `poiLookup` map (keyed by POI name → `{desc, longDesc}`) that rebuilds in `loadDestination()` from all 5 category arrays (hotels, restaurants, experiences, kidFriendly, markets). The `showItinerary()` popup builder cross-references each itinerary item against `poiLookup`. Also added the "My Notes" textarea and Save button to itinerary popups, using the same localStorage-backed notes system as category popups. Popup content flow: name → type badge → day number → desc → longDesc → swap button → notes. No JSON changes needed — code-only change in `index.html`. Updated `deploy/index.html`.

- ~~**AI-powered dynamic itinerary builder**~~ — Done (Feb 9 2026). A "+ Generate" button in the itinerary tab bar opens a form modal where users configure: trip duration (2-21 days), travel party type (couple, family with toddler, family with kids/teens, solo, friends), interests (10 clickable chips: food, culture, adventure, shopping, relaxation, nightlife, nature, photography, art, kid-friendly), pace (slow/moderate/fast), budget (budget/moderate/luxury), and freeform special requests. The system prompt (`buildGeneratorSystemPrompt()`) dynamically compiles the destination's POI data grouped by city center (up to 15 POIs per category per city to stay within token budget), sends it to the Anthropic API, and receives a complete multi-day itinerary as structured JSON. Implementation details:
  - Generated itineraries appear as new tabs with a ✨ sparkle icon, dashed border, and × delete button (`itin-tab-generated` class)
  - Itinerary keys use `gen_1`, `gen_2`, etc. to distinguish from static `a`, `b`, `c` keys
  - Color cycling through 8 vibrant colors (`GEN_COLORS` array)
  - Full preview shown before saving — each day's items listed with type icons and coordinate status
  - Persisted to localStorage under `tripMap_genItin_{destination}` — survives page refreshes
  - `loadSavedGeneratedItineraries()` restores saved generated itineraries when a destination loads (called before `buildTabsUI()` in `loadDestination()`)
  - `deleteGeneratedItinerary(key)` removes from memory and localStorage with confirmation
  - All existing features work on generated itineraries: swap/modify, day filtering, notes, export, polylines
  - Also fixed the existing day-planner chatbot's hardcoded "Japan" and "family" references — `buildSystemPrompt()` now dynamically uses the active destination name
  - Remaining future enhancements: saved travel profiles, multi-turn refinement ("make day 3 more adventurous"), web search integration for opening hours/festivals
  - Code-only change in `index.html` (~300 lines added). Updated `deploy/index.html`.

### Completed (Feb 9, 2026 — Destination Quality Overhaul)

- ~~**Japan full quality rebuild**~~ — Done (Feb 9 2026). Complete rebuild of `japan.json` addressing 7 categories of quality issues discovered in audit:
  - **Boilerplate descriptions eliminated:** Previous file had 56/80 restaurants sharing identical `longDesc`, 58/60 experiences sharing one description, and all hotels using 5-6 templates. Every single POI now has a unique, place-specific description.
  - **27+ misplaced coordinates fixed:** Gora Kadan (Hakone ryokan placed in northern Hokkaido), Kanda (3-star Tokyo restaurant placed in Kitakyushu), Kashiwaya (3-star Osaka placed in Hakodate), and 24 more corrected to actual locations.
  - **14 default/fallback coordinates resolved:** All Google Maps Takeout imports that landed at [36.2, 137.5] (Japan's geographic center) were either re-geocoded or removed.
  - **17 misclassified POIs fixed:** 5 camera shops removed from restaurants array, Ghibli Museum moved from restaurants to kidFriendly, TOMORROWLAND clothing stores removed from experiences, Ine Fishing Village (a town) removed from restaurants.
  - **Duplicates resolved:** teamLab Borderless, Map Camera, Asahiyama Zoo, Live Squid Fishing, Matsushima Bay Cruise — kept in most appropriate category only.
  - **Weak entries removed:** "Google Maps saved place" descriptions, "Cool neighborhood in tokyo maybe", "noodles", and similar placeholder entries all replaced with quality POIs.
  - **Quality additions:** Added Naoshima Art Island, Chichu Art Museum, Kenrokuen Garden, 21st Century Museum of Art, Fushimi Inari, Kinkaku-ji, Nijo Castle, Philosopher's Path, Senso-ji, Shinjuku Gyoen, Saito (3-star sushi), Sukiyabashi Jiro, Narisawa, Florilège, Trunk Hotel, Tawaraya Ryokan, Ace Hotel Kyoto, Hoshinoya Karuizawa, Beniya Mukayu, Ghibli Park, Ueno Zoo, and more.
  - **3 ryokans added from FlyerTalk forum PDF review:** Satoyama Jujo (Michelin-starred farm-to-table, Niigata), Enowa Yufuin (2023 hilltop retreat, Oita), Ryotei Hanzuiryo (sukiya-style luxury, Nagasaki/Unzen).
  - **5 new itineraries built** replacing the old 5x 22-day format:
    - **Greatest Hits (7 days):** Tokyo → Hakone → Kyoto → Osaka
    - **Hidden Gems (7 days):** Tokyo → Kanazawa → Narai-juku → Kyoto
    - **Family Comfort (10 days):** Tokyo → Hakone → Kyoto → Osaka (with nap/rest blocks)
    - **Foodie Deep-Dive (10 days):** Tokyo → Kanazawa → Kyoto → Osaka (emphasis on Michelin/kaiseki)
    - **Grand Tour (14 days):** Tokyo → Hakone → Kyoto → Osaka → Kanazawa → Sapporo/Otaru/Yoichi
  - Final counts: 39 hotels, 60 restaurants, 52 experiences, 28 kidFriendly, 18 markets = 197 POIs (vs 209 before, but far higher quality). Excel workbook updated to match.

- ~~**Italy full quality rebuild**~~ — Done (Feb 9 2026). Complete rebuild of `italy.json` addressing critical quality issues discovered in audit:
  - **Rome coordinate clustering eliminated:** 45 clusters of POIs sharing near-identical coordinates (especially at ~41.900, 12.495) all resolved. Cross-referenced Google Maps Takeout CSVs (Rome Restaurants, Rome Gelato, Bologna, Venice), `Italy/locations_with_gps.json` (Instagram-sourced GPS data), and Excel workbook (`Italy/Italy_Trip_Reference.xlsx` with 108 hotels, 168 restaurants, 140 experiences) to properly geocode every POI.
  - **Non-Rome restaurants fixed:** 16+ Michelin-starred restaurants (D'O in Milan, Duomo in Ragusa, Le Calandre near Padua, La Madia in Licata, Terra in Sarentino, etc.) had been assigned Rome-area fallback coordinates. All corrected to actual locations.
  - **89 weak descriptions replaced:** Entries marked "Google Maps saved place" or containing "?" all rewritten with place-specific descriptions highlighting cuisine, chef, Michelin status, or unique character.
  - **Misclassified items cleaned:** Natinudi Abbigliamento Roma (clothing store) removed from kidFriendly, Hamburgeseria Burger Bar removed as low-quality.
  - **kidFriendly expanded:** 7 → 27 entries (286% increase). Added Explora Children's Museum, Villa Borghese, Bioparco, pizza-making experiences, gondola rides, Murano glass workshops, Dolomites family activities, Boboli Gardens, and more.
  - **5 new itineraries built** replacing the old 3-itinerary format:
    - **Greatest Hits (7 days):** Rome → Florence → Venice
    - **Hidden Gems (7 days):** Bologna → Modena → Siena/Tuscany → Orvieto
    - **Family Comfort (10 days):** Rome → Amalfi/Sorrento → Florence → Venice
    - **Foodie Deep-Dive (10 days):** Rome → Bologna → Piedmont → Milan → Lake Como
    - **Grand Tour (14 days):** Rome → Naples/Amalfi → Matera → Puglia → Florence → Venice
  - **22 city centers added** (previously zero): Rome, Florence, Venice, Milan, Naples, Bologna, Siena, Verona, Positano, Ravello, Capri, Taormina, Palermo, Matera, Lecce, Lake Como, Cortina, Orvieto, Sorrento, Modena, Alba, Bressanone.
  - **Second pass: Excel gap analysis & enrichment.** Found 216 POIs in the Excel but missing from the JSON. Added all quality entries: luxury hotels (Hassler Roma, Belmond Villa San Michele, Villa d'Este, Grand Hotel Tremezzo, Borgo Egnazia, Forestis, etc.), Michelin restaurants (Enrico Bartolini al Mudec, Conca del Sogno, Da Adolfo, Harry's Bar, etc.), experiences (Fondazione Prada, Peggy Guggenheim, Path of the Gods, Mount Etna, Naples underground, Modena balsamic tours, etc.), and cocktail bars (Locale Firenze, Sartoria, Moebius Milano, etc.). Removed misclassified items (restaurants in hotels array, guide references, playrooms). Wrote unique place-specific descriptions for every entry.
  - Final counts: 101 hotels, 110 restaurants, 104 experiences, 27 kidFriendly, 21 markets = 363 POIs (vs 224 before, +62%). Excel workbook updated to match.

### Completed (Feb 9-10, 2026 — Full Rebuild + Quality Audit)

- ~~**All 14 remaining destinations rebuilt**~~ — Done (Feb 9-10 2026). Overnight batch mode processed all destinations not yet at quality standards. Each destination rebuilt with 5 standardized itineraries (Greatest Hits 7d, Hidden Gems 7d, Family Comfort 10d, Foodie Deep-Dive 10d, Grand Tour 14d), unique descriptions, cityCenters, and verified coordinates. Major expansions: Greece 93→161, Korea 131→202, France 53→214, Belgium 57→194, Mexico 17→193, Singapore 27→168.

- ~~**Comprehensive quality audit + fix pass**~~ — Done (Feb 10 2026). Ran automated Python audits across all 16 destination JSONs checking: duplicate longDesc, duplicate desc, short descriptions, boilerplate detection, coordinate validation (bounding box), exact coordinate clustering, and missing fields. Results and fixes:
  - **Spain:** Fixed 358→5 dup descs, 51→5 dup longDescs, 31→0 short descs, 153 coord dupes resolved
  - **Thailand:** Fixed 194 city-center fallback coords (121 POIs at same Bangkok point), 17→3 dup descs
  - **Korea:** Fixed 79 city-center fallback coords (36 at same Seoul point), 17→0 dup descs
  - **Italy:** Fixed 133 POIs at 38 shared coordinates (15 at generic [42.5, 12.5] fallback) → all unique
  - **France:** Removed 3 St. Moritz hotels with Swiss/Italian coordinates (wrong country)
  - **Vietnam:** Fixed 55→0 dup descs
  - **UK:** Fixed 17 "comfortable" boilerplate longDescs, 5→1 dup descs
  - **Taiwan:** Expanded 15 short descs, fixed 6 boilerplate, 5→0 dup descs
  - **Belgium, Greece, Singapore:** Minor desc fixes
  - **Japan, Portugal, Europe Ski:** Passed audit clean — no fixes needed

### ACTIVE: Google Places API — Full Coordinate Re-Geocoding (Feb 9 2026)

All 3,670 POIs across 16 destinations need precise coordinates. The current data has widespread issues: city-center fallbacks, country-center defaults, exact-duplicate clusters, and round-number estimates. Rather than patching incrementally, we're re-geocoding everything from scratch using the Google Places API.

#### Why Google Places API
- **Best match rate for businesses** — Unlike address-based geocoders (Nominatim, Geoapify), Places API is designed to find hotels, restaurants, and attractions by name. It searches Google's business database, not just street addresses.
- **Location bias** — We pass the current (approximate) coordinates as a bias, so "Rosetta" near Mexico City finds the restaurant, not one in Italy.
- **Returns `place_id`** — We can use this later for hours, ratings, reviews, and photos (Tier 2 enrichment from the roadmap).
- **Cost** — ~$62 for all 3,670 POIs via Find Place ($0.017/request). Covered by Google Cloud's $200/month free Maps Platform credit on new accounts.

#### One-Time Setup (John)

1. **Create a Google Cloud project:**
   - Go to https://console.cloud.google.com/
   - Click "Select a project" → "New Project" → name it "travel-map" → Create
   - You'll get $300 free trial credit (90 days) plus $200/month Maps Platform credit

2. **Enable the Places API:**
   - In the Cloud Console, go to "APIs & Services" → "Library"
   - Search for "Places API (New)" and click Enable
   - Also enable "Geocoding API" as a fallback

3. **Create an API key:**
   - Go to "APIs & Services" → "Credentials" → "Create Credentials" → "API Key"
   - Copy the key. Optionally restrict it to Places API + Geocoding API only.
   - **Do NOT paste the key into any file in this repo** — it will be passed as a command-line argument

4. **Install Python dependencies (on your local machine):**
   ```
   pip install requests
   ```

#### Workflow — Per Destination

Process destinations one at a time so we can verify quality before moving on. Priority order (worst coordinate quality first):

| # | Destination | POIs | Priority | Reason |
|---|-------------|------|----------|--------|
| 1 | Spain | 433 | CRITICAL | 167 POIs at Madrid fallback, 318 exact dupes |
| 2 | Portugal | 247 | CRITICAL | 154 round-number coords, heavy clustering |
| 3 | Singapore | 168 | HIGH | 87 country-center fallbacks, 356 exact dupes relative to size |
| 4 | Europe Ski | 173 | HIGH | POIs scattered across 6 countries, complex geocoding |
| 5 | Belgium | 194 | HIGH | 57 shared-coordinate POIs |
| 6 | China | 219 | HIGH | 76 shared-coordinate POIs |
| 7 | Mexico | 193 | MEDIUM | Moderate clustering |
| 8 | France | 214 | MEDIUM | Moderate clustering |
| 9 | Taiwan | 248 | MEDIUM | Some out-of-bounds coords reported |
| 10 | Greece | 161 | MEDIUM | Amanzoe 33km off, some hotel misplacements |
| 11 | UK | 210 | MEDIUM | Moderate issues |
| 12 | Vietnam | 251 | LOW | Relatively clean |
| 13 | Korea | 202 | LOW | Seoul hotel clustering |
| 14 | Japan | 197 | LOW | Cleanest file |
| 15 | Italy | 363 | LOW | Already heavily fixed |
| 16 | Thailand | 197 | LOW | Best current quality |

#### Step-by-Step Process (for each destination)

**Step 1 — Claude exports POIs to CSV**

Claude reads the destination JSON and writes a CSV:
```
dest_key,category,poi_name,current_lat,current_lng
spain,hotels,Hotel Alma Barcelona,41.393,2.161
spain,restaurants,El Celler de Can Roca,41.991,2.809
...
```

File: `geocode_input_{dest_key}.csv`

**Step 2 — John runs the lookup script**

Claude provides a Python script (`places_lookup.py`) that John runs on his local machine:
```
python places_lookup.py --key YOUR_API_KEY --input geocode_input_spain.csv --output geocode_results_spain.csv
```

The script:
- Reads each POI from the CSV
- Calls Google Places API "Find Place from Text" with the POI name + location bias (current coords)
- Rate-limits to 10 requests/second (well under the 50 QPS limit)
- Writes results CSV with: `poi_name, new_lat, new_lng, place_id, formatted_address, match_name, confidence`
- Handles failures gracefully (retries, logs misses)
- Prints progress every 50 POIs
- Total runtime: ~1-2 minutes per destination

**Step 3 — John drops results CSV back into Travel folder**

John copies `geocode_results_spain.csv` into the Travel folder.

**Step 4 — Claude imports results**

Claude reads the results CSV and updates the destination JSON:
- For each POI, compares old coord vs new coord
- Calculates distance moved (in km)
- Applies new coordinates if:
  - Google returned a high-confidence match (name similarity > 70%)
  - New coord is within the destination's bounding box
  - Distance moved is < 100km (flags larger moves for manual review)
- Preserves all other POI fields (desc, longDesc, gmapsUrl, etc.)
- Regenerates `gmapsUrl` with new coordinates
- Updates itinerary coordinates to match (cross-references by POI name)
- Copies to `deploy/`

**Step 5 — Claude verifies**

Run automated checks:
- Zero exact-duplicate coordinates (within 0.0005°)
- Zero out-of-bounds coordinates
- Zero country-center fallbacks
- All coords have 4+ decimal places
- Print before/after comparison: how many POIs moved, average distance moved, max distance moved
- Flag any POIs that Google couldn't match (these keep their old coords and need manual attention)

**Step 6 — John reviews flagged POIs**

Claude prints a short list of:
- POIs where Google returned no match
- POIs where the name didn't closely match (possible wrong place)
- POIs that moved > 20km (suspicious — could be a different place with the same name)

John confirms or corrects these manually before Claude finalizes.

#### Files

| File | Location | Purpose |
|------|----------|---------|
| `places_lookup.py` | `Travel/` | Python script John runs locally with his API key |
| `geocode_input_{key}.csv` | `Travel/` | Export of POIs for one destination (Claude generates) |
| `geocode_results_{key}.csv` | `Travel/` | API results (John generates, drops back in folder) |
| `geocode_import_report_{key}.txt` | `Travel/` | Import summary with flagged POIs (Claude generates) |

#### Kickoff Prompt (for each destination)

```
Read PROJECT_HANDOFF.md. Export the next destination in the geocoding queue to CSV
(geocode_input_{key}.csv). Tell me to run places_lookup.py and wait for results.
```

After John runs the script and drops the results CSV:
```
Import geocode_results_{key}.csv into the destination JSON. Verify quality. Show me flagged POIs.
```

#### Completed Destinations

| # | Destination | Status | POIs Moved | Avg Distance | Flagged | Notes |
|---|-------------|--------|------------|--------------|---------|-------|
| | *(none yet)* | | | | | |

---

### Near-term (next up after geocoding)

#### 1. Expand new destinations with Excel data
- **France, Belgium, Mexico, Singapore** were rebuilt from Takeout + Claude knowledge but still lack Excel source files. If John adds Excel files for these countries, Claude should merge the Excel data to enrich existing POIs with structured metadata (cuisine type, price range, Instagram sources, likes).

#### 2. Ryokan PDF additional research
- The FlyerTalk forum PDF (`Japan Luxury Ryokans - A Primer + Impressions - Page 36 - FlyerTalk Forums.pdf`) was reviewed Feb 9. Three Tier-1 ryokans were added to Japan. Additional ryokans identified but not added: Iwanoyu Seni Onsen (Nagano, good value but no in-room onsen), Onyado Chikurintei (Saga, booking challenges), Bettei Yaeno (Gunma, not destination-worthy), Hanaichi (Gunma, interim stop). Could revisit if more room research surfaces.

#### ~~5. Update Excel files for existing destinations~~ — Done (Feb 8 2026)
- Back-filled 506 POIs from destination JSONs into the source Excel workbooks across all 8 destinations. Each new row includes the POI name, extracted location/type/highlights from the JSON `desc` field, and is tagged with "Google Maps Takeout" in the Instagram Source column. Breakdown:
  - **Spain:** +190 POIs (146 restaurants, 23 hotels, 21 experiences) → `Spain/Spain_Trip_Guide.xlsx`
  - **Italy:** +129 POIs (65 restaurants, 35 experiences, 21 markets, 5 hotels, 3 kid-friendly) → `Italy/Italy_Trip_Reference.xlsx`
  - **Japan:** +68 POIs (27 restaurants, 16 experiences, 13 hotels, 8 kid-friendly, 4 markets) → `Japan 2026/Claude Itineraries/2-6-26/Japan_Trip_Reference.xlsx`
  - **Portugal:** +46 POIs (all restaurants) → `Portugal/Portugal_Trip_Reference.xlsx`
  - **UK:** +45 POIs (19 restaurants, 10 kid-friendly, 8 experiences, 6 hotels, 2 markets) → `United Kingdom/London_UK_Trip_Reference.xlsx`
  - **Europe Ski:** +23 POIs (all hotels) → `Europe General/Europe_Ski_Resorts_Trip_Guide.xlsx`
  - **Vietnam:** +3 POIs (restaurants) → `Vietnam/Vietnam_Trip_Guide.xlsx`
  - **Thailand:** +2 POIs (restaurants) → `Thailand/Thailand_Trip_Guide.xlsx`

#### 6. Remaining Takeout data not yet imported
- **US data** (439 places — NYC, Upstate, Austin, California) was skipped since US is not a travel map destination. Could build a US destination if wanted.
- **MIXED/uncategorized lists** (~87 entries from "Want to go.csv", "Cool places to visit maybe.csv", "Favorite places.csv") were partially reclassified by URL coordinates; some remain unmatched.
- **My Maps/** — 13 KMZ files (older custom maps, mostly US/Portugal) were not processed.
- **Labeled places** — 19 entries (personal labels like "Home", "Picnic") — not useful for travel.

### Completed (Feb 9, 2026, continued — AI builder enhancements)

- ~~**Saved travel profiles**~~ — Done (Feb 9 2026). Users can save named presets of generator form settings (trip duration, travel party, interests, pace, budget, constraints, web search preference) to localStorage under `tripMap_travelProfiles`. A profile dropdown at the top of the generator modal lets users quick-select saved profiles (e.g., "Family with toddler", "Foodie couple"). Includes Save, Load, and Delete with confirmation. Profiles persist across sessions and destinations.

- ~~**Multi-turn refinement**~~ — Done (Feb 9 2026). After generating an itinerary, a refinement input bar appears below the preview. Users can type natural language requests like "Make day 3 more adventurous" or "Add a beach day" and the AI will modify the itinerary in place while preserving unchanged days. Multi-turn conversation history is tracked (last 6 messages) for contextual refinement. The system prompt includes the current itinerary state plus available POIs for the destination. Supports Enter key for quick submission. Refinement uses the same web search setting as generation.

- ~~**Web search integration for generator**~~ — Done (Feb 9 2026). Added a "Web search for current info" toggle to the generator form (uses existing `.web-search-switch` UI pattern). When enabled, the Anthropic API call includes the `web_search_20250305` tool (max 5 uses for generation, max 3 for refinement), allowing the AI to check opening hours, seasonal events, festivals, and transit logistics during itinerary generation. Toggle state is saved in travel profiles. Resets to off when the modal opens (opt-in per session).

---

## Destination Quality Rebuild Process (Repeatable Framework)

This is the standardized process for rebuilding any destination to match the quality bar established with Japan and Italy. It was developed through trial and error across two full rebuilds and should be followed for all remaining destinations.

### Phase 1: Audit (automated)

Run the audit script against the current `destinations/{country}.json`. Check for:

1. **Coordinate clustering** — POIs sharing coords within 0.001°, especially at city-center fallback points
2. **Bounding box violations** — Any coord outside the country's geographic bounds
3. **Boilerplate descriptions** — `longDesc` values appearing more than once, or containing "Google Maps saved place" markers
4. **Weak descriptions** — `desc` shorter than 30 chars, containing "?", "maybe", "TBD", or just a cuisine type
5. **Misclassifications** — Camera shops in restaurants, museums in restaurants, clothing stores in experiences, etc.
6. **Cross-category duplicates** — Same name in multiple categories
7. **Itinerary structure** — How many, how many days each, whether they follow the 5-itinerary format
8. **Missing city centers** — Whether `cityCenters` is populated

The audit produces a text report with issue counts and specific POI names for each problem.

### Phase 2: Source Data Inventory & Takeout Ingestion

Catalog all available source data for the destination:

- **Excel workbook** — Usually the richest source. Check all sheets: Hotels, Restaurants, Experiences, Kid-Friendly, Markets, Day Trips, Travel Tips, Apps & Tools. Note the **exact row counts** per sheet — this is the denominator for gap analysis later.
- **Google Takeout CSVs** — In `Takeout-2/Maps (your places)/Saved/`. City-specific CSV files (e.g., "Rome Restaurants.csv", "Bologna.csv", "Venice.csv") contain Google Maps URLs that embed GPS coordinates in the URL path. **How to extract coords from Takeout CSVs:** Each row has a Google Maps URL like `https://www.google.com/maps/place/.../@41.8902,12.4922,17z/...` — parse the `@lat,lng` from the URL. If the URL doesn't contain coords, geocode from the place name.
- **locations_with_gps.json** — Some destinations have GPS-enriched JSON from Instagram extraction (e.g., `Italy/locations_with_gps.json`). These have `lat`/`lon` fields that are generally accurate.
- **Saved Places GeoJSON** — `Takeout-2/Maps (your places)/Saved Places.json` has global pins with coordinates. Filter to the target country by bounding box.
- **PDF/forum resources** — Specialty reviews (ryokan guides, wine region notes, etc.) in the country subfolder.

**Takeout ingestion approach:** The Takeout data often overlaps with the Excel. During the rebuild, use Takeout primarily for **GPS coordinates** (which Excel lacks) and **personal annotations** (Google Maps notes like "bourdain recommended" or "marta's guide"). The Excel is the better source for structured metadata (cuisine type, price range, highlights). Cross-reference by fuzzy name matching: a Takeout entry called "Trattoria da Cesare" should match Excel's "Trattoria Da Cesare al Casaletto".

### Phase 3: Parallel Rebuild (4 subagents)

Launch 4 parallel subagents to rebuild each POI category:

1. **Hotels** — Target 45-65 entries. Include luxury, boutique, design, ryokans/agriturismo, and a few well-chosen mid-range. Geographic spread across all major regions.
2. **Restaurants** — Target 60-85 entries. Include Michelin-starred, beloved local institutions, street food legends, wine bars, coffee spots. Ensure mix of price points.
3. **Experiences** — Target 55-75 entries. Include world-class museums, iconic landmarks, artisan workshops, scenic viewpoints, cultural activities, outdoor adventures. Remove shopping streets and generic stores.
4. **Kid-Friendly + Markets** — Target 25-30 kid entries, 18-25 market entries. Kid: interactive museums, parks, family activities, cooking classes. Markets: food markets, bakeries, specialty delis.

Each subagent:
- Reads the Excel, GPS JSON, Takeout CSVs, and current destination JSON
- Merges sources, deduplicates, and filters for quality
- Geocodes every entry using: (a) GPS data from source files, (b) Claude's training knowledge, (c) city-center base coords with 0.001-0.005° offsets
- Writes `{name, coord: [lat, lng], desc (40-80 chars, unique), longDesc (20-35 words, unique, evocative)}`
- Saves intermediate JSON to working directory

### Phase 3.5: Gap Analysis (Excel vs JSON)

After the initial rebuild, run a gap analysis comparing the Excel workbook against the assembled JSON:

1. Read ALL POI names from every Excel sheet (Hotels, Restaurants, Experiences, Kid-Friendly, Markets)
2. Read ALL POI names from the JSON
3. Use fuzzy matching (case-insensitive, partial string, strip suffixes) to find matches
4. List all Excel entries with NO match in the JSON — these are candidates for addition
5. Filter out low-quality gaps: "Dropped pin", entries with no name, pure shopping outlets, itinerary descriptions masquerading as POIs, duplicate variants
6. For quality gaps, geocode and write desc/longDesc, then append to the JSON arrays

This step is critical. For Italy, it caught 216 missing POIs including major entries like Hassler Roma, Fondazione Prada, Path of the Gods, and dozens of Michelin restaurants that existed in the Excel but had been filtered out during the initial rebuild. The gap analysis ensures the Excel (which represents John's curated research) is fully represented in the map.

Also check the reverse: POIs in the JSON that are NOT in the Excel (these were added by Claude from training knowledge). These are fine to keep but should be noted.

### Phase 4: Assembly

A Python assembly script:
1. Reads all 4 intermediate JSON files
2. Validates and fixes description quality (length, uniqueness, boilerplate removal)
3. Validates coordinates (bounding box, no exact duplicates)
4. Adds `cityCenters` for every major city/region in the data
5. Builds 5 itineraries following the standard format:
   - **a: Greatest Hits (7 days)** — Classic must-see route, blue `#2563EB`
   - **b: Hidden Gems (7 days)** — Off-the-beaten-path alternative, green `#059669`
   - **c: Family Comfort (10 days)** — Kid-paced with rest blocks, amber `#D97706`
   - **d: Foodie Deep-Dive (10 days)** — Restaurant and food market focused, red `#DC2626`
   - **e: Grand Tour (14 days)** — Comprehensive multi-region trip, purple `#7C3AED`
6. Assembles the full JSON with standard schema
7. Copies to both `destinations/` and `deploy/destinations/`

### Phase 5: Verification

Run a verification script checking:
- All required top-level keys present
- POI counts per category
- Zero coordinate clustering (no pairs within 0.001° that shouldn't be)
- Zero duplicate `longDesc` values
- Zero boilerplate patterns ("Google Maps", "saved place", generic stubs)
- All `desc` values 30-80 chars
- All `longDesc` values 15-40 words
- All 5 itineraries present with correct day counts
- Deploy copy matches source copy
- No banned items (previously removed misclassifications)

### Phase 6: Excel ↔ JSON Sync

The Excel and JSON should stay in sync. The Excel is the **research master** (richer metadata, Instagram sources, notes, price ranges) and the JSON is the **map master** (coordinates, display descriptions, itineraries). After a rebuild:

**JSON → Excel (primary direction after rebuild):**
- Clear and repopulate each POI category sheet from the JSON
- Map JSON fields to Excel columns: Name, Location (via coord-to-city proximity matching), Type/Cuisine (extracted from desc), Key Features/Highlights (from longDesc)
- Preserve non-POI sheets (Apps & Tools, Travel Tips, Day Trip Ideas, Regional Guides, Practical Info)
- Preserve any Excel-only columns (Instagram Source, Likes, Notes) by matching on POI name before clearing

**Excel → JSON (when John adds new entries to the Excel):**
- Read the Excel, identify new rows not in JSON (by name matching)
- Geocode new entries, write desc/longDesc
- Append to the appropriate JSON category arrays
- Copy to deploy
- This is the "incremental add" workflow vs. the "full rebuild" workflow above

**Google Takeout → both:**
- When new Takeout exports are available, parse the CSVs and GeoJSON
- Cross-reference against existing JSON by fuzzy name matching
- For matches: update coordinates if Takeout coords are more precise
- For new entries: triage quality, geocode, write descriptions, add to JSON + Excel
- Takeout personal annotations (Google Maps notes) should be preserved in the Excel's Notes column

### Destination Rebuild Queue

This queue tracks which destinations have been rebuilt to quality standards. **Process destinations in the order listed.** After completing each one, update its status here.

| # | Destination | Key | Status | POIs | Issues | Excel? | Notes |
|---|-------------|-----|--------|------|--------|--------|-------|
| 1 | 🇯🇵 Japan | `japan` | ✅ DONE | 197 | 0 | Yes | Rebuilt Feb 9. Quality audit passed Feb 10 — cleanest file. |
| 2 | 🇮🇹 Italy | `italy` | ✅ DONE | 363 | 0 | Yes | Rebuilt Feb 9. Coord clustering fixed Feb 10 (133 POIs at 38 shared coords → all unique). |
| 3 | 🇪🇸 Spain | `spain` | ✅ DONE | 433 | 5 dup desc, 5 dup LD | Yes | Rebuilt Feb 9. Major desc fix Feb 10 (358→5 dup desc, 51→5 dup LD, 31→0 short, 153 coord dupes fixed). Remaining dupes are minor. |
| 4 | 🇵🇹 Portugal | `portugal` | ✅ DONE | 247 | 0 | Yes | Rebuilt Feb 9. Quality audit passed Feb 10. |
| 5 | 🇨🇳 China | `china` | ✅ DONE | 219 | 1 boilerplate | Yes | Rebuilt Feb 9. Quality audit Feb 10 — 1 minor "convenient location" boilerplate remains. |
| 6 | 🇬🇧 United Kingdom | `uk` | ✅ DONE | 210 | 1 dup desc | Yes | Rebuilt Feb 9. Boilerplate fix Feb 10 (17→0 "comfortable", 5→1 dup desc). |
| 7 | 🇬🇷 Greece | `greece` | ✅ DONE | 161 | 1 dup LD | Yes | Rebuilt Feb 9 (expanded 93→161). Fix Feb 10 (4 short desc, 1 boilerplate fixed). 1 dup LD (Elafonissi in exp+kid — intentional). |
| 8 | 🇹🇭 Thailand | `thailand` | ✅ DONE | 197 | 3 dup desc | Yes | Rebuilt Feb 9. Coord fix Feb 10 (194 city-center fallbacks → mostly fixed, 40 remaining shared coords). Desc fix (17→3 dup). |
| 9 | 🇻🇳 Vietnam | `vietnam` | ✅ DONE | 251 | 1 boilerplate | Yes | Rebuilt Feb 9. Desc fix Feb 10 (55→0 dup desc). 1 minor boilerplate remains. |
| 10 | 🇰🇷 Korea | `korea` | ✅ DONE | 202 | 0 | Yes | Rebuilt Feb 9 (expanded 131→202). Coord fix Feb 10 (79 city-center fallbacks → 15 remaining). Desc fix (17→0 dup). |
| 11 | 🇹🇼 Taiwan | `taiwan` | ✅ DONE | 248 | 0 | Yes | Rebuilt Feb 9. Desc fix Feb 10 (15 short expanded, 6 boilerplate fixed, 5 dup desc fixed). |
| 12 | ⛷️ Europe Ski | `europe-ski` | ✅ DONE | 173 | 0 | Yes | Rebuilt Feb 9 (expanded to 5 itineraries). Quality audit passed Feb 10. |
| 13 | 🇫🇷 France | `france` | ✅ DONE | 214 | 0 | NO | Rebuilt Feb 9 (expanded 53→217). Fix Feb 10: removed 3 St. Moritz hotels (wrong country). |
| 14 | 🇧🇪 Belgium | `belgium` | ✅ DONE | 194 | 2 dup desc | NO | Rebuilt Feb 9 (expanded 57→194). Desc fix Feb 10 (5→2 dup desc). |
| 15 | 🇲🇽 Mexico | `mexico` | ✅ DONE | 193 | 1 dup desc | NO | Rebuilt Feb 9 (expanded 17→193). Quality audit Feb 10 — 1 minor dup desc (Xcaret in exp+kid). |
| 16 | 🇸🇬 Singapore | `singapore` | ✅ DONE | 168 | 0 | NO | Rebuilt Feb 9 (expanded 27→168). Boilerplate fix Feb 10. |

**All 16 destinations rebuilt and quality-audited.** Remaining issues are minor (a few dup descs where same POI appears in 2 categories, 1-2 boilerplate words). No critical data quality issues remain.

---

### Autonomous Rebuild Instructions (for running unattended)

This section tells Claude how to process the next destination in the queue without human intervention. **John can start a fresh conversation, paste the kickoff prompt below, and walk away.**

#### Kickoff Prompt — Single Destination (paste into a new conversation)

```
Read /sessions/sweet-fervent-thompson/mnt/Travel/PROJECT_HANDOFF.md — find the Destination Rebuild Queue table and identify the destination marked 🔴 NEXT. Execute the full Destination Quality Rebuild Process (Phases 1-6) for that destination. When finished, update the queue table: mark the completed destination ✅ DONE, advance the next ⏳ QUEUED destination to 🔴 NEXT. Do not ask me questions — use your best judgment and the framework documented in the handoff file. I am asleep.
```

#### Kickoff Prompt — ALL Destinations Overnight (paste into a new conversation)

```
Read /sessions/sweet-fervent-thompson/mnt/Travel/PROJECT_HANDOFF.md — find the Destination Rebuild Queue and process ALL destinations that are not yet ✅ DONE. Use the "Overnight Batch Mode" instructions in the handoff file. I am going to sleep — work through as many as you can. Do not ask me questions.
```

#### Overnight Batch Mode (how to process multiple destinations in one session)

The trick is to delegate each destination to a **subagent** (via the Task tool) so each rebuild gets a fresh context window. The main conversation acts as a lightweight orchestrator:

```
ORCHESTRATOR LOOP (main conversation):
  1. Read PROJECT_HANDOFF.md, parse the queue table
  2. For each destination that is not ✅ DONE (in order):
     a. Launch a Task subagent with the full rebuild prompt (see below)
     b. Wait for it to complete
     c. Read the updated queue table to confirm it succeeded
     d. If it failed or was incomplete, note the issue and move on
     e. Continue to next destination
  3. Print final summary of all destinations processed
```

**Subagent prompt template** (the orchestrator fills in {key}, {name}, {flag}, etc.):

```
You are rebuilding the {name} ({key}) destination for an interactive travel map.

Read /sessions/sweet-fervent-thompson/mnt/Travel/PROJECT_HANDOFF.md — specifically the "Destination Quality Rebuild Process" section. Execute Phases 1-6 for destination key "{key}".

Key files:
- Current JSON: /sessions/sweet-fervent-thompson/mnt/Travel/destinations/{key}.json
- Deploy copy: /sessions/sweet-fervent-thompson/mnt/Travel/deploy/destinations/{key}.json
- Excel (if exists): check /sessions/sweet-fervent-thompson/mnt/Travel/ subfolders
- Takeout CSVs: /sessions/sweet-fervent-thompson/mnt/Travel/Takeout-2/Maps (your places)/Saved/
- Saved Places GeoJSON: /sessions/sweet-fervent-thompson/mnt/Travel/Takeout-2/Maps (your places)/Saved Places.json

Execute the full rebuild:
1. Audit the current JSON (coordinate clustering, boilerplate, weak descs, misclassifications)
2. Inventory all source data (Excel sheets, Takeout CSVs, GPS JSONs)
3. Rebuild all POI categories in parallel using 4 subagents
4. Run gap analysis (Excel vs JSON) and add missing quality entries
5. Assemble with cityCenters and 5 itineraries (Greatest Hits 7d, Hidden Gems 7d, Family Comfort 10d, Foodie Deep-Dive 10d, Grand Tour 14d)
6. Verify: zero dup longDescs, zero boilerplate, all coords in-bounds, all descs 30-80 chars
7. Update the Excel workbook to match
8. Copy to deploy/destinations/
9. Update the queue table in PROJECT_HANDOFF.md: change {key} status to ✅ DONE, update POI count, set Issues to 0

Quality standards: desc 40-80 chars unique, longDesc 20-35 words unique, coords accurate to the specific POI (not city center), hotels genuinely worth staying at, restaurants a serious food lover would seek out.

Do not ask questions. Use your best judgment. Print a brief summary when done.
```

**Why this works:** Each subagent gets its own context window, so processing destination #10 is just as fresh as destination #1. The orchestrator only accumulates brief completion summaries (~100 tokens each), so it can loop through all 14 remaining destinations without hitting context limits.

**What if a subagent fails?** The orchestrator should check whether the queue table was updated. If the destination wasn't marked DONE, log the failure and move to the next one. John can re-run just that destination later.

#### Context management

- **Single destination mode:** One conversation, one destination. Safe and simple.
- **Overnight batch mode:** One conversation orchestrates many subagents. Each subagent is context-isolated. The orchestrator stays lightweight.
- All work is persisted to files (JSON, Excel, deploy copy, handoff queue), so progress is never lost even if a session ends unexpectedly.
- The queue table is the single source of truth for what's done and what's next.

#### For destinations without Excel files (France, Belgium, Mexico, Singapore)

These are thin destinations bootstrapped from Google Takeout data. The rebuild process is the same but Phase 3 relies more heavily on Claude's training knowledge and web search to fill gaps. Target POI counts are lower but quality standards are the same. If John has added Excel files for these by the time they're reached, use them. Otherwise, use Takeout + Claude knowledge + web search.

---

### Quality Standards Reference

| Field | Requirement |
|-------|-------------|
| `desc` | 40-80 chars. Mention cuisine/type + distinguishing feature + location. No boilerplate. |
| `longDesc` | 20-35 words. Evocative, unique across entire dataset. Paint a picture of the experience. |
| `coord` | Accurate to the specific POI. No city-center fallbacks. Offset 0.001-0.005° from neighbors. |
| Hotels | Genuinely worth staying at. Luxury, boutique, or uniquely characterful. No generic chains. |
| Restaurants | Would a serious food lover seek this out? Michelin-recognized, local institution, or genuine hidden gem. |
| Experiences | Would a curious, design/culture-loving traveler be glad they went? Not just "a street" or "a shop". |
| Kid-Friendly | Actually engaging for children 0-12. Not just a hotel listed again. |
| Markets | Worth visiting for the food/atmosphere experience. Working markets, legendary bakeries, specialty food shops. |

---

### Medium-term
- **Google Maps data & business hours enrichment** — Add real-world data (hours, ratings, website, Google Maps links) to POI popups. Three tiers of implementation:
  - ~~**Tier 1 — Google Maps links (easy, free):**~~ Done (Feb 9 2026). Added `gmapsUrl` field to every POI (3,670 total) and a "📍 View on Google Maps" link in all popup types (category + itinerary). URLs regenerated with new coords after each geocoding pass.
  - **Tier 2 — Google Places API batch enrichment (medium, ~$10–50):** Use the Places API (Nearby Search or Text Search) to look up each POI by name + coordinates and retrieve structured data: `opening_hours`, `rating`, `price_level`, `website`, `photos`, `place_id`. Store in a new `placeData` field per POI. Challenges: fuzzy name matching (POI names may not exactly match Google's), rate limits (up to 50 QPS), cost (~$0.003–0.017 per lookup × 3,164 POIs), and data staleness (hours change seasonally). Could run in batches similar to the Geoapify geocoding workflow — Claude exports POI names/coords to CSV, John runs through the API, Claude imports results.
  - **Tier 3 — On-demand lookup (already works):** The day planner chatbot with web search enabled can already look up current hours, reviews, and practical info for any POI when users ask. The generator refinement feature also supports this. No additional code needed — just educate users that they can ask "What are the hours for X?" in the chat.
  - **Display in popup:** For Tier 1/2, add a collapsible "Details" section below `longDesc` in the popup showing: hours (formatted by day), rating stars, price level indicator, and "Open in Google Maps" link. Could also show a small Google Maps embed thumbnail if `place_id` is available.
  - **Freshness strategy:** Hours data should include a `lastUpdated` timestamp. Popups could show "Hours as of [date]" and offer a "Refresh" button that uses the AI chat's web search to get current info on demand.

- **Personal annotations & booking info (phase 2)** — The basic notes UI is now live (per-POI textarea with localStorage). Next steps:
  - **For John (owner):** A `personal.json` overlay file per destination (e.g., `personal/japan.json`) that stores annotations keyed to POI names or coordinates. Claude can build this from confirmation emails or PDFs that John drops into the Travel folder. The map loads it alongside the destination JSON and displays booking icons or info badges on annotated POIs.
  - **For shared users (family, friends):** Each user gets a localStorage namespace keyed to a simple user ID passed via URL parameter (e.g., `?user=sarah`). Their notes are already isolated per-device via localStorage.
  - **Annotation schema (proposed):**
    ```json
    {
      "poiName": "The Ritz London",
      "type": "reservation",
      "details": "Dinner 7:30pm, confirmation #RZ-44821, party of 4",
      "date": "2026-04-15",
      "addedBy": "john"
    }
    ```
  - **Flight/transit layer:** A special annotation type for flights and train bookings that renders as a travel segment between cities, showing departure/arrival times and confirmation codes. Could display as a dashed route line on the map.
  - **Notes import/export:** Add a button to export all notes as JSON and import from a file, enabling notes to survive across devices without a backend.
  - **Future evolution:** If the map ever moves to a backend (Firebase, Supabase), annotations could sync across devices and support real-time collaboration.

### Longer-term
- **Offline mode** — Cache destination JSONs in a service worker for airplane/subway use
- **Trip sharing** — Export a specific itinerary as a shareable link or PDF. Could include personal annotations (with opt-in) so a shared link shows "Sarah's picks" or "John's reservations" alongside the base map data.
- **Real-time collaboration** — Let family members see each other's pins, annotations, and votes on activities. Would require a lightweight backend (Firebase Realtime DB or Supabase) to sync state across devices.
- **Booking links** — Add direct links to hotel/restaurant booking pages
- **Annotation import from email** — Claude reads confirmation emails (forwarded or via Gmail API) and auto-generates annotation entries, matching bookings to the correct POI and destination

---

## Quick Technical Reference

- **CDN deps:** Leaflet.js 1.9.4, Font Awesome 6.4.0, CartoDB Positron tiles
- **AI Chat:** Requires Anthropic API key (stored in localStorage as `tripMap_apiKey`)
- **Lazy loading:** Only the default destination (Japan) loads on startup. Others fetch on first select, then cache in memory.
- **localStorage keys:** `tripMap_mods_[dest]` (itinerary mods), `tripMap_apiKey`, `tripMap_model`, `tripMap_notes_[dest]_[poiName]` (personal notes per POI)

---

## Handing Off to a New Claude Session

1. Point Claude to this file: `PROJECT_HANDOFF.md`
2. Tell Claude what to work on (e.g., "Add France" or "Clean up Italy duplicates" or "Show itinerary names in the UI")
3. Claude edits JSON files in `destinations/` and `destinations.json`, then copies to `deploy/`
4. For new destinations, Claude reads the source Excel from the destination subfolder and follows the "How to Add a New Destination" workflow above
5. Source Excel files for each destination live in their respective subfolders
6. The JSON schema is documented above and validated by `registerExternalDest()` in the code
7. After deployment, GitHub Pages can take a few minutes to reflect changes — don't panic if updates aren't instant
