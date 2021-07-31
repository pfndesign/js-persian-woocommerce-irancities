# js-persian-woocommerce_irancities
3d array of Iran state and cities for with Woocommerce compatible keys for Reactnative or any JavaScript project
iran state and cities array with woocommerce compatible keys for javascript projects

## Installation

import the file in your project

```javascript
import { IranCities } from "./Irancities";
```
wolah 
## Template example

```javascript
{
    key: "ABZ", // state key
    name: "البرز", // state name
    cities: [ // state cities array
      { key: "3351", name: "کرج" },
      { key: "3821", name: "اشتهارد" },
      { key: "3850", name: "گلسار" },
      { key: "3587", name: "نظرآباد" },
      { key: "3591", name: "هشتگرد ـ ساوجبلاغ" },
      { key: "5618", name: "شهر جدید هشتگرد" },
      { key: "3620", name: "رباط کریم" },
      { key: "5611", name: "مشکین شهر" },
      { key: "5612", name: "محمدشهر" },
      { key: "5613", name: "ماهیدشت" },
      { key: "5614", name: "کمال شهر" },
      { key: "5615", name: "صفادشت" },
      { key: "5616", name: "فردوسیه" },
      { key: "5617", name: "چهارباغ" },
    ],
  },
```
## Finding a specific state by key
example :
```javascript
var searchstate = new RegExp("state key", "i");
var statedata = IranCities.find((item) => searchstate.test(item.key));
```
## Finding a specific state by name
example :
```javascript
var searchstate = new RegExp("state name", "i");
var statedata = IranCities.find((item) => searchstate.test(item.name));
```
## Searching in cities
example :
```javascript
var searchstate = new RegExp("state name", "i");
var searchcity = new RegExp("city name", "i");
var statedata = IranCities.find((item) => searchstate.test(item.name));
var citydata = statedata.cities.find((item) => searchcity.test(item.name));
```
