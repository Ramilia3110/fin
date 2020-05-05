<template>
  <div class="contact-form">
    <div class="contact-form__container">
      <div class="img-box">
        <h1>We'd love to hear from you ...</h1>
      </div>
      <div class="form-blog">
        <div class="form-box">
          <h1>contact us</h1>
          <form>
            <div class="text-box">
              <label for="fullname">Full Name :</label>
              <input
                type="text"
                name="fullname"
                id="fullname"
                placeholder="Enter Your Name"
                required
              />
            </div>
            <div class="text-box">
              <label for="email">Email :</label>
              <input
                type="email"
                name="email"
                id="email"
                placeholder="Enter Your Email"
                required="required"
              />
            </div>
            <div class="text-box">
              <label for="phonenumber">Phone Number :</label>
              <input
                type="text"
                name="phonenumber"
                id="phonenumber"
                placeholder="Enter Your Phone Number"
                required
              />
            </div>
            <div class="text-box">
              <label for="message">Message :</label>
              <textarea id="message"></textarea>
            </div>
            <input type="submit" class="btn" value="Send" />
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@mixin flexCenter {
  display: flex;
  justify-content: center;
  align-items: center;
}
.contact-form {
  margin-top: 9rem;
}
.contact-form__container {
  display: grid;
  grid-auto-columns: 1fr 1fr;
  grid-template-areas: "img-box form-blog";
}
.form-blog {
  grid-area: form-blog;
}
.form-box {
  min-width: 40rem;
  background: #fbfcfc;

  transform: translateX(-50%, -50%);
  padding: 3rem 4rem;
  border-radius: 0.8rem;
  text-align: center;
  box-shadow: 0 0 0.3rem #000000b3;
}
.form-box h1 {
  margin-top: 0;
  font-weight: 300;
  font-size: 2.2rem;
  color: #061b2e;
  text-transform: uppercase;
}
.text-box {
  border: 1px solid gray;
  margin: 0.8rem 0;
  padding: 1.2rem 1.8rem;
  border-radius: 0.8rem;
}
.text-box label {
  display: block;
  text-align: left;
  color: #25598d;
  text-transform: uppercase;
  font-size: 1.4rem;
}
.text-box input,
.text-box textarea {
  width: 100%;
  border: none;
  background: none;
  outline: none;
  font-size: 1.4rem;
  margin-top: 6px;
}
.btn {
  display: inline-block;
  background: #245688;
  padding: 1.4rem 0;
  color: #fff;
  text-transform: uppercase;
  cursor: pointer;
  border-radius: 0.8rem;
  margin-top: 0.8rem;
  width: 100%;
  font-size: 1.4rem;
  &:hover {
    background: #2c69a5;
  }
}
.img-box {
  grid-area: img-box;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-right: 3rem;
  text-align: center;

  h1 {
    color: #245688;
    font-size: 3rem;
    letter-spacing: 0.3rem;
    line-height: 5rem;
    font-weight: 500;
    text-align: center;
    padding: 0 5rem;
    text-transform: uppercase;
  }
}
@media only screen and (max-width: 992px) {
  .contact-form__container {
    @include flexCenter();
    flex-direction: column;
  }
  .form-blog {
    order: 2;
  }
  .img-box {
    order: 1;
    text-align: center;
    h1 {
      font-size: 3rem;
      padding: 3.8rem 1rem;
    }
  }
}
</style>
