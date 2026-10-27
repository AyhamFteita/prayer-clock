# Prayer Clock — iPad 2 only (no Pi)

Clock · Gregorian + Hijri date · prayer times (ISNA, 77407) · countdown · weather · adhan at every prayer.
Everything runs on the iPad. Prayer times and the Hijri date work offline; only the weather needs internet.

## 1. Put it online (GitHub Pages, free)
1. Sign up at github.com.
2. Click **+ → New repository**. Name it `prayer-clock`, set it **Public**, click **Create repository**.
3. Click **uploading an existing file**. Drag in `index.html` and the whole `audio` folder → **Commit changes**.
4. Go to **Settings → Pages**. Under *Branch*, pick **main** and **/(root)** → **Save**.
5. Wait about 1 minute. Your link is `https://YOUR-USERNAME.github.io/prayer-clock/`.
   Open it on your Mac first to check it works.

## 2. Set up the iPad
1. Open **Safari** → go to your link.
2. Tap **Share → Add to Home Screen → Add**.
3. **Settings → General → Auto-Lock → Never.**
4. **Settings → Do Not Disturb → Manual: On.**
5. **Settings → General → Accessibility → Guided Access → On**, set a passcode.
6. Open **Prayer Clock** from the Home Screen.
7. **Tap the screen once** to turn on the adhan sound (bottom-right shows "🔊 Adhan on").
8. **Triple-click Home → Start** to lock it on the display.
9. Turn the volume up and keep it plugged in.

## Daily use
- Tap anywhere while the adhan plays to stop it.
- If the iPad restarts or the page is reopened, tap once again to turn the sound back on.
- The screen dims from 11 PM to 5:30 AM.

## Changing settings
Open `index.html` on GitHub (pencil icon) and edit the **SETTINGS** block at the top:
location (latitude/longitude), Asr method (`asrFactor: 2` for Hanafi), minute adjustments to match
your masjid, which adhan plays for each prayer, 24-hour clock, night dim. Commit, then on the iPad
exit Guided Access, reopen the page, and tap once.

## If something's off
- **Weather says unavailable**: the clock, prayers and adhan still work. The page tries Open-Meteo, then the US National Weather Service as a backup.
- **Times a minute different from your masjid**: use the `adjust` minutes in SETTINGS.
- **No sound at prayer time**: check "🔊 Adhan on" is showing, the mute switch on the side is off, and the volume is up.
