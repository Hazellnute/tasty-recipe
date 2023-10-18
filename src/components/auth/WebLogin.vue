<template>
    <div class="container-fluid py-5" style="background-color: #f5f5f5;">
      <div style="background-color: #ffffff; width: 400px min-height: 100vh;" class="p-5 m-auto login-form">
        <div class="text-center">
          <img src="../../assets/images/Logo.png" alt="Logo" />
          <h2 class="mt-4">Log in to your account</h2>
          <p>Welcome back! Please enter your details.</p>
        </div>
        <form>
          <div class="my-4">
            <base-input type="email" identity="email" placeholder="Your username" label="Email"></base-input>
          </div>
          <div class="my-4">
            <base-input type="password" identity="password" placeholder="Your password" label="Password"></base-input>
          </div>
          <base-button class="w-100 login my-3"> Register </base-button>
        </form>
        <div class="text-center mt-4">
          <p class="fw-semibold">
            Don’t have an account?<span style="color: #4c4ddc">
              <router-link to="/signup" class="text-decoration-none"> Signup</router-link></span>
          </p>
        </div>
      </div>
    </div>
  </template>

<script setup>
import BaseInput from "../ui/BaseInput.vue" ;
import BaseButton from "../ui/BaseButton.vue";
</script>