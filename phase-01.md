# Auto Market website 

## Phase 1 - AutoMarket as an 2nd-hand car store 

The website is a simple auto dealer website with these below features 

+ Simple role-based access control
    + User: update profile, view car listing, view cart listings by brand, rate car listing, create meeting requests to a car dealer related to a specific car listing based on available time of the car dealer (30 mins). 
    + Admin: manage users, assign to or remove role from users, car brands, disable car listing. 
    + Car dealer: post car listing, update car listing status, activate / deactive a car listing, configure the available time for each day.   

+ Entities 
    + Users 
        + Email 
        + Firstname 
        + Lastname 
        + Phone 
        + Photo 
        + Address 
    + Car brands
        + Auto Maker 
        + Brand 
        + Logo
        + Type
        + Description  
    + Car listing TBU  
    + Meeting request
        + User 
        + Car Dealer 
        + Meeting Time 

+ Back-end: rest API 
  + Database: postgresql, using Digital Ocean or Neon SaaS
  + Car brand CRUD
    + Logo should be jpeg or png file, to be uploaded to S3 or Cloudinary (free for 20GB storage and photo transforming)
    + Paging with custom page size
  + Authentication
    + First version: JWT authentication API
    + Second version: integrate with Firebase, allow OAuth with Google & Facebook account
  + Authorization: see above
+ Front-end
  + Administation   
