## InMobi iOS Mediation Adapter Changelog

#### Version 7.4.0.0
- Verified compatibility with InMobi SDK 7.4.0.

#### Version 7.3.2.1
- Fixed an issue where the adapter fails to initialize due to invalid mediation configurations.

#### Version 7.3.2.0
- Verified compatibility with InMobi SDK 7.3.2.
- Added open bidding capability to the adapter for banner, interstitial and rewarded ad formats.

#### Version 7.3.0.0
- Verified compatibility with InMobi SDK 7.3.0.
- Removed support for Native Content and App Install ad requests. Apps must use the Unified Native Ads API to request native ads.
- Now requires Google Mobile Ads SDK version 7.46.0 or higher.

#### Version 7.2.7.0
- Verified compatibility with InMobi SDK 7.2.7.
- Updated the adapter to use the new rewarded API.
- Now requires Google Mobile Ads SDK version 7.42.2 or higher.
- Added support for flexible banner ad sizes.

#### Version 7.2.4.0
- Verified compatibility with InMobi SDK 7.2.4.

#### Version 7.2.1.0
- Verified compatibility with InMobi SDK 7.2.1.

#### Version 7.2.0.0
- Verified compatibility with InMobi SDK 7.2.0.

#### Version 7.1.2.0
- Verified compatibility with InMobi SDK 7.1.2.

#### Version 7.1.1.2
- Added `adapterDidCompletePlayingRewardBasedVideoAd:` callback to the adapter.

#### Version 7.1.1.1
- Added the `GADInMobiConsent` class which provides `updateGDPRConsent` and `getConsent` methods.

#### Version 7.1.1.0
- Verified compatibility with InMobi SDK 7.1.1.

#### Version 7.1.0.0
- Verified compatibility with InMobi SDK 7.1.0.

#### Version 7.0.4.1
- Fixed an issue causing duplicate symbol errors when the adapter was used with
  those of other networks.

#### Version 7.0.4.0
- Updated the adapter to make it compatibility with InMobi SDK 7.0.4.
- Added support for native video ads.
- InMobi's SDK does not provide images for ads containing video assets. To avoid
  potential NullPointerExceptions, when the adapter receives one of these ads it
  will automatically create a blank NativeAd.Image and include it in the images
  asset array in the ad object received by the app. Publishers using this
  adapter are encouraged to avoid using the image assets directly when mediating
  to InMobi, and instead use GADMediaView in their UI. GADMediaView will
  automatically display video assets for ads that contain them, and an image
  asset for ads that don't.

#### Version 6.2.1.0
- Verified compatibility with inMobi SDK 6.2.1

#### Earlier versions
- Support for banners, interstitials, rewarded video and native ad formats.
