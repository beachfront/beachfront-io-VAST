beachfront-io-VAST
==================

Beachfront.iO VAST Integration

## Overview  ##

Beachfront.iO Supports VAST 2.0 output via an additional request parameter V=1.

## VAST Request Format: ##

```http://beachfrontio.com:3000/getAd?aid=[YOUR APP ID]&uid=[YOUR AD UNIT ID]&v=1```

## STEPS FOR INTEGRATION: ##

1. Log in or Register for an Account
2. Create at least 1 Application
3. Open the Edit dialog for the desired Application
4. Retrieve your App ID and Ad Unit ID
5. Add the above VAST URL to your Player or Ad Server replacing [Your APP ID] and [YOUR AD UNIT ID] with the App ID and Ad Unit ID retrieved from step 4.



