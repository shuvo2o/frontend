<template>
    <div class="min-h-screen flex items-center justify-center bg-gradient-to-r from-blue-500 to-indigo-600">
      <div class="w-full">
        <div class="card bg-white p-10 rounded-lg shadow-2xl transform transition-transform hover:scale-105 md:w-3/4 mx-auto lg:w-1/3">
          <!-- Title -->
          <h3 class="text-center gap-5 text-3xl font-bold mb-10 text-gray-800 dark:text-white">User Registration</h3>
          
          <!-- Form -->
          <form class="max-w-sm mx-auto space-y-5">
            <!-- Name Fields -->
            <div class="grid md:grid-cols-2 gap-6 mt-10">
              <div class="relative z-0 w-full">
                <input type="text" id="floating_first_name" class="block py-4 px-0 w-full text-lg text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 focus:outline-none focus:ring-0 focus:border-indigo-600 peer dark:text-white dark:border-gray-600 dark:focus:border-indigo-500" placeholder=" " required />
                <label for="floating_first_name" class="absolute text-lg text-gray-500 dark:text-gray-400 peer-focus:text-indigo-600 dark:peer-focus:text-indigo-500 transition-all scale-75 -translate-y-8 top-4">First name</label>
              </div>
              <div class="relative z-0 w-full">
                <input type="text" id="floating_last_name" class="block py-4 px-0 w-full text-lg text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 focus:outline-none focus:ring-0 focus:border-indigo-600 peer dark:text-white dark:border-gray-600 dark:focus:border-indigo-500" placeholder=" " required />
                <label for="floating_last_name" class="absolute text-lg text-gray-500 dark:text-gray-400 peer-focus:text-indigo-600 dark:peer-focus:text-indigo-500 transition-all scale-75 -translate-y-8 top-4">Last name</label>
              </div>
            </div>
  
            <!-- Contact Fields -->
            <div class="relative z-0 w-full">
              <input type="tel" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" id="floating_phone" class="block py-4 px-0 w-full text-lg text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 focus:outline-none focus:ring-0 focus:border-indigo-600 peer dark:text-white dark:border-gray-600 dark:focus:border-indigo-500" placeholder=" " required />
              <label for="floating_phone" class="absolute text-lg text-gray-500 dark:text-gray-400 peer-focus:text-indigo-600 dark:peer-focus:text-indigo-500 transition-all scale-75 -translate-y-8 top-4">Phone Number</label>
            </div>
           
            <!-- Email and Password -->
            <div class="relative z-0 w-full">
              <input type="email" id="floating_email" class="block py-4 px-0 w-full text-lg text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 focus:outline-none focus:ring-0 focus:border-indigo-600 peer dark:text-white dark:border-gray-600 dark:focus:border-indigo-500" placeholder=" " required />
              <label for="floating_email" class="absolute text-lg text-gray-500 dark:text-gray-400 peer-focus:text-indigo-600 dark:peer-focus:text-indigo-500 transition-all scale-75 -translate-y-8 top-4">Email address</label>
            </div>
            <div class="relative z-0 w-full">
              <input type="password" id="floating_password" class="block py-4 px-0 w-full text-lg text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 focus:outline-none focus:ring-0 focus:border-indigo-600 peer dark:text-white dark:border-gray-600 dark:focus:border-indigo-500" placeholder=" " required />
              <label for="floating_password" class="absolute text-lg text-gray-500 dark:text-gray-400 peer-focus:text-indigo-600 dark:peer-focus:text-indigo-500 transition-all scale-75 -translate-y-8 top-4">Password</label>
            </div>
            <div class="relative z-0 w-full">
              <input type="password" id="floating_repeat_password" class="block py-4 px-0 w-full text-lg text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 focus:outline-none focus:ring-0 focus:border-indigo-600 peer dark:text-white dark:border-gray-600 dark:focus:border-indigo-500" placeholder=" " required />
              <label for="floating_repeat_password" class="absolute text-lg text-gray-500 dark:text-gray-400 peer-focus:text-indigo-600 dark:peer-focus:text-indigo-500 transition-all scale-75 -translate-y-8 top-4">Confirm password</label>
            </div>
  
            <!-- Submit Button -->
            <button type="submit" class="w-full bg-indigo-600 text-white text-lg rounded-lg py-4 font-semibold hover:bg-indigo-700 transition-transform focus:ring-4 focus:ring-indigo-300 dark:bg-indigo-500 dark:hover:bg-indigo-600 dark:focus:ring-indigo-800">Register</button>
          </form>
        </div>
      </div>
    </div>
  </template>
  