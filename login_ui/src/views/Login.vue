<template>
  <section class="container-fluid">
      <div class="row justify-content-center">
          <div class="col-lg-4">
              <div class="login-panel bg-white text-left">
                  <h1 class="display-3 font-weight-bold">MY MILL</h1>
                  <br>
                    <br>
                    <form action="">
                        <div class="form-group">
                            <label for="email" class="text-sm-left font-weight-bold input-label ">E-MAIL</label>
                            <input class="form-control" type="email" placeholder="Enter email">
                        </div>
                        <br>
                        <div class="form-group">
                            <label for="pass" class="font-weight-bold input-label">PASSWORD</label>
                            <input class="form-control" id="password-field" type="password" placeholder="Enter password">
                        </div>
                        <div class="form-group text-center">
                            <p >Forgot password?<span><a href="#">  Recover hier</a><img class="icon" src="../assets/lock.png" alt=""></span></p>
                        </div>
                        <br>
                        <br>
                        <div class="form-group text-center">
                            <label class="checkbox">
                               <input type="checkbox"><span>I agree to the TERMS AND CONDITIONS</span> 
                            </label>
                            
                        </div>
                        
                        <div class="form-group text-center">
                            <button type="button" class="btn btn-primary btn-lg">LOG IN</button>
                        </div>
                    </form>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    .display-3{
       margin-left: -40px;
       font-weight: 10000px;
   }
   .font-weight-bold{
       font-weight: 10000px;
   }
    p{
        color:gray;
    }
    .login-panel{
        padding: 100px 0;

    }
    .login-panel h1{
        font-size: 50px;
        font-weight: 10px;
    }
    input[type='email']{
        border: none;
        background-color: rgba(222, 245, 247, 0.8);
        border-bottom: 2px solid rgb(8, 8, 105);
    }
    input[type='password']{
        background-image: url(../assets/eye.png);
        background-position: right;
        background-repeat: no-repeat;
        background-size: 30px;
        background-color: rgba(222, 245, 247, 0.8);
        border: none;
        border-bottom: 2px solid rgb(8, 8, 105);
    
       }
       
   
   .icon{
       margin-left: 3px;
       width: 10px;
   }
   a{
       text-decoration: underline;
    }
    span a{
     color: gray;
    }
    .btn-lg{
        background: rgb(8, 8, 105);
        width: 85%;
    }
    // custom für checkbox
    input[type=checkbox]{
        margin-right: 7px;
        
    }
   
    .checkbox {
        display: inline-flex;
        cursor: pointer;
        position: relative;
    }

    .checkbox > span {
        color: #34495E;
        padding: 0.5rem 0.25rem;
    }

    .checkbox > input {
        height: 25px;
        width: 25px;
        -webkit-appearance: none;
        -moz-appearance: none;
        -o-appearance: none;
        appearance: none;
        border: 1px solid #34495E;
        border-radius: 4px;
        outline: none;
        transition-duration: 0.3s;
        background-color:rgb(8, 8, 105);
        cursor: pointer;
    }

    .checkbox > input:checked {
        border: 1px solid #41B883;
        background-color: rgb(189, 189, 194);
    }

    .checkbox > input:checked + span::before {
        content: '\2713';
        display: block;
        text-align: center;
        color: rgb(8, 8, 105);
        position: absolute;
        left: 0.7rem;
        top: 0.2rem;
    }

    .checkbox > input:active {
        border: 2px solid #34495E;
    }

   
 

</style>