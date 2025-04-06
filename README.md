# Spoofer – Universal Spoofing Tool for HWID, MAC, IP, DNS, Location, Device ID and more

![Status](https://img.shields.io/badge/status-active-brightgreen)

**Spoofer** is a universal spoofing toolkit that allows you to mask or change virtually any device identifier – from your PC’s hardware IDs to your phone’s GPS location – all in one application. This open-source tool is designed for a wide range of users: gamers seeking to bypass hardware bans, mobile users faking GPS locations (e.g. in Pokémon GO), developers testing apps under different device profiles, and privacy enthusiasts wanting to reduce tracking. Spoofer supports multiple spoofing types (Hardware ID, MAC address, IP address, DNS, GPS location, and mobile device ID) and is compatible with Windows, Linux, and Android (with limited iOS support via external methods).

### This video works for every game/app etc. ▶️▶️
[![Spoofer Setup Guide](https://img.youtube.com/vi/b8XyEwxpccE/0.jpg)](https://www.youtube.com/watch?v=b8XyEwxpccE)

## Overview

**What is a universal spoofer?** A universal spoofer is an all-in-one solution that disguises or alters a device’s identifying information across various categories. In technical terms, spoofing is a technique to **impersonate another device or manipulate how systems recognize your device**​

. Normally, achieving this requires separate tools or manual tweaks for each identifier (one program for MAC addresses, another for GPS location, etc.). Spoofer brings these capabilities together under one roof with a unified interface. This means you can change your hardware serials, network addresses, and geolocation from one toolkit, simplifying the process and ensuring the changes play well together.

**Why use Spoofer?** There are many legitimate scenarios for device spoofing:

-   **Bypass Hardware Bans in Games:** If you’ve been HWID-banned by an anti-cheat system, you can spoof hardware identifiers to appear as a new PC and regain access.
    
-   **Privacy on Public Networks:** Randomize your MAC and IP address to avoid tracking on Wi-Fi hotspots and hide your online identity from snoopers.
    
-   **Access Region-Locked Content:** Change your apparent IP location or GPS coordinates to use services and games available in other regions (or to play location-based games remotely).
    
-   **Testing and Development:** Developers can simulate different device environments (new device IDs, varied network settings, fake locations) to test app behavior.
    
-   **Fun and Miscellaneous:** Play AR games like Pokémon GO by “teleporting” your location, or prank friends by appearing to be in a different part of the world.
    

Spoofer is designed to be **user-friendly** – offering both a graphical interface with presets and a command-line interface for advanced scripting. It does not require deep technical knowledge for basic usage; each feature comes with guidance. Under the hood, Spoofer carefully modifies system parameters or routes your connection as needed, but it does **not** permanently alter hardware. Most spoofing actions are temporary or virtualized, meaning they can be reversed by rebooting or disabling the spoofer (except where you choose to apply persistent changes). This approach ensures that you can safely test the waters of spoofing without permanently messing up your device.

## Table of Contents

-   Overview
    
-   HWID Spoofing (Game Ban Bypass)
    
-   MAC Address Spoofing
    
-   IP Address Spoofing
    
-   DNS Spoofing
    
-   Location Spoofing (GPS)
    
-   Device ID Spoofing
    
-   Installation & Usage
    
-   Video Tutorial
    
-   FAQ
    
    -   HWID Spoofing FAQ
        
    -   MAC Spoofing FAQ
        
    -   IP Spoofing FAQ
        
    -   DNS Spoofing FAQ
        
    -   Location Spoofing FAQ
        
    -   Device ID Spoofing FAQ
    
-   Disclaimer
    

## HWID Spoofing (Game Ban Bypass)

**What is HWID and why spoof it?** HWID stands for Hardware ID, which is a unique fingerprint of your computer derived from hardware component identifiers (e.g. motherboard serial, disk volume ID, network card MAC, etc.). Many modern online games impose **HWID bans** to crack down on cheaters – meaning if you’re banned, the game blocks not just your account but your **computer’s hardware** from connecting​

. This is a particularly tough punishment since creating a new account won’t help if your device is flagged. HWID spoofing makes your machine look like a different computer by altering those hardware identifiers that games track. It’s essentially a way to dodge the “hardware ban” so you can play again without buying a new PC.

**Spoofer’s HWID module:** Spoofer can temporarily change or mask all the key hardware identifiers that anti-cheat systems commonly log. With one click, it will:

-   Generate new serials for your motherboard, BIOS, CPU, GPU, and disk drives (without flashing your firmware).
    
-   Reset or randomize unique system GUIDs and product IDs stored in the registry.
    
-   Optionally change your network adapter’s MAC address (also covered in the MAC section below) if the game links that to your HWID.
    
-   Clear out certain files/registry entries that anti-cheat programs use to track banned systems.
    

By doing this, **Spoofer makes it appear as if you are using a different PC** to the game’s servers​

[github.com](https://github.com/yoga5535/HWID-Spoofer-Hardware-ID-Changer#:~:text=HWID%20bans%20are%20one%20of,for%20anyone%20facing%20such%20restrictions)

. It also includes a “cleaner” function that **wipes leftover ban traces** (such as cached user identifiers or log files from your system)​

. These steps are essential because games often employ both hardware scanning and software checks; simply changing one ID might not be enough if traces of the old banned identity remain​

.

_Example use-case:_ Imagine you were banned in a game like _Fortnite_ or _Valorant_ for a violation. After installing Spoofer and running the HWID spoof, your system will report different hardware serial numbers. You’d then create a new game account and be able to play again as if on a fresh machine. Gamers have found HWID spoofing to be a quick way to get unbanned and continue playing their favorite games​

– just be sure not to repeat the original offense, or you risk getting banned again on the new IDs!

**How to use HWID Spoofing:** Close any running games and launch the Spoofer application on Windows. Navigate to the **Hardware ID** tab (or run `spoofer.exe --hwid` via command-line). You’ll see a list of hardware components with checkboxes – by default, all common identifiers are selected to be spoofed. You can customize which IDs to spoof if needed (for example, you might leave your disk serial unchanged if you’re concerned about Windows activation, as explained below). Click the **“Spoof HWID”** button, and the tool will begin applying changes. Within seconds, it will prompt you to restart your PC to finalize certain changes (like registry-level IDs). After reboot, your PC is effectively “new” to the games. You can confirm the changes by checking logs in the Spoofer interface, which will show new randomized IDs for each component.

**Note:** HWID changes made by Spoofer are **temporary in software.** They will persist until you decide to revert them or (in some cases) until a Windows update or major hardware reconfiguration occurs. You can restore your original HWID via the Spoofer tool’s **Restore** function, which puts back your real hardware values from a backup it creates. This means you don’t have to worry about permanently losing your PC’s identity – Spoofer ensures you can always go back.

## MAC Address Spoofing

**What is a MAC address?** A MAC (Media Access Control) address is the unique identifier assigned to your network interface card (wired or wireless). For example, your Wi-Fi card has a MAC address like `AB:CD:EF:12:34:56` that identifies it on local networks. Normally, MAC addresses are hard-coded in hardware, but they can be overridden in software (this is what MAC spoofing does). MAC addresses are used only on the local network segment, not across the internet, but they can still be used to track devices or restrict network access. For instance, some Wi-Fi networks use MAC filtering to only allow known devices, and public networks can log your MAC when you connect.

**Why spoof your MAC?** The primary reasons are **privacy and bypassing network filters.** If you connect to a public Wi-Fi or a campus network, your device’s MAC can be recorded; by spoofing it (changing it to a random new value), you make it harder to be tracked or identified next time. Privacy-conscious users consider MAC spoofing a basic step, since otherwise your devices broadcast the same MAC everywhere they go. In fact, modern operating systems have started implementing random MAC address features for Wi-Fi for this reason (Android, iOS, Windows 10+ can use randomized MACs when scanning or connecting to networks). Additionally, if a network or service has blocked your device’s MAC (or if an ISP only permits one specific MAC to use their service), spoofing can let you circumvent that restriction by impersonating an allowed device’s address​

[en.wikipedia.org](https://en.wikipedia.org/wiki/MAC_spoofing#:~:text=Many%20ISPs%20%20register%20the,this%20is%20generally%20a%20legitimate)

​
. Spoofing your MAC is **legal in most jurisdictions** (it’s essentially like changing the license plate on your own car)​

, though its misuse can raise controversy in certain cases (e.g., it was noted in a famous court case involving Aaron Swartz)​

.

**Spoofer’s MAC module:** Spoofer provides a quick way to change your MAC address on Windows, Linux, or Android:

-   On Windows, it utilizes the registry/driver method to set a new MAC for the selected network adapter (Ethernet or Wi-Fi) and then resets the adapter so the new MAC takes effect.
    
-   On Linux and macOS, it can issue the appropriate system commands (like `ifconfig`/`ip` or `networksetup`) to bring an interface down and back up with a new MAC.
    
-   On Android, if you have root access, Spoofer’s companion app can change the Wi-Fi MAC by manipulating system files or network interfaces. (On Android 10+, non-root MAC randomization is often enabled by the OS for Wi-Fi networks, but our tool gives you control to set your own value when rooted.)
    

You can choose to **randomize** the MAC (Spoofer will generate a random address each time, preserving the vendor prefix by default), or **set a specific MAC** of your choice. Setting a specific MAC can be useful if you want to **impersonate another device** – for example, if you have a router that only allows a certain MAC to connect, you could copy that. Spoofer also checks that the new MAC isn’t in use on your current network to avoid conflicts.

_Example use-case:_ You are at a library that only gives one hour of internet access tied to your device’s MAC address. After your hour is up, you can run Spoofer to change your MAC, and the network will see you as a new device – granting another hour. Another example: your ISP locks your connection to the first device you connect (recording its MAC). Instead of rebooting the modem when you want to switch devices, you can just spoof your new device’s MAC to match the old one to get instant access​

. These legitimate uses show how MAC spoofing can save time and bypass arbitrary limits.

**Using MAC spoofing:** In the Spoofer interface, go to the **Network** or **MAC Spoofing** section. You’ll see a list of network interfaces (e.g., “Ethernet – Intel(R) XYZ” or “Wi-Fi – Qualcomm ABC”). Select the interface you want to modify. You have two options: click **“Randomize MAC”** to have the tool pick a new address for you, or enter a specific MAC value in the field (the format is `XX:XX:XX:XX:XX:XX`). Then click **“Apply”**. Your network connection on that interface will momentarily drop as the adapter resets. Within a few seconds, it comes back up with the new MAC. Spoofer will display the old and new MAC for confirmation. You can verify it manually by typing `ipconfig /all` on Windows or `ifconfig` on Linux – you should see the MAC you set. The new MAC will remain active until you either change it again or disable spoofing. Spoofer can also restore the original MAC (it remembers the factory MAC) if you hit **“Restore original”**.

**Note:** MAC spoofing effects are usually **temporary** – if you reboot your computer or turn your Wi-Fi off and on, the system might revert to the hardware MAC unless the spoof is re-applied. Spoofer can be set to re-apply your chosen MAC at startup (there’s a toggle for “Apply on boot” for Windows/Linux). On Android, a reboot will reset to the real MAC, since our changes are in-memory (except on some rooted setups where you can make it persistent). Also note that MAC spoofing only affects the local network; it does _not_ hide your public IP on the internet. For that, see IP spoofing below.

## IP Address Spoofing

**What is IP spoofing in this context?** Typically, “IP address spoofing” refers to faking the source IP in network packets – a tactic used in certain cyberattacks to hide the sender or impersonate another system​

. However, in normal two-way communications, you **cannot simply send out packets with a false IP** and expect to get data back – the responses would go to the faked address. So, for everyday use, IP spoofing means **hiding or changing your public IP address** seen by websites or game servers by routing your traffic through another server. In practice, this is achieved by using proxies or VPNs. Spoofer’s IP module functions essentially as a user-friendly VPN/proxy tool integrated with the other spoofers.

**Why spoof your IP?** Two main reasons: **ban avoidance** and **privacy/geo-access**. If you’ve been IP-banned from a service or game (e.g., a forum blocked your IP, or a game server bans by IP in addition to account), changing your IP lets you regain access. Also, by changing your IP you can appear to be in a different region – many people use this to access region-locked content (like video streaming services or game servers not normally available in their country). From a privacy standpoint, using a different IP (especially one not easily traced to you) can help mask your online activity from websites or trackers. While it’s not complete anonymity, it prevents basic IP-based tracking and profiling.

**Spoofer’s IP module:** Spoofer offers a built-in VPN/proxy integration to **route your internet traffic through a different IP**. We maintain a small network of VPN servers in multiple regions that the tool can connect to (similar to a commercial VPN service). Alternatively, you can configure your own proxy/VPN details if you prefer. The module supports both full tunneling (all applications go through the new IP) and app-specific or game-specific tunneling (on Windows, it can create a proxy that you point a particular game to).

Key features:

-   Choose from multiple server locations (e.g. **USA, Europe, Asia** servers available). For example, selecting a European server will give you a European IP address.
    
-   Secure encryption: Spoofer uses standard VPN protocols (OpenVPN/WireGuard) under the hood, so not only is your IP changed, but your traffic is encrypted for safety when on public networks.
    
-   Kill-switch: If the VPN connection drops, Spoofer can temporarily cut internet connectivity to prevent your real IP from leaking.
    

_Example use-case:_ You were banned from a game’s servers by IP. Before launching the game, you use Spoofer to connect to a new IP address (say via a Germany server). Now the game sees you coming from that German IP and the ban is circumvented (assuming your new IP isn’t also banned for someone else). In another scenario, let’s say you want to play a game that’s only released in Japan. You can connect Spoofer’s IP module to a Japan node, and the game’s launcher will think you have a Japanese IP, potentially allowing download/play. This also works for websites – e.g., accessing a video or site that’s “not available in your country”.

**Using IP spoofing:** Open the **IP Spoofing** or **VPN** section in Spoofer. You’ll see a list of regions or a map. Select your desired location (or enter custom VPN credentials in advanced settings). Click **“Connect”**. The first time, you may need to grant network/tunnel permissions (Windows will ask to allow the VPN, Android will show a confirmation dialog for VPN usage). Once connected, you’ll see your new IP address displayed. All internet traffic on your device now goes through that IP. You can verify by checking your IP on an external site (Spoofer provides a “Check my IP” button which opens a webpage that shows the IP, or use `ping icanhazip.com` from command line).

If you only want a specific app to use the spoofed IP (for instance, route a game through a proxy without affecting the rest of your PC), you can use **proxy mode**: Spoofer will give you a local SOCKS proxy address (e.g. `127.0.0.1:1080`) after connecting, which you can configure in that application. By default, however, it’s simplest to use the full VPN mode to cover all apps.

**Note:** While using the IP spoof/VPN, your connection speeds might be slightly lower and your latency higher (especially if connecting to a far-away region). This is normal for VPN usage. Also, remember that **this does not make you invincible** – websites or games will see a different IP, but other identifiers (cookies, accounts, hardware ID, etc.) can still link back to you if not changed. For true anonymity, additional steps are needed beyond the scope of Spoofer. Our goal here is to make changing your IP easy for the purposes of ban bypassing and basic privacy, not to facilitate illegal activity. We do not condone using IP spoofing for any malicious attacks (as in true packet-level IP spoofing used in DDoS attacks​

– Spoofer does not provide tools for that kind of activity).

## DNS Spoofing

**What is DNS spoofing?** DNS (Domain Name System) is what translates human-friendly addresses (like `example.com`) to IP addresses that computers use. DNS spoofing, also known as DNS cache poisoning, traditionally refers to an attack where false DNS entries are inserted into a DNS server or resolver cache​

. For example, an attacker could cause `bank.com` to resolve to a malicious IP. In our context, we are _not_ attacking anyone’s DNS – instead, we’re essentially performing **local DNS spoofing** on _your own device._ This means **overriding DNS entries on your machine** so that certain domain names resolve to IPs you specify. It’s like editing the phone book that your computer uses, for fun and profit (and testing).

**Why spoof DNS locally?** There are several benign and useful reasons:

-   **Custom Servers / Modding:** Gamers may use DNS spoofing to redirect a game’s server address to a fan-made server. For instance, an online game might always connect to `official.game.com`; by spoofing that to an IP of a private server, you can play on unofficial servers without modifying the game client.
    
-   **Blocking or Filtering:** You can effectively “block” certain domains by spoofing them to an invalid address (like `127.0.0.1` which is your own machine). This is a common technique to block ads or malicious domains system-wide.
    
-   **Bypass DNS-based censorship:** If your ISP or network blocks a website by hijacking DNS (e.g., returning an error or wrong IP), you can override it with the correct IP of the site (assuming you know it or can get it via an alternative DNS service). This gets around basic DNS-level blocking.
    
-   **Testing and development:** Developers can map a production domain to a localhost or test server for debugging, without changing configs in multiple places. Just add an override: `myapi.com -> 127.0.0.1` when you want to test against a local instance.
    

**Spoofer’s DNS module:** Spoofer provides an easy interface to manage custom DNS mappings (similar to editing the hosts file, but with a nicer UI and without the risk of syntax errors). Under the hood on Windows and Linux, it modifies the hosts file or runs a lightweight local DNS service depending on complexity of rules. On Android (with root), it can modify the hosts file as well; without root, DNS changes system-wide are not possible, but Spoofer does offer an _in-app VPN-based DNS interceptor_ (so if you enable the VPN mode, it can intercept DNS queries and respond with your custom entries).

Features:

-   Add, edit, remove DNS entries (domain-to-IP mappings).
    
-   Wildcard domain support (e.g., redirecting any subdomain of `example.com` to a given IP).
    
-   Flush DNS cache button – after making changes, Spoofer will flush the OS DNS cache so changes take effect immediately.
    
-   Preconfigured templates for common uses (like “Block Telemetry” which adds known tracking domains to 0.0.0.0).
    

_Example use-case:_ Let’s say you play a mobile game that has an official server and a fan-run server. The game client doesn’t let you choose – it always connects to `game.example.com`. The fan server admin gives you an IP like `5.6.7.8` to use. You add an entry in Spoofer: `game.example.com -> 5.6.7.8`. Now when the game runs on your device (with Spoofer’s DNS spoof active), `game.example.com` will resolve to `5.6.7.8` instead of the real official IP. The game will unknowingly connect to the fan server. When you want to go back to official, you just disable or remove that entry.

Another example: You want to block `analytics.example.com` (an annoying tracker domain present in some apps). Adding `analytics.example.com -> 0.0.0.0` will blackhole those requests – the domain will just resolve to nowhere.

**Using DNS spoofing:** Open the **DNS Spoofing** section in Spoofer. You’ll see a table of custom DNS entries (initially it might be empty or have a few example entries commented out). To add a new mapping, click **“Add Entry”**. Enter the domain name (e.g. `pokemon.go.com`) and the IP address you want it to go to (e.g. `127.0.0.1` or another IP). You can add a comment for your reference. Click **Save**. The new rule is now active. If you try to visit that domain (or if an app tries to connect), it will go to the IP you set.

If you want to disable a mapping without deleting it, you can uncheck the enabled box next to it. Changes are applied on the fly; Spoofer will ensure the system’s DNS cache is updated accordingly. There’s also a **“Flush DNS”** button you can use if needed (on Windows this runs `ipconfig /flushdns` internally, on Linux `systemd-resolve --flush-caches` or similar, on Android it toggles the DNS listener).

**Note:** Be careful with DNS spoofing – it can lead to confusion if you forget about an entry. For example, if you map a domain to localhost for testing and then later that service isn’t running, you might wonder why the site is down. Always remove or disable entries that you no longer need. Also, understand that this only affects your device’s resolution of names. It doesn’t “hack” other devices’ DNS. (In other words, using Spoofer to redirect `netflix.com` to some other IP will _not_ give you free Netflix – your device would try another IP but the real Netflix service won’t be there!). Use this feature for legitimate purposes like testing, customization, or blocking unwanted content.

## Location Spoofing (GPS)

**What is location/GPS spoofing?** Many apps and games use your device’s GPS or location services to provide features or enforce restrictions. Location spoofing is making your device report a fake GPS location, different from where you actually are. This can be done by sending out false GPS signals or manipulating the location data that apps receive​

. On smartphones, this is often achieved via “mock location” developer options or specialized apps. On a PC (with no GPS), location is usually determined by network data or manually set in browser – Spoofer can also influence that by simulating coordinates.

**Why spoof your location?** The most popular example is **Pokémon GO spoofing** – players of the AR game have historically used location spoofers to teleport to different cities and catch region-exclusive Pokémon without traveling​

. By 2025, spoofing in Pokémon GO remains popular (albeit against the game’s terms). Aside from games, people spoof location in apps like dating apps (to see profiles in other cities), social media (to tag a different city on a post), or any location-based service to test or access features elsewhere. Privacy is another reason: maybe you don’t want every app to know exactly where you live, so you feed a generic fake location. Some users also spoof GPS when testing geofencing in apps – developers can simulate moving around the globe to test how their app behaves.

**Spoofer’s location module:** Spoofer enables GPS location spoofing primarily on **Android devices** (and Android emulators). It offers:

-   A **map interface** where you can pick a location or search for a place, and set that as your device’s current location.
    
-   A **Joystick mode** (on Android) that overlays a small joystick on your screen, allowing you to move your fake location gradually – useful for games like Pokémon GO to walk around virtually without triggering alarms by teleporting too abruptly.
    
-   Support for setting custom speed and routes (you can draw a path on the map and have the app simulate walking or driving along that path).
    
-   Cooldown timer guidance for games: if you jump long distances, Spoofer will advise a cooldown period (e.g. if you jump from New York to London, wait X hours) based on community guidelines to avoid bans.
    
-   On **iOS devices**, Spoofer cannot directly run (unless jailbroken), but we provide a companion desktop tool that can spoof an iPhone’s location when connected via USB (leveraging Apple’s developer debug features). This is a bit more advanced and not as seamless as on Android, but it’s available for iOS users who can’t jailbreak.
    

_Example use-case:_ You’re playing Pokémon GO and you live in a rural area with few Pokéstops. Using Spoofer on your Android phone, you open the map and select Central Park in New York as your new location. Instantly, Pokémon GO thinks you’re in Central Park – now you can catch Pokémon specific to that area and access many Pokéstops. You use the joystick to “walk” around the park within the game. Meanwhile, Spoofer’s cooldown timer notes how far you moved and reminds you to wait an appropriate amount of time before jumping to another far location, to avoid Niantic’s automated bans​

. Another scenario: You’re testing a delivery app that only activates in certain cities. Rather than physically traveling, you spoof your GPS to that city and test the app’s functionality.

**Using location spoofing (Android):** On your Android device, you need to do a one-time setup: enable **Developer Options** (by going to Settings > About Phone and tapping Build Number 7 times), then in Developer Settings enable **Allow mock locations** and set the **Spoofer app as the mock location provider**. (Spoofer’s app will guide you through this the first time). Once set, open the **Location Spoofing** feature in Spoofer. You’ll see a map. You can pan/zoom or use the search bar to find a place. Tap on the map to drop a pin at your desired fake location. A marker appears – tap the marker and hit the **“Set Location”** button. Now your GPS coordinates are fixed to that spot. If you enable joystick mode, a floating joystick will appear; use it to move north/south/east/west gradually – the map will update and your device’s location will follow accordingly.

If you want to simulate movement along a route, tap the **Route** icon, then draw a path on the map or pick a preset route. Set a movement speed (walking, cycling, driving speeds). Start the route, and Spoofer will start “moving” your GPS along that line. You can pause or stop anytime. While the spoof is active, apps that request location will get the fake coordinates. You can confirm by opening Google Maps – it should show you at the spoofed location (just be careful not to let Google Maps navigate you off-course, as it might use other signals like Wi-Fi; typically, however, the mock location overrides everything).

For desktop usage (Windows) to spoof an iPhone’s location: connect your iPhone via USB, open Spoofer on PC, go to the iOS Location tab. Enter a latitude/longitude or search for a place, then click “Set iPhone Location”. The tool uses Apple’s API to simulate that location on the device. It’s a bit slower and cannot live-move with joystick, but you can teleport and set static locations this way. (Note: this requires the iPhone to trust your computer and have the proper drivers or iTunes installed).

**Note:** **Use location spoofing responsibly.** Apps like Pokémon GO have policies against it – if you violate their rules aggressively, you risk temporary or permanent bans (e.g., a soft ban of ~2 hours for a first offense of jumping too far​

). Spoofer provides tools (like cooldown timers and realistic movement simulation) to help mitigate detection, but there’s always risk if you’re manipulating a game. Also, remember to turn off the spoof and return to your real location before using apps that rely on genuine location (e.g., don’t leave your phone mapped to New York if you’re actually in London when using Uber or you’ll get very confused drivers!).

## Device ID Spoofing

**What do we mean by Device ID?** This refers to various unique identifiers of a **mobile device** (or emulator) beyond just the MAC or IP. On Android, a key one is the **Android ID** – a 64-bit identifier that Android assigns on first setup (and which apps commonly use to uniquely identify your device). There’s also the **IMEI** (for devices with cellular radios), the **MEID/ESN**, the SIM’s IMSI and phone number, the hardware serial number, etc. On iOS, there was historically the **UDID** (Unique Device ID) which is now deprecated for apps, and instead iOS has an **Identifier for Vendors (IDFV)** per app vendor, and an **Identifier for Advertising (IDFA)** for ad tracking. Emulated devices (like BlueStacks, Nox, etc.) often emulate these IDs or have their own identification strings and model names.

Apps and games might ban or track devices using some of these IDs. For instance, some mobile games will ban a device so that even new accounts on that same phone get flagged. Or an app might enforce a “one trial per device” limit using the device ID. **Device ID spoofing means altering these identifiers so the device looks like a different/new device.**

**Why spoof device IDs?** If you’ve been device-banned in a mobile game (common in games like PUBG Mobile, for example), changing your device IDs can let you play again without buying a new phone. It’s also useful for testing apps – e.g., QA testers might need to simulate many unique devices. Privacy-wise, resetting or changing your device’s identifiers can help decouple your activities (some people regularly reset their advertising ID to avoid targeted profiling; Spoofer can automate that). In emulator environments, device spoofing can help avoid detection (some apps try to detect if you’re on an emulator by checking device model or certain IDs; if you spoof those to realistic values, the app might assume it’s a real phone).

**Spoofer’s device ID module:** Spoofer’s capabilities here are mostly for **Android (rooted)** or **Android emulators**. This feature is advanced and should be used with caution:

-   It can change your **Android ID** (the Settings Secure ID). Normally changing Android ID requires root or a factory reset​
        
    . Spoofer (with root privileges) will edit the appropriate system settings database to set a new random Android ID.
    
-   It can randomize your **Device build fingerprint, model, manufacturer, and other build.prop properties** on rooted devices. This makes the phone present itself as a different model (e.g., you can make a Samsung phone look like a Google Pixel to apps). On emulators, it can alter the emulator config or build.prop similarly.
    
-   For rooted devices, it can spoof the **IMEI** of the device if needed (note: this is experimental and may not work on all devices; also IMEI spoofing can violate carrier policies and is illegal in some regions, so it’s turned off by default and hidden under an “Advanced” toggle with warnings).
    
-   It can reset the **Advertising ID** (which normally you can do in Android settings manually – Spoofer just automates it).
    
-   For iOS (jailbroken only): There is limited support via a tweak that can change the device name, and possibly the IDFV/IDFA if you use additional tools, but Spoofer’s direct support for iOS device ID spoofing is minimal. If you’re on jailbroken iOS, you might use third-party tweaks like “UDID faker” in conjunction with our guidelines.
    

In an Android emulator scenario (say you’re using BlueStacks on PC), Spoofer’s PC application can connect to the emulator and modify its configuration files to change the emulated phone model, IMEI, GUID, etc. Many emulator users do this to evade game checks that normally block emulators or to get around device bans affecting the emulator’s virtual hardware.

_Example use-case:_ You got banned in a mobile game on your Android phone. They banned not just your account but your device – any new account you create on that phone gets insta-banned. Using Spoofer (with root), you change your Android ID, device model, and reset the advertising ID. Now, to the game’s servers, your phone looks like a completely different device. You create a new account and the ban no longer applies. Another scenario: You use a dating app that only allows one account per device; you want a second account, so you clone the app and spoof your device identifiers so the app thinks it’s on a different phone, allowing a second account login.

**Using device ID spoofing (Android):** **Important:** This feature requires root access on Android. Ensure your device is rooted and you grant Spoofer root (superuser) permissions when prompted. In Spoofer’s **Device ID** section, you will see various fields (Device Model, Manufacturer, Android ID, etc.) with current values and options to change them. You can hit **“Randomize All”** to generate a new device profile automatically (it will pick a popular device model from a list, randomize the IDs). Or you can manually edit specific fields. For example, you might type “SM-G975F” as the model (to pretend to be a Galaxy S10) and adjust manufacturer to “Samsung”. For Android ID, you can click “New ID” to randomize it.

After making changes, click **“Apply Device Profile”**. The app will apply changes to system settings. For some changes (like build fingerprint), you will be asked to reboot the device for them to take effect (especially if they are in build.prop). Spoofer will remind you if a reboot is needed. Once rebooted, your device will be presenting the new identity. You can verify by going to Settings > About Phone to see the model name, or using any device info app to check Android ID etc., which should now show the spoofed values.

If you’re using an **Android emulator** on PC, launch the emulator and the Spoofer desktop app. Go to the emulator section, select which emulator (currently BlueStacks and Nox are supported). You’ll see similar options to spoof the emulator’s reported device model, IMEI, GUID, etc. Apply and restart the emulator.

**Note:** Spoofing device IDs can have side effects. Changing things like your device model can make some apps behave differently (you might get a different version of an app from the Play Store if it thinks you have a different device, for example). Also, if you change an IMEI or certain cellular identifiers on a real phone, your phone’s ability to make calls or use mobile data could be affected until reverted. Spoofer by default does **not** spoof the IMEI unless you explicitly enable that advanced option, specifically to avoid interfering with your phone’s network registration. Typically, for game ban purposes, changing the Android ID and maybe device fingerprint is sufficient. Always keep note of your original IDs (Spoofer does attempt to save original values when possible; use the Restore button to put them back). And as always, ensure you are not violating any laws – e.g., in some countries, altering IMEI is illegal. Our tool is intended for legitimate uses such as testing and ban recovery under fair use.

----------

## Installation & Usage

Spoofer consists of a **Windows application** (which also covers Linux/macOS functionality via command-line tools) and an **Android app**. Below are step-by-step instructions to get started:

### 1. Download and Install

-   **Windows:** Download the latest release from our GitHub Releases page (it’s a portable `.exe` for now). Optionally, you can compile from source using Visual Studio (see CONTRIBUTING.md for build instructions). No installation is required – but it’s recommended to run Spoofer as Administrator on Windows (right-click -> Run as Administrator) so that it can modify system settings.
    
-   **Linux/macOS:** We provide a Python-based CLI in the repository. Install Python 3 and run `pip install spoofer-tool` to get the `spoofer` command. (GUI is coming soon for Linux/macOS.) Note: On Linux, you’ll need to run the tool with root privileges (e.g., `sudo spoofer ...`) for it to change MAC or DNS settings.
    
-   **Android:** Download the Spoofer APK from Releases and install it on your device. You will need to enable “Install from unknown sources” since it’s not on the Play Store. The app is called “Spoofer” with our logo. If your device is not rooted, you’ll still be able to use the location spoofing and IP VPN features; for device ID spoofing and MAC spoofing on Android, root is required.
    
-   **iOS:** No direct app (App Store rules forbid this kind of tool). If you are jailbroken, you can manually use some open-source tweaks in conjunction with our documentation. If not jailbroken, you can use the Windows Spoofer application when your iPhone is connected to leverage the limited location spoof support as described earlier.
    

### 2. Preparation and Compatibility

-   **Windows prep:** Close any applications (especially games) that you plan to spoof things for, to ensure Spoofer can access all necessary resources. It’s also wise to temporarily disable any antivirus that might interfere with tools that change system settings (some antivirus software might flag a tool that changes MAC or registry as suspicious – our code is open-source so you can verify it’s safe).
    
-   **Android prep:** Enable Developer Options if using location spoofing, and enable root (Magisk/SU) if using device ID spoofing. Grant the app location permissions (for it to be able to control GPS) and root permissions when prompted.
    
-   **Network prep:** If you plan to use the VPN/IP spoofing, ensure your network allows VPN connections (some restrictive networks might block VPN protocols). Also, on Windows, the first time you start the IP spoof, Windows Firewall might ask to allow it – choose “Yes” or “Private Networks”.
    

### 3. Using Spoofer – Quick Start

Now you’re ready to spoof! Here’s a quick step-by-step for a common scenario (bypassing a game ban):

1.  **Launch Spoofer (Windows):** You’ll see the main dashboard with buttons for each spoofing category.
    
2.  **HWID Spoof:** Click “HWID Spoof” and then “Spoof HWID” with default settings. Within a few seconds, it will prompt to reboot. Reboot your PC.
    
3.  **IP Spoof:** After reboot, launch Spoofer again. Go to “IP Spoof” and connect to a VPN server of your choice (pick one near your target game server for lower ping).
    
4.  **MAC Spoof (optional):** If the game also banned your MAC or you just want extra caution, go to “MAC Spoof”, select your network adapter, and hit “Randomize MAC”. Your internet will reconnect with a new MAC.
    
5.  **Launch the Game:** Now open your game. It should not recognize your hardware or IP – you appear as a new user. Create a new account if required. Play the game.
    

For other use-cases:

-   **MAC spoofing for privacy:** Simply use the MAC module each time you connect to an untrusted Wi-Fi. You might set Spoofer to auto-run on login and auto-randomize your Wi-Fi MAC for you.
    
-   **Location spoofing on phone:** Open Spoofer app -> Location -> choose location -> enable. Then minimize Spoofer and open your location-based app. When done, either stop the spoof or just close the app (you can quickly toggle the mock location off in Spoofer to return to real location).
    
-   **DNS spoof for custom server:** On Windows, add the DNS entry in Spoofer, hit apply. It will edit your hosts file (you may see a UAC prompt if not running as admin – allow it). Then launch the game/app that uses that domain. It will now go to the spoofed IP.
    

### 4. Verification (recommended)

After spoofing, it’s good practice to verify the changes:

-   For **HWID**, you can use tools like `wmic` commands or built-in DXDiag to see if some identifiers changed, but some are tricky to verify. A quick check: in Spoofer’s HWID tab, it will list old and new values for each component – review those.
    
-   For **MAC**, open a command prompt and type `getmac` or `ipconfig /all` and ensure the MAC matches what you set.
    
-   For **IP**, visit a site like whatismyip.com to confirm it shows the new IP/location.
    
-   For **DNS**, use `nslookup domain.name` in a terminal to see where it resolves – confirm it shows the IP you set.
    
-   For **Location**, open a maps app or a GPS status app to ensure it thinks you are at the new coordinates.
    
-   For **Device ID**, install an app like Device Info HW on your phone to read out the device ID, Android ID, etc., and see that they changed according to your settings.
    

If any spoofing did not take effect, double-check that you ran the tool with appropriate permissions and followed the prep steps. Some changes (especially HWID) may require a restart or re-opening the target app to take effect.

### 5. Automation and Scripting

Spoofer supports command-line usage for advanced users who want to automate tasks (for example, you could script it to randomize MAC and connect VPN on startup). Run `spoofer.exe --help` (or `spoofer --help` on Linux) to see available commands and flags. You can combine multiple actions in one command. Example:

bash

CopyEdit

`# On Windows, in PowerShell or CMD: spoofer.exe --hwid --mac=random --vpn=us-newyork` 

The above would spoof HWID, spoof the MAC to a random value, and connect to the New York VPN, all in one go. This is useful if you want a one-click or one-command solution to set everything up before launching a game. You can also use the **profiles** feature: save a set of spoofing actions as a profile (e.g., “GameA_Unban”) and later just activate that profile via GUI or CLI.

----------

## Video Tutorial

For a visual demonstration, check out the **Spoofer video tutorial** below. This video walks through the process of using Spoofer for various scenarios (including an example of location spoofing in Pokémon GO):

_Click the thumbnail to watch on YouTube._ In the video, you’ll see how to set up a mock location and safely use it in-game, as well as tips that apply to other spoofing features. (Credits to the video creator for the Pokémon GO spoofing guide.)

----------

## FAQ

Below is an extensive FAQ, categorized by spoofing type, addressing common questions and concerns.

### HWID Spoofing FAQ

**Q: Is HWID spoofing permanent?**  
**A:** No, not by default. Spoofer applies HWID changes at the software/registry level, which generally last until you undo them or reinstall your OS. They are not burned into your hardware. If you reboot your PC, the spoofed HWIDs remain active (because they are stored in Windows registry) – so you don’t need to re-spoof each boot, but if you choose to restore original values, that will revert them. Some identifiers (like RAM serials) can’t truly be changed and are just masked to applications. Essentially, the spoof can persist across reboots _until_ you deliberately restore or Windows resets those values (Windows updates or hardware driver updates might occasionally restore original values). Always keep your original HWID info backed up (Spoofer does this) in case you want to revert.

**Q: Do I need to run the HWID spoofer every time I play a game?**  
**A:** Typically, you run it once before playing on a new account after a ban. The spoofed HWID will stay in effect for subsequent sessions until you change it again. Some people choose to re-spoof (generate new random HWID) every time as an added precaution – that’s up to you. It’s not strictly necessary unless the game somehow detected your new HWID and banned it too, which is rare on first reuse. For safety, you might re-spoof if you’re switching games or after a long time, just to get a fresh identity.

**Q: Can anti-cheat systems detect Spoofer?**  
**A:** We design Spoofer to be as stealthy as possible. It doesn’t remain running in memory during your gameplay except for the VPN part (which just appears as any VPN). The HWID changes it makes are indistinguishable from you simply having different hardware. That said, nothing is 100% undetectable. If an anti-cheat specifically looked for traces of our tool (like known file hashes or opened handles), it could _in theory_ detect it. We have no reports of detection at this time. We also update Spoofer frequently to stay ahead of anti-cheat measures. Many users successfully use it on BattlEye, Easy Anti-Cheat, Vanguard (Valorant) and others without issue. **Important:** Spoofer helps you bypass bans, but if you cheat again and get caught, anti-cheat might ban your new HWID as well. It’s not a license to cheat freely – it’s a second chance tool.

**Q: Will HWID spoofing mess up my Windows or other software?**  
**A:** In rare cases, changing certain hardware IDs could trigger Windows activation to require re-activation. For example, Windows might treat a drastically changed motherboard ID as a new PC​

. In our experience, using Spoofer’s default settings has not deactivated Windows, because it tries to avoid altering the specific combination that Windows uses for license validation. But if it does happen, you may need to log into your Microsoft account and reactivate (or revert the spoof, activate, then spoof again with slightly different settings). Other software that uses hardware binding (some professional software licenses) might also need reactivation if they detect a change. Use the persistent HWID spoof only when needed for gaming – you can always restore originals for doing work that requires your genuine hardware ID. We recommend not spoofing your hardware _unless_ you have a specific need (like a ban), just to minimize any side effects.

**Q: What if I still can’t play even after spoofing my HWID?**  
**A:** If you’ve HWID-spoofed and made a new game account but are immediately getting kicked or banned, it could be due to:

1.  **IP ban or other identifier:** Make sure you also changed your IP (use the IP spoof/VPN) because some games ban IPs. Also clear any game cache or identifiers (Spoofer’s cleaner should handle known ones).
    
2.  **Incomplete spoof:** It’s possible the game is checking something you didn’t spoof. For example, some games might read your monitor’s serial or peripheral IDs (rare, but some anti-cheats are very thorough). Spoofer covers most common ones, but if you suspect something, let us know – we might need to add a new item to spoof.
    
3.  **Kernel-level anti-cheat detection:** A very aggressive anti-cheat might block you if it detects anomalous behavior in the system. This is uncommon for just a spoofer, but ensure no other cheat program is running that could trigger it.
    

In summary, combine HWID, IP, and other spoofers for a clean slate. And don’t log back in with the old banned account at all – that can re-link your new HWID to a ban.

**Q: Does Spoofer also handle game files or registries (“cleaning”)?**  
**A:** Yes, the HWID module includes a cleaning process for various games. It deletes or nulls out known files and registry keys that games use to track past bans (for example, some games drop log files or hidden identifiers on your system). We have a database of these locations which is updated with community input. This cleaning runs automatically when you perform an HWID spoof for a given game profile. Always run the cleaner (it’s on by default) – otherwise a game might still recognize you from those leftover traces even if your HWIDs are changed.

### MAC Spoofing FAQ

**Q: How can I verify my MAC address was spoofed?**  
**A:** After using Spoofer, you can verify the MAC change easily:

-   On Windows, open Command Prompt and type `ipconfig /all`. Find the network adapter you changed and look for “Physical Address”. It should show the new MAC.
    
-   On Linux/macOS, open Terminal and use `ifconfig` or `ip addr show` to see the MAC (HWaddr) for the interface.
    
-   On Android, some devices show the Wi-Fi MAC in Settings > About Phone > Status. You can check there (though some phones might show the factory MAC regardless; in that case, use a network scanner app on another device to see your phone’s MAC on Wi-Fi). If the MAC still shows the old one, the spoof might not have applied – ensure you ran as admin/root and that the network interface was reinitialized.
    

**Q: Will changing my MAC address affect my internet connection or speed?**  
**A:** Only momentarily. When you change your MAC, your network interface typically disconnects and reconnects with the new address. During that reconnection, you might lose network for a second or two and you might get a new IP address from the router (since from the router’s perspective a “new device” connected). After that, everything works as before. MAC spoofing does not inherently slow down your connection – it’s just an ID change. There is no ongoing performance overhead. Just be aware that any existing network sessions (like ongoing downloads) could be interrupted when the MAC changes due to the brief reconnection.

**Q: Is MAC spoofing legal to do?**  
**A:** Yes, generally speaking. There’s no law in most places that forbids altering your device’s MAC address. In fact, major operating systems do it for privacy (randomization features). However, using it to impersonate another device on a network without permission could violate terms of service or, if done for malicious intent, other laws. For example, spoofing your MAC to access an ISP service that you’re not paid for might breach contract. The act of changing your MAC is legal​

; it’s the _use_ that could cross into illegality if you’re doing something like unauthorized access. Spoofer is intended for privacy and legitimate uses, so using it won’t get you in legal trouble by itself.

**Q: My MAC reverts after reboot. How do I make it permanent?**  
**A:** On Windows, if you use Spoofer’s “apply on boot” option, it will re-spoof the MAC at each startup (effectively making it consistently spoofed). Windows doesn’t permanently store a spoofed MAC in all cases – it might for some adapters via registry, but some drivers ignore that. Our tool just sets it each time. On Linux, you can configure a startup script or NetworkManager config to spoof at boot (Spoofer can integrate with those). Essentially, to have a “permanent” spoofed MAC, you either let our tool run at startup to set it, or manually configure your OS to always use the desired MAC. There isn’t a way to change the factory burned-in address except on some hardware/firmware level, but that’s not necessary for most purposes.

**Q: Can two devices share the same MAC address?**  
**A:** Not on the same network segment without causing problems. MAC addresses are supposed to be unique on a local network. If you spoof your MAC to exactly match another device _that is currently on the same Wi-Fi or LAN_, you’ll have an address conflict – network switches/routers will get confused, and one or both devices will have connectivity issues. So avoid duplicating a MAC that’s in use around you. Spoofer generates random MACs by default that preserve the vendor OUI portion, greatly reducing the chance of collision. If you manually set a MAC, double-check it’s not one already active on your network. It’s fine if two devices on _different networks_ share a MAC (since they never meet each other). In fact, many devices come from factory with sequential MACs that eventually repeat by coincidence in the wider world – but locally they must be unique.

**Q: Why do I see a different MAC on the router than in my device settings?**  
**A:** Some modern phones use MAC randomization per network SSID. So, your phone’s settings might show the hardware MAC, but the router sees a randomized one. Or vice versa, if you spoofed via Spoofer, your phone might still show the original in About Phone (some UIs don’t update that display) while the router gets the spoofed one. Trust the network’s view (e.g., what your router’s client list or a PC sees) to confirm what MAC is actually in use.

### IP Spoofing FAQ

**Q: How is Spoofer’s IP spoof different from a normal VPN service?**  
**A:** Under the hood, it is a VPN service – we use standard VPN protocols and you’re essentially connecting to our servers. The difference is integration and automation. Spoofer ties the IP change together with other spoofing actions. It also provides an easy UI for gamers who might not be familiar with VPN setups. Additionally, we allow some flexibility like per-app proxying or quick region switching geared towards gaming (where latency matters). If you already have a favorite VPN, you can absolutely continue using it instead of our IP module – Spoofer doesn’t force you to use its VPN. Just be sure to activate your VPN manually when needed. Our IP spoofing is offered as a convenience so you don’t need a separate app or subscription for basic IP changing. (It’s currently free with fair-use limits, as it’s in beta).

**Q: Can I choose a specific city or just country for the new IP?**  
**A:** At the moment, Spoofer offers region choices by country (and in some cases, east/west for large countries). We have servers in multiple locations in the US, a couple in Europe, and Asia-Pacific. You can’t pick an exact city yet, but usually the IP geolocation will put you near where you want. We plan to label them more granularly (like “US – New York” vs “US – Los Angeles”) in future updates as we expand our network. If you need a very specific location, you can also input a custom OpenVPN config for a server of your choice (say you have a private VPN in a certain city). Spoofer will use that config to connect, so you effectively can connect anywhere if you bring your own server.

**Q: Will using the IP spoof (VPN) affect my ping in online games?**  
**A:** It can, yes. Any VPN adds an extra hop between you and the game server. If the VPN server is close to the game server, sometimes it’s not too bad – possibly +20 to 50 ms ping. If the VPN server is far, ping could be much higher. We recommend choosing a VPN endpoint that is in the same region as the game server you intend to play on, to minimize lag. For example, if you’re in Asia but playing on a European game server (because you got banned in Asia), connecting to a Europe VPN might actually help since it exits in Europe and then goes to the server locally (though your own latency to Europe is still a factor). Always test with a throwaway match to see if the latency is playable. You can toggle Spoofer’s VPN off and on to compare pings. Also note that VPNs can sometimes stabilize a connection or route around ISP issues, but they can also introduce variability. It’s a trade-off for anonymity/unbanning.

**Q: Does the VPN protect all my traffic?**  
**A:** If you use full-tunnel mode, yes – all your device’s network traffic will go through the encrypted VPN to the Spoofer server, then out to the internet. This hides your activity from your local network/ISP (except that they see you using a VPN). It also means any online service you use sees the VPN’s IP, not yours. If you use the “app-specific” proxy mode instead, then only the traffic from apps configured to use that proxy will go through the VPN. For general privacy, full-tunnel is the way to go. Spoofer’s kill-switch (if enabled) will prevent your traffic from leaking out your normal connection if the VPN drops unexpectedly. Keep in mind, DNS queries will also go through the VPN (by default we use the VPN server’s DNS), so you shouldn’t have DNS leaks.

**Q: My internet is not working after disconnecting the VPN.**  
**A:** Occasionally, if the program or system crashes, a VPN connection might not shut down cleanly, leaving your network in a waiting state. If that happens, you can usually fix it by:

-   On Windows: Going to Network & Internet settings -> Change adapter options -> find the “Spoofer VPN” adapter (likely a TAP adapter) and disable it, then re-enable your main adapter if needed. Or simply reboot which resets network interfaces.
    
-   In Spoofer, there’s a “Reset Network” function in the IP section – this will try to reset the Windows network stack or flush any lingering routes. Typically, disconnecting via the app should restore your normal network instantly. If it doesn’t, check that the kill-switch isn’t still active (the kill-switch will block internet when VPN is off to prevent leaks – so if you turned it on, you need the VPN on or disable kill-switch).
    

**Q: Can I use Spoofer’s VPN just for privacy even if I’m not spoofing anything else?**  
**A:** Absolutely. You can run Spoofer and just connect to the VPN to hide your IP on the web, even if you don’t need the other features at that moment. It works like a regular VPN service. Some users might prefer to have one app that can do VPN and other spoofing as needed rather than subscribing to a separate VPN. We don’t impose usage limits currently, but we might enforce fair usage if servers get overloaded (we’ll be transparent if that happens). Always follow our usage guidelines.

### DNS Spoofing FAQ

**Q: How do I remove or reset a DNS spoof entry?**  
**A:** In the Spoofer DNS interface, you can simply delete the entry from the list or toggle it off. When you delete it (and save/apply), Spoofer will remove it from the hosts file or its DNS cache. If you had an entry that pointed a domain to a wrong IP and you remove it, your system will go back to using the normal DNS for that domain. If it doesn’t seem to revert immediately, do a DNS flush (the tool has a button, or you can manually run flush commands). Also, check if perhaps you have multiple entries (duplicates) – the app should warn you if the same domain is mapped more than once.

**Q: Can DNS spoofing be used to block ads/malware?**  
**A:** Yes, similar to how some ad-blockers use hosts file entries. You could import a list of known ad domains and map them to `0.0.0.0` (which means “nowhere”). Spoofer allows bulk import – you can copy-paste a hosts file list into it. However, maintainability of that list is up to you (we might add subscription lists in future). Keep in mind if you have a very large hosts file (say thousands of entries), DNS resolution might slow down a tiny bit or the system might handle it differently (Windows is fine with large hosts files, but extremely large ones can cause slight delays). For most users, using a dedicated ad-blocker or DNS-based blocker (like Pi-hole or NextDNS) is more comprehensive. Spoofer’s DNS feature is more aimed at specific overrides. But yes, it can serve as a basic blocker.

**Q: Does Spoofer’s DNS module support wildcard or subdomains?**  
**A:** Basic hosts files don’t support wildcards – you have to list each domain or subdomain. Spoofer’s own DNS resolver mode (when not using the system hosts) does have wildcard capability. For example, you could add an entry `*.example.com -> 1.2.3.4` in the UI. This will internally catch any subdomain of example.com. But note: to use wildcard entries, Spoofer switches to running a local DNS service on port 53 to handle queries (because the OS hosts file can’t do it). This should be seamless, but on Windows it might ask for firewall permission for Spoofer to act as a DNS server for your machine. As long as Spoofer is running, your DNS queries go to itself first. When you close it, the system goes back to normal DNS. We mention this because if you add a wildcard entry, you may see an alert or so – just allow it to function. And be careful with wildcards; don’t inadvertently redirect all domains (`*.*`) or something broad that catches more than intended.

**Q: My custom DNS entry isn’t working – the domain still goes to the old IP.**  
**A:** A few things to check:

-   Spelling of the domain in the entry (DNS entries are exact match in hosts). `example.com` is not the same as `www.example.com` – if you want both, you need entries for each, or use a wildcard as mentioned.
    
-   DNS cache: maybe the domain was resolved recently and cached. Flush the DNS cache (button or `ipconfig /flushdns`). Some applications also cache DNS internally (browsers especially); you might need to restart the app or in Chrome go to `chrome://net-internals/#dns` and clear host cache.
    
-   Ensure no conflicting entries: if you accidentally have two entries for the same domain (one pointing to A, another to B), results may be unpredictable. The app tries to prevent duplicates.
    
-   On Android without root: remember, Spoofer uses a VPN-based workaround to intercept DNS. If you didn’t activate the location/IP spoof (which triggers the VPN), the DNS spoof might not actually be active. Solution: enable the “DNS Proxy” in the app (it sets up a local VPN just for DNS). This will show as a VPN connection but only handling DNS queries.
    
-   Lastly, your network’s router or ISP might be intercepting DNS (some ISPs ignore your device’s DNS and force their own, or a corporate network might override). Using Spoofer’s local DNS should bypass that since it intercepts on device, but if something is off, check that your device’s DNS server is either 127.0.0.1 (when using our local mode) or not something malicious. You can also try a different approach: instead of our DNS spoof, you could run a known DNS (like 1.1.1.1) if just trying to circumvent ISP, but for specific mapping our method is needed.
    

**Q: Is DNS spoofing the same as using a custom DNS service (like Google DNS or Cloudflare)?**  
**A:** Not exactly. Using a custom DNS like Google (8.8.8.8) means your queries go to that DNS server on the internet which might be faster or uncensored, but you still get whatever answer that server provides. DNS spoofing as we implement it ensures _your device_ gets the answer you specify for certain domains. It takes precedence over any external DNS. In fact, if an entry is not in your custom list, it will fall back to whatever normal DNS you have configured (which could be Google, your ISP, etc.). So you can use both: set your primary DNS to a service like Cloudflare for overall resolution, and use Spoofer to override specific domains. They complement each other. (When Spoofer runs a local DNS, it will forward non-matching queries to the configured upstream DNS server, which you can set in settings – by default it might use your system default or a trusted public DNS).

### Location Spoofing FAQ

**Q: How do I avoid getting banned in Pokémon GO while spoofing?**  
**A:** The key is to **not teleport recklessly**. Niantic (the company behind Pokémon GO) has a system where moving unrealistically fast or far triggers a soft ban (you can’t interact with Pokémon/gyms for a couple hours)​

. Repeated offenses can lead to permanent bans. Here are tips for safer spoofing:

-   Use the **cooldown rule**: If you jump to a new location, wait an appropriate time before interacting. A common guideline is: for distance that would normally take X hours to travel, wait X hours. Spoofer helps by showing a timer if you jump large distances.
    
-   Prefer **gradual movement** with the joystick or route feature instead of instant teleports across the globe. If you need to go far, consider doing a series of hops (with waiting in between) rather than one huge jump.
    
-   Avoid obvious impossible actions, like sniping a Pokémon from Tokyo then one from New York within minutes.
    
-   Do not abuse multiple accounts on one device in different locations too quickly. Despite precautions, always understand there is a risk. Many spoofers have successfully used these techniques for long periods. Niantic’s detection also looks at other factors like consistency (if you always play from one city and suddenly you’re always elsewhere, that flags). Some people use multiple devices or an alt account to spoof while keeping their main legit. Ultimately, **never use your main account to spoof if you aren’t willing to lose it.** Use a secondary account to play around if possible.
    

**Q: I set a location but some apps (like Uber or weather apps) still detect my real location. Why?**  
**A:** Some apps have multiple ways to get location:

-   They might use Wi-Fi/cell tower geolocation in addition to GPS. If you’re at home on Wi-Fi, the Wi-Fi SSID might clue them into your real city (since databases link Wi-Fi networks to coordinates). Pokémon GO relies mostly on GPS, but apps like Uber use a mix of GPS and network location. To mitigate this, Spoofer has an option “Simulate moving (keep GPS active)” which tries to override network-based location too by feeding dummy data, but it’s not foolproof.
    
-   Some apps actively detect if the “Allow mock locations” setting is on (Android). If they find any app with that permission, they might refuse to work (some banking apps do this for security). In such cases, you might need to hide the spoofing. Tools like Xposed with modules (e.g., RootClock or Mock Mock Locations) can hide the mock location status. This is advanced – essentially you trick apps into not seeing that you have a mock location active.
    
-   On iOS, apps can’t normally tell if you’re using a dev spoof method, but if you’re not jailbroken you can’t hide it either; thankfully few apps detect that.
    
-   Ensure you turned off any location accuracy features that might override things (on Android, in Developer Options there’s “GPS only” vs “high accuracy” – using GPS only can help force it to use the fake GPS and ignore Wi-Fi). In summary, some apps have anti-spoof measures. You might have to use additional tools or settings to get around those. Spoofer aims to handle the basics (GPS), but it can’t directly change how third-party apps verify location beyond that. Check our wiki or community for app-specific notes.
    

**Q: Do I need to root my Android phone to spoof the location?**  
**A:** No, not for basic GPS spoofing. Android’s Developer Options include the mock location feature specifically so developers (and by extension users) can test fake locations without root. Spoofer uses this API if you are not rooted: you just select Spoofer as the mock location app. That covers apps that use the normal location APIs. However, if an app has security measures (see above), a rooted device with Xposed might be needed to conceal the mock flag. For 99% of casual uses (games like Pokémon GO, etc.), **no root is needed** to fake the GPS. For device ID spoofing or MAC on Android, root is needed, but not for plain location. On iOS, unfortunately, if you don’t jailbreak, the only method is via a computer like we provide – which doesn’t require the phone to be jailbroken but does require tethering to a PC during use.

**Q: Will GPS spoofing affect my whole device? For example, will Google Maps also show the fake location?**  
**A:** Yes, when Spoofer is active and set as the mock location provider, it feeds the fake coordinates into the global location service. So all apps using location will get the spoofed location. Google Maps will think you’re wherever you set. This system-wide effect is convenient when you want everything to use the same fake location. If you want to limit the fake location to only certain apps, that’s trickier – Android doesn’t support per-app mock locations by default. One approach on rooted devices is to use Xposed modules (like AppSettings or others) to only feed mock location to specific apps while letting others see real location. Spoofer doesn’t currently have per-app controls – it’s either on or off globally. So remember to turn it off when you want to use real location in other apps.

**Q: I followed the steps to spoof on my iPhone using the PC tool, but my location on the iPhone didn’t change. What did I miss?**  
**A:** Make sure:

-   Your iPhone is **unlocked** and **trusted** the computer (you should see the “Trust this computer?” prompt and accept it).
    
-   You have **iTunes or Apple Mobile Device Support** installed on the PC so that the necessary drivers are there.
    
-   After clicking “Set iPhone Location” in Spoofer, give it several seconds. On iOS, sometimes the Maps app might not update immediately. Try opening Apple Maps on the iPhone; if done right, Apple Maps should show the spoofed location as current.
    
-   Keep the iPhone connected; the spoof persists until the device either moves significantly on its own or possibly until a reboot. It’s not as persistent as on Android. Some users report that the location snaps back after a few minutes if the phone has other location sources – it’s a cat-and-mouse. Our tool uses a method that should hold until reboot or until you stop it via the PC. Ensure you don’t disconnect the phone or close the Spoofer PC tool immediately – let it stay running if possible while you use the spoofed location. If issues persist, it could be an iOS version limitation – Apple occasionally changes how their internal location overrides work. Check our documentation for iOS for any version-specific notes.
    

### Device ID Spoofing FAQ

**Q: What exactly can Spoofer change on my Android device ID?**  
**A:** The main thing is the **Android ID (SSAID)**, which many apps use to identify you. We also change the **Google Services Framework (GSF) ID** sometimes, which is another unique ID used by Google apps. If you enabled advanced mode, Spoofer can randomize the **IMEI/MEID** on some phones (mostly Qualcomm-based, rooted, with proper modules – it uses Xposed or Magisk modules under the hood to intercept calls to getDeviceId). It can change the **device model, manufacturer, brand, and device name** as seen by apps (by modifying the build properties). It resets **Advertising ID** by calling the internal API to do so (same as going to settings and resetting it). It can also clear app caches that might store old IDs for safety. Essentially, it covers the IDs that are _software-accessible_. It does not (and cannot) change things like the actual Wi-Fi MAC through this module (that’s in the MAC module) or the SIM’s IMSI (that is on the SIM card). But many apps won’t see those anyway due to permission restrictions.

**Q: Do I need to reinstall apps after changing device ID to avoid them linking old info?**  
**A:** In some cases, yes, you might. For example, if an app has already stored your old Android ID or reported it to a server, it might get suspicious if it sees a new one suddenly. Some aggressive games might flag device-binding mismatches. A clean approach after device spoofing is:

-   Change the device IDs with Spoofer.
    
-   Create a fresh user profile on the device (or at least clear the app’s data/cache).
    
-   Install the app/game fresh or clear its data so it registers as a new device. This way, the app will only ever know the spoofed identity and can’t correlate with the old one stored in its cache. Spoofer’s cleaning can automate clearing data for some known problematic apps (with your permission). But generally, if you’re doing this to evade a device ban, it’s wise to start the app completely fresh after spoofing.
    

**Q: Is changing IMEI safe and legal?**  
**A:** **Important:** Changing the IMEI of a device is illegal in some countries (for example, in the UK it’s illegal, in many others it’s a gray area or requires carrier permission). Spoofer does not change IMEI by default. The option is hidden behind warnings. If you absolutely need to (perhaps for a device ban on a cellular game that somehow tracked IMEI), proceed at your own risk and check your local laws. Technically, changing IMEI can also disrupt your phone’s cellular connection – carriers use IMEI for identification on the network and might block unknown or suspicious ones. We generally advise _against_ changing IMEI unless you know what you are doing and it’s legal for you to do so. Many device bans on Android don’t even use IMEI (they use Android ID or hardware serials) because apps often can’t read IMEI easily anymore. So focus on the other IDs. If you did change IMEI and something goes wrong (no signal, etc.), you can revert it in Spoofer by restoring or, worst case, by manually using tools like `AT` commands or QPST to reflash the original IMEI (advanced). Back up your original IMEI (note it down from your phone’s info) before any attempt.

**Q: After spoofing my device ID, Google Play Store or other Google apps are acting weird.**  
**A:** This can happen because Google ties certain things to your device’s GSF ID or model. If you suddenly change those, Google might treat the device as new or uncertified. You might see a warning in Play Store “Device is not certified by Google”. One way to fix that is to get a new Google Services Framework ID and register it. Spoofer can generate a new GSF ID (clearing Google Play data can also do it). There is a known workaround: after changing device model/ID, go to Google Play Services info, clear data, then launch Play Store and it will sync and issue a new ID. It may ask you to sign in again. Alternatively, some users go to the SafetyNet fix route if using Magisk. This is a complex area – basically Google SafetyNet might detect a mismatch or an unexpected change and fail. If Play Store access is important, you might limit device spoofing to when you need it for a specific app, and not leave it on all the time. Or use work profiles/Island app to have a “spoofed environment” separate from your main Google account apps. This is advanced usage, but worth mentioning. For a quick fix, try re-logging into your Google account after a spoof, or restoring original values when you’re done spoofing.

**Q: Can Spoofer change the device ID on an emulator like BlueStacks?**  
**A:** Yes, the Windows version of Spoofer has a section for popular Android emulators. For BlueStacks, it can edit the `Settings` and `Registry` entries where BlueStacks stores its device info (like Android ID, GUID, Model, IMSI, phone number, etc.). It will prompt you to close the emulator first, apply changes, then reopen. For other emulators like Nox or Memu, support is in progress – but you can often manually supply the file paths for config if you’re savvy. Emulators are easier in some ways because there’s no legal concern – you’re just editing configuration. Just make sure the emulator is not running while editing those values. Spoofer includes presets to emulate various phone models on BlueStacks to bypass games that check for emulator (for example, some games look for “Bluestacks” in the build fingerprint – Spoofer will replace that with a real phone fingerprint).

**Q: Does device ID spoofing help with app store/device compatibility issues?**  
**A:** It can. If an app says “not compatible with your device” in Play Store, changing your device model to something that is compatible often works. For instance, some apps only allow installation on specific brands or with certain specs. By spoofing your device to a popular model, you might gain access. Keep in mind, if your actual hardware is lacking a feature, the app might still not work right, but at least you can attempt installation. We’ve had users spoof low-end phones as higher-end ones to download games that otherwise said not supported. Use with caution: there’s a reason some devices are marked incompatible (performance or missing sensors). But it’s a neat trick. Similarly, in an emulator, changing the model to a known supported phone can let you download apps that usually block emulators.

----------
_Universal spoofer, HWID spoofer, hardware ID changer, HWID ban bypass, game ban fix, anti-cheat evasion, MAC address spoofing, MAC changer, change MAC address, network anonymity, IP address spoofing, hide IP address, VPN alternative, proxy tool, DNS spoofing, DNS cache poisoning (local), hosts file hack, domain redirection, fake DNS records, GPS spoofing, fake GPS location, location changer, Pokémon GO spoofer, teleport GPS, location-based game hack, device ID spoofing, Android ID changer, fake device identity, emulator device faker, IMEI changer (root), privacy tool, bypass device ban, multi-account trick, digital identity spoofing, anti-detect, all-in-one spoofing toolkit_

## Disclaimer

**Disclaimer:** Spoofer is intended for **educational and personal use** to protect privacy or regain access to services you lawfully own. Use of this tool to violate game terms of service, engage in cheating, or commit fraud is **strongly discouraged**. While Spoofer can help bypass bans and restrictions, any consequences of misuse (such as account bans or legal issues) are **your responsibility**. The developers provide no guarantee that spoofing will always be undetected or permissible. Before spoofing device identifiers, especially on mobile networks, ensure that it’s legal in your jurisdiction. By using this tool, you agree that you understand the risks (including potential bans or stability issues) and will use Spoofer in compliance with all applicable laws and platform rules. Always use spoofing responsibly and ethically – for privacy, testing, and legitimate access restoration, not for unlawful activities. The contributors to Spoofer are not liable for any damage or losses arising from its use. Enjoy the freedom Spoofer provides, but please **act responsibly**.
