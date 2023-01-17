<template >
  <section id="resume">
    <div class="row" id="head">
      <div class="col">
        <h2>Resume</h2>
      </div>
    </div>
    <div class="container">
      <h3 class="py-3">Education:</h3>
      <div class="row" id="education">
        <div class="col">
          <div class="row p-2">
            <div class="col-4 col-md-4">
              <p>March 2022 - present</p>
            </div>
            <div class="col-2 col-md-1">
              <span>-</span>
            </div>
            <div class="col-6 col-md-7">
              <p>
                I am attendiing Life Choices Academy where I am learning to
                code, where we recently covered HTML, CSS, Bootstrap, mySQL,
                JavaScript and Vuex
              </p>
            </div>
          </div>
          <div class="row p-2">
            <div class="col-4 col-md-4">
              <p>2015 - 2019</p>
            </div>
            <div class="col-2 col-md-1">
              <span>-</span>
            </div>
            <div class="col-6 col-md-7">
              I attended Grassy Park high School and got my NQ4 form Grassy Park
              High School from which I matriculated with a Diploma pass
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container" >
      <h3 class="py-3">Skills:</h3>
      <div class="row" id="skills">
        <div class="col">
          
          <h4 class="">Technical Skills</h4>
          <div class="row">
            <div class="col text-start">
              <div class="row">
                <div class="col">
                  <h6>Html</h6>
                  <div class="progress">
                    <div class="progress-bar progress-bar-striped active rounded-pill" role="progressbar" style="width: 78%"
                    aria-valuenow="70%" aria-valuemin="0" aria-valuemax="100">
                    <span>78%</span>
                </div>
              </div>
            </div>
            <div class="col">
              <h6>CSS</h6>
              <div class="progress">
                <div class="progress-bar progress-bar-striped active rounded-pill" role="progressbar" style="width: 73%"
                  aria-valuenow="55" aria-valuemin="0" aria-valuemax="100">
                  <span>73%</span>
                </div>
              </div>
            </div>
            <div class="col">
              <h6>Bootstrap</h6>
              <div class="progress">
                <div class="progress-bar progress-bar-striped active rounded-pill" role="progressbar" style="width: 70%"
                aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
                <span>70%</span>
              </div>
            </div>
          </div>
          </div>
          <div class="row">
            <div class="col">
              <h6 class="p-1">mySQL</h6>
              <div class="progress">
                <div class="progress-bar progress-bar-striped active rounded-pill" role="progressbar" style="width: 68%"
                aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
                <span>68%</span>
              </div>
            </div>
          </div>
          <div class="col">
            <h6 class="p-1">JavaScript</h6>
            <div class="progress">
              <div class="progress-bar progress-bar-striped active rounded-pill" role="progressbar" style="width: 57%"
              aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
              <span>57%</span>
            </div>
          </div>
        </div>
        <div class="col">
          <h6 class="p-1">Vuex</h6>
          <div class="progress">
            <div class="progress-bar progress-bar-striped active rounded-pill" role="progressbar" style="width: 56%"
            aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
            <span>56%</span>
          </div>
        </div>
            </div>
          </div>
          <div class="row">
            <div class="col">
              <h6 class="p-1">Node.js</h6>
              <div class="progress">
                <div class="progress-bar progress-bar-striped active rounded-pill" role="progressbar" style="width: 40%"
                  aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
                  <span>40%</span>
                </div>
              </div>
            </div>
            <div class="col">
              <h6 class="p-1">Express.js</h6>
              <div class="progress">
                <div class="progress-bar progress-bar-striped active rounded-pill" role="progressbar" style="width: 37%"
                aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
                <span>37%</span>
              </div>
            </div>
          </div>
          <div class="col">
              
          </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  </div>
    <div class="row d-flex justify-content-center">
      <h4 class="p-1">Soft Skills</h4>
      <div class="col text-center">
        <ul class="list-group">
          <li class="list-group-item m-1 p-2">Creativity</li>
          <li class="list-group-item m-1 p-2">Critical thinking</li>
          <li class="list-group-item m-1 p-2">Time management</li>
          <li class="list-group-item m-1 p-2">Communication</li>
        </ul>
      </div>
    </div>
  </section>
</template>
  
<script>
</script>

<style scoped>
#head {
  height: 20vh;
  display: flex;
  justify-content: center;
  align-items: center;
  border: solid #151414;
}

#resume {
  min-height: 100vh;
  padding: 80px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

h2 {
  font-size: 70px;
  text-shadow: 1.5px 1.5px gray;
}

h3 {
  font-size: 30px;
  text-shadow: 1.2px 1.2px gray
}

h4 {
  /* font-size: 35px; */
  text-shadow: 0.9px 0.9px gray;
}

span {
  color: blue;
}

#education {
  height: 30vh;
  padding: 20px;
  border-bottom: 0.5px solid black;
  border-top: 0.5px solid black;
  display: flex;
  justify-content: center;
  align-items: center;
}

#skills {
  height: 30vh;
  padding: 20px;  
  border-top: 0.5px solid black;
}
</style>