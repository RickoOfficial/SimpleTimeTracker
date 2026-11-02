# Simple Time Tracker

How much time spend on tasks? Start tracking it right now with Simple Time Tracker. Tired of complicated time tracking applications? No need any registration, permissions or unnecessary features. Add a task, start and stop the timer. And that's it 🎉

## Supported browsers

Simple Time Tracker supports Opera and Yandex Browser. It is distributed through Opera Add-ons; the public listing URL will be added after the first publication.

## Install locally

1. Open `opera://extensions` in Opera.
2. Enable Developer mode.
3. Select **Load unpacked** and choose this repository directory.

Yandex Browser users can install the published extension from Opera Add-ons when it becomes available.

## Publishing and updates

`manifest.json` uses Opera's official update service, so Opera Add-ons delivers published updates automatically.

For a release:

1. Increase `version` in `manifest.json`.
2. Run `npm ci` and `npx gulp zip`.
3. In `opera://extensions`, use **Pack extension** for this repository directory; Opera creates a CRX package in its parent directory.
4. Upload the CRX as a new package in Opera Add-ons.
5. Keep the Opera signing key outside this repository; it is required for later releases under the same extension identity.

# CHANGELOG

## 2.3.1

- Added Opera Add-ons distribution and update configuration.
- Documented Opera and Yandex Browser installation.

## 2.3.0

- Fix reset tasks
- Added dynamic ordering and sort by option

## 2.2.0

- More compact view
- Improved default order by tasks

## 2.1.0

- Added Migration WebSQL to IndexedDB (Origin Trials for WebSQL) and will be removed v3. Up to Chrome 123 (ends with the rollout of next Chrome release), no later than 29 May 2024

## 2.0.0

- Switched to IndexedDB from WebSQL (Attention: Backup your tasks before the upgrade)
- Add hourly rate field
- Add notes field
- Improved UI

## 1.0.3

- Added total time counter

## 1.0.2

- Fixed delete confirmations

## 1.0.1

- Added reset all feature
- Improved UI

## 1.0.0

- Initial version
