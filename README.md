# Smartphone Hardening Guide *DRAFT*
This guide should be a practical guide with concrete recommendations.
Its focus is on Android phones, even though most points are also valid for iPhones.

Do you have suggestions, improvements, or comments? Contact me at aron@securityguide.me or open an issue at this GitHub project.

![You need privacy](assets/you_need_privacy.jpg)

## Choosing a phone 
Make sure you trust your manufacturer and the country it is coming from. Do you think that Google is evil? Then don't take a Google/Motorola (maybe rather take an iPhone then). Do you think the Chinese government will place backdoors into devices? Don't choose Chinese manufacturers (even though most phones will be produced there).

Do not choose a smartphone from a brand you don't know or trust. They might be [shipped with malware](https://www.cnet.com/tech/mobile/these-cheap-phones-are-costing-you-your-privacy/). Or with [censorship functionalities](https://www.independent.co.uk/life-style/gadgets-and-tech/xiaomi-phones-blacklist-censorship-lithuania-b1926365.html).

Choose a phone that is guaranteed to receive security updates over a long time. The German Federal Office for Information Security (BSI) demands five years. In reality, it's mostly 2 to max. 4 years.

If you are tech-savvy, you might want to have a look at officially supported devices by [LineageOS](https://wiki.lineageos.org/devices/) and replace the manufacturer's Android version. You'll probably have support for a longer time, and you might eliminate some preinstalled shady apps. (Don't get it done in a seedy phone shop.)

## Installation
If possible, you might want to perform a factory reset of your phone before the initial operation. Make sure to regularly install system and app updates.  
Make sure that your phone is encrypted (look up in settings) and that developer options are disabled.

For your screen lock use a PIN or password. Do not use swipe or biometrics. Note that law enforcement is allowed to unlock your device using biometrics in most countries. In many countries, you cannot be forced to expose your PIN or password.

Enable Auto Factory Reset if your Android version supports it (e.g. Samsung devices do). This will factory reset your phone after 15 failed unlock attempts (there is an enforced time delay between failed attempts).

Make sure to use a strong password and multi-factor authentication for your Google account.

If you do not want Google to know your contact list, make sure to save contacts to your local phone book only (saving contacts in the Google cloud is often the default and easily overlooked).

Decide whether you want to use the "Find my phone" feature. This may enable anyone with access to your Google account (e.g. if hacked or by law enforcement) to track your location.

## Reducing the attack surface
Do not install apps you don't need. Uninstall apps you do not need.

Make sure you grant your apps only permissions that seem to make sense (e.g. if you want to share an image in a messenger app, the app will want to access your local files; it does not make sense if a flashlight app asks for your location).

I recommend using Google Play Store. If you are tech-savvy you can also use FDroid (I'd rather don't).

Never install alternative keyboards if you do not know what you are doing.

## Messengers
There are messengers. And there are "secure" messengers.  
Use "secure" messengers if you can: Signal or Threema.

WhatsApp is an acceptable messenger (not "secure"). Use it if you don't want to give it up. But do not believe it is secure.

### Security settings for WhatsApp and Signal
* Enable security notifications (WhatsApp) and do not ignore them ([find out what such notification means](https://securityguide.me/issues/how-messenger-apps-get-compromised))
* Enable two-step verification (WhatsApp)/registration lock (Signal) (this prevents account takeover)
* Verify your main contacts' security numbers (WhatsApp)/safety numbers (Signal)
* Do not store backups in plain text (WhatsApp currently does; backup encryption is currently an optional feature in beta)

## Browsers
I recommend the Firefox browser. It is not the default browser on Android and iOS (which might be a security benefit), supports add-ons (important for ad blockers), and allows all security settings we want to use.

Ads are not only annoying but are also often used to distribute malware. Therefore, I recommend the "content blocker" [uBlock Origin](https://addons.mozilla.org/en/firefox/addon/ublock-origin/).

Additionally, I recommend the following settings:
* Do not synchronize with your Firefox account (do it if you can't help it)
* Never save logins, passwords, or credit cards
* Use "strict tracking protection" to block...
  * Third-party cookies
  * Tracking content
  * Cryptominers
  * Fingerprinters
  * Redirect trackers
* "Ask to allow" or block everything under "site permissions" (like camera, microphone, location, etc.)
* Disable all types of data collection (like usage data, marketing data, studies, etc.)
* Uninstall all add-ons (if you don't have a good reason to keep them) except uBlock Origin
* Make sure external download managers and remote debugging are disabled

## Afraid to be hacked?
Do you fear being hacked by nation-state attackers? Then check out the [dirty phone/clean phone concept](clean_dirty_concept.md).