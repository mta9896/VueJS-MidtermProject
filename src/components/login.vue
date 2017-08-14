<template>
  <div>
    <div class="navbar">
             <span class = "navbar_icon">
                <i class="material-icons md-36">perm_identity</i>
            </span>
            <span class = "navbar_name">
                ceitgames
            </span>
        </div>

        <div class="form_container">
            <div class="login_box">
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
                <div class="sign_up">
                    حساب کاربری ندارید؟
                    <a class="form_link" href="register.html">
                         ثبت نام کنید
                    </a>
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
  .login_box{
    background-color: white;
    margin: auto;
    position: relative;
    margin-top: 10%;
    margin-bottom: 20%;
    padding-left: 5%;
    padding-right: 5%;
    border-radius: 5px;
    box-shadow: 2px 2px 3px 3px #006080;
    direction: rtl;
}

.form_container{
    display: flex;
    width: 100%;
}

input[type=text], input[type=password] {
    width: 80%;
    border-top: 2px solid white;
    border-right: 2px solid white;
    border-left: 2px solid white;
    border-bottom: 2px solid #ccc;
    padding-top: 9%;

}

input:focus{
    outline: none;
    color:#cc0066;
    border-bottom: 2px solid #cc0066;
}

input:focus ~ .form-icon{
    color: #CC0066;
}


.login_button{
    width: 100%;
    font-family: 'Shabnam';
    margin-top: 15%;
    background-color: #cc0066;
    border: none;
    color: white;
    text-align: center;
    padding: 3%;
}

.login_button:hover{
    background-color: #99004d;
}

input, .login_button{
    font-size: 1.3em;
    font-family: 'Shabnam';
}

.forgot_password{
    margin-top: 4%;
    text-align: center;
    font-size: 1.2em;
}

.forgot_password a{
    color: gray;
}

.forgot_password a:hover{
    color: #cc0066;
}

.form_item{
    color:#b3b3b3;
    padding-bottom: 12%;
    /*display: flex;*/
    /*justify-content: center;*/
}


.form_title{
    color: #707070;
    font-weight: bold;
    font-size: 1.5em;
    text-align: center;
    margin-top: 10%;
    margin-bottom: 13%
}

.sign_up{
    background-color: #e5e5e5;
    margin-top: 15%;
    padding:5%;
    margin-left:-30.5%;
    margin-right: -30.5%;
    border-bottom-left-radius: 5%;
    border-bottom-right-radius: 5%;
    text-align: center;
}

.form_link{
    color: #4653ff;
}

.form-icon{
    color: inherit;
    margin-left: 2%;
    order:1;
}

.float-left{
    float: left;
}


</style>
