WEYOU — TMDB + AniList API Edition
===================================

මෙය Acode සඳහා responsive OTT-style metadata catalogue prototype එකකි.

ප්‍රධාන අංග
- Premium black + violet design
- TMDB: trending movies, trending TV, search, upcoming movies, movie/TV details
- AniList: popular anime, anime search, upcoming anime, genre data
- Main categories: Anime, Anime Movies, Live Action, TV Series, Cartoons
- Genre chips (API results වලින් සකස් වේ), sort by popular/rating/newest/A-Z
- Poster images, ratings, release dates, synopsis, detail popup
- Watchlist saved locally on device
- Local video file player
- User-provided .SRT / .VTT subtitles
- Responsive mobile layout

Acode setup
1. ZIP extract කරන්න.
2. Acode > Open Folder > WEYOU.
3. index.html Preview/Run කරන්න.
4. ⚙ Settings > TMDB API key එක ඇතුළත් කරන්න.
5. API key එකක් ලබාගන්න: https://www.themoviedb.org/settings/api
6. Internet connection තිබිය යුතුයි. API calls සඳහා browser preview එකේ network access අවශ්‍යයි.

API විස්තර
- TMDB REST API: movies, TV series, trending, search, upcoming, posters.
- AniList GraphQL: anime discovery, search, genres, upcoming anime.
- AniList public GraphQL endpoint එක API key එකක් නොමැතිව භාවිතා කරයි (rate limits අදාළ වේ).
- TMDB key එක config.js හි හිස්ව තබා ඇත; UI settings හරහා key ඇතුළත් කළ හැක.

වැදගත් ආරක්ෂාව / ප්‍රකාශන හිමිකම්
- TMDB සහ AniList APIs metadata/poster discovery සඳහාය. ඒවායෙන් full movie/anime video streams හෝ WEB-DL downloads ලබාගත නොහැක.
- මෙම project එක pirated links scrape කිරීම, DRM bypass කිරීම, හෝ අවසර නැති වීඩියෝ auto-download/upload කිරීම සිදු නොකරයි.
- Video player එක ඔබගේ device එකේ ඇති media files සඳහාය. Online streaming සඳහා ඔබට අයිතිය/බෙදාහැරීමේ අවසරය ඇති video URLs හෝ licensed provider integration එකක් වෙනම backend එකකින් එක් කළ යුතුය.
- Public production deployment එකක TMDB API key browser JavaScript තුළ තබන්න එපා. Server-side proxy/backend එකක් භාවිතා කරන්න; TMDB branding, attribution සහ usage rules පිළිපදින්න.
- AniList API terms/rate limits සහ metadata source attribution පිළිපදින්න.
- Browser localStorage watchlist සහ optional TMDB key එක එම device/browser එකේම තබයි. Public/shared device එකක key remember නොකරන්න.

Production OTT platform එකකට තවම අවශ්‍ය දේ
- Backend (Node/Python/etc.), database, user accounts, secure API proxy
- Licensed video hosting/storage/CDN, HLS/DASH transcoding and playback
- Rights management, takedown/contact process, privacy/security
- Real server-side subtitle storage, upload moderation and user sync
- Android app packaging (වෙනම build process)

මෙය fully working frontend prototype එකකි; complete commercial OTT backend එකක් හෝ Android APK එකක් නොවේ.
