# km200prometheus

Python crwaler for a Buderus Heating System Web KM200 endpoint.
When the crawler is called, all known APIs are called recursively and the obtained information is made available as prometheus metric.

The heating system can be controlled via the Buderus website <https://www.buderus-connect.de> or by the [Buderus MyDevice](https://play.google.com/store/apps/details?id=com.bosch.tt.buderus) app from your mobile phone.

## requirements

The crawler needs a password you first have to set via the mobile phone app.

## example

    python3 crawler.py --km200_gateway_password=GATEWAY-PASSWORD --km200_private_password=MOBILE-APP-PASSWORD --km200_host=buderus.fritz.box

## changelog

### [0.0.1] - 2020-01-04

#### Added

- Functionalitiy to provide buderus heating system data as prometheus metric