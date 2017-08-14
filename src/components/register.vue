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
            <div class="register_box">
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
                    <label class="accept_conditions">
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
                    </label>



                </form>

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
  .register_box{
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

.form-icon{
    color: inherit;
    margin-left: 2%;
}


input:focus{
    outline: none;
    color:#cc0066;
    border-bottom: 2px solid #cc0066;
}

input:focus ~ .form-icon{
    color: #CC0066;
}


.register_button{
    width: 100%;
    font-family: 'Shabnam';
    margin-top: 15%;
    background-color: #4452cc;
    border: none;
    color: white;
    text-align: center;
    padding: 3%;
}

.register_button:hover{
    background-color: #2c2acc;
}

input, .register_button{
    font-size: 1.3em;
    font-family: 'Shabnam';
}

.form_item{
    color:#b3b3b3;
    padding-bottom: 12%;
    /*display: flex;*/
    /*justify-con   tent: center;*/
}


.form_title{
    color: #707070;
    font-weight: bold;
    font-size: 1.5em;
    text-align: center;
    margin-top: 10%;
    margin-bottom: 13%
}


.accept_conditions{
    margin-top: 9%;
    font-size: 1.3em;
    color: #707070;
}

conditions_link{
    color: blueviolet;
}


.accept_conditions input {display:none;}


input ~ .checked{
    display: none;
}


input:checked + .unchecked {
    display:none;
}

input:checked ~ .checked {
    display:inline;
}

.checked{
    color: #cc0066;
}

button{
    opacity: 0.65;
    cursor: not-allowed;
}

input:checked ~ .register_button{
    opacity: 1;
    cursor: pointer;
}

.float-left{
    float: left;
}











</style>
