### Hotel Reservation schema

<img src="http://twintoe.com/UI/inbox_hotel[2].png" alt="Hotel Reservation Schema" />


1. Hotel Reservation HTML mark up

```HTML
<!--Schema.org reservation-->
<!-- https://developers.google.com/gmail/markup/reference/hotel-reservation -->

<!-- Basic Hotel Reservation-->
<span itemscope itemtype="http://schema.org/LodgingReservation" style="line-height:0;font-size:0;heighty:0;">
  <meta itemprop="reservationNumber" content="FFF-483-505"/> 				<!-- Reservation: number -->
  <link itemprop="reservationStatus" href="http://schema.org/Confirmed"/>
  <span itemprop="underName" itemscope itemtype="http://schema.org/Person">
  <meta itemprop="name" content="Fistname Lastname"/> 						<!-- Billing contact -->
  <meta itemprop="email" content="email@address.com "/> 						<!-- Email address - person or organization the reservation or ticket is for. -->
  </span>
  <span itemprop="reservationFor" itemscope itemtype="http://schema.org/LodgingBusiness">
    <meta itemprop="name" content="Hotel Name "/> 					<!-- Property name -->
	<meta itemprop="url" content="https://hotel.com"/> 	<!-- Business URL (with shortname)  -->
	<meta itemprop="telephone" content="+44 000 111 222"/> 				<!-- Business tel number -->
    <span itemprop="address" itemscope itemtype="http://schema.org/PostalAddress">
      <meta itemprop="streetAddress" content="Address"/> 					<!-- Address line 1, address line 2, address line 3  -->
      <meta itemprop="addressLocality" content="London"/> 					<!-- City -->
      <meta itemprop="addressRegion" content="Devon "/> 					<!-- Region -->
      <meta itemprop="postalCode" content="T00 974 "/> 						<!-- Postcode -->
      <meta itemprop="addressCountry" content="United Kingdom"/> 			<!-- Country -->
    </span>   				
  </span>
  <meta itemprop="numAdults" content="2"/> 									<!-- Number of adults -->
  <meta itemprop="numChildren" content="0"/> 								<!-- Number of children -->
  <meta itemprop="price" content="1085.0"/> 							    <!-- Total reservation price -->
  <meta itemprop="priceCurrency" content="GBP"/> 							<!-- The currency (in 3-letter ISO 4217 format)  -->
  <meta itemprop="checkoutDate" content="2018-04-13T11:00:00-08:00"/> 		<!-- Check in date -->
  <meta itemprop="checkinDate" content="2018-04-10T16:00:00-08:00"/> 		<!-- Check out date -->
</span>
```

2. Hotel Update Reservation HTML mark up

```HTML

<!-- Update reservation -->
<span itemscope itemtype="http://schema.org/LodgingReservation" style="line-height:0;font-size:0;heighty:0;">
  <meta itemprop="reservationNumber" content="FOJ-483-505"/> 				<!-- Reservation: number -->
  <link itemprop="reservationStatus" href="http://schema.org/Confirmed"/>
  <span itemprop="underName" itemscope itemtype="http://schema.org/Person">
      <meta itemprop="name" content="Fistname Lastname"/> 						<!-- Billing contact -->
  </span>
  <span itemprop="reservationFor" itemscope itemtype="http://schema.org/LodgingBusiness">
    <meta itemprop="name" content="Bayards Cove Inn "/> 					<!-- Property name -->
    <span itemprop="address" itemscope itemtype="http://schema.org/PostalAddress">
      <meta itemprop="streetAddress" content="Address lines 1 to 3"/> 					<!-- Address line 1, address line 2, address line 3  -->
      <meta itemprop="addressLocality" content="London"/> 					<!-- City -->
      <meta itemprop="addressRegion" content="Devon "/> 					<!-- Region -->
      <meta itemprop="postalCode" content="TQ6 9AN "/> 						<!-- Postcode -->
      <meta itemprop="addressCountry" content="United Kingdom"/> 			<!-- Country -->
    </span>
    <meta itemprop="telephone" content="+44 180 3839 278"/> 				<!-- Business tel number -->
  </span>
  <meta itemprop="checkoutDate" content="2018-04-13T11:00:00-08:00"/> 		<!-- Check in date -->
  <meta itemprop="checkinDate" content="2018-04-10T16:00:00-08:00"/> 		<!-- Check out date -->
  <meta itemprop="modifiedTime" content="2018-05-01T08:00:00-08:00"/>		<!-- Modified time -->
  <link itemprop="modifyReservationUrl" href="http://linkToModify.com"/> 	<!-- Url to modify booking page -->
</span>```
