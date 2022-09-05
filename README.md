# Read Me



![Project Image](https://user-images.githubusercontent.com/62770500/188496559-4dcc028e-f158-4c56-a37a-62189a5495d5.png)
---

### Project Name :

- DataPuller

---

### Project Link :

- DataPuller - [click here](https://charming-crepe-c4e9d2.netlify.app/)

---

### Table of Contents
You're sections headers will be used to reference location of destination.

- [Description](#description)
- [How To Use](#how-to-use)
- [References](#references)
- [License](#license)
- [Author Info](#author-info)

---

## Description

Have you ever wondered how browsers always seem to know your location? You’ve probably noticed that many websites display your location on their homepage, indicating that they know (exactly) where you are. the objective of this project is to show you, how much information can a website collect about and the interaction you do with the website, like the time you spent, your first visit, last visit...etc

#### Technologies & libraries

- Next.js
- Nodejs
- Google API
- cookie-cutter
- detect-browser
- detect-gpu
- react-leaflet

[Back To The Top](#read-me-template)

---

## How To Use

#### Installation & Set Up
##### Step 1 : cloning the repo to your local machine

```sh
    git clone https://github.com/hktitof/DataPuller
```

##### Step 2 : Dependencies installation
in the root of the project "DataPuller", execute in your terminal the command "***yarn***"

###### ***Note: make sure you installed node & yarn package manager***

```bash
    yarn
```

##### Step 3 (OPTIONAL) : Add .env file to the root project 
 
```bash
    touch .env
```

##### Step 4 (OPTIONAL) : Add your Google API key inside .env file.

###### ***Note :***
###### ***1- ***
###### ***2- make sure you enabled Geolocation to this API***

```Javascript
    NEXT_PUBLIC_KEY_GOOGLE_API="your API key"
```

##### Step 5 : Start the development server

```sh
    yarn dev
```

#### 🚀 Building and Running for Production

1. Generate a full static production build

   ```sh
   yarn build
   ```

## API Description :
##### Endpoint 1 :
the following endpoint will return a json object contains a bunch of information about the ip address  

```api
    /api/userInfoByIP/[IP-Address]
```
example :

```api
    /api/userInfoByIP/159.89.173.104
```
###### ***Get Request to above endpoint will return the following json data :***
```JavaScript
    {"zip":"560002","country":"India","countryCode":"IN","region":"KA","regionName":"Karnataka","city":"Bengaluru","datetime":"9/6/2022, 1:24:30 AM","lat":12.9634,"lon":77.5855,"timezone":"Asia/Kolkata","isp":"DigitalOcean, LLC","org":"Digital Ocean","as":"AS14061 DigitalOcean, LLC","query":"159.89.173.104"}
```

##### Endpoint 2 :
the following endpoint will return a json object contains the zip code for the latitude and logitude

```api
    "/api/userInfoByLatLon/" + lat + "/" + lon
```
example :

```api
    /api/userInfoByIP/159.89.173.104
```
###### ***Get Request to above endpoint the zipcode of the lat and long provided :***
```JavaScript
    {"zipcode" : "56998"}
```
###### ***the Response below is returned if the lat and long provided has no zip code in Google maps :***
```JavaScript
    {"zipcode" : "00000"}
```
---
### 🎨 Color Reference

- ![#64FFDA](https://via.placeholder.com/15/64FFDA/64FFDA.png)`#64FFDA`
- ![#0A192F](https://via.placeholder.com/15/0A192F/0A192F.png) `#0A192F`
- ![#D1D5DB](https://via.placeholder.com/15/D1D5DB/D1D5DB.png) `#D1D5DB`


---

## License

MIT License

Copyright (c) [2022] [Abdellatif Anaflous]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.



---

## Author Info

- Linkedin - [@abdellatif-anaflous](https://www.linkedin.com/in/abdellatif-anaflous/)
- Website - [Abdellatif Anaflous](https://anaflous.com)

[Back To The Top](#description) :

