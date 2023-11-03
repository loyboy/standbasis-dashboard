<template>
  <div class="container" style=" padding-right: 4px; padding-left: 4px; margin: 0px 45px 0px 45px; max-width: 1240px; ">

    <header class="my-8">
      <h1>Standbasis School Dashboard</h1>
    </header>

    <div class="row">
      
      <div class="col-4 mt-4 border-inside">
        <div class="rounded p-4 text-center" style="background: #002060;">
          <p class="text-white" style="font-size: 18px; font-weight: bold;"> Promoting Data-culture in school(s) operation</p>
          <p class="text-white" style="font-size: 18px; font-weight: bold;"> Benefits: </p>
          <ul style="font-size: 12px; color: #dee2e6; line-height: 20px; ">
            <li>  Track and trend your school(s) health indicators in figures and graphics. </li>
            <li>  Benchmark your school performance in Curriculum Teaching, Teacher Resource, Learning environment, Student Development, Sustainability, Academic Performance and ‘Safety-Health-Environment-Security </li>
            <li>  Create and manage your school(s) internal standards. </li>
            <li>  Acquire data-driven early indicators for evidence-based planning, targeted intervention and intervention impact evaluation </li>
            <li>  Advertise your school(s) strengths to the world via direct web address to your School Data Dashboard  or quick-link from your school(s) website to your Dashboard.
Discover other tools and intelligence locked in your school(s) operations data.
 </li>
          </ul>
        </div>
      </div>

      <div class="col-6">
       
        <div class="row">
          <!-- First Row of Divs -->
          <div class="col-12">
            <div class="content-div">
              <!-- Content for the first div -->
              <img src="~/assets/dashboardpic1.png" class="img-fluid" />
            </div>
          </div>

          <div class="col-6">
            <div class="content-div">
              <!-- Content for the second div -->
              <img src="~/assets/dashboardpicsmall1.png" class="img-fluid"/>
            </div>
          </div>
          <div class="col-6">
            <div class="content-div">
              <!-- Content for the second div -->
              <img src="~/assets/dashboardpicsmall3.png" class="img-fluid"/>
            </div>
          </div>

          <div class="col-6 pt-2">
            <div class="content-div">
              <!-- Content for the third div -->
              <img src="~/assets/dashboardpicsmall2.png" class="img-fluid"/>
            </div>
          </div>

          <div class="col-6 pt-2">
            <div class="content-div">
              <!-- Content for the third div -->
              <img src="~/assets/dashboardpicsmall5.png" class="img-fluid"/>
            </div>
          </div>

        </div>       
        
      </div>

      <div class="col-2">
         <div class="content-div">
              <!-- Content for the third div -->
              <img src="~/assets/offerto.png" class="img-fluid"/>
        </div>
        <div class="mt-2">
          <ul class="list-unstyled">

            <li class="mb-4">
              <div class="rounded p-4 text-center w-100" style="background: #002060;">
                <a href="https://www.school-digital-transformation.com/login" _blank> Login </a>
              </div>
            </li>

            <li class="mb-4">
             <div class="rounded p-4 text-center w-100" style="background: #002060;">
                <a href="#" style=""> Activate School </a>
              </div>
            </li>

            <li class="mb-4">
              <div class="rounded p-4 text-center w-100 " style="background: #002060;">
                <a href="#" @click="showVideoModal"> About Us </a>
              </div>
            </li>

            <li class="mb-4">
              <div class="rounded p-4 text-center w-100 " style="background: #002060;">
                <a href="#" style=""> Forum </a>
              </div>
            </li>

          </ul>
        </div>
      </div>

    </div>

    <footer class="text-white mt-4 bg-dark p-3">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <p class="text-right">
              &copy; 2023 Standbasis
            </p>
          </div>
        </div>
      </div>
    </footer>

    <div class="modal fade" id="videoModal" tabindex="-1" role="dialog" ref="myModal" aria-labelledby="myModalLabel" aria-hidden="true">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-body">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"> <span aria-hidden="true">&times;</span> </button>
            <video controls>
              <source src="" type="video/mp4">
            </video>
          </div>
        </div>
      </div>
    </div>

    <div class="modal" tabindex="-1" role="dialog" ref="myModal">
      <div class="modal-dialog" role="document">
        <div class="modal-content">
          <form @submit.prevent="submitForm">
            <!-- Form fields go here -->
            <div class="modal-footer">
              <button type="button" class="btn btn-secondary" @click="hideModal">Close</button>
              <button type="submit" class="btn btn-primary">Submit</button>
            </div>
          </form>
        </div>
      </div>
    </div>

  </div>

  
</template>

<script>
export default {
  methods: {
    showVideoModal() {
      this.$refs.myModal.classList.add('show');
    },
    hideVideoModal() {
      this.$refs.myModal.classList.remove('show');
    },
   
  },
};
</script>

<style scoped>
.footer {
  background-color: #333;
  color: #fff;
  padding: 20px;
}

.footer p {
  font-size: 18px;
}

.border-inside {
    border: 2px solid #333; /* Adjust the color and width as needed */
    padding: 10px; /* Add padding to separate the border from the content */
  }

</style>
