<!DOCTYPE html>
<html>
<head>
	<title></title>
	<!--<link rel="stylesheet" type="text/css" href="index.css"> -->
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
   
</head>

<style type="text/css">
  @import url('https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@300&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

*{
  border: 0px;
  margin: 0px;
  padding: 0px;
  -webkit-box-sizing: border-box;
   -moz-box-sizing: border-box;
   box-sizing: border-box;
   outline: none;
}

.image-container {
  position: absolute;
  top: 0;
  width: 100%;
  height: 550px; 
  overflow: hidden;
}

.image-container > img {
  max-width: 100%;
  height: auto;
  filter: blur(2px);
  background-size: 100%;
}



.overlay h1{
    position:absolute;
    top: 20%;
    left: 50%;
    transform: translate(-50%,-50%);
}

#quote {
  position: absolute;
  top: 85%;
  left: 50%;
  transform: translate(-50%,-50%);
  font-family: 'Josefin Sans', sans-serif;
  font-size: 200%;
  color: white;
  text-align: center;
}

.overlay img {
  position: absolute;
  border-radius: 50%;
  min-width: 15%;
  width: 15%;
  height: auto;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}

.overlay h1{
  font-family: 'Josefin Sans', sans-serif;
  color: white;
  white-space: nowrap;
}



@media screen and (min-width: 811px) {
  .overlay h1{
    font-size: 50px;
    text-align: center;
    white-space: nowrap;
  }
}

/* If the screen size is 600px wide or less, set the font-size of <div> to 30px */
@media screen and (max-width: 810px) {
  .overlay h1{
    font-size: 30px;
    text-align: center;
    white-space: nowrap;
  }

  .overlay img {
    width: 35%;
    height: auto;
  }

#cover-image {
    height: 550px;
   }

}

/* WorkSHOP gallery view CSS */

.lightbox {
  /* Default to hidden */
  display: none;

  /* Overlay entire screen */
  position: fixed;
  z-index: 999;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  
  /* A bit of padding around image */
  padding: 1em;

  /* Translucent background */
  background: rgba(0, 0, 0, 0.8);
}

/* Unhide the lightbox when it's the target */
.lightbox:target {
  display: block;
}

.lightbox span {
  /* Full width and height */
  display: block;
  width: 100%;
  height: 100%;

  /* Size and position background image */
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
}

/* Workshop CSS ends */

/* Skills CSS */


/* Skills CSS END /*

/*
TIMELINE CSS STARTS HERE

*/
.aboutme {
  margin-top: 550px;
  background-color: #3E7CB1;
}



.timeline{
   margin-top: 550px;
   padding: 30px 0;
   font-family: 'Roboto', sans-serif;
   background: #F1F2F6;

}

#cover-image {
    height: 550px;
    width: 100%;
   }

#timeline-title {
   margin-top: 30px;
   text-align: center;
   font-weight: 300;
   color: #777
}

#timeline-title span {
   font-weight: 600;
}

.container {
   width: 80%;
   padding: 50px 0;
   margin: 30px auto;
   position: relative;
   overflow: hidden;
}

.container:before {
   content: '';
   position: absolute;
   top: 0;
   left: 50%;
   margin-left: -1px;
   width: 2px;
   height: 100%;
   background: #CCD1D9;
   z-index: 1
}

.timeline-block {
   width: -webkit-calc(50% + 8px);
   width: -moz-calc(50% + 8px);
   width: calc(50% + 8px);
   display: -webkit-box;
   display: -webkit-flex;
   display: -moz-box;
   display: flex;
   -webkit-box-pack: justify;
   -webkit-justify-content: space-between;
   -moz-box-pack: justify;
   justify-content: space-between;
   clear: both;
}

.timeline-block-right {
   float: right;
}

.timeline-block-left {
   float: left;
   direction: rtl
}

.marker {
   width: 16px;
   height: 16px;
   border-radius: 50%;
   border: 2px solid #F5F7FA;
   background: #4FC1E9;
   margin-top: 10px;
   z-index: 1
}

.timeline-content {
   width: 95%;
   padding: 0 15px;
   color: #666
}

.timeline-content h3 {
   margin-top: 5px;
   margin-bottom: 5px;
   font-size: 25px;
   font-weight: 500
}

.timeline-content span {
   font-size: 15px;
   color: #8B94A3;
}

