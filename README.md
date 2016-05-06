beachfront-io-VAST
==================

Beachfront.iO VAST Integration

## Overview  ##

Beachfront.iO Supports VAST 2.0 output via an additional request parameter V=1.

## VAST Request Format: ##

```
http://ads.bfmio.com/getAd?aid=[YOUR APP ID]&uid=[YOUR AD UNIT ID]&appurl=[APP STORE or Site URL]

&osvers=[Operating System Version]&network=[Network Type w, c, or u for unknown]

&carrier=[Network Carrier Name]&idfa=[Android ID or iOS ID for Advertisers]&te=[target ad tracking enabled]&age=[end user age in years]

&gender=[end user gender m, f, or u for unknown]&v=1
```

## Required Parameters ##

aid - Your Beachfront.io App ID

uid - Your Beachfront.io Ad Unit ID

idfa - iOS ID for Advertisers or Android ID

te - Target Ad Tracking Enabled ( true or false )

appurl - App Store URL or Mobile Web domain URL

osvers - uuencoded End User Operating System Version

network - Network Type, w for wifi, c for cellular or u for unknown

carrier - uuencoded network carrier name

## Required Parameters for Server-to-Server integration ##

ip - Device IP address

ua - Device User agent 

pageurl - Page URL (Mobile Web)

bundleid - Store unique identifier (Native Apps)

idfa - iOS ID for Advertisers or Android ID (Native Apps)

## Additional Parameters ##

age - End user age in years

gender - End user gender, m for male, f for female or u for unknown

lat - Latitude

lng - Longitude

width - Player Width

height - Player Height

i_type - Inventory Type, Possible values (pre, mid, post, inte, out, feed)


## STEPS FOR INTEGRATION: ##

1. Log in or Register for an Account
2. Create at least 1 Application
3. Open the Edit dialog for the desired Application
4. Retrieve your App ID and Ad Unit ID
5. Add the above VAST URL to your Player or Ad Server replacing [Your APP ID] and [YOUR AD UNIT ID] with the App ID and Ad Unit ID retrieved from step 4, make sure to pass all necessary parameters.



