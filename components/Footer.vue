<template>
  <div class="bg-[#F6F6F7] px-4 pt-16 md:px-24 lg:px-8">
    <!-- <div class="bg-[#F6F6F7] px-4 pt-16 md:px-24 lg:px-8"> -->
    <div class="mx-auto md:w-[80%] w-[95%]"> 

      <div class="grid gap-16 row-gap-10 mb-8 lg:grid-cols-6">
        <div class="md:max-w-md lg:col-span-2">
          <a href="/" aria-label="Go home" title="Company" class="inline-flex items-center">
            <svg class="w-8 text-deep-purple-accent-400" viewBox="0 0 24 24" stroke-linejoin="round" stroke-width="2" stroke-linecap="round" stroke-miterlimit="10" stroke="currentColor" fill="none">
              <rect x="3" y="1" width="7" height="12"></rect>
              <rect x="3" y="17" width="7" height="6"></rect>
              <rect x="14" y="1" width="7" height="6"></rect>
              <rect x="14" y="11" width="7" height="12"></rect>
            </svg>
            <span class="ml-2 text-xl tracking-wide text-gray-800">Adnegs<span class="font-bold">Blog</span></span>
          </a>
          <div class="mt-4 lg:max-w-sm">
            <p class="text-sm text-gray-800">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam.
            </p>
            <p class="mt-4 text-sm text-gray-800">
              Eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </p>
          </div>
        </div>
        
        <div class="grid gap-5 row-gap-8 lg:col-span-4 md:grid-cols-4">
          <div class="mb-2 md:mb-0">
            <p class="font-semibold tracking-wide text-gray-800">Quick Link</p>
            <ul class="mt-2 space-y-2">
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Home</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">About</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Blog</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Archived</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Author</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Contact</a>
              </li>
            </ul>
          </div>
          
          <div class="mb-2 md:mb-0">
            <p class="font-semibold tracking-wide text-gray-800">Category</p>
            <ul class="mt-2 space-y-2">
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Lifestyle</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Technology</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Travel</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Business</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Economy</a>
              </li>
              <li>
                <a href="/" class="text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Sports</a>
              </li>
            </ul>
          </div>
          
          <div class="w-full p-5 text-center bg-white rounded-md shadow md:max-w-md lg:col-span-2">
          <span class="text-lg font-bold text-[#181A2A]">Weekly newsletter</span>
          <p class="text-[#696A75]">Get blog articles and offers via email</p>
          <form class="flex flex-col mt-4">
            <input
              placeholder="Email"
              required=""
              type="text"
              class="flex-grow w-full h-12 px-4 mb-3 transition duration-200 bg-white border border-gray-300 rounded-md focus:outline-[#4B6BFB]"
            />
            <button
              type="submit"
              class="inline-flex items-center justify-center h-12 px-6 font-medium text-white transition duration-200 rounded-md bg-[#4B6BFB]"
            >
              Subscribe
            </button>
          </form>
        </div>
    
        </div>
      </div>

      <div class="flex flex-col-reverse justify-between pt-5 pb-10 border-t lg:flex-row">
        <p class="text-sm text-gray-600">
          © Copyright 2024 Lorem Inc. All rights reserved.
        </p>
        <ul class="flex flex-col mb-3 space-y-2 lg:mb-0 sm:space-y-0 sm:space-x-5 sm:flex-row">
          <li>
            <a href="/" class="text-sm text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">F.A.Q</a>
          </li>
          <li>
            <a href="/" class="text-sm text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Privacy Policy</a>
          </li>
          <li>
            <a href="/" class="text-sm text-gray-600 transition-colors duration-300 hover:text-deep-purple-accent-400">Terms &amp; Conditions</a>
          </li>
        </ul>
      </div>

    </div>
  </div>
</template>