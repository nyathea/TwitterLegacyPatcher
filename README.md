# TwitterLegacyPatcher&nbsp;<img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Logo_of_Twitter.svg" alt="Twitter" height="25"/>

A tweak to restore functionality to older Twitter versions for iOS/iPadOS. 

This effectively makes it possible to use Twitter again on devices where it was broken previously.

## What does this do?

**TwitterLegacyPatcher** works by:
- Bypassing certificate pinning in the app
- Spoofing the app version to bypass update nags
- Fixes issues with images not being displaying correctly by replacing `pic.x.com` with `pic.twitter.com` in links
- Patches out the now deprecated 1.1 endpoints and return the newer graphql endpoints

It also includes several QoL improvements such as:
- Hides the (now useless) Fleets bar on versions that have it
- Removes all ads
- Hides the "Discover More" section under tweets
- Enables Birdwatch (Community Notes) on supported versions

## Tested Versions

- v7.29.1
- v8.58
- v8.71
- v9.10.1

Every 7.x - 9.x version *should* somewhat work. this tweak isn't neccesary yet for 9.44+

## Nightly builds
If you wanna test the newest nightly builds, you can by visiting the link below. keep in mind things can and will break. please report any issues you find.

`rootful-build` is for devices on iOS 14 and below

`rootless-build` is for devices on iOS 15 and above

[Link to Nightly Build](https://nightly.link/nyathea/TwitterLegacyPatcher/workflows/makefile/main)

## Known Issues

- On some 8.x versions, attempting to log in will freeze the app and eventually cause an crash. A workaround is to log in using 7.29.1 first, then upgrade to your preferred version.
- The Search page and Quote tweets doesnt work
- You may not be able to like tweets on some versions because of deprecated v1.1 endpoints. (this will be fixed soon)
- Banners disappear once the profile view is refreshed
- latest (following) timeline doesnt work yet

Please let me know if theres any other issues! pleae open a bug report and i'll get to you as soon as i can
