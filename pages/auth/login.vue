<script setup>
import { reactive } from 'vue';
import InputText from '~/components/Form/InputText.vue';

const form = reactive({
  email: '',
  password: '',
});

const Submit = () => {
  console.log(form);
};
</script>

<template>
  <div class="min-h-screen flex items-center justify-center bg-gradient-to-r from-blue-500 to-indigo-600">
    <div class="w-full">
      <div class="card bg-white p-8 rounded-lg shadow-2xl transform transition-transform hover:scale-105 md:w-3/4 mx-auto lg:w-1/3">
        <h3 class="text-center text-3xl font-bold mb-6 text-gray-800 dark:text-white">User Login</h3>
  
        <form @submit.prevent="Submit" class="max-w-sm mx-auto space-y-5">
          
          <!-- Email Field -->
          <div class="relative z-0 w-full mb-5 group">
            <FormInputText id="email" type="email" :modalValue="form.email" @update:modalValue="form.email = $event" />
            <FormLabel for="email">Your Email</FormLabel>
          </div>

          <!-- Password Field -->
          <div class="relative z-0 w-full mb-5 group">
            <InputText id="password" type="password" :modalValue="form.password" @update:modalValue="form.password = $event" />
            <FormLabel for="password">Password</FormLabel>
          </div>

          <!-- Remember Me Checkbox -->
          <div class="flex items-center">
            <input id="remember" type="checkbox" class="w-4 h-4 text-indigo-600 border-gray-300 rounded focus:ring-indigo-500 dark:bg-gray-700 dark:border-gray-600 dark:ring-offset-gray-800 dark:focus:ring-indigo-600" />
            <label for="remember" class="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300">Remember me</label>
          </div>

          <!-- Login Button -->
          <ButtonPrimary>Login</ButtonPrimary>
        </form>

        <SocialLogin />
      </div>
    </div>
  </div>
</template>
