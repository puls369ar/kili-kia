# Traveling Europe
## Notes
* I am observing the possiility of using intercity transport as an overnight stay between the cities on which we don't want to spend much money and time. Meaning we organize the transportation in a way to enter the city in the morning, explore it during the day and leaving it in late night
* The problems of this strategy is that time to move between some destinations is 3-4 hours which means that in this cases we'll have 4 hours of not very good sleeping experience. But this problem is solved if we don't travel such transit cities more then once in order, so we get a proper sleep when arriving at non transit City where we have comfortable hostel/room taken.
* The cities that are marked as *Transit* will have the exploration time of approximately the day due to the way of exploring some cities described above
* Duration of transportation between cities are overestimated from the values given by *Google Maps*'s algorithm. This is done to avoid arrival calculation rough errors
* We choose only hostels/rooms that have the possibility to refund full amount of money at the time we get a negative response to our VISA request.

## Steps
* Figure out failback mechanism of returning airbnb and bus tickets
* Now we draw the route and define dates and duration of staying at each city, simultaneously calculating prices and times of buses
* Having this information we define airbnb prices

## Data
* Time: 2-5 days each city, overall duration 1 Month
* Flights: Yerevan->Rome 45USD, Prague->Yerevan 70USD (Jun, Jul)
* Route: [Google Maps 1]([https://www.google.com/maps/place/Nuremberg,+Germany/@45.5669433,6.0002951,7.74z/data=!4m70!1m63!4m62!1m11!1m2!1s0x13258a111bd74ac3:0x3094f9ab2388100!2sRome,+Italy!2m2!1d12.7135121!2d41.9214534!3m4!1m2!1d10.42454!2d44.4355092!3s0x12d54e113c5f9735:0x812ca89832873fc6!1m16!1m2!1s0x47789935e87299ef:0xea3df95f0281f48c!2sLevico+Terme!2m2!1d11.301007!2d46.0116173!3m4!1m2!1d11.1111849!2d46.0660255!3s0x47827146011cfd5f:0xe7928e12c20ecf2!3m4!1m2!1d9.1432663!2d45.4753521!3s0x4786c1767b4853d3:0x6d506290e6f0c34b!1m3!2m2!1d7.6859307!2d45.0448018!1m6!1m2!1s0x47f4ea516ae88797:0x408ab2ae4bb21f0!2sLyon,+France!2m2!1d4.835659!2d45.764043!1m6!1m2!1s0x47e66e1f06e2b70f:0x40b82c3688c9460!2sParis,+France!2m2!1d2.3513765!2d48.8575475!1m6!1m2!1s0x47bd096f477096c5:0x422435029b0c600!2sFrankfurt,+Germany!2m2!1d8.6821267!2d50.1109221!1m6!1m2!1s0x470b939c0970798b:0x400af0f66164090!2sPrague!2m2!1d14.4378005!2d50.0755381!3e0!3m5!1s0x479f57aeb5b61cd3:0xdd5daf85a98c21b7!8m2!3d49.4542881!4d11.0745641!16zL20vMDVia2Y?entry=ttu&g_ep=EgoyMDI0MTExOS4yIKXMDSoASAFQAw%3D%3D](https://www.google.com/maps/place/Nuremberg,+Germany/@46.2551083,2.1770131,7.67z/data=!4m109!1m102!4m101!1m11!1m2!1s0x13258a111bd74ac3:0x3094f9ab2388100!2sRome,+Italy!2m2!1d12.7135121!2d41.9214534!3m4!1m2!1d10.42454!2d44.4355092!3s0x12d54e113c5f9735:0x812ca89832873fc6!1m21!1m2!1s0x47789935e87299ef:0xea3df95f0281f48c!2sLevico+Terme!2m2!1d11.301007!2d46.0116173!3m4!1m2!1d9.1728621!2d45.4435708!3s0x4786c3f4430493dd:0x30b090ed646c7f5!3m4!1m2!1d8.2727143!2d45.4449896!3s0x4786375d8999ea47:0xcdddee381ca79d6f!3m4!1m2!1d7.6821926!2d45.0391367!3s0x478812acf97d38e1:0x79f7d9dc4155fcb7!1m6!1m2!1s0x12cdc26f7b3f8531:0x74f7784c3ac49cfc!2sMonaco!2m2!1d7.4246158!2d43.7384176!1m6!1m2!1s0x12c9bf4344da5333:0x40819a5fd970220!2sMarseille,+France!2m2!1d5.3690743!2d43.3025742!1m6!1m2!1s0x12cdd0106a852d31:0x40819a5fd979a70!2sNice,+France!2m2!1d7.2619532!2d43.7101728!1m16!1m2!1s0x47f4ea516ae88797:0x408ab2ae4bb21f0!2sLyon,+France!2m2!1d4.835659!2d45.764043!3m4!1m2!1d4.930687!2d46.797514!3s0x47f2e38794cdb975:0x5a661038b1d99e61!3m4!1m2!1d5.0789429!2d47.3119565!3s0x47f29e42ffc2f79b:0x93f5eeac38ea93c5!1m6!1m2!1s0x47e66e1f06e2b70f:0x40b82c3688c9460!2sParis,+France!2m2!1d2.3513765!2d48.8575475!1m6!1m2!1s0x479545b9ca212147:0x64db60f602d392ef!2sLuxembourg!2m2!1d6.129583!2d49.815273!1m6!1m2!1s0x47bd096f477096c5:0x422435029b0c600!2sFrankfurt,+Germany!2m2!1d8.6821267!2d50.1109221!1m6!1m2!1s0x470b939c0970798b:0x400af0f66164090!2sPrague!2m2!1d14.4378005!2d50.0755381!3e0!3m5!1s0x479f57aeb5b61cd3:0xdd5daf85a98c21b7!8m2!3d49.4542881!4d11.0745641!16zL20vMDVia2Y?entry=ttu&g_ep=EgoyMDI0MTExOS4yIKXMDSoASAFQAw%3D%3D))
* Prague/Nuremberg(Transit) - 20Jun 7:30 - 11:45 23 USD
* Nuremberg(Transit)/Frankfurt 21 jun 2:55 - 06:00  18 eur [link](https://shop.global.flixbus.com/checkout)
* Frankfurt Central Station/Luxemburg(Transit) P+R Bouillon - 25Jun 22:45 - 01:55 | 19EUR [link](https://shop.global.flixbus.com/search?departureCity=40d90407-8646-11e6-9066-549f350fcb0c&arrivalCity=40da71d6-8646-11e6-9066-549f350fcb0c&route=Frankfurt-Luxembourg&rideDate=25.06.2025&adult=1&_locale=en&departureCountryCode=DE&arrivalCountryCode=LU&features%5Bfeature.enable_distribusion%5D=1&features%5Bfeature.train_cities_only%5D=0&features%5Bfeature.auto_update_disabled%5D=0&features%5Bfeature.webc_search_us_veterans_promoted%5D=0&features%5Bfeature.darken_page%5D=1)
* Luxemburg(Transit) P+R Bouillon/Paris(Bercy Seine) - 26Jun 9:00-14:10 | 17EUR [link](https://shop.global.flixbus.com/search?departureCity=40da71d6-8646-11e6-9066-549f350fcb0c&arrivalCity=40de8964-8646-11e6-9066-549f350fcb0c&route=Luxembourg-Paris&rideDate=26.06.2025&adult=1&_locale=en&departureCountryCode=LU&arrivalCountryCode=FR&features%5Bfeature.enable_distribusion%5D=1&features%5Bfeature.train_cities_only%5D=0&features%5Bfeature.auto_update_disabled%5D=0&features%5Bfeature.webc_search_us_veterans_promoted%5D=0&features%5Bfeature.darken_page%5D=1)
* Paris/Dijon(Transit) - 29Jun 23:30-03:05 | 16EUR [link](https://shop.global.flixbus.com/search?departureCity=40de8964-8646-11e6-9066-549f350fcb0c&arrivalCity=40df6b63-8646-11e6-9066-549f350fcb0c&route=Paris-Dijon&rideDate=29.06.2025&adult=1&_locale=en&departureCountryCode=FR&arrivalCountryCode=FR&features%5Bfeature.enable_distribusion%5D=1&features%5Bfeature.train_cities_only%5D=0&features%5Bfeature.auto_update_disabled%5D=0&features%5Bfeature.webc_search_us_veterans_promoted%5D=0&features%5Bfeature.darken_page%5D=1)
* Dijon(Transit)/Lyon - 30Jun 12:10-14:45 | 9EUR [link](https://shop.global.flixbus.com/search?departureCity=40df6b63-8646-11e6-9066-549f350fcb0c&arrivalCity=40df89c1-8646-11e6-9066-549f350fcb0c&route=Dijon-Lyon&rideDate=30.06.2025&adult=1&_locale=en&departureCountryCode=FR&arrivalCountryCode=FR&features%5Bfeature.enable_distribusion%5D=1&features%5Bfeature.train_cities_only%5D=0&features%5Bfeature.auto_update_disabled%5D=0&features%5Bfeature.webc_search_us_veterans_promoted%5D=0&features%5Bfeature.darken_page%5D=1)
* Lyon/Valence(Transit) - 2Jul 22:00-12:50 | 12EUR (https://shop.global.flixbus.com/search?departureCity=40df89c1-8646-11e6-9066-549f350fcb0c&arrivalCity=40e075fa-8646-11e6-9066-549f350fcb0c&route=Lyon-Valence+%28France%29&rideDate=02.07.2025&adult=1&_locale=en&departureCountryCode=FR&arrivalCountryCode=FR&features%5Bfeature.enable_distribusion%5D=1&features%5Bfeature.train_cities_only%5D=0&features%5Bfeature.auto_update_disabled%5D=0&features%5Bfeature.webc_search_us_veterans_promoted%5D=0&features%5Bfeature.darken_page%5D=1)
* Valence(Transit)/Marsel - 3Jul 08:45-11:30 | 15EUR [link](https://shop.global.flixbus.com/search?departureCity=40e075fa-8646-11e6-9066-549f350fcb0c&arrivalCity=40df8e99-8646-11e6-9066-549f350fcb0c&route=Valence+%28France%29-Marseille&rideDate=02.07.2025&adult=1&_locale=en&departureCountryCode=FR&arrivalCountryCode=FR&features%5Bfeature.enable_distribusion%5D=1&features%5Bfeature.train_cities_only%5D=0&features%5Bfeature.auto_update_disabled%5D=0&features%5Bfeature.webc_search_us_veterans_promoted%5D=0&features%5Bfeature.darken_page%5D=1)
* Marsel/Nice - 5Jul 23:00-01:15 | 15EUR [link](https://shop.global.flixbus.com/search?departureCity=40df8e99-8646-11e6-9066-549f350fcb0c&arrivalCity=40e13a46-8646-11e6-9066-549f350fcb0c&route=Marseille-Nice&rideDate=05.07.2025&adult=1&_locale=en&departureCountryCode=FR&arrivalCountryCode=FR&features%5Bfeature.enable_distribusion%5D=1&features%5Bfeature.train_cities_only%5D=0&features%5Bfeature.auto_update_disabled%5D=0&features%5Bfeature.webc_search_us_veterans_promoted%5D=0&features%5Bfeature.darken_page%5D=1)
* Nice/Monaco/Nice
* Nice/Turin(Transit) - 24EUR [link](https://shop.global.flixbus.com/search?departureCity=40e13a46-8646-11e6-9066-549f350fcb0c&arrivalCity=40deee02-8646-11e6-9066-549f350fcb0c&route=Nice-Turin&rideDate=05.07.2025&adult=1&_locale=en&departureCountryCode=FR&arrivalCountryCode=IT&features%5Bfeature.enable_distribusion%5D=1&features%5Bfeature.train_cities_only%5D=0&features%5Bfeature.auto_update_disabled%5D=0&features%5Bfeature.webc_search_us_veterans_promoted%5D=0&features%5Bfeature.darken_page%5D=1)
* Turin(Transit)/Milan
* Milan/Levico
* Levico/Dolomites(Transit)/Levico
* Levico/Venice/Levico
* Levico/Bologna(Transit)
* Bologna(Transit)/Florence
* Florence/Rome - 4h
* Rome/Naples(Transit) - 2h 30min
  
* Accomodation:
  * [Prague](https://www.airbnb.com/rooms/818157380348087977?adults=2&search_mode=regular_search&check_in=2025-06-20&check_out=2025-06-21&source_impression_id=p3_1732391513_P3479uc-O3xjVcop&previous_page_section_name=1000&federated_search_id=c742ae85-b7d8-4f07-ae6a-5fcf519db156) - 20 USD - 3 nights
  * [Frankfurt](https://www.airbnb.com/rooms/1151984779721981753?adults=2&category_tag=Tag%3A8678&enable_m3_private_room=true&location=Prague%2C%20Czechia&photo_id=1911876383&search_mode=regular_search&check_in=2025-06-22&check_out=2025-06-23&source_impression_id=p3_1732391661_P3Do9ZIe8qcV0Wu5&previous_page_section_name=1001&federated_search_id=ea1ebe7c-c492-45cc-8272-a3bdeee20112) - 10 USD - 2 nights
  * [Paris](https://www.airbnb.com/rooms/1086830488380122662?adults=2&location=Luxembourg%2C%20Luxembourg&search_mode=regular_search&source_impression_id=p3_1732388472_P3fj2yEpvOLAVKiY&previous_page_section_name=1001&federated_search_id=0dc62ea3-a90c-4f64-8fb4-9954be676b4c&guests=2&check_in=2025-06-26&check_out=2025-06-29) - 43USD/3nights
  * Lyon - Host - 2 nights
  * [Marcel](https://www.hostelworld.com/pwa/wds/hosteldetails.php/Le-Bungalow-Guesthouse/Marseille/59031?from=2025-07-03&to=2025-07-05&guests=2) - 50 USD/2 days
  * Monaco - >80USD prices only, check other possibilites - 1 nights
  * [Milan](https://www.airbnb.com/rooms/1182470702543162841?adults=2&location=Milan%2C%20Lombardy%2C%20Italy&search_mode=regular_search&check_in=2025-06-24&check_out=2025-06-25&source_impression_id=p3_1732447177_P3sWKepsWTF3sgnl&previous_page_section_name=1001&federated_search_id=dfa0f1a9-94b9-418b-9173-206abf49e83d) - 13 USD - 3 nights
  * Levico - Host - 3 nights
  * [Florence](https://www.airbnb.com/rooms/12299075?adults=2&category_tag=Tag%3A8678&enable_m3_private_room=true&location=Florence%2C%20Italy&photo_id=215570191&search_mode=regular_search&check_in=2025-06-24&check_out=2025-06-25&source_impression_id=p3_1732447337_P3B_48O71_Pe-yKE&previous_page_section_name=1001&federated_search_id=2b07f686-099e-4c7f-8773-3731c9bf5898) - 22 USD - 2 nights
  * [Rome](https://www.airbnb.com/rooms/470817?adults=2&category_tag=Tag%3A8678&enable_m3_private_room=true&photo_id=4242614&search_mode=regular_search&check_in=2025-06-24&check_out=2025-06-25&source_impression_id=p3_1732447474_P3Wo7FapCD4HIRj3&previous_page_section_name=1000&federated_search_id=883d25f9-b27f-4cee-a512-2cffe9c9f24c) - 15 USD | Also host possible - 3 nights


* Visa: Only Poland Shengen C-type Visa is needed. [Guide](https://www.gov.pl/web/hayastan/c--------)

  Application Fields
   * e-konsulat request paper
   * 3x4 Photo
   * Passport
   * Passport Xerox
   * Insurance Paper
   * Airplane Tickets
   * Hostel reserves
   * MoneyProof: ~1500USD
 ```
     Այցի նպատակը հիմնավորող վերոնշյալ բոլոր գրավոր դիմումները պետք է պարունակեն հետևյալ ամբողջական տեղեկությունը.

1) հրավիրված անձի համար` անունը և ազգանունը, ծննդյան տարեթիվը, սեռը, քաղաքացիությունը, անձնագրի համարը, ճամփորդության ժամկետը և նպատակը, մուտքերի թիվը և հիմնավորված դեպքերում նաև՝ ամուսնու ու երեխաների անունները, ովքեր ուղեկցում են հրավիրված անձին,

     2) հրավիրող անձի համար` անունը, ազգանունը և հասցեն,

3) հրավիրող իրավաբանական անձի, ընկերության կամ կազմակերպության համար` լրիվ անվանումը, հասցեն, ինչպես նաև

ա) եթե դիմումը տրվել է կազմակերպության կամ իշխանության մարմնի կողմից, դիմումը ստորագրող անձի անունը և պաշտոնը,

բ) եթե հրավիրողը իրավաբանական անձ կամ ընկերություն կամ նման իրավաբանական անձի կամ ընկերության գրասենյակ կամ մասնաճյուղ է, որը գործում է անդամ պետության տարածքում, ապա նաև՝ գրանցման համարը այն տարբերակով, որը պահանջվում է տվյալ անդամ պետության ազգային իրավունքով:

Մուտքի արտոնագրի համար դիմորդները, որոնց այցի նպատակն այլ է, քան վերևում նշվածները, կամ դիմորդները, որոնք ՀՀ քաղաքացի չեն, կախված այցի նպատակից ներկայացնում են նաև հետևյալ փաստաթղթերը․

1․ Զբոսաշրջություն․

Անդամ բոլոր պետություններում կեցության վայրի մասին ապացույց, եթե դիմողը պատրաստվում է այցելել մի քանի անդամ պետություն
 ```

  - Apply in local consulate (35EUR)
  - Apply maximum 6 months before (Apply in  Feb to be eligible in Jul)