.timeline-content p {
   font-size: 14px;
   line-height: 1.5em;
   word-spacing: 1px;
   color: #888;
}


@media screen and (max-width: 768px) {
   .container:before {
      left: 8px;
      width: 2px;
   }
   .timeline-block {
      width: 100%;
      margin-bottom: 30px;
   }
   .timeline-block-right {
      float: none;
   }

   .timeline-block-left {
      float: none;
      direction: ltr;
   }

   #cover-image {
    height: 550px;
   }
}


/*
TIMELINE CSS ENDS HERE
*/


/* FOOTER CSS */

/* FOOTER CSS END */

/* Hamburger menu CSS */
#menu__toggle {
  opacity: 0;
  z-index: 999;
}

#menu__toggle:checked ~ .menu__btn > span {
  transform: rotate(45deg);
}
#menu__toggle:checked ~ .menu__btn > span::before {
  top: 0;
  transform: rotate(0);
}
#menu__toggle:checked ~ .menu__btn > span::after {
  top: 0;
  transform: rotate(90deg);
}
#menu__toggle:checked ~ .menu__box {
  visibility: visible;
  left: 0;
}

.menu__btn {
  display: flex;
  align-items: center;
  position: fixed;
  top: 20px;
  left: 20px;

  width: 26px;
  height: 26px;

  cursor: pointer;
  z-index: 2;
}

.menu__btn > span,
.menu__btn > span::before,
.menu__btn > span::after {
  display: block;
  position: absolute;

  width: 100%;
  height: 2px;

  background-color: #616161;

  transition-duration: .25s;
}
.menu__btn > span::before {
  content: '';
  top: -8px;
}
.menu__btn > span::after {
  content: '';
  top: 8px;
}

.menu__box {
  display: block;
  position: fixed;
  visibility: hidden;
  top: 0;
  left: -100%;

  width: 200px;
  height: 100%;

  margin: 0;
  padding: 80px 0;
  z-index: 1;
  list-style: none;

  background-color: #ECEFF1;
  box-shadow: 1px 0px 6px rgba(0, 0, 0, .2);

  transition-duration: .25s;
}

.menu__item {
  display: block;
  padding: 12px 24px;

  color: #333;

  font-family: 'Roboto', sans-serif;
  font-size: 20px;
  font-weight: 600;

  text-decoration: none;

  transition-duration: .25s;
}
.menu__item:hover {
  background-color: #CFD8DC;
}

/* Hamgurger CSS ends */
</style>

<body>
	<div class="image-container">
		
      <img src="cover.jpg" id="cover-image">
		
      <div class="overlay">
			<h1>Hi, I'm Rahul Mahadevan!</h1>
			<img src="photo.jpeg" alt="My Photo">
			<p id="quote">"Being the Universe's way of Experiencing itself."</p>
      
      </div>
	</div>
 
	<div class="timeline">
		
      <h1 id="timeline-title"><span>Bachelor's of Technology</span> in Information Technology (2016-20)</h1>

<div class="container">

   <div class="timeline-block timeline-block-right">
     
     <div class="marker"></div>
      
      <div class="timeline-content">
         <h3>First Year</h3>  
         <span>Skills acquired: C, C++</span><br><br>
         
         <p>Project: <a href="CollegeRadioDoc.pdf" target="_blank" title="View Project Doc">College Radio Automation Program</a> <a href="https://github.com/rahulmahadevan/College-Radio-Automation" aria-label="Homepage" class="footer-octicon" title="View Repo on GitHub" target="_blank">
    


      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a><br>Description: The RJs of College Radio had routine task of playing National Song at 09:00AM and National Anthem at 04:30PM on a computer connected to the Radio speakers in the campus. Using simple C++ code the tasks were programmed to work by itself. A bell was also added to the program to follow college timings.</p><br>
      </div>
   </div>

   <div class="timeline-block timeline-block-left">
      <div class="marker"></div>
      <div class="timeline-content">
         <h3>Second Year</h3>
         <span>Skills acquired: Java, MySQL, Android Application Development</span><br><br>
         <p>Project: <a href="https://github.com/rahulmahadevan/Android-ATRI-Attendance.git" aria-label="Homepage" class="footer-octicon" title="View Repo on GitHub" target="_blank">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a> <a href="https://play.google.com/store/apps/details?id=xyz.atriams.atri" target="_blank" title="Get it on GooglePlay">ATRI Attendance Faculty & CR</a><br>Description: A user-friendly app for faculty to take and post daily attendance from app directly to database in server with many useful options to handle everything related to attendance. Followed SDLC and developed by taking continuous feedback from HoDs. Used by 100s of users</p><br>
      </div>
   </div>

   <div class="timeline-block timeline-block-right">
      <div class="marker"></div>
      <div class="timeline-content">
         <h3>Third Year</h3>
         <span>Skills acquired: Software Engineering, Web development, Networking and Security</span><br><br>
         <p>Project: <a href="https://github.com/rahulmahadevan/Android-Location-Based-Trade-System.git" target="_blank">Location based Trade/E-commerce System</a> <a href="https://github.com/rahulmahadevan/Android-Location-Based-Trade-System.git" aria-label="Homepage" class="footer-octicon" title="View Repo on GitHub" target="_blank">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a><br>Description: The project is based on the idea that every locality has different range of traders that sell almost everything a customer will ever need. This project is aimed to solve problems in most e-commerce systems. This project can be used to help customers find the products they need from the traders in their locality, thereby, helping both to make a trade.
