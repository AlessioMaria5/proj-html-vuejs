<template>
  <div id="footer">

    <div class="mainFooter">
      <div class="info">
        <div class="logo-wrapper">
          <img src="../assets/img/footer-logo-1.png" alt="">
        </div>

        <p>Providing Life Changing Experiences Thorugh Education. Class That Fit Your Busy Life. Closer to Home.</p>
        
        <div class="phone info-c">1-677-124-44227</div>
        <div class="openDays info-c">Mon - Sat 8.00 - 18.00</div>
      </div>

        <ul>
          <h2>Popular courses</h2>
          <li>
            <h5>Business English</h5>
            <a href="#">Preston Marshall</a>
          </li>

          <li>
            <h5>Business English</h5>
            <a href="#">Preston Marshall</a>
          </li>

          <li>
            <h5>Business English</h5>
            <a href="#">Preston Marshall</a>
          </li>


        </ul>

        <ul>
          <h2>Support</h2>
          <li><a href="#">User Dashboard</a></li>
          <li><a href="#">Contact Us</a></li>
          <li><a href="#">Faq</a></li>
          <li><a href="#">Course Offer</a></li>
          <li><a href="#">Events</a></li>
        </ul>

      <div class="flex-learning">
        <h2>Flexible Learning</h2>
        <div class="map-wrap">
          <img src="../assets/img/footer-img-1.png" alt="">
        </div>
      </div>
    </div>

    <div class="contacts">
      <hr>
      <div class="in-contacts">
        <p>Copyrights 2017 @Mikado Themes</p>
        <div class="socials">
          <span>CALL: +44 300 303 0266</span>
          <span>FOLLOW US</span>
          <div class="social-icons">
            <span>FB</span>
            <span>TW</span>
            <span>IN</span>
          </div>
        </div>
        
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  @import '../style/main.scss';
  #footer {
    background-color: #1F1F1F;
    

    h1,h2,h3,h4 {

      color: white;
      font-size: 0.9em;
    }

    h2 {
      margin-bottom: 10px;
    }

    h5 {

      color: #9c9999;
    }

    a {
        text-decoration: none;
        color: grey;
        font-size: 0.7em;

        
    }

    .mainFooter {

      display: flex;
      justify-content: space-around;
      align-items: flex-start;
      padding: 50px;
     

     .info , ul , .flex-learning{

       width: 25%;

     }

     ul {
      list-style:none;
     }

     .info {
      
        font-size: 0.8em;
        color: #9d9d9d;
        
      p {
        width: 80%;
        font-size: 0.9em;
        color: #9d9d9d;
        margin-top: 10px;
        margin-bottom: 20px;
      }

      .info-c {
        margin-bottom: 10px;
      }
     }

    }

    

    .logo-wrapper {
      width: 100%;

      img {
        width: 40%;
      }

      
    }

    .flex-learning {
      width: 50%;

      h2 {
        text-align: center;
      }
    }

    .map-wrap {
        
        width: 100%;
        
        img {

          
          width: 90%;
        }

        }
  }

  .contacts {
     padding: 50px 50px 20px 50px;

     hr {
       opacity: 0.1;
       margin-bottom: 20px;
     }
     .in-contacts{

      display: flex;
      justify-content: space-between;
      color: $primary_font;
      font-size: 0.7em;
      .socials {
        display: flex;
        gap: 20px;

        .social-icons {
          display: flex;
          gap:10px;
        }
      }
     }
     
  }

</style>