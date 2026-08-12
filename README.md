Here is the updated, comprehensive `README.md` file. It merges your step-by-step setup guide—including TV setup, phone/PC configuration, family member login flow, and important streaming notes—with the existing file structure, catalog listings, and addon templates.

---

# "Stream app" Configuration Templates



This repository contains a fully optimized collection of configuration templates and formatting files for **AIOStreams**, **AIOMetadata**, and **CustomFusionBadges**.

This guide provides the easiest path to streaming on a TV using Android and Windows devices. Everything is synced automatically inside the streaming app across all your devices.

---

## 📋 Prerequisites & Things You Need



### Devices Required



1. **For Watching (TV):** An Android TV, Google TV, or Android TV Box connected to your TV.


2. **For Setup:** An Android phone/tablet or a Windows PC.



### Accounts & API Keys



Before starting, ensure you have set up the following accounts:

1. **An active Debrid Subscription** (e.g., RealDebrid, AllDebrid, Premiumize, etc.).


2. **Accounts and API Keys** for metadata and layout providers (you will input these keys during configuration):


* [`Google Gemini API`](https://ai.google.dev/)

* [`OpenRouter API`](https://openrouter.ai/)

* [`TMDB`](https://www.themoviedb.org/)

* [`TVDB`](https://thetvdb.com/)

* [`Fanart.tv`](https://fanart.tv/)

* [`Rating Poster DB (RPDB)`](https://ratingposterdb.com/)

* [`TopPoster`](https://topposter.com/)

* [`MdbList`](https://mdblist.com/)

* [`Trakt.tv`](https://trakt.tv/)

* [`Simkl`](https://simkl.com/)

* [`AniList`](https://anilist.co/)



3. **Addon Instance Uptime Status:** Select active addon instances and monitor their real-time status at [IbbyLabs Uptime](https://www.google.com/search?q=https://uptime.ibbylabs.dev/).



⚠️ **Important Infrastructure Advice:** For optimal performance and system stability, use **only one instance for AIOMetadata** and **one instance for AIOStreams** (or a single secondary instance strictly as a backup).

---

## 🛠️ Repository File Structure



* [`aiometadata-config.json`](https://www.google.com/search?q=https://github.com/djgenesis/stream/blob/main/aiometadata-config.json) – Master configuration template for AIOMetadata.


* [`aiostreams-config.json`](https://www.google.com/search?q=https://github.com/djgenesis/stream/blob/main/aiostreams-config.json) – Base configuration template for AIOStreams.


* [`aiostreams-template.json`](https://www.google.com/search?q=https://github.com/djgenesis/stream/blob/main/aiostreams-template.json) – Core template layout for media streams.


* [`gold_badges_complete.json`](https://www.google.com/search?q=https://github.com/djgenesis/stream/blob/main/gold_badges_complete.json) – Custom gold badges layout for stream resolution, audio formats, and video codecs.


* [`formatter-usingbadges.json`](https://www.google.com/search?q=https://github.com/djgenesis/stream/blob/main/formatter-usingbadges.json) – Stream formatting optimized for visual badges.


* [`formatter-notusingbadges.json`](https://www.google.com/search?q=https://github.com/djgenesis/stream/blob/main/formatter-notusingbadges.json) – Plain text stream formatting.



---

## 🚀 Complete Step-by-Step Setup Guide



### Step 1: Prepare Your TV / TV Box



1. Turn on your TV or Android TV Box.


2. Open the **Google Play Store** and install the **streaming app**.


3. Open the app on your TV. It will display a **QR Code** and a **Web URL Link**.


4. **Leave this screen open on your TV.** *(We do this first to confirm your TV operating system supports the application before configuring addons)*.



---

### Step 2: Set Up the App on Your Setup Device (Phone or PC)



1. On your Android phone/tablet (via Google Play Store) or Windows PC (via official website), open the streaming app.


2. **Sign Up** using your email and log in to your account.



---

### Step 3: Retrieve Your Debrid API Key



1. Open a web browser, go to your chosen Debrid service (RealDebrid, AllDebrid, Premiumize, etc.), and log in.


2. Navigate to **Account Settings**.


3. Copy your **API Key**. Keep this browser tab open as you may need it later.



---

### Step 4: Configure AIOStreams



1. Open the configuration page for an active **AIOStreams** instance (check [IbbyLabs Uptime](https://www.google.com/search?q=https://uptime.ibbylabs.dev/)).


2. Click **Upload / Import Template** and select `aiostreams-config.json` or `aiostreams-template.json` from this repository.


3. Paste your **Debrid API Key** under your debrid service section.


4. Choose your preferred formatting route:


* **Route A (Recommended - Custom Badges):** Load `formatter-usingbadges.json`.


* **Route B (Plain Text):** In Formatter settings, click Save and load `formatter-notusingbadges.json`.




5. Click **Install / Generate Link**. This will automatically prompt to open the Addon in the streaming app.


6. Click **Install** inside the streaming app.



---

### Step 5: Configure AIOMetadata



1. Open the configuration page for an active **AIOMetadata** instance (check [IbbyLabs Uptime](https://www.google.com/search?q=https://uptime.ibbylabs.dev/)).


2. Select **Upload Template** and upload `aiometadata-config.json` from this repository.


3. Input all your personalized API keys (TMDB, TVDB, Gemini, OpenRouter, Fanart, RPDB, TopPoster, MdbList, etc.) into their respective fields.


4. Click **Install / Generate Link**.


5. Click **Install** inside the streaming app.



---

### Step 6: Link Your Account to Your TV



1. Go back to your TV screen where the QR code and link are displayed.


2. **If using an Android Phone/Tablet:** Scan the QR code on the TV screen using your phone camera/scanner.


3. **If using a Windows PC:** Open a browser, visit the web link shown on the TV, and log in with your credentials if requested.


4. Your TV / TV Box will automatically authorize and enter the app interface!


5. Go to **Settings — Advanced and select "Remember Last Profile** 



---

### Step 7: Player & Subtitle Settings (Recommended for Optimum Experience)



1. In the streaming app, go to **Settings — Streams**.


2. Paste the raw URL of `gold_badges_complete.json` (`[https://raw.githubusercontent.com/djgenesis/stream/refs/heads/main/gold_badges_complete.json](https://raw.githubusercontent.com/djgenesis/stream/refs/heads/main/gold_badges_complete.json)`) into **Fusion Badges URLs**. Disable size badges and addon logo, and set the badge position to **Top**.


3. Go to **Settings — Advanced** and select **Remember last profile**.


4. Click the **Settings (Gear Icon)** on the left sidebar:


* Select your preferred **Interface Language**.


* Set your **Default Subtitles Language**.


* Enable **Autoplay next episode** (recommended for TV series).





---

### Step 8: Watchlist Sync & Tracking (Recommended)



1. Create a free account at [trakt.tv](https://trakt.tv/) if you don't have one.


2. Inside the app, go to **Settings → Tracking** and connect your Trakt account to back up your watch history and sync watchlists.



---

### Step 9: Test Your Setup



1. Go to the **Discover** section on your TV app.


2. Click on any Movie or TV show.


3. Select a stream from the results list.


4. The video should start playing within 2 to 5 seconds depending on file size and internet connection.



*And voilà! WE ARE DONE!*

---

## 👥 Family / Extra Member Login Process



Follow these steps when setting up an extra device or family member profile:

### Things Required



* An Android TV, Google TV, or Android TV Box connected to the TV.


* An Android phone/tablet or Windows PC.



### Steps



1. **On TV / TV Box:** Install the streaming app from the Google Play Store. Open it so the QR code and login link are displayed.


2. **On Phone / PC:** Open the streaming app website or mobile app and log in using the **original primary member's account credentials**.


3. **Sync TV:** Scan the QR code with your phone or enter the web link on your PC browser.


4. Your TV / TV Box will automatically log into the account.


5. **Profile Customization:**
* Go to **Settings — Advanced** and enable **Remember last profile**.


* Go to **Settings → Tracking** and connect an individual Trakt.tv account if personal watch history tracking is desired.




6. **Test:** Head to **Discover**, select a stream, and start watching!



---

## 📌 Important Notes & FAQ



* **VPN Requirement:** You **do NOT need a VPN** to stream content using this setup. Your ISP will not flag or throttle your connection because streams are delivered via secure web servers (HTTPS direct streaming) rather than peer-to-peer torrents.


* **Cross-Device Syncing:** Everything you configure (adding/removing addons, organizing watchlists, updating settings) automatically syncs across every device logged into your account.



Happy streaming! 🎬

---

## 📁 Included Movie & Series Catalogs



By importing `aiometadata-config.json`, the following dynamic metadata catalogs will be automatically integrated into your library interface:

### 🎬 Movies Lists



* **-Trakt Watchlist**

* **Movies Recommended for you**

* **[New Streaming Releases: Movies](https://mdblist.com/lists/snoak/latest-movies-digital-release)**

* **[Latest 4K Movies](https://www.google.com/search?q=https://mdblist.com/lists/maniac2021/latest-4k-releases)**

* **[In Cinemas Now](https://www.google.com/search?q=https://mdblist.com/lists/24hz/in-theatres)**

* **[Trending Movies on Trakt](https://mdblist.com/lists/snoak/trending-movies)**

* **[Top Movies of the Month](https://www.google.com/search?q=https://mdblist.com/lists/antonio0101/top-movies-of-the-week)**

* **[Top 100 Classic Movies](https://www.google.com/search?q=https://trakt.tv/lists/11632963)**

* **[Top Action Movies](https://www.google.com/search?q=https://mdblist.com/lists/hdlists/latest-hd-action-movies-from-1980-to-today)**

* **[New Action Releases](https://www.google.com/search?q=https://mdblist.com/lists/snoak/latest-action-movies)**

* **[Modern Action](https://www.google.com/search?q=https://letterboxd.com/sisamim/list/modern-action/)**

* **[Action Movies (2000 - 2020)](https://www.google.com/search?q=https://trakt.tv/lists/11255166)**

* **[Top 10 Action Movies Of 21st Century](https://www.google.com/search?q=https://trakt.tv/lists/4297336)**

* **[Top Comedy Movies](https://mdblist.com/lists/hdlists/comedy-movies-2001-2020)**

* **[New Releases in Comedy](https://www.google.com/search?q=https://mdblist.com/lists/snoak/latest-comedy-movies)**

* **[Stand-ups](https://www.google.com/search?q=https://mdblist.com/lists/notamongo5/stand-up-comedy)**

* **[Popular Thriller Movies](https://www.google.com/search?q=https://mdblist.com/lists/snoak/thriller-movies)**

* **[New Thriller Releases](https://www.google.com/search?q=https://mdblist.com/lists/snoak/latest-thriller-movies)**

* **[Psychological Thriller](https://www.google.com/search?q=https://mdblist.com/lists/rizreflects/psychological-thrillers)**

* **[IMDb's Top Thriller Movies](https://www.google.com/search?q=https://trakt.tv/lists/22847415)**

* **[Top Horror Movies](https://mdblist.com/lists/hdlists/latest-hd-horror-movies-top-rated-from-1980-to-today)**

* **[New Horror Releases](https://mdblist.com/lists/snoak/latest-horror-movies)**

* **[Rotten Tomatoes: Best Horror Movies Of All Time](https://www.google.com/search?q=https://trakt.tv/lists/4203408)**

* **[Top Fantasy/Sci-Fi Movies](https://mdblist.com/lists/hdlists/latest-hd-fantasy-sci-fi-movies-top-rated-from-1980-to-today)**

* **[Popular Romance Movies](https://www.google.com/search?q=https://mdblist.com/lists/snoak/popular-romance-movies)**

* **[Best of Romance](https://www.google.com/search?q=https://mdblist.com/lists/rjchignell/best-of-romance)**

* **[Forbidden Love in Movies](https://www.google.com/search?q=https://trakt.tv/lists/11142103)**

* **[IMDb's Top Romance Movies](https://www.google.com/search?q=https://trakt.tv/lists/22847343)**

* **[Popular Animation Movies](https://www.google.com/search?q=https://mdblist.com/lists/snoak/animationanime-movies)**

* **[IMDb's Top Animation Movies](https://www.google.com/search?q=https://trakt.tv/lists/22847039)**

* **[Japanese Anime Movies](https://www.google.com/search?q=https://trakt.tv/lists/23471533)**

* **[Shrek Collection](https://letterboxd.com/fantic/list/shrek/)**

* **[Robert De Niro](https://www.google.com/search?q=https://mdblist.com/lists/mokono/robert-de-niro)**

* **[Al Pacino](https://www.google.com/search?q=https://mdblist.com/lists/mokono/al-pacino)**

* **[Anthony Hopkins](https://www.google.com/search?q=https://mdblist.com/lists/mokono/anthony-hopkins)**

* **[Morgan Freeman](https://www.google.com/search?q=https://mdblist.com/lists/mokono/morgan-freeman)**

* **[Daniel Day-Lewis](https://www.google.com/search?q=https://letterboxd.com/fernanp_23/list/daniel-day-lewis/)**

* **[Christian Bale](https://www.google.com/search?q=https://mdblist.com/lists/mokono/christian-bale)**

* **[Jake Gyllenhaal](https://www.google.com/search?q=https://mdblist.com/lists/andyjacoo/jake-gyllenhaal-2kin4hpskb)**

* **[Ryan Gosling](https://www.google.com/search?q=https://mdblist.com/lists/billryan/ryan-gosling-films)**

* **[Margot Robbie](https://www.google.com/search?q=https://mdblist.com/lists/itsall4meplease/margot-robbie)**

* **[Natalie Portman](https://www.google.com/search?q=https://mdblist.com/lists/reachingout/natalie-portman-month)**

* **[Timothée Chalamet](https://www.google.com/search?q=https://mdblist.com/lists/nobnobz/actor-timoth%25C3%25A9e-chalamet-1dy5dcud8e)**

* **[Joaquin Phoenix](https://www.google.com/search?q=https://mdblist.com/lists/mokono/joaquin-phoenix)**

* **[Florence Pugh](https://www.google.com/search?q=https://mdblist.com/lists/nobnobz/actor-florence-pugh-t50c8h9o4g)**

* **[Scarlett Johansson](https://www.google.com/search?q=https://mdblist.com/lists/caballitopalo/scarlett-johanssons-movies)**

* **[Cate Blanchett](https://www.google.com/search?q=https://mdblist.com/lists/jossbosses/cate-blanchett)**

* **[Emma Stone](https://www.google.com/search?q=https://mdblist.com/lists/billryan/emma-stone-films)**

* **[Peter Sellers](https://www.google.com/search?q=https://mdblist.com/lists/billryan/peter-sellers-films)**

* **[Leonardo Dicaprio](https://www.google.com/search?q=https://mdblist.com/lists/mokono/leonardo-dicaprio-movies)**

* **[Mark Wahlberg](https://www.google.com/search?q=https://mdblist.com/lists/mokono/mark-wahlberg)**

* **[Tom Hanks](https://www.google.com/search?q=https://mdblist.com/lists/mokono/tom-hanks)**

* **[Denzel Washington](https://www.google.com/search?q=https://mdblist.com/lists/mokono/denzel-washington)**

* **[Michael Caine](https://www.google.com/search?q=https://mdblist.com/lists/mokono/michael-caine)**

* **[James Stewart](https://www.google.com/search?q=https://mdblist.com/lists/mokono/james-stewart)**

* **[Robin Williams](https://www.google.com/search?q=https://mdblist.com/lists/mokono/robin-williams)**

* **[Robert Duvall](https://www.google.com/search?q=https://mdblist.com/lists/mokono/robert-duvall)**

* **[Jeff Bridges](https://www.google.com/search?q=https://mdblist.com/lists/mokono/jeff-bridges)**

* **[Clint Eastwood](https://www.google.com/search?q=https://mdblist.com/lists/mokono/clint-eastwood)**

* **[Gene Hackman](https://www.google.com/search?q=https://mdblist.com/lists/mokono/gene-hackman)**

* **[Philip Seymour Hoffman](https://www.google.com/search?q=https://mdblist.com/lists/mokono/philip-seymour-hoffman)**

* **[Russell Crowe](https://www.google.com/search?q=https://mdblist.com/lists/mokono/russell-crowe)**

* **[Tommy Lee Jones](https://www.google.com/search?q=https://mdblist.com/lists/mokono/tommy-lee-jones)**

* **[Sean Connery](https://www.google.com/search?q=https://mdblist.com/lists/mokono/sean-connery)**

* **[Chistopher Walken](https://www.google.com/search?q=https://mdblist.com/lists/mokono/chistopher-walken)**

* **[Joe Pesci](https://www.google.com/search?q=https://mdblist.com/lists/mokono/joe-pesci)**

* **[Jon Voight](https://www.google.com/search?q=https://mdblist.com/lists/mokono/jon-voight)**

* **[Heath Ledger](https://www.google.com/search?q=https://mdblist.com/lists/mokono/heath-ledger)**

* **[Johnny Depp](https://www.google.com/search?q=https://mdblist.com/lists/mokono/johnny-depp)**

* **[Matthew McConaughey](https://www.google.com/search?q=https://mdblist.com/lists/mokono/matthew-mcconaughey)**

* **[Edward Norton](https://www.google.com/search?q=https://mdblist.com/lists/mokono/edward-norton)**

* **[Brad Pitt](https://www.google.com/search?q=https://mdblist.com/lists/mokono/brad-pitt)**

* **[Matt Damon](https://www.google.com/search?q=https://mdblist.com/lists/mokono/matt-damon)**

* **[Hugh Jackman](https://www.google.com/search?q=https://mdblist.com/lists/mokono/hugh-jackman)**

* **[Robert Downey Jr](https://www.google.com/search?q=https://mdblist.com/lists/mokono/robert-downey-jr)**

* **[Liam Neeson](https://www.google.com/search?q=https://mdblist.com/lists/mokono/liam-neeson)**

* **[Mel Gibson](https://www.google.com/search?q=https://mdblist.com/lists/mokono/mel-gibson)**

* **[Bill Murray](https://www.google.com/search?q=https://mdblist.com/lists/mokono/bill-murray)**

* **[Samuel L Jackson](https://www.google.com/search?q=https://mdblist.com/lists/mokono/samuel-l-jackson)**

* **[Jim Carrey](https://www.google.com/search?q=https://mdblist.com/lists/mokono/jim-carrey)**

* **[Will Smith](https://www.google.com/search?q=https://mdblist.com/lists/mokono/will-smith)**

* **[John Goodman](https://www.google.com/search?q=https://mdblist.com/lists/mokono/john-goodman)**

* **[Bruce Willis](https://www.google.com/search?q=https://mdblist.com/lists/mokono/bruce-willis)**

* **[Director: Nolan](https://www.google.com/search?q=https://letterboxd.com/discovery_17/list/nolan/)**

* **[Argentinian Movies](https://www.google.com/search?q=https://mdblist.com/lists/mxtrakttv/argentina-movies)**

* **[Introduction to French Cinema](https://www.google.com/search?q=https://mdblist.com/lists/roskoe88/intro-to-french-cinema)**

* **[French Movies](https://www.google.com/search?q=https://mdblist.com/lists/jarvis-13128907/france-movies)**

* **[Latest French Cinema](https://www.google.com/search?q=https://mdblist.com/lists/factoor/latest-french-cinema)**

* **[Recommended Korean Movies](https://www.google.com/search?q=https://mdblist.com/lists/molemovies/recommended-korean-cinema)**

* **[Korean Movies](https://www.google.com/search?q=https://mdblist.com/lists/narmeian/korean-cinema)**

* **[Popular Korean Movies](https://www.google.com/search?q=https://mdblist.com/lists/an-kah/popular-korean-movies)**

* **[Spanish Movies](https://www.google.com/search?q=https://mdblist.com/lists/ftor327/spain-movies)**

* **[Popular Spanish Movies](https://www.google.com/search?q=https://mdblist.com/lists/snafuki/spain-popular-movies)**

* **[Introduction to Italian Cinema](https://www.google.com/search?q=https://letterboxd.com/richardjduffy/list/italian-cinema/)**

* **[Italian Movies](https://www.google.com/search?q=https://letterboxd.com/murraldo/list/italian-movies-1/)**

* **[Introduction to Japanese Cinema](https://www.google.com/search?q=https://letterboxd.com/tomodachi/list/intro-to-japanese-film-history/)**

* **[Japanese Movies](https://www.google.com/search?q=https://mdblist.com/lists/jarvis-15299542/japanese-cinema)**

* **[UK Movies](https://www.google.com/search?q=https://mdblist.com/lists/andemer/latest-streaming-movies)**

* **[Latest UK Movies](https://www.google.com/search?q=https://mdblist.com/lists/amything/latest-uk-movies)**

* **[Introduction to German Cinema](https://www.google.com/search?q=https://letterboxd.com/nvdw/list/germany-cinema-around-the-world/)**

* **[German Movies](https://www.google.com/search?q=https://mdblist.com/lists/itsdrewy97/germany)**

* **[Introduction to Mexican Cinema](https://www.google.com/search?q=https://letterboxd.com/dawnofthedead/list/mexican-cinema/)**

* **[Top Mexican Movies](https://letterboxd.com/official/list/top-250-mexican-films/)**

* **[More Mexican Movies](https://www.google.com/search?q=https://letterboxd.com/kon0787/list/mexican-movies/)**

* **[Introduction to Brazilian Cinema](https://www.google.com/search?q=https://letterboxd.com/coffeejazzlofi/list/an-introduction-to-brazilian-film-history/)**

* **[Brazilian Movies](https://www.google.com/search?q=https://mdblist.com/lists/biracosme/brazilian-movies)**

* **[Introduction to Indian Cinema](https://www.google.com/search?q=https://letterboxd.com/mithras_/list/bollywood-essentials-and-my-intro-to-indian/)**

* **[Indian Movies](https://www.google.com/search?q=https://letterboxd.com/mcl/list/indian-cinema/)**

* **[Best Picture Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/oscar/)**

* **[Best Actress Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/actress-in-a-leading-role/)**

* **[Best Actor Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/actor-in-a-leading-role/)**

* **[Best Director Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/director/)**

* **[Best Original Song Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/original-song/)**

* **[Best International Film Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/international-feature/)**

* **[Best Sound Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/sound/)**

* **[Best Documentary Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/documentary-feature/)**

* **[Best Visual Effects Winners](https://www.google.com/search?q=https://letterboxd.com/thaais/list/visual-effects/)**

* **[Cannes Winners](https://www.google.com/search?q=https://letterboxd.com/lukas1999/list/cannes/)**

* **[Venice Festival Winners](https://www.google.com/search?q=https://mdblist.com/lists/atalante421/venice-film-festival-winners)**

* **[BAFTA Winners](https://www.google.com/search?q=https://letterboxd.com/jacquard/list/bafta/)**

* **[Golden Globe Winners](https://www.google.com/search?q=https://mdblist.com/lists/nobnob/collection-golden-globes-winners)**

* **[2026 Golden Globe Nominees](https://www.google.com/search?q=https://mdblist.com/lists/bsm-venger/golden-globes-2026-nominees)**

* **[1960s Movies](https://www.google.com/search?q=https://mdblist.com/lists/ryankeast/movies-decades-1960s-4oulwbhwix)**

* **[1970s Movies](https://www.google.com/search?q=https://mdblist.com/lists/ryankeast/movies-decades-1970s)**

* **[Best of the 1970s](https://www.google.com/search?q=https://mdblist.com/lists/rjchignell/best-of-the-1970-s)**

* **[1980s Movies](https://www.google.com/search?q=https://mdblist.com/lists/ryankeast/movies-decades-1980s)**

* **[1990s Movies](https://www.google.com/search?q=https://mdblist.com/lists/ryankeast/movies-decades-1990s)**

* **[Best of the 1990s](https://www.google.com/search?q=https://mdblist.com/lists/rjchignell/best-of-the-1990-s)**

* **[2000s Movies](https://www.google.com/search?q=https://mdblist.com/lists/ryankeast/movies-decades-2000s)**

* **[2010s Movies](https://www.google.com/search?q=https://mdblist.com/lists/ryankeast/movies-decades-2010s)**

* **[2020s Movies](https://www.google.com/search?q=https://mdblist.com/lists/ryankeast/movies-decades-2020s-a2h6mk0dh0)**

* **[Christmas Movies](https://mdblist.com/lists/hdlists/christmas-movies)**

* **[Thanksgiving Movies](https://mdblist.com/lists/hdlists/thanksgiving-movies)**

* **[Best Halloween Movies of All Time](https://www.google.com/search?q=https://mdblist.com/lists/hdlists/halloween-movies-the-best-of-all-time)**

* **[Top Valentine's Movies](https://www.google.com/search?q=https://mdblist.com/lists/craigywulse23/top-valentines-movies)**

* **[St. Patrick's Day](https://www.google.com/search?q=https://letterboxd.com/blood_countess/list/st-patricks-day/)**

* **[Day of the Dead: Mexican Horror](https://letterboxd.com/cinemathek_zlb/list/dia-de-los-muertos-mexican-horror-the-full/)**

* **[Movies Based on True Stories](https://www.google.com/search?q=https://mdblist.com/lists/slander2328/movies-based-on-a-true-story)**

* **[Superhero & Comic Book Movies](https://www.google.com/search?q=https://mdblist.com/lists/jmla/superhero-based-on-comic-superhuman-abilities)**

* **[Movies Based on Video Games](https://www.google.com/search?q=https://mdblist.com/lists/awesomeaustn/movies-based-on-video-games-live-action)**

* **[Movies Based on Books](https://www.google.com/search?q=https://mdblist.com/lists/godzgiftmm/based-on-a-book-uncollected)**

* **[Biographies](https://www.google.com/search?q=https://letterboxd.com/nislav2001/list/biographies/)**

* **[60 Minutes or Less](https://www.google.com/search?q=https://mdblist.com/lists/roolfer/higesht-rated-unwatched-60-minutes-or-less)**

* **[90 Minutes or Less](https://www.google.com/search?q=https://mdblist.com/lists/roolfer/highest-rated-unwatched-90-minutes-or-less)**

* **[Under 2 Hours](https://www.google.com/search?q=https://mdblist.com/lists/stephenwall95/popular-movies-under-2-hours)**

* **[Long Movies](https://www.google.com/search?q=https://letterboxd.com/frantz/list/long-movies/)**

* **Trakt Most Favorited - Weekly**


### 📺 Series Lists



* **-Trakt Watchlist**

* **Series Recommended for you**

* **[New Streaming Releases: Series](https://mdblist.com/lists/garycrawfordgc/latest-tv-shows)**

* **[Trending Series on Trakt](https://www.google.com/search?q=https://mdblist.com/lists/snoak/trakt-s-trending-shows)**

* **[IMDb Top 250 Series](https://www.google.com/search?q=https://trakt.tv/lists/2143363)**

* **[Comedy Series](https://mdblist.com/lists/garycrawfordgc/comedy-shows)**

* **[Popular Thriller Series](https://mdblist.com/lists/snoak/thriller-shows)**

* **[Horror Series](https://mdblist.com/lists/garycrawfordgc/horror-shows)**

* **[Fantasy Series](https://www.google.com/search?q=https://mdblist.com/lists/MaxtronTV/fantasy-tv-shows)**

* **[Popular Romance Series](https://www.google.com/search?q=https://mdblist.com/lists/snoak/popular-romance-shows)**

* **[New Romance Series](https://www.google.com/search?q=https://mdblist.com/lists/snoak/latest-romance-shows)**

* **[Popular Animation Series](https://www.google.com/search?q=https://mdblist.com/lists/snoak/animationanime-shows)**

* **[Adult Animation](https://www.google.com/search?q=https://mdblist.com/lists/breon64/adult-animation)**

* **[Warner Bros. Television Studios - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/warner-bros-television-studios-series)**

* **[Universal Television - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/universal-television-series)**

* **[Sony Pictures Television - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/sony-pictures-television-series)**

* **[20th Television - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/20th-television-series)**

* **[Paramount Television Studios - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/paramount-television-studios-series)**

* **[CBS Studios - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/cbs-studios-series)**

* **[Lionsgate Television - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/lionsgate-television-series)**

* **[MGM Television - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/mgm-television-series)**

* **[ABC Signature - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/abc-signature-series)**

* **[FX Productions - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/fx-productions-series)**

* **[NBCUniversal Content Studios - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/nbcuniversal-content-studios-series)**

* **[Bad Robot Production](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/sony-pictures-television-studios-series)**

* **[Fremantle North America - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/fremantle-north-america-series)**

* **[Skydance Television - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/skydance-television-series)**

* **[A+E Studios - Series](https://www.google.com/search?q=https://mdblist.com/lists/jstinchcombe8642/ae-studios-series)**

* **[Argentinian Series](https://www.google.com/search?q=https://mdblist.com/lists/mxtrakttv/argentina-series)**

* **[Best Korean Series](https://www.google.com/search?q=https://mdblist.com/lists/saltydude/top-rated-korean-tv-shows)**

* **[Spanish Series](https://www.google.com/search?q=https://mdblist.com/lists/ftor327/spain-series)**

* **[Popular Spanish Series](https://www.google.com/search?q=https://mdblist.com/lists/snafuki/spain-popular-tv-shows)**

* **[Japanese Series](https://www.google.com/search?q=https://mdblist.com/lists/nuguns17/japanese-shows)**

* **[UK Series](https://www.google.com/search?q=https://mdblist.com/lists/garycrawfordgc/channel-4-shows)**

* **[Brazilian Series](https://www.google.com/search?q=https://mdblist.com/lists/gussouzanow/brazilian-shows)**

* **[Indian Series](https://www.google.com/search?q=https://mdblist.com/lists/cakepopcorn/top-rated-indian-shows)**


---

## 🤝 Credits & Acknowledgments



* Shoutout to the creator of [SEL-Filtering-and-Sorting](https://github.com/Tam-Taro/SEL-Filtering-and-Sorting) for the underlying sorting rules and filtering framework.


* The open-source developers behind the AIOStreams and AIOMetadata projects.
