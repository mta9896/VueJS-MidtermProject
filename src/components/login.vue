<template>
    <!--<meta name="viewport" content="width=device-width" />-->
  <div>
    <div class="container-fluid">
        <div class="row navbar">
             <span class = "col-md-6 col-sm-12 navbar_icon">
                <i class="material-icons md-36">perm_identity</i>
            </span>
            <span class = "col-md-6 col-sm-12 navbar_name">
                ceitgames
            </span>
        </div>
        <div class="form_container">
            <div class="login_box">
                <div class="header">
                <div class="form_title">
                     ورود
                </div>
                <form>
                    <div class="form_item">


                        <input type="text" name="email_phone" class="float-left" placeholder="ایمیل یا شماره تلفن">
                        <i class="material-icons md-36 form-icon">email</i>

                    </div>
                    <div class="form_item">

                        <input type="password" name="password" class="float-left" placeholder="رمز عبور">
                        <i class="material-icons md-36 form-icon">https</i>

                    </div>
                    <button class="login_button" type="submit">
                            ورود
                    </button>
                    <div class="forgot_password">
                        <a href="#">
                            رمزمو یادم رفته
                        </a>
                    </div>
                </form>
                </div>
                <div class="sign_up">
                    حساب کاربری ندارید؟
                    <a class="form_link" href="register.html">
                         ثبت نام کنید
                    </a>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {}
  }
}
</script>

<style>
  @import '../statics/global.css';
  @import '../statics/login.css';
  @import "https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css";
  @import "https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css";
  body{
      background-color: #0086b3;
      font-family: Shabnam;
  }

</style>
