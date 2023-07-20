# Host Localisation

## Problem

Data storage is not without its environmental implications, as it requires energy consumption. The specific impact on CO2 emissions can vary depending on the geographical location of the servers and the energy mix of the host country.

The carbon footprint associated with data storage is influenced by the energy sources used to power the servers. Different regions have varying energy mixes, which can range from fossil fuels to renewable sources. Consequently, the CO2 emissions resulting from data storage activities differ depending on the location.

## Measure

For this indicator, you need to make a list of all the servers used by your app and each country it is hosted by.

If you are using GCP for example, you can type "zone" in the search bar to see where are your instances. Then you can see [here](https://cloud.google.com/compute/docs/regions-zones?hl=en) to which country it matches. Each country's CO2 consumption is given in the sources of this page.
Finally, you can compute the average of CO2 consumption by weighting each country by the number of threads used in each one.
Example: You are using a server with 3 threads in France and a server with 2 threads in Ireland:

```
(3*0.055 + 2 * 0.458) / 5 = 0.2162 kgCO2 / kWh
```

### Grading

- A: < 0,25 kgCO2e / kWh
- B: < 0,45 kgCO2e / kWh
- C: < 0,7 kgCO2e / kWh
- D: ≥ 0,7 kgCO2e / kWh

**Weight in the final calculation** : 3

## Other information

### How to improve my grade ?

Try to migrate your server in a low carbon country.

### Sources

- ADEME, calculated from IEA 2013 WEO: [ADEME, calculated from IEA 2013 WEO: ](https://www.bilans-ges.ademe.fr/documentation/UPLOAD_DOC_FR/index.htm?moyenne_par_pays.htm)

### Table of CO2 consumption by country

| Country                      | CO2 kg/kWh |
| ---------------------------- | :--------: |
| Albania                      |   0,002    |
| Algeria                      |   0,548    |
| Angola                       |    0,44    |
| Germany                      |   0,461    |
| Argentina                    |   0,367    |
| Armenia                      |   0,181    |
| Australia                    |   0,841    |
| Austria                      |   0,188    |
| Azerbaijan                   |   0,584    |
| Bahrain                      |    0,64    |
| Bangladesh                   |   0,593    |
| Belgium                      |    0,22    |
| Belarus                      |   0,585    |
| Benin                        |    0,72    |
| Bolivia                      |   0,423    |
| Bosnia and Herzegovina       |   0,729    |
| Botswana                     |   2,517    |
| Brazil                       |   0,087    |
| Brunei Darussalam            |   0,798    |
| Bulgaria                     |   0,579    |
| Cambodia                     |   0,804    |
| Cameroon                     |   0,804    |
| Canada                       |   0,186    |
| Chile                        |    0,41    |
| Colombia                     |   0,176    |
| Congo                        |   0,142    |
| Costa Rica                   |   0,056    |
| Croatia                      |   0,305    |
| Cuba                         |   1,012    |
| Cyprus                       |   0,702    |
| Czech Republic               |   0,589    |
| Democratic Rep. of the Congo |   0,003    |
| Denmark                      |    0,36    |
| Dominican Republic           |   0,589    |
| Ecuador                      |   0,389    |
| Egypt                        |    0,45    |
| El Salvador                  |   0,223    |
| Eritrea                      |   0,646    |
| Estonia                      |   1,014    |
| Ethiopia                     |   0,007    |
| European Union of 27         |   0,429    |
| Finland                      |   0,229    |
| France                       |   0,055    |
| Gabon                        |   0,383    |
| Ghana                        |   0,259    |
| Gibraltar                    |   0,762    |
| Greece                       |   0,718    |
| Guatemala                    |   0,286    |
| Georgia                      |   0,071    |
| Haïti                        |   0,538    |
| Honduras                     |   0,332    |
| Hungary                      |   0,317    |
| Inde                         |   0,912    |
| Indonesia                    |   0,709    |
| Iraq                         |   1,003    |
| Iceland                      |     0      |
| Ireland                      |   0,458    |
| Israel                       |   0,689    |
| Italia                       |   0,406    |
| Ivory Coast                  |   0,445    |
| Jamaica                      |   0,711    |
| Japan                        |   0,416    |
| Jordania                     |   0,566    |
| Kazakstan                    |   0,766    |
| Kenya                        |   0,274    |
| Kosovo                       |   1,287    |
| Kuwait                       |   0,842    |
| Kyrgyzstan                   |   0,094    |
| Latvia                       |   0,227    |
| Lebanon                      |   0,709    |
| Libya                        |   0,885    |
| Lithuania                    |   0,548    |
| Libya                        |   0,885    |
| Luxembourg                   |    0,41    |
| Macedonia                    |   0,687    |
| Malaysia                     |   0,727    |
| Malta                        |   0,872    |
| Morocco                      |   0,718    |
| Mexico                       |   0,455    |
| Moldova                      |   0,583    |
| Mongolia                     |   1,492    |
| Montenegro                   |   0,405    |
| Mozambique                   |   0,001    |
| Namibia                      |   0,197    |
| Nepal                        |   0,001    |
| Netherlands                  |   0,415    |
| Netherlands Antilles         |   0,707    |
| New Zealand                  |    0,15    |
| Nicaragua                    |    0,46    |
| Nigeria                      |   0,405    |
| North Korea                  |   0,465    |
| Norway                       |   0,017    |
| Oman                         |   0,794    |
| Pakistan                     |   0,425    |
| Panama                       |   0,298    |
| Paraguay                     |     0      |
| Philippines                  |   0,481    |
| Poland                       |   0,781    |
| Portugal                     |   0,255    |
| Peru                         |   0,289    |
| Qatar                        |   0,494    |
| Romania                      |   0,499    |
| Russia                       |   0,639    |
| Saudi Arabia                 |   0,737    |
| Senegal                      |   0,637    |
| Serbia                       |   0,724    |
| Singapore                    |   0,499    |
| Slovakia                     |   0,197    |
| Slovenia                     |   0,325    |
| Sudan                        |   0,344    |
| South Africa                 |   0,927    |
| South Korea                  |   0,533    |
| Spain                        |   0,238    |
| Sri Lanka                    |   0,379    |
| Switzerland                  |   0,027    |
| Sweden                       |    0,03    |
| Syria                        |   0,594    |
| Tajikistan                   |   0,024    |
| Tanzania                     |   0,329    |
| Tawain                       |   0,768    |
| Thailand                     |   0,513    |
| Togo                         |   0,195    |
| Trinidad and Tobago          |    0,7     |
| Tunisia                      |   0,463    |
| Turkmenistan                 |   1,898    |
| Turkey                       |    0,46    |
| Ukraine                      |   0,419    |
| United Arab Emirates         |   0,598    |
| United Kingdom               |   0,457    |
| United States of America     |   0,522    |
| Uruguay                      |   0,081    |
| Uzbekistan                   |   0,734    |
| Venezuela                    |   0,264    |
| Vietnam                      |   0,432    |
| Yemen                        |   0,655    |
| Zambia                       |   0,003    |
| Zimbabwe                     |    0,66    |
