<template>
    <div>
        <div class="container-fluid">
            <div class="row navbar">
                <div class = "col-md-6 col-sm-12 navbar_icon">
                    <i class="material-icons md-36">perm_identity</i>
                </div>
                <div class = "col-md-6 col-sm-12 navbar_name">
                    ceitgames
                </div>
            </div>
        </div>

        <div class="form_container">
            <div class="register_box">
                <div class="header">
                <div class="form_title">
                     ثبت نام
                </div>
                <form>
                    <div class="form_item">
                        <input type="password" name="username" class="float-left" placeholder="نام کاربری من">
                        <i class="material-icons md-36 form-icon" >perm_identity</i>

                    </div>
                    <div class="form_item">
                        <input type="text" name="email_phone" class="float-left" placeholder="رایانامه">
                        <i class="material-icons md-36 form-icon" >email</i>

                    </div>
                    <div class="form_item">
                        <input type="password" name="password" class="float-left" placeholder="رمز عبور">
                        <i class="material-icons md-36 form-icon">https</i>

                    </div>
                    <div class="accept_conditions">
                            <input type="checkbox" name="check">
                                <span class="unchecked"> <i class="material-icons md-36 form-icon">check_box_outline_blank</i> </span>
                                <span class="checked"> <i class="material-icons md-36 form-icon">check_box</i> </span>
                        <a href="#">
                            قوانین
                        </a>
                        را می پذیرم
                        <button class="register_button" type="submit">
                            ثبت نام
                        </button>
                    </div>



                </form>
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
  @import '../statics/register.css';
  @import "https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css";
  @import "https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css";
  body{
      background-color: #0086b3;
      font-family: Shabnam;
  }

</style>
