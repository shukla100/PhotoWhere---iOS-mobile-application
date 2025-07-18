<h1>PhotoWhere - a native iOS mobile application</h1>
PhotoWhere is a passion project I designed, built and launched on the iOS App Store. This repo outlines how I took an idea — from concept to live app: including the problem, feature prioritization, wireframes & mockups, MVP1 build, customer feedback, and MVP2 roadmap.
<br />
<br>
<p>
  iOS App Store:
  <a href="https://apps.apple.com/us/app/photowhere-snap-smarter/id6748592837" target="_blank">PhotoWhere - Snap Smarter. Anywhere. </a>
</p>

<h2>Problem</h2>
Photographers often lack efficient ways to discover vetted, high-quality photography locations in real time — filtered by city and lighting conditions for their exact location. (traditional location scouting is time-consuming and incompatible with dynamic travel plans)

<h2>Solution</h2>
PhotoWhere is a native iOS application that dynamically detects user location (via device GPS or manual input) and applies real-time filtering to surface photography spots. Each result aggregates metadata on lighting conditions (i.e. golden hour/blue hour) and location context, along with a “View on Map” feature that deep-links to exact GPS coordinates in Google Maps for seamless, one-click navigation.
<br />


<h2> MVP1 Feature List + Prioritization </h2>
<p align="center">
<br/>
<img src="https://i.imgur.com/SRxFc38.png" height="60%" width="60%"/>
<br />


<h2> Wireframing the Product Experience / Mock-ups </h2>
<p align="center">
Home View / Results View
<br/>
<img src="https://i.imgur.com/r37TwyH.png" height="30%" width="30%"/> <img src="https://i.imgur.com/Z5thT2G.png" height="30%" width="30%"/>
<br />

<h2> Build - MVP1</h2>

<p>
Environments Used: <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Bubble.io native mobile (visual development platform) <br>
&nbsp;&nbsp;&nbsp;&nbsp;- bubble native DB <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Responsive, mobile-optimized UI 
</p>

<br>
<p>
API Integrations: <br>
&nbsp;&nbsp;&nbsp;&nbsp;1. Flickr API (public) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Used to query geotagged images in real time based on latitude/longitude/radius <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Get request (https, rest-API), JSON output <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Contextual static parameters (tags, geo metadata, sort order) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Dynamic location (lon, lat) url parameters <br>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;2,3. Google Places & Geocoding APIs <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Enabled location resolution from user input or device GPS to structured geographic coordinates (lon,lat) <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Location names (city,state,country) are dynamically populated via Google Places Autocomplete Service <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Get request (https, rest-API), JSON output <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Dynamic address (lon, lat) url parameters <br>
</p>


<br>
<p>
Image Unique URL Generation: <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Constructed the sources URL for a photo via image ID, server ID, secret (returned by Flicker API call) <br>
&nbsp;&nbsp;&nbsp;&nbsp;- example pull: https://live.staticflickr.com/{server-id}/{id}_{secret}_{size-suffix}.jpg <br>
</p>

<br>
<p>
iOS Deployment: <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Deployed as a native iOS application via BDK Native (iOS wrapper) <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Packed as .ipa binary file for iOS distribution (complied assets) <br>
</p>


<p align="center">
<br/>
<img src="https://i.imgur.com/4W72EP4.jpeg" height="20%" width="18.7%"/> <img src="https://i.imgur.com/8Yxq7CA.jpeg" height="20%" width="18.7%"/> <img src="https://i.imgur.com/uhAaTnB.jpeg" height="20%" width="18.7%"/><img src="https://i.imgur.com/g0POeSg.jpeg" height="20%" width="18.7%"/> <img src="https://i.imgur.com/Q2akhXs.jpeg" height="20%" width="18.7%"/>
<br />


<h2> Feedback - User Interviews + Key Insights </h2>
<p align="center">
<br/>
<img src="https:" height="50%" width="50%"/>
<br />


<h2> Iterate + MVP2 Feature List </h2>
<br/>
a
<br />

