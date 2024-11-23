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
* Route: [Google Maps 1](https://www.google.com/maps/place/Nuremberg,+Germany/@45.5669433,6.0002951,7.74z/data=!4m70!1m63!4m62!1m11!1m2!1s0x13258a111bd74ac3:0x3094f9ab2388100!2sRome,+Italy!2m2!1d12.7135121!2d41.9214534!3m4!1m2!1d10.42454!2d44.4355092!3s0x12d54e113c5f9735:0x812ca89832873fc6!1m16!1m2!1s0x47789935e87299ef:0xea3df95f0281f48c!2sLevico+Terme!2m2!1d11.301007!2d46.0116173!3m4!1m2!1d11.1111849!2d46.0660255!3s0x47827146011cfd5f:0xe7928e12c20ecf2!3m4!1m2!1d9.1432663!2d45.4753521!3s0x4786c1767b4853d3:0x6d506290e6f0c34b!1m3!2m2!1d7.6859307!2d45.0448018!1m6!1m2!1s0x47f4ea516ae88797:0x408ab2ae4bb21f0!2sLyon,+France!2m2!1d4.835659!2d45.764043!1m6!1m2!1s0x47e66e1f06e2b70f:0x40b82c3688c9460!2sParis,+France!2m2!1d2.3513765!2d48.8575475!1m6!1m2!1s0x47bd096f477096c5:0x422435029b0c600!2sFrankfurt,+Germany!2m2!1d8.6821267!2d50.1109221!1m6!1m2!1s0x470b939c0970798b:0x400af0f66164090!2sPrague!2m2!1d14.4378005!2d50.0755381!3e0!3m5!1s0x479f57aeb5b61cd3:0xdd5daf85a98c21b7!8m2!3d49.4542881!4d11.0745641!16zL20vMDVia2Y?entry=ttu&g_ep=EgoyMDI0MTExOS4yIKXMDSoASAFQAw%3D%3D)
* Prague/Nuremberg(Transit) - 4h
* Frankfurt/Luxemburg(Transit) - 4h
* Paris/Dijon(Transit) - 4h
* Lyon - Turin(Transit) - Milan(Transit) - Levico - Rome
  
* Rent:
  * [Prague]() - 20 USD
  * Frankfurt - 20 USD
  * [Paris](https://www.airbnb.com/rooms/1086830488380122662?adults=2&location=Luxembourg%2C%20Luxembourg&search_mode=regular_search&check_in=2025-06-26&check_out=2025-06-27&source_impression_id=p3_1732388472_P3fj2yEpvOLAVKiY&previous_page_section_name=1001&federated_search_id=0dc62ea3-a90c-4f64-8fb4-9954be676b4c&guests=2) - 12 USD

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







