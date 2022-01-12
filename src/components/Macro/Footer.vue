<template>
  <div id="Footer" class="container-fluid">
    <div class="row ">
      <div class="col-lg-6 col-md-12 l-column">
        <div class="row">

          <!-- first column -->
          <div class="col-lg-4 col-md-6 col-sm-12 first-col">
            <h3>Find our Resturant</h3>
            <div class="info" v-for="(el, index) in location" :key="index">
              <h5>{{el.address}}</h5>
              <h5>{{el.place}}</h5>
              <h5>{{el.num}}</h5>
            </div>
            
          </div>

          <!-- second column  -->
          <div class="col-lg-4 col-md-6 col-sm-12 second-col">
            <h3>Working hours</h3>
            <div class="info" v-for="(il, ind) in days" :key="ind">
             <h4>{{il.day}}</h4>
             <h5>{{il.work}}</h5>
            </div>

            <!-- text -->
            <div class="socials">
              <h4>Follow Us:</h4>
              <i class="fab fa-twitter"></i>
              <i class="fab fa-facebook"></i>
              <i class="fab fa-instagram"></i>
              <i class="fab fa-linkedin"></i>
            </div>
          </div>
          <div class="col-lg-4 col-md-12 third-col">
            <h3>The don peppe crew first and foremost values an authentic, well baked slice of pizza.</h3>
          </div>


        </div>
        <div class="row">

        </div>
      </div>
      <div class="col-lg-6 col-md-12 r-column">
        <img src="../../assets/Img/footer-img-1.jpg" alt="">
      </div>
    </div>

  </div>
</template>

<script>
export default {
    name:"Footer",

    data() {
      return {
        location: [
          {
            address:"1614 E. Bell Rd #104.",
            place:"Salerno, AZ 85022",
            num:"(602) 867-1010"
          },
          {
            address:"204 E. Piazzetta Tommaso",
            place:"Sorrento, AZ 85022",
            num:"(358) 867-1010"
          },
          {
            address:"Vale Puglia 54",
            place:"Torre Del Greco AZ 85022",
            num:"(359) 867-1010"
          },
           {
            address:"Corso Itali AA",
            place:"Naples. AZ 85022",
            num:"(989) 867-1010"
          }
        ],
        days: [
          {
            day:"Monday",
            work:"Kitchen Closed"
          },
          {
            day:"Tueseday until friday",
            work:"9:00 - 22:00"
          },
          {
            day:"Saturday*",
            work:"Saturday 11am to midnight"
          },
          {
            day:"Sunday",
            work:"9:00 - 22:00"
          },

        ]


      }
    }
}
</script>

<style lang="scss" scoped>
    #Footer {

      .r-column{
        padding: 0;

        img {
          width: 100%;
      }
      }
      .l-column {
        background-color: black;
        padding: 45px;

        .first-col, .second-col, .third-col {
          h3 {
            text-transform: uppercase;
            color:#B7903C  ;
            margin:35px 0px
          }

         .info {
            margin:50px 0px;

            h5 {
              color: grey;
              font-size: 15px ;
            }
         }
        }

        .second-col {
          .close, .close>h5 {
            color:#Ab4027;
          }
          h4 {
            text-transform: uppercase;
            color:#B7903C  ;
            font-size: 20px ;

          }
          .socials {
            display: flex;
            align-items: center;

            i {
              color: white;
              margin: 0px 5px;
              font-size: 12px;
            }
          }
          
        }

         .third-col>h3{
             color: white;
           }
      }
    }
</style>