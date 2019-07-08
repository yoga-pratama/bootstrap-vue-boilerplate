<template>
  <login-layout>
    <section class="h-100">
      <div class="container h-100">
        <div class="row justify-content-md-center h-100">
          <div class="card-wrapper">
           <!--  <div class="brand"></div> -->
            <div class="card fat">
              <div class="card-body">
                <h4 class="card-title">Login</h4>
                <form>
                  <div class="form-group">
                    <label for="email">Username</label>
                    <input
                      id="username"
                      type="text"
                      class="form-control"
                      name="username"
                      value
                      required
                      autofocus
                      v-model="username"
                    >
                    <div class="invalid-feedback">Username is invalid</div>
                  </div>

                  <div class="form-group">
                    <label for="password">
                      Password
                      <!--  <a href="forgot.html" class="float-right">Forgot Password?</a> -->
                    </label>
                    <input
                      id="password"
                      type="password"
                      class="form-control"
                      name="password"
                      required
                      data-eye
                      v-model="password"
                    >
                    <div class="invalid-feedback">Password is required</div>
                  </div>

                  <!--  <div class="form-group">
                    <div class="custom-checkbox custom-control">
                      <input
                        type="checkbox"
                        name="remember"
                        id="remember"
                        class="custom-control-input"
                      >
                      <label for="remember" class="custom-control-label">Remeber Me</label>
                    </div>
                  </div>-->

                  <div class="form-group m-0">
                    <button type="submit" class="btn btn-primary btn-block">Login</button>
                  </div>
                  <div class="mt-4 text-center"></div>
                </form>
              </div>
            </div>
            <div class="footer">Copyright &copy; {{ new Date().getFullYear() }} &mdash; Company</div>
          </div>
        </div>
      </div>
    </section>
  </login-layout>
</template>

<style>
    .img-set{
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 35%;
    }

    .centering-text{
      display: block;
      margin-left:  auto;
      margin-right:  auto;
      text-align: center;
    }
</style>


<script>
import LoginLayout from "../layouts/LoginLayout.vue";
export default {
  name: "login",
  components: {
    LoginLayout
  },
  data(){
      return {
          username : null,
          password : null
      }
  }
};
</script>

