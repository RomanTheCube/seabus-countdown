# SeaBus Countdown

A real-time countdown app for Vancouver's SeaBus ferry service, available for iOS and watchOS.

## Overview

SeaBus Countdown provides live departure times for the SeaBus ferry that connects Waterfront Station (downtown Vancouver) and Lonsdale Quay (North Vancouver). The app uses location detection to automatically show you the most relevant departure information.

## Features

- **Location-Aware**: Automatically detects which terminal you're near and shows relevant departures
- **Dual Terminal View**: See departures from both Waterfront and Lonsdale Quay when away from terminals
- **watchOS Support**: Full Apple Watch app with complications for at-a-glance departure times
- **Offline Fallback**: Shows scheduled times when real-time data is unavailable
- **No Service Detection**: Displays when the next service resumes during off-hours

## Requirements

- iOS 17.6+ / watchOS 11+
- iPhone or Apple Watch
- Location services (optional, for automatic terminal detection)

## How It Works

The app uses:
- **CoreLocation** for geofencing to detect your nearest terminal (1km radius)
- **AdMob** for banner ads (iOS only)

## Terminal Detection

- Within 1km of Waterfront Station → Shows Waterfront departures with switch button
- Within 1km of Lonsdale Quay → Shows Lonsdale departures with switch button  
- Outside both geofences → Shows both terminals simultaneously

## Privacy

This app uses your location only to determine which SeaBus terminal you're closest to. Location data is:
- Processed entirely on your device
- Never stored or transmitted to external servers (except TransLink's public API for schedules)
- Used solely for improving the user experience

For complete details, see our [Privacy Policy](privacy-policy.md).

## Data Source

All departure times come from [TransLink](https://www.translink.ca/), Metro Vancouver's regional transportation authority. This is an unofficial third-party app and is not affiliated with or endorsed by TransLink.

## Disclaimer

This app provides estimated departure times based on real-time transit data. Always verify departure times with official TransLink sources. The developer is not responsible for missed departures or schedule changes.

## License

Copyright © 2025. All rights reserved.

## Support

Report issues or request features at: [GitHub Issues](https://github.com/RomanTheCube/seabus-countdown/issues)

---

**Note**: SeaBus is a registered trademark of TransLink. This app is an independent project and is not affiliated with TransLink.
