<template>
  
    <!-- SERVICES -->
    
    <div id="services" class="container-fluid mt-content-container mt-container-services">
      
      <div class="row mt-top-row text-muted">
        
        <div class="col-md-4 col-md-offset-4">
          <h1>WHAT I DO</h1>
          <div class="mt-block-line"></div>
          <p class="lead">These are the skills I can offer to help build and deploy your web application<p>          
       </div>
 
      </div> <!-- .row -->
      
      <!-- SERVICE THUMBNAILS -->

      <div class="row mt-service-thumb-row">
        

        <div class="col-md-4">
          <a href="#services" alt="Web Programming">            
            <div class="thumbnail mt-service-thumb">
              <div class="caption mt-service-thumb-text">
                <span class="fa fa-code fa-5x"></span>
                <h3>Web Programming</h3>
                <p>I can help you build your web applications using technologies that include HTML, CSS, Javascript, Bootstrap, JQuery, AngularJS, PHP, and MySQL</p>
              </div>
            </div>
          </a>   
        </div>
  
        <div class="col-md-4">
          <a href="#services" alt="Cloud Hosting">
            <div class="thumbnail mt-service-thumb">
              <div class="caption mt-service-thumb-text">
                <span class="fa fa-cloud fa-5x"></span>
                <h3>Cloud Hosting</h3>
                <p>I can help you provision cloud hosting solutions that include Amazon Web Services (AWS), Microsoft Azure, Google Cloud, Google Apps, and WireNine</p>
              </div>
            </div>
          </a>
        </div>
        
        <div class="col-md-4">
          <a href="#services" alt="Development Process">
            <div class="thumbnail mt-service-thumb">
              <div class="caption mt-service-thumb-text">
                <span class="fa fa-puzzle-piece fa-5x"></span>
                <h3>Development Process</h3>
                <p>I can help you organize your projects using standard Agile SDLC methodologies like SCRUM, KANBAN, and LEAN</p>
              </div>
            </div>
          </a>
        </div>
      </div> <!-- .row -->
      
      <!-- END SERVICE THUMBNAILS -->
      
    </div> <!-- .container -->
    
    <!-- END SERVICES -->
    
</template>

<script>
export default {

}
</script>

<style scoped>
.mt-container-services {
	background-color: #F5F5F5;
}

.mt-service-thumb-row {
	margin-top: 50px;
}

.mt-service-thumb-row a:hover {
	text-decoration: none;
}

.mt-service-thumb {
	background-color: #F5F5F5;
	border-color: #13456C;
	height: 225px;
}

.mt-service-thumb-text {
	text-align: center;
	color: #777777 !important;
}

.fa-code, .fa-cloud, .fa-puzzle-piece {
	color: #13456C !important;
}

.mt-service-thumb:hover {
	background-color: white !important;
}


/***************************/
/*** PORTFOLIO CONTAINER ***/
/***************************/


.mt-container-portfolio {
	background: 
		linear-gradient(
          rgba(19, 69, 108, 0.4),
          rgba(19, 69, 108, 0.6)
          );
	width: 100%;
	background-size: cover;
}

.mt-portfolio-thumb-row {
	margin-top: 25px;
}

.mt-portfolio-thumb {
	background-color: #13456C;
	box-shadow: 5px 5px 10px #BBBBBB;
}

.mt-portfolio-thumb-text {
	text-align: center;
	color: white !important;
}

.mt-portfolio-thumb:hover {
	background-color: white !important;
}

.mt-portfolio-thumb:hover h4 {
	background-color: white !important;
	color: #13456C !important;
}


/*************************/
/*** CONNECT CONTAINER ***/
/*************************/


.mt-container-connect {
	background-color: #F5F5F5;
}

.mt-social-links-row {
	padding-bottom: 30px;
}

.mt-social-links {
	padding-top: 20px;
	padding-bottom: 0px;
}

.mt-social-links a {
	color: #13456C;
}

.mt-fa-social {
	color: #13456C;
	text-shadow: 4px 4px 5px #BBBBBB
}

.mt-social-links a:hover {
	text-decoration: none;
}

.mt-social-links a:hover .mt-fa-social {
	color: #777777;
}

.mt-connect-form-row {
	padding-top: 20px;
}

.btn {
	color: #777777;
}

.form-control {
	font-size: 125%;
}

.mt-fa-button {
	color: #13456C;
}
</style>