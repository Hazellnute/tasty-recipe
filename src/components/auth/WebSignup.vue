<template>
  <div class="container-fluid py-5" style="background-color: #f5f5f5">
    <div style="background-color: #ffffff" class="p-5 m-auto signup-form">
      <div class="text-center">
        <img src="@/assets/images/Logo.png" alt="Logo" />
        <h2 class="mt-4">Create your account</h2>
        <p>Enter your details to use all the app features.</p>
      </div>
      <form class="mt-3">
        <div class="row">
          <div class="col-md-6"><base-input type="text" identity="firstname" placeholder="Ex: Jack" label="Firstname"></base-input>
          </div>
          <div class="col-md-6">
            <base-input type="text" identity="lastname" placeholder="Ex: Daniel" label="Lastname"></base-input>
          </div>
        </div>
        <div class="my-4">
          <base-input type="text" identity="username" placeholder="Your username" label="Username"></base-input>
        </div>
        <div class="my-4">
          <base-input type="email" identity="email" placeholder="Your email address" label="Email"></base-input>
        </div>
        <div class="my-4">
          <base-input type="password" identity="password" placeholder="Your password" label="Password"></base-input>
        </div>
        <div class="my-4">
          <base-input type="email" identity="confirmationPassword" placeholder="Same with Password" label="Confirmation Password"></base-input>
        </div>
        <div class="my-4">
          <base-input type="file" identity="recipeImage" label="Profile Photo" isImage="true">
            <div>
  	          <div class="border p-1 mt-2 rounded-circle" >
                <img src="../../assets/images/user.png" class="rounded-circle" width="140" height="150" style="object-fit: cover"/>
              </div>
              <div class="text-center" style="transform: translateY(-24px)" >
                <i class="fa-solid fa-camera fs-5 p-2 rounded-circle bg-white" ></i>
              </div>
          </div>
          </base-input>
        </div>
        <base-button class="w-100 login my-3"> Register </base-button>
      </form>
      <div class="text-center mt-4">
        <p class="fw-semibold">
          Already have account?<span style="color: #4c4ddc"
            ><router-link to="/login" class="text-decoration-none">
              Login</router-link
            ></span
          >
        </p>
      </div>
    </div>
  </div>
</template>

<script setup>
import BaseInput from "../ui/BaseInput.vue";
import BaseButton from "../ui/BaseButton.vue";
</script>
