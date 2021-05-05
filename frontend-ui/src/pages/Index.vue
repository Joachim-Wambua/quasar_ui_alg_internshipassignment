<template>
 <div class="q-pa-md">
   <!-- Define the row -->
   <div class="row align-center">
     <!-- The class below makes the Layout Responsive -->
 <div padding class="col-12 col-md" >
     <div class="pagetitle text-h5">Study different areas of web 
       design easily in 3 steps:</div>
    <div ><p padding class="bullettext"><span padding class="bulletnumber">.01</span> Visit our website</p></div>
    <div ><p padding class="bullettext"><span padding class="bulletnumber">.02</span> Sign up</p></div>
    <div ><p padding class="bullettext"><span padding class="bulletnumber">.03</span> Find the course you want</p></div>
    <div class="signindiv"><q-btn class="signinbutton" no-caps label="Sign In"/></div>
 </div>
 
 <div padding class=" col-12 col-md">
   <!-- Card Section Column -->
   <q-card class="my-card text-white">
      <div class="q-pa-md">
          <q-img class="main_img" src="../statics/stationery_image.png"
          />
        </div>
      <!-- <div class="text-h6">Our Changing Planet</div> -->
    </q-card>
 </div>
   </div>
 </div>

</template>

<script>
export default {
  name: 'PageIndex'
}
</script>


<style lang="sass" scoped>
.row > div
  display: block
  padding: 10px 15px
  border: 1px solid #fff
.row + .row
  margin-top: 1rem

.column > div
  padding: 10px

.my-card
  padding: 0px
  background-color: #80c2ff
  width: 95%
  height:95%
  justify-content: center
  align-content: center
  border-radius: 36px
  
.main_img
  padding: 10px
  justify-content: center
  align-content: center
  size: 150px
  
.pagetitle
  padding-top: 90px 
  padding-bottom: 75px
  padding-left: 90px
  width: 75%
  display: inline-block
  font-family: "Montserrat ExtraBold"
  word-wrap: break-word
  overflow-wrap: break-word
  text-justify: left
  font-size: 36px
  line-height: 45px


.bulletnumber
  font-family: Montserrat SemiBold
  font-size: 12px
  font-weight: bolder
  color: #839eff
  padding-left: 90px
  padding-right: 15px

.bullettext
  padding-bottom: 15px
  font-family: Montserrat Medium
  font-size: 18px
   

.signinbutton
  background-color: #839eff
  color: #fff
  padding: 10px
  padding-left: 45px
  font-family: Montserrat Semibold
  padding-right: 45px 
  border-radius: 45px
  box-shadow: #839eff
  
.signindiv
  padding-left: 90px

</style>