<br><br>
Project: <a href="Hackzone-Team-Brogrammers.pdf" target="_blank">Hackathon- A user-friendly website for NGO by Brogrammers</a><a href="https://github.com/rahulmahadevan/Web-Brogrammers-NGO.git" aria-label="Homepage" class="footer-octicon" title="View Repo on GitHub" target="_blank">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a><br>Description: During the 8hrs hackathod, our team was tasked with developing a responsive and user-friendly website for an NGO with some specific requirements. We also added a payment gateway for donations towards NGO as per requirements.
<br><br>Certification acheived: <a href="https://www.youracclaim.com/badges/a5bf968a-fbaa-4db2-bf4f-48ce6a5f460c/linked_in_profile" target="_blank">Oracle Certified Associate Java SE 8 Programmer</a><br><br>

Organised <a href="#img1">Workshop on Android Application Development</a> for 70 Students
<a href="#" class="lightbox" id="img1">
  <span style="background-image: url('workshop.JPG')"></span>
</a>
</p><br>
      </div>
   </div>

   <div class="timeline-block timeline-block-left">
      <div class="marker"></div>
      <div class="timeline-content">
         <h3>Fourth Year</h3>
         <span>Skills acquired: Python, Blockchain Architecture Design, Cloud</span><br><br>
         <p>Project: <a href="https://github.com/rahulmahadevan/Web-Crime-Reporting-System.git" aria-label="Homepage" class="footer-octicon" title="View Repo on GitHub" target="_blank">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a><a href="https://github.com/rahulmahadevan/Web-Crime-Reporting-System.git" target="_blank">Crime Registration System using Chatbot</a><br>Description: The system is a client-server based web application for reporting and viewing crime based information.The chatbot is used to gather crime data from the user and store in the database. The chatbot gives the users a feeling of talking to an actual person and therefore helps in registering crime data efficiently<br><br>

Project: <a href="https://github.com/rahulmahadevan/Web-Poshan-Abhyaan.git" aria-label="Homepage" class="footer-octicon" title="View Repo on GitHub" target="_blank">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a><a href="https://github.com/rahulmahadevan/Web-Poshan-Abhyaan.git" target="_blank">Hackathon- Portal for Holistic Nutrition for Poshan Abhyaan</a><br>Description: The system consists of Health Care Workers, Nutrition Centres and women and children as users. Using this web app, health care workers can view details of all the users and nutrition centres. The default check up for dose is set monthly for every user by Health care worker. Users can check notifications from health care workers, schedule/cancel appointments, view locations of nutrition centres and be notified of upcoming check ups<br><br>Certification achieved: <a href="https://www.youracclaim.com/badges/55e78f35-7027-46d6-8b6f-6db120795e86/linked_in_profile" target="_blank">Oracle Cloud Infrastructure Foundations Certified</a></p>
      </div>
   </div>
</div>
</div>


<div class="hamburger-menu">
    <input id="menu__toggle" type="checkbox" />
    <label class="menu__btn" for="menu__toggle">
      <span></span>
    </label>

    <ul class="menu__box">
      <li><a class="menu__item" href="#">Tech Blogs</a></li>
         <li><a class="menu__item" href="#">Science Blogs</a></li>
         <li><a class="menu__item" href="#">Contact</a></li>
    </ul>
  </div>

</body>

</html>
