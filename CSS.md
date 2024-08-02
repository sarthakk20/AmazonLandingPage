#Respnsive CSS

```style.css
*{
    margin:0;
    font-family: arial;
    border:border-box;
}
.border{
   border:1.5px solid transparent;
}
.border:hover{
   border:1.5px solid white;
}
/* NAV-BAR */

/* BOX-1 */
.Navbar{
   height:60px;
   background-color: #121921;
   color:white;
   display: flex;
   align-items: center;
   justify-content: space-around;
}
.Nav-logo{
    width:110px;
    height:45px;
    margin-left:1px;
    margin-right:1px;
    background-image: url(amazon.in1.jpeg);
    background-size: contain;
}

/* BOX-2 */

.Nav-add{
   margin-left:10px;
}
.add-one{
      color:#cccccc;
      margin-left:16px;
      font-family: sans-serif;
      font-size: 14px;
}
.add-two{
    font-size: 1rem;
    margin-left:4px;
    font-weight: 500px;
}
.location-sym{
    display:flex; 
    align-items: center;   
}

/* BOX-3 */

.Nav-search{
   display:flex;
   height:40px;
   width:600px;
   border:none;
   background-color: #faebd7;
   border-radius: 4px;
   margin-left:15px;
}
.Nav-search:hover{
   border:2.5px solid orange;
} 
.search-select{
    width:50px;
    height:40px;
    text-align: center;
    background-color: #E6E6E6;
    border:none;
    border-top-left-radius: 4px;
    border-bottom-left-radius: 4px;   
}
.search-input{
    width:100%;
    font-size: 1rem;
    border:none;
    padding:7px 10px 7px 0px;
}
.searchIcon{
    width:45px;
    height:40px;
    display:flex;
    justify-content: center;
    align-items: center;
    background-color: orange;
    border-top-right-radius: 4px;
    border-bottom-right-radius: 4px;
    font-size: 1.5rem;
    color:#0f1111;
}

 /* BOX-4  */

.Nav-region{
   height:30px;
   width:70px;
   display: flex;
   justify-content: center;
   align-items: center;
}
.Language{
   padding:8px 0px 8px 0px;
   font-size: 1rem;
   color:white;
   background-color: #0f11111d;
   border: 0;
}
.Language option{
   background-color: rgba(0, 0, 0, .8);
   color: #ffffff;

}

 /* BOX-5 */

 .addtocart{
    display:flex;
 }
 span{
    font-size:0.7rem;
 }
 .accountOrder{
    font-size: 14px;
    font-weight: 700px;
 }
 #cart{
    margin-right:3px;
    font-size: 27px;;
 }

 /* NAV-MENU */
 /* BOX-1 */
.Nav-menu{
   height:39px;
   color:white;
   font-size: 0.8rem;
   background-color: #232F3E;
   display:flex;
   justify-content: space-evenly;
   /* justify-content: space-around; */
}
#sidebar{
   position: absolute;
   width:300px;
   height: 100vh;
   color: #fff;
   /* background-color: #0f1111; */
   background-color: #fff;
   color: #7a7575;
   left: -300px;
   transition: .4s ease-in;
   z-index: 1;

}
#sidebar.active{
   left: 0px;
   box-shadow: 9px 5px 20px 2px rgba(0, 0, 0, .4);
   
}

#sidebar ul li{
   list-style: none;
   padding: 25px 0;
   font-size: large;
   font-weight: 300;
}
#sidebar ul a{
   text-decoration: none;
   color: #7a7575;
}
#sidebar span{
background-color:#232F3E;
color: white;
font-weight: 600;
font-size: 1rem;
height: 39px;
width: 100%;
display:block;
align-content: center;
/* padding-left: 10px; */
}

#toggle-btn{
   position: absolute;
   top: 10px;
   left: 298px;
   height: 25px;
   width: 40px;
   display: flex;
   justify-content: center;
   align-content: center;
   color: #fff;
   padding: 3px 5px 3px 1px;
   margin-right: 10px;
}
#toggle-btn i {
   cursor: pointer;
}

/* .allcontent{
   height:12px;
   width:20px;
   font-size: 0.9rem;
   justify-content: center;
   padding: 0px 0px 0px 2px;
   font-weight: 700px;
} */
 /* NAV-SHOP */
 /* BOX-2 */
.Nav-shop{
   display:flex;
   justify-content: space-evenly;
   align-items: center;
   margin-left: 30px;
}
.minitv{
   padding:5px 0px 5px 5px;
    /* margin-left: 30px; */
}
.tv{
   text-decoration: none;
   height:25;
   width:110px;
   color:white; 
}
.shop{
   margin-left:10px;
   padding:5px;
}
#prime{
   color: white;
   border:none;
   background-color: #232F3E;
}
.img1{
   padding:0px 0px 0px 18px;    
}
   .search-select{
      background-color: rgb(233, 233, 233);
   }
   .search-select option{
      text-align: left;
      background-color: #fff;
   }

 /* HEROIC SECTION */

.slider{
   position:relative;
   width:100%;
   margin:auto;
   overflow:hidden;
} 
.slider img{
   width:100%;
   display:none;
   z-index: 0;
}
img.displaySlide{
   display:block;
   animation: fade 1s;
}

.slider button{
position: absolute;
top:50%;
transform: translateY(-50%);
font-size: 50px;
border:none;
background-color: rgba(0, 0, 0, 0.123);
padding: 15px 12px;
color:rgba(255, 255, 255, 0.831);
cursor: pointer;
}
.prev{
   left: 0;
}
.next{
   right: 0;
}
@keyframes fade {
   from{opacity: 0.5;}
   to{opacity: 1;}
}
.hero-msg{
   background-color: white;
   color:black;
   height:45px;
   width:100%;
   display:flex;
   position: absolute;
   top:70%;
   justify-content: center;
   align-items: center;
   font-size: 0.85rem;
   margin-bottom:25px;
}
.hero-msg a{
   color:#007185;
}
 /* boxes */
.shop_content{
   display: flex;
   flex-wrap: wrap;
   justify-content: space-evenly;
   background-color: rgba(245, 245, 220, 0.815);   
   /* z-index: 1; */
}
.box_img{
   height:300px;
   background-size: cover;
   margin:10px 0px 10px 0px;
}
.boxmaterial{
   padding:0px 20px 0px 20px;
   margin:0px 0px 40px;
}
.boxmaterial h2{
   margin-top: 10px;
}
.box{
 /* border:2px solid black; */
   background-color: white;
   height:380px;
   width:23%;
   margin:20px 0px 15px;   
}
 /* FOOTER */

 /* FOOTER-CONTENT-1 */
 .footer-content-1{
    height:49px;
    background-color:#35485e;
    color:white;
    display:flex;
    justify-content: center;
    align-items: center;
}
/* FOOTER-CONTENT-2 */
 .footer-content-2{
    height:400px;
    background-color: #232F3E;
    color:white;
    display: flex;
    justify-content: space-evenly;   
 }
 .footer-content-2 a{
    text-decoration: none;
    color:#DDDDDD;
    display: block;
    justify-content: space-evenly;
    margin-top: 5px;
}
 .footer-content-2 a:hover{
    text-decoration: underline;
 }
 .foot-text{
    font-weight: 700px;
    margin: 50px 0px 15px 0px;
 }
/* FOOTER-CONTENT-3 */
.footer-content-3{
    height:68px;
    background-color:#232F3E;
    color:white;
    border-top:0.5px solid whitesmoke;
    display: flex;
    justify-content: center;
    align-items: center;
}
.logo2{
    height:50px;
    width:100px;
}

/* FOOTER-CONTENT-4 */

.footer-content-4{
   height: 60px;
   background-color: #0f1111;
   color:white;
   padding:25px;
   text-align: center;
}
.foot-first{
font-size: 0.75rem;
}
.foot-sec{
   font-size: 0.75rem;
   padding-top:7px;
}


/* Responsiveness */


@media (max-width:1248px) {
   /* BOX 1 */
   .Nav-add{
      /* padding:10px; */
      margin-left:10px;
   }
   .add-one{
      color:#cccccc;
      margin-left:16px;
      font-family: sans-serif;
      font-size: 12px;
   }
   .add-two{
      font-size: 0.7rem;
      margin-left:4px;
      font-weight: 500px;
   }
   .location-sym{
      display:flex; 
      align-items: center;   
   }
   /* BOX 2 */

   .Nav-search{
      width:525px;
   }  
   .search-select{
      font-size: 10px;
   }
   .search-input{
      width:100%;
      font-size: 0.9rem;
      border:none;
      padding:6px 0px;
   }
   .img1{
      display: none;
   }

   .Nav-region{
      height:30px;
      width:65px;
      display: flex;
      justify-content: center;
      align-items: center;
   }
}
@media (max-width:1150px){
   .Nav-search{
      width:460px;
   }  
   .search-select{
      font-size: 12px;
   }
   .search-input{
      width:100%;
      font-size: 0.9rem;
      border:none;
      padding:6px 0px;
   }
   .Nav-region{
      height:30px;
      width:60px;
      display: flex;
      justify-content: center;
      align-items: center;
   }
   /* NAV-BAR2 */
   .Nav-menu{
      font-size: 0.7rem;
   }
   .Nav-shop{
      display:flex;
      justify-content: space-evenly;
      align-items: center;
      margin-left: 30px;
   }
   .hero-section{
      width: 100%;
      height: 454px;
   }

    /* boxes */
.box_img{
   height:220px;
}
.boxmaterial h2{
   font-size: 20px;
}
.box{
   /* box-shadow: 7px 10px 15px  black; */
   height:300px;
   width:23%; 
}
}

@media (max-width:1038px) {
   .Nav-add{
      margin: 5px 10px;
   }
   .add-one{
      color:#cccccc;
      margin-left:16px;
      font-family: sans-serif;
      font-size: 10px;
   }
   .add-two{
      font-size: 0.7rem;
      margin-left:4px;
      font-weight: 500px;
   }

   .Nav-search{
      height:40px;
      width:350px;
      border:none;
      background-color: #faebd7;
      border-radius: 4px;
      margin-left:5px;
   }  
   .Nav-region{
      height:30px;
      width:55px;
      display: flex;
      justify-content: center;
      align-items: center;
   }
   .search-input{
      font-size: 0.7rem;
   }
   .search-select{
      width:40px;
      height:40px;
      text-align: center;
      background-color: #E6E6E6;
      border:none;
      border-top-left-radius: 4px;
      border-bottom-left-radius: 4px;   
   }

   .hero-section{
      width: 100%;
      height: 408px;
   }

   /* NAV-BAR2 */
   .Nav-menu{
      font-size: 0.65rem;
   }
   .shop #prime{
      font-size: 0.8rem;
   }

    /* boxes */

.box_img{
   height:180px;
}
.boxmaterial h2{
   font-size: 17px;
}
.box{
   /* box-shadow: 7px 10px 15px  black; */
   height:260px;
   width:22%; 
}

   /* FOOTER */

   .footer-content-1{
      height:45px;
      font-size: 12px;
   }
  /* FOOTER-CONTENT-2 */
   .footer-content-2{
      height:300px;
   }
   .footer-content-2 a{
      font-size: 12px;
   }
   .foot-text{
      font-weight: 600px;
   }
  /* FOOTER-CONTENT-3 */
   .footer-content-3{
      height:60px;
   }
   .logo2{
      height:40px;
      width:90px;
   }
   .footer-content-4{
      height: 50px;
   }
   .foot-first{
   font-size: 0.7rem;
   }
   .foot-sec{
      font-size: 0.7rem;
      padding-top:6.5px;
   }
}
@media(max-width:935px){
   .Nav-search{
      display:flex;
      height:40px;
      width:300px;
      border:none;
      background-color: #faebd7;
      border-radius: 4px;
      margin-left:5px;
   }  
   .Nav-region{
      height:30px;
      width:50px;
      display: flex;
      justify-content: center;
      align-items: center;
   }
   .Language{
      padding:8px 0px 8px 0px;
      font-size: 0.8rem;
      color:white;
      background-color: #0f111118;
      border: 0;
   }

   span{
      font-size:0.6rem;
   }
   .accountOrder{
      font-size: 12px;
      font-weight: 600px;
   }
   #cart{
      margin-right:3px;
      font-size: 20px;
   }
   .addtocart{
      margin-right: 3px;
   }

   .Nav-add{
      margin: 5px 10px;
   }
   .add-one{
      color:#cccccc;
      margin-left:14px;
      font-family: sans-serif;
      font-size: 7px;
   }
   .add-two{
      font-size: 0.6rem;
      margin-left:8px;
      font-weight: 450px;
   }
   .location-sym i{
      display:flex; 
      align-items: center;
      height: 6px;
      width: 6px;   
      margin-bottom: 5px;
   }

   .Nav-menu{
      font-size: 0.6rem;
   }
   .shop #prime{
      font-size: 0.7rem;
   }

   .slider button{
      top:45%;
      font-size: 60px;
      padding: 10px 8px;
      }
   .hero-msg{
      font-size: 0.76rem;
      top:70%;
      height: 45px;
   }

   .box_img{
      height:290px;
   }
   .boxmaterial h2{
      font-size: 20px;
   }
   .box{
      /* box-shadow: 7px 10px 15px  black; */
      height:370px;
      width:40%; 
   }
}

@media(max-width:880px){

   .Nav-search{
      display:flex;
      height:40px;
      width:280px;
      border:none;
      background-color: #faebd7;
      border-radius: 4px;
      margin-left:4px;
   }  
   .Nav-region{
      height:30px;
      width:50px;
      display: flex;
      justify-content: center;
      align-items: center;
   }

   span{
      font-size:0.5rem;
   }
   .accountOrder{
      font-size: 10px;
      font-weight: 670px;
   }

   .Nav-menu{
   font-size: 0.5rem;
   }
   .shop #prime{
      font-size: 0.6rem;
   }

   .box_img{
      height:260px;
      
   }
   .boxmaterial h2{
      font-size: 18px;
   }
   .box{
      /* box-shadow: 7px 10px 15px  black; */
      height:340px;
      width:38%; 
   }

}
@media(max-width:780px){
   .Nav-search{
      width:280px;
   }  
   .Language{
      font-size: 0.55rem;
      background-color: #0f111111;
   }

   span{
      font-size:0.45rem;
   }
   .accountOrder{
      font-size: 8px;
      font-weight: 600px;
   }

   .Nav-add{
      margin:0 3px;
   }
   .add-one{
      color:#cccccc;
      margin-left:13px;
      font-family: sans-serif;
      font-size: 7px;
   }
   .add-two{
      font-size: 0.49rem;
      margin-left:10px;
      font-weight: 450px;
   } 
   .location-sym i{
      display:flex; 
      align-items: center;
      height: 3px;
      width: 3px;   
      margin-bottom: 4px;
   }
   .Nav-menu{
      font-size: 0.45;

   }
   .shop{
      margin-left: 8px;
   }
   .shop #prime{
      font-size: 0.45rem;
   }
   .slider button{
      top:45%;
      font-size: 60px;
      padding: 10px 8px;
      }
   .hero-msg{
      font-size: 0.66rem;
      top:70%;
      height: 40px;
   }

   .box_img{
      height:230px;
      
   }
   .boxmaterial h2{
      font-size: 16px;
   }
   .box{
      /* box-shadow: 7px 10px 15px  black; */
      height:310px;
      width:38%; 
   }

       /* FOOTER */

   .footer-content-1{
      height:40px;
      font-size: 10px;
   }
  /* FOOTER-CONTENT-2 */
   .footer-content-2{
      height:250px;
   }
   .footer-content-2 a{
      font-size: 10px;
   }
   .foot-text{
      font-weight: 500px;
      font-size: 12px;
   }
  /* FOOTER-CONTENT-3 */
   .footer-content-3{
      height:40px;
   }
   .logo2{
      height:30px;
      width:80px;
   }
   .footer-content-4{
      height: 40px;
      padding:20px;
   }
   .foot-first{
   font-size: 0.6rem;
   padding-top: 5px;
   }
   .foot-sec{
      font-size: 0.6rem;
      padding-top:6px;
   }
}
@media (max-width:660px) {

   .Nav-logo{
      width:100px;
      height:40px;
      margin-left:1px;
      margin-right:1px;
      background-image: url(amazon.in1.jpeg);
      background-size: contain;
   }

   .Nav-search{
      margin-left:1px;
   }  
   .search-select{
      font-size: 9.2px;
   }
   .search-input{
      width:100%;
      font-size: 0.8rem;
      border:none;
      padding:6px 0px;
   }

   .signin{
      display: none;
   }
   span{
      font-size:0.45rem;
   }
   .accountOrder{
      font-size: 8px;
      font-weight: 600px;
   }

   .Nav-add{
      margin:0 2px;
   }
   .add-one{
      color:#cccccc;
      margin-left:13px;
      font-family: sans-serif;
      font-size: 7px;
   }
   .add-two{
      font-size: 0.49rem;
      margin-left:8.5px;
      font-weight: 450px;
   } 
   .location-sym i{
      display:flex; 
      align-items: center;
      height: 4px;
      width: 4px;   
      margin-bottom: 4px;
   }
   .Nav-menu{
      font-size: 0.4rem;
   }
   .shop{
      margin-left: 10px;
   }
   .shop #prime{
      font-size: 0.4rem;
   }
   #toggle-btn{
      font-size: 0.4rem;
   }
   .hero-msg{
      font-size: 0.58rem;
      top:70%;
      height: 35px;
   }
   .box_img{
      height:200px;
      
   }
   .boxmaterial h2{
      font-size: 16px;
   }
   .box{
      /* box-shadow: 7px 10px 15px  black; */
      height:280px;
      width:38%; 
   }
   .box p{
      font-size: .8rem;
   }
}
@media (max-width:600px) {

   .signin{
      display: none;
   }
   .return{
      display: none;
   }

   .Nav-add{
      margin:0 2px;
   }
   .add-one{
      color:#cccccc;
      margin-left:13px;
      font-family: sans-serif;
      font-size: 6px;
   }
   .add-two{
      font-size: 0.4rem;
      margin-left:8.5px;
      font-weight: 450px;
   } 
   .location-sym i{
      display:flex; 
      align-items: center;
      height: 3px;
      width: 4px;   
      margin-bottom: 6px;
   }
   .Language{
      padding:8px 0px 8px 0px;
      font-size: 0.5rem;
      color:white;
      background-color: #0f111100;
      border: 0;
   }
   .Nav-menu{
      font-size: 0.4rem;
   }
   .shop{
      margin-left: 5.5px;
   }
   .shop #prime{
      font-size: 0.5rem;
   }
   .slider button{
      top:45%;
      font-size: 50px;
      padding: 8px 6px;
      }
   .hero-msg{
      font-size: 0.5rem;
      top:70%;
      height: 32px;
   }
   .box_img{
      height:160px;
      
   }
   .boxmaterial h2{
      font-size: 16px;
   }
   .box{
      /* box-shadow: 7px 10px 15px  black; */
      height:240px;
      width:38%; 
   }
   .box p{
      font-size: .7rem;
   }
}

@media (max-width:510px) {
   .add-one{
      display: none;
   }
   .add-two{
      display: none;
   } 
   .location-sym i{
      display:flex; 
      align-items: center;
      height: 4px;
      width: 4px;   
      margin-bottom: 4px;
      margin-right: 9px;
      display: none;
   }
   #cart{
      margin:0 3px;
   }
   
   .Nav-search{
      display:flex;
      height:40px;
      width:290px;
      border:none;
      background-color: #faebd7;
      border-radius: 4px;
      margin-left:3px;
   }  
   .search-select{
      width:30px;
      height:40px;
      text-align: center;
      background-color: #E6E6E6;
      border:none;
      border-top-left-radius: 4px;
      border-bottom-left-radius: 4px; 
      font-size: 8px;
   }
   .search-input{
      width:100%;
      font-size: 0.65rem;
      border:none;
      padding:6px 0px;
   }
   .Language{
      padding:8px 0px 8px 0px;
      font-size: .4rem;
      color:white;
      background-color: #0f111117;
      border: 0;
   }
   .Nav-menu{
      font-size: 0.35rem;
   }
   .shop{
      margin-left: 5.2px;
   }
   .shop #prime{
      font-size: 0.4rem;
   }
   #toggle-btn{
      font-size: 0.3rem;
      top:13px
   }
   .slider button{
      top:45%;
      font-size: 50px;
      padding: 8px 6px;
      }
   .hero-msg{
      font-size: 0.4rem;
      top:70%;
      height: 25px;
   }

   .box_img{
      height:140px;
      
   }
   .boxmaterial h2{
      font-size: 14px;
   }
   .box{
      /* box-shadow: 7px 10px 15px  black; */
      height:210px;
      width:38%; 
   }
   .box p{
      font-size: .6rem;
   }

      /* FOOTER */

   .footer-content-1{
      height:35px;
      font-size: 8px;
   }
  /* FOOTER-CONTENT-2 */
   .footer-content-2{
      height:200px;
      /* padding-left: 30px; */
   }
   .footer-content-2 a{
      font-size: 7px;
   }
   .footer-content-2 ul{
      padding-left: 30px;
   }
   .foot-text{
      font-weight: 400px;
      font-size: 8px;
   }
  /* FOOTER-CONTENT-3 */
   .footer-content-3{
      height:30px;
   }
   .logo2{
      height:20px;
      width:60px;
   }
   .footer-content-4{
      height: 30px;
      padding:18px;
   }
   .foot-first{
   font-size: 0.5rem;
   padding-top: 5px;
   }
   .foot-sec{
      font-size: 0.5rem;
      padding-top:6px;
   }
}

@media (max-width:480px) {
   .Nav-logo{
      display: none;
   }
   .Nav-menu{
      font-size: 0.2rem;
   }
   .shop{
      margin-left: 4px;
   }
   .shop #prime{
      font-size: 0.2rem;
   }
   #toggle-btn{
      font-size: 0.2rem;
      top:13px
   }
   .slider button{
      top:45%;
      font-size: 50px;
      padding: 8px 6px;
      }
   .hero-msg{
      font-size: 0.35rem;
      top:70%;
      height: 22px;
   }
   #sidebar{
      width:180px;
      left: -180px;
   }
   #sidebar.active{
      left: 0px;
      box-shadow: 9px 5px 20px 2px rgba(0, 0, 0, .4);
   }
   #sidebar ul li{
      font-size: small;
      padding:20px 0;
   }
   #sidebar span{
   font-weight: 500;
   font-size: 0.6rem;
   }
   #toggle-btn{
      left: 178px;
   }

   .box_img{
      height:110px;
      
   }
   .boxmaterial h2{
      font-size: 10px;
      font-weight: 550;
   }
   .box{
      /* box-shadow: 7px 10px 15px  black; */
      height:180px;
      width:38%; 
   }
   .box p{
      font-size: .5rem;
   }
}


@media (max-width:370px) {
   .Nav-menu{
      font-size: 0.19rem;
   }
   /* .Nav-shop{
   margin-left: 10px; 
   } */
   .shop{
      margin-left: 3.5px;
   }
   .shop #prime{
      font-size: 0.2rem;
      width: 30px;
   }
   .hero-msg{
      font-size: 0.3rem;
      top:70%;
      height: 18px;
   }
   .hero-section{
         width: 100%;
         height: 135px;
   }

   .box_img{
      height:90px;
      
   }
   .boxmaterial h2{
      font-size: 9px;
      font-weight: 550;
   }
   .box{
      /* box-shadow: 7px 10px 15px  black; */
      height:150px;
      width:38%; 
   }
   .box p{
      font-size: .4rem;
   }

      /* FOOTER */

   .footer-content-1{
      height:30px;
      font-size: 7px;
   }
  /* FOOTER-CONTENT-2 */
   .footer-content-2{
      height:180px;
   }
   .footer-content-2 a{
      font-size: 5.5px;
   }
   .foot-text{
      font-weight: 400px;
      font-size: 6px;
   }
  /* FOOTER-CONTENT-4 */
   .footer-content-4{
      height: 20px;
      padding:16px;
   }
   .foot-sec{
      padding-top:4px;
   }

}

```
