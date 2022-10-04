<template>
    <div id="contact" class="container-fluid">
      <div class="row">
        <div class="col">
          <h1 class="display-4">Contact...</h1>
          <div class="row">
            <div class="col border border-1 rounded-4">
              <form
                class="rounded p-4"
                id="fs-frm"
                name="simple-contact-form"
                accept-charset="utf-8"
                action="https://formspree.io/f/xdobpjrz"
                method="post"
              >
                <br />
                <fieldset id="fs-frm-inputs">
                  <div class="row">
                    <div class="col">
                      <label for="full-name">Name</label>
                    </div>
                    <div class="col">
                      <input
                        class="form-control"
                        type="text"
                        name="name"
                        id="full-name"
                        placeholder="name"
                        required
                      />
                    </div>
                  </div>
                  <br />
                  <div class="row">
                    <div class="col">
                      <label for="surname">Surname</label>
                    </div>
                    <div class="col">
                      <input
                        class="form-control"
                        type="text"
                        name="name"
                        id="surname"
                        placeholder="surname"
                        required
                      />
                    </div>
                  </div>
                  <br />
                  <div class="row">
                    <div class="col">
                      <label for="email-address">Email Address</label>
                    </div>
                    <div class="col">
                      <input
                        class="form-control"
                        type="email"
                        name="_replyto"
                        id="email-address"
                        placeholder="email@gmail.com"
                        required
                      />
                    </div>
                  </div>
                  <br />
                  <div class="row">
                    <div class="col">
                      <label for="phone numbeer">Phone</label>
                    </div>
                    <div class="col">
                      <input
                        class="form-control"
                        type="number"
                        name="number"
                        id="phone number"
                        placeholder="+27 123 456 789"
                        required
                      />
                    </div>
                  </div>
                  <br />
                  <div class="row">
                    <div class="col">
                      <label for="subject">Subject</label>
                    </div>
                    <div class="col">
                      <input
                        type="text"
                        class="form-control"
                        name="_subject"
                        id="subject"
                        placeholder="what is up?"
                        required
                      />
                    </div>
                  </div>
                  <br />
                  <div class="row justify-content-center">
                    <label for="message">Message</label>
                    <div class="col">
                      <textarea
                        class="form-control"
                        rows="4"
                        name="message"
                        id="message"
                        placeholder="leave a message"
                      ></textarea>
                    </div>
                    <input
                      type="hidden"
                      name="_subject"
                      id="email-subject"
                      value="Contact Form Submission"
                    />
                  </div>
                </fieldset>
                <br />
                <input
                  type="submit"
                  value="Submit"
                  class="btn btn-outline-primary"
                />
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {};
  </script>
  
  <style scoped>
  #contact {
    padding-top: 10vh;
    min-height: 100vh;
    padding-bottom: 10vh;
  }
  </style>