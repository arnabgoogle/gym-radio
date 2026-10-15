# GymRadio 🏋️‍♂️⚡

**Live Zero-Login Mobile Web App:** [https://arnabgoogle.github.io/gym-radio/](https://arnabgoogle.github.io/gym-radio/)

GymRadio is a participatory gym audio platform and autonomous floor jukebox. Gym-goers can discover clean, high-energy workout music, submit requests, and upvote tracks on a live community leaderboard with **zero corporate login barriers** on any mobile phone. At the gym reception desk, a dedicated Receptionist DJ console streams the highest-voted tracks continuously using the YouTube IFrame Player API. When the request queue is empty, the autonomous player seamlessly loops through a curated 200-track gym workout playlist.

---

## 🚀 Key Features

1. **Zero-Login Mobile Experience**:
   - Access directly from any mobile or desktop browser: [https://arnabgoogle.github.io/gym-radio/](https://arnabgoogle.github.io/gym-radio/)
   - No SSO, LDAP password, or authentication walls required.
   - Non-blocking athlete handle auto-generation (`@Athlete_XX`) with optional 1-tap customization.

2. **Universal Hero Playback Controls**:
   - Play / Pause / Skip (Next) / Previous controls directly on the Now Playing hero card.
   - Optional local phone audio streaming toggle so users can listen privately on their headphones without receptionist hardware.

3. **Upcoming 5 Songs Leaderboard**:
   - The queue always displays exactly 5 tracks at all times.
   - Active user requests take top rank (sorted by upvotes DESC, submission time ASC).
   - Automatically padded from the curated 200 default gym songs with a 1-tap **"⚡ Boost"** button to promote backup tracks into the live request queue.

4. **Autonomous Client-Side State Machine & Monotonic Timer**:
   - Continuous high-precision playback tracking without timer reset bugs.
   - Seamless auto-advance on track completion (`YT.PlayerState.ENDED` or natural duration).
   - Automatic 1-second auto-skip on unplayable or restricted video embeds.

5. **Multi-Gym Location Management**:
   - Defaults to **"Ananta"**.
   - Supports switching locations or dynamically adding new gym locations with localStorage persistence.

6. **Curated 200-Track Default Mix**:
   - Clean, verified high-energy workout anthems spanning EDM, Phonk, Synthwave, Pop, Rock, and Hip-Hop with real YouTube video IDs.
