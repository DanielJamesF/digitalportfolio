<template>
  <section id="contact">
    <div class="row" id="head">
      <div class="col">
        <h2>Contact</h2>
      </div>
    </div>
    <div class="row">
      <div class="col">
        <form class="p-1" id="fs-frm" name="simple-contact-form" accept-charset="utf-8"
          action="https://formspree.io/f/xdobpjrz" method="post">
          <br />
          <fieldset id="fs-frm-inputs">
            <div class="row">
              <div class="col-md-3">
                <label for="full-name">Name</label>
              </div>
              <div class="col-md-9">
                <input class="form-control" type="text" name="name" id="full-name" placeholder="name" required />
              </div>
            </div>
            <br />
            <div class="row">
              <div class="col-md-3">
                <label for="surname">Surname</label>
              </div>
              <div class="col-md-9">
                <input class="form-control" type="text" name="name" id="surname" placeholder="surname" required />
              </div>
            </div>
            <br />
            <div class="row">
              <div class="col-md-3">
                <label for="email-address">Email Address</label>
              </div>
              <div class="col-md-9">
                <input class="form-control" type="email" name="_replyto" id="email-address"
                  placeholder="email@gmail.com" required />
              </div>
            </div>
            <br />
            <div class="row">
              <div class="col-md-3">
                <label for="phone numbeer">Phone</label>
              </div>
              <div class="col-md-9">
                <input class="form-control" type="number" name="number" id="phone number" placeholder="enter phone num"
                  required />
              </div>
            </div>
            <br />
            <div class="row">
              <div class="col-md-3">
                <label for="subject">Subject</label>
              </div>
              <div class="col-md-9">
                <input type="text" class="form-control" name="_subject" id="subject" placeholder="what is up?"
                  required />
              </div>
            </div>
            <br />
            <div class="row justify-content-center">
              <label for="message">Message</label>
              <div class="col">
                <textarea class="form-control" rows="4" name="message" id="message"
                  placeholder="leave a message"></textarea>
              </div>
              <input type="hidden" name="_subject" id="email-subject" value="Contact Form Submission" />
            </div>
          </fieldset>
          <br />
          <input type="submit" value="Submit" class="btn btn-outline-primary" />
        </form>
      </div>
    </div>
  </section>
</template>
  
<script>
export default {};
</script>
  
<style scoped>
#head {
  height: 20vh;
  display: flex;
  justify-content: center;
  align-items: center;
  border: solid #151414;
}

#contact {
  min-height: 100vh;
  padding: 80px;
}

h2 {
  font-size: 70px;
  text-shadow: 1.5px 1.5px gray;
}

textarea:hover, input:hover {
  border-color: #151414;
}
</style>