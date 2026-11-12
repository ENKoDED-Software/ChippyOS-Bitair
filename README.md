# ChippyOS for the Heatbit Bitair

ChippyOS is free firmware for the Heatbit Bitair. It runs your unit on your own network, mining to the pool you choose, with no
Heatbit servers, no account, and no phone number or location required.

ChippyOS is independent. It is not made by, affiliated with or endorsed by Heatbit. "Heatbit" and "Bitair" are named only to say
which hardware it runs on.

**To install it, go to [chippyos.com](https://chippyos.com).** You don't need to download anything from this page.

## What it does

- **Three modes:** Normal (about 1.1 - 1.3 TH/s), Boosted (about 1.3 - 1.5 TH/s) and Overdrive (about 1.4 - 1.7 TH/s), changed
  any time from the unit's page; hash rate varies per ASIC.
- **Your choice of fan:** Normal can run on Low, Medium or High, Boosted on Medium or High, and Overdrive on High only. Choose it
  on the page or with the panel's fan button; for the mode that is running, whichever you changed last wins.
- **Built-in protection:** if the miner gets too warm, the fan goes to High by itself. If Boosted or Overdrive reaches a firm
  limit on temperature, current or power, it drops to a lower mode and keeps mining; the lower mode stays until you choose the
  mode again on the page or the unit loses power. Mining stops with the fan on High when Normal reaches one of those limits, on a
  problem with the supply, or after 5 power dips in a row.
- **A page on the unit,** opened from any browser on your network: a dashboard with a 24-hour chart, the case's air quality,
  temperature and humidity, the local weather and outdoor air for a place you set, your pool's results, settings and a live log.
- **Your pools:** a primary pool and a fallback the unit switches to by itself if the primary stops working. The pool must
  support version rolling (BIP 310); the page says so if it doesn't.
- **Updates over your network,** checked daily and installed only when you choose.
- **Works with [Hashboard](https://hashboardapp.com),** to monitor, control and automate your Bitair alongside your other miners
  for free.

## What you need

- A Mac, Windows or Linux computer with **Google Chrome, Microsoft Edge or Opera**. Safari, Firefox and phone browsers can't
  connect to the unit over USB.
- A **USB-C data cable** (not a charge-only one) for the computer.
- Comfort with **opening the unit**, as the miner's USB-C port is inside.
- About 15 minutes.

You only need the cable and the open unit for the first install. Updates after that come over your network.

## Installing

1. Keep the Heatbit power adapter plugged into the Bitair's outside power port, marked "15V Type C", with the unit on. **Use that
   port for the Heatbit power adapter only:** never plug a computer, another charger or any other cable into it.
2. Open the unit and connect the miner board's own USB-C port to your computer with the data cable.
3. Go to [chippyos.com](https://chippyos.com) and follow the steps there: connect, save a backup (recommended), then install.
4. After the install, the unit opens its own Wi-Fi network, named **ChippyAir-** and six letters and digits. Join it from your phone
   and choose your home Wi-Fi: a 2.4 GHz network, preferably secured with a WPA2 or WPA3 password. If the setup page doesn't open
   by itself, go to http://192.168.77.7.
5. The setup page then shows the unit's address on your home network. Reconnect to your home Wi-Fi, open that address, and enter
   your pool in Settings. Mining starts by itself.
6. Unplug the USB cable and close the unit. If the page then shows a stop for the regulator, power the unit off and on: unplug all
   cabling; wait 10 seconds; plug the Heatbit power adapter back in and power it on.

**While the unit is open,** it stays powered:
- Keep fingers, tools and anything metal off the board, and don't touch the heatsink, which can be hot.
- Keep the fan and its air path clear. The fan that cleans the air also cools the miner.
- While the installer is connected, the unit's own firmware isn't running, so nothing is watching its temperature. Don't leave it
  connected longer than you need. With its tab open, the installer restarts the unit after 2 minutes without a step; if the tab
  was closed or the computer slept, unplug all cabling; wait 10 seconds; plug the Heatbit power adapter back in and power it on.

## Using ChippyOS

- **The panel's Power button starts and stops mining,** as with Heatbit's firmware. After a power cut the panel stays off until you
  press Power, and mining comes back in the mode you chose last.
- **The Bitair's panel display doesn't show changes made in the ChippyOS UI.** Heatbit designed it with only one-way communication
  to the miner, so the panel can't be told about them; the ChippyOS UI always shows what is really running.
- **After a stop or restart,** mining starts again as soon as it's safe, usually within a minute. After a crash or a power dip, a
  restart while a mode is dropped for heat, or when a pool rejects work or accepts none, it waits at least 3 minutes first.
- **After a safety stop,** the fan stays on High and mining stays off until you turn the panel's Power off and on again, or
  power the unit off and on. A stop for the regulator clears only by powering the unit off and on: unplug all cabling; wait 10
  seconds; plug the Heatbit power adapter back in and power it on. After the panel's Power off and on, mining starts no sooner
  than 3 minutes after the stop; after powering the unit off and on, it starts once the start's own checks pass.
- **Mining needs a pool.** If your internet or your pools go down, mining stops within a few minutes and starts again by itself
  once a pool is back.
- **The red restart button** at the top right of the page restarts the unit. A new name for the unit takes effect after a restart.
- **Settings are saved within about a minute.** A power cut right after a change can lose it.
- **The Heatbit app shows nothing from this unit while ChippyOS runs,** and doesn't automatically mine to Heatbit's pool: it mines
  only to the pools you configure. Returning to Heatbit's firmware brings the app back. You can monitor the miner in [Hashboard](https://hashboardapp.com)
  for free when running ChippyOS.

## Updates

- The unit checks for a new version 5 minutes after it starts and then once a day, and an hour later if a check failed. You can
  turn that off in About, on the unit's settings page.
- **Nothing installs until you choose it,** in About. Mining pauses during the install and resumes after the restart.
- **A new version is on trial.** It's kept once it has run 10 minutes with its Wi-Fi and web server working. If it doesn't get
  there, the unit goes back to the version before by itself.
- **Go back to the previous version** from About, if a new version doesn't suit you.
- Your unit and the installer accept only ChippyOS releases signed by us.

## Going back to Heatbit's firmware

- **Return to stock,** in Settings under Danger zone, or in the installer at chippyos.com. It erases ChippyOS's settings on the
  unit. The Heatbit firmware your unit came with is never changed, so you can always go back. Heatbit's own settings, such as its
  Wi-Fi, are never changed either.
- **Restore a backup** in the installer, to put the unit back exactly as it was when you saved the backup. If your unit had a
  newer Heatbit version than the one it came with, a backup is one way to get that exact version back after ChippyOS has updated.
  The Heatbit app will also automatically update from older versions after restoration.

Afterwards, check that the Heatbit app shows the unit mining. **If it's not mining after 5 minutes,** unplug all cabling; wait 10
seconds; plug the Heatbit power adapter back in and power it on.

## Privacy

ChippyOS sends nothing to Heatbit, us or anyone else. The unit connects only to:
- **your router and the DNS server it names,** to join your network and look up the names below; the router also sees the unit's
  name, ChippyAir- and six letters and digits unless you change it;
- **the pools you set;**
- **for the time,** the time server your router names, if it names one, then **time.cloudflare.com** and **pool.ntp.org;**
- **GitHub,** with its download servers, to see whether an update exists (5 minutes after each start, then once a day) and to
  download one when you choose to install it. You can turn the daily check off.

If you set a location, the weather and outdoor air are fetched **by your browser, not by the unit,** from Open-Meteo, Zippopotam.us
and the FCC's Area API. As with any website, those services see your internet address, and your browser also tells them the
address you opened the unit's page at.

## Security on your network

- **Turn on password protection** (Settings, Password protection). It's off at first, and until you turn it on, anyone on your
  network can open the unit's page, see your worker name, Wi-Fi name and location, and change any setting. Choose a long
  password, not something easy to guess: the unit slows guessing to about one try every 3 seconds, but anyone on your network can
  keep trying.
- The page and password travel unencrypted on your network. A password keeps other people on your network out, not someone who can
  watch its traffic.
- **Forgot the password?** Start with the panel's Power on, then press Power 10 times, about 1 second apart, within a minute (off
  and back on, five times), so it ends back on. Only password protection turns off.
- **Give your Wi-Fi a WPA2 or WPA3 password.** On an open network, someone nearby could put up a network with the same name, and
  the unit could join theirs instead of yours. With a password, the unit joins only a network that knows it.
- **The unit's own Wi-Fi network is open.** During setup your home Wi-Fi password is sent over it, so set up close to the unit and
  finish promptly. It closes two minutes after the unit joins your Wi-Fi.
- **It comes back if your Wi-Fi goes away** for 10 minutes, so a new router or password can be set from your phone. Anyone in
  range can join it and open the unit's page; with protection off, they can see everything the page shows. Over that network the
  unit takes only a sign-in and a new Wi-Fi network, and with protection off a new Wi-Fi network also needs you at the unit: turn the
  panel's Power off and on within 10 seconds, then save within 5 minutes. A password is the better protection.
- **Keep backup files private.** ChippyOS's saved settings in them, passwords included, are scrambled, not encrypted, and Heatbit's
  own settings, your Wi-Fi password among them, are kept as Heatbit's firmware stores them, which may be readable.
- **Before you sell or give away a unit,** use Forget settings (Settings, Danger zone), or return it to Heatbit's firmware: either
  clears ChippyOS's settings. Heatbit's own Wi-Fi and account settings stay on the unit, as Heatbit's firmware keeps them; to
  take the unit off your Heatbit account, use Disconnect this device on the Bitair's settings page in the Heatbit app.

## Help

Ask a question or report a problem [here](mailto:support@hashboardapp.com?subject=ChippyOS%20-%20Bitair%20Issue). Please leave
out your worker name or wallet address, Wi-Fi name, location, passwords, and IP or MAC addresses. To include the log, keep the log
open (the Logs button in Settings) while the problem happens, then use its Download, which hides most of these. Read the file
before you attach it.

## Terms

ChippyOS is free to use, but not open source. Its license terms are in [LICENSE](LICENSE). It comes with no warranty, and you
install and run it at your own risk: it changes how your unit runs.

ChippyOS includes open source software from others, listed with their licenses at
[chippyos.com/ChippyAir/licenses.html](https://chippyos.com/ChippyAir/licenses.html) and in [NOTICES.md](NOTICES.md).
