
<template>
  
    <div class=" left-0 w-full h-full flex items-center justify-center bg-white z-50">

        
        <div class="flex top-8  items-center justify-center space-x-2">
       
            <div
                class="fixed top-0 left-0 right-0 bottom-0 w-full h-screen z-50 overflow-hidden bg-gray-700 opacity-75 flex flex-col items-center justify-center">
                <div v-if="myString === 'Succses'"
                    class="flex flex-row items-center rounded shadow-lg overflow-hidden w-full sm:w-11/12 md:max-w-2xl hover:shadow-xl bg-white hover:bg-green-50 dark:bg-gray-800 dark:hover:bg-gray-800 transition-transform hover:scale-95 group">
                    <div
                        class="h-full py-8 px-2 bg-green-300 group-hover:bg-green-400 dark:bg-gray-100 dark:group-hover:bg-gray-200">
                     <svg xmlns="http://www.w3.org/2000/svg"  
                            class="h-8 w-8 text-green-700 group-hover:text-green-800 dark:text-gray-600 dark:group-hover:text-gray-700"
                            fill="none" viewBox="0 0 24 24" stroke="currentColor" >
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                        </svg>
                    </div>
                    <div class="mx-4 flex-row w-full">
                        <div class="flex flex-row items-center justify-between">
                            <h1 class="text-lg sm:text-xl font-bold text-gray-800 dark:text-gray-200">
                                Sucsess
                            </h1>
                            <svg xmlns="http://www.w3.org/2000/svg" @click="Buutton" 
                                class="h-4 w-4 cursor-pointer text-gray-500 hover:text-gray-600 dark:text-gray-300 dark:hover:text-gray-200"
                                viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                                    clip-rule="evenodd" />
                            </svg>
                        </div>
                        <p class="text-xs sm:text-sm font-medium text-gray-500 pr-2 sm:pr-0 dark:text-gray-300">
                            Text Desc
                        </p>
                    </div>
                </div>
                <div v-if="myString === 'Warning'"
                    class="flex flex-row items-center rounded shadow-lg overflow-hidden w-full sm:w-11/12 md:max-w-2xl hover:shadow-xl bg-white hover:bg-yellow-50 dark:bg-gray-800 dark:hover:bg-gray-800 transition-transform hover:scale-95 group">
                    <div
                        class="h-full py-8 px-2 bg-yellow-300 group-hover:bg-yellow-400 dark:bg-gray-100 dark:group-hover:bg-gray-200">
                        <svg xmlns="http://www.w3.org/2000/svg"
                            class="h-8 w-8 text-yellow-700 group-hover:text-yellow-800 dark:text-gray-600 dark:group-hover:text-gray-700"
                            fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z" />
                        </svg>
                    </div>
                    <div class="mx-4 flex-row w-full">
                        <div class="flex flex-row items-center justify-between">
                            <h1 class="text-lg sm:text-xl font-bold text-gray-800 dark:text-gray-200">
                                Warning
                            </h1>
                            <svg xmlns="http://www.w3.org/2000/svg"  @click="Buutton"
                                class="h-4 w-4 cursor-pointer text-gray-500 hover:text-gray-600 dark:text-gray-300 dark:hover:text-gray-200"
                                viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd"   
                                    d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                                    clip-rule="evenodd" />  
                            </svg>
                        </div>
                        <p class="text-xs sm:text-sm font-medium text-gray-500 pr-2 sm:pr-0 dark:text-gray-300">
                            Text Desc
                        </p>
                    </div>
                </div>
                <div v-if="myString === 'Error'"
                    class="flex flex-row items-center rounded shadow-lg overflow-hidden w-full sm:w-11/12 md:max-w-2xl hover:shadow-xl bg-white hover:bg-green-50 dark:bg-gray-800 dark:hover:bg-gray-800 transition-transform hover:scale-95 group">
                    <div
                        class="h-full py-8 px-2 bg-pink-300 group-hover:bg-pink-400 dark:bg-gray-100 dark:group-hover:bg-gray-200">
                        <svg xmlns="http://www.w3.org/2000/svg"
                            class="h-8 w-8 text-pink-700 group-hover:text-pink-8    00 dark:text-gray-600 dark:group-hover:text-gray-700"
                            fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                        </svg>
                    </div>
                    <div class="mx-4 flex-row w-full">
                        <div class="flex flex-row items-center justify-between">
                            <h1 class="text-lg sm:text-xl font-bold text-gray-800 dark:text-gray-200">
                                Error
                            </h1>
                            <svg xmlns="http://www.w3.org/2000/svg"  @click="Buutton"
                                class="h-4 w-4 cursor-pointer text-gray-500 hover:text-gray-600 dark:text-gray-300 dark:hover:text-gray-200"
                                viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                                    clip-rule="evenodd" />
                            </svg>
                        </div>
                        <p class="text-xs sm:text-sm font-medium text-gray-500 pr-2 sm:pr-0 dark:text-gray-300">
                            Text Desc
                        </p>
                    </div>
                </div>
                <div v-if="myString === 'Info'"
                    class="flex flex-row items-center rounded shadow-lg overflow-hidden w-full sm:w-11/12 md:max-w-2xl hover:shadow-xl bg-white hover:bg-blue-50 dark:bg-gray-800 dark:hover:bg-gray-800 transition-transform hover:scale-95 group">
                    <div
                        class="h-full py-8 px-2 bg-blue-300 group-hover:bg-blue-400 dark:bg-gray-100 dark:group-hover:bg-gray-200">
                        <svg xmlns="http://www.w3.org/2000/svg"
                            class="h-8 w-8 text-blue-700 group-hover:text-blue-800 dark:text-gray-600 dark:group-hover:text-gray-700"
                            fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                        </svg>
                    </div>
                    <div class="mx-4 flex-row w-full">
                        <div class="flex flex-row items-center justify-between">
                            <h1 class="text-lg sm:text-xl font-bold text-gray-800 dark:text-gray-200">
                                Info
                            </h1>
                            <svg xmlns="http://www.w3.org/2000/svg"  @click="Buutton"
                                class="h-4 w-4 cursor-pointer text-gray-500 hover:text-gray-600 dark:text-gray-300 dark:hover:text-gray-200"
                                viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                                    clip-rule="evenodd" />
                            </svg>
                        </div>
                        <p class="text-xs sm:text-sm font-medium text-gray-500 pr-2 sm:pr-0 dark:text-gray-300">
                            Text Desc
                        </p>
                    </div>
                </div>
                <div class="button m-auto flex flex-row gap-6" v-if="myString === 'Button'">
  
                    <button @click="Warning" ><div
                        class="border-2 border-yellow-600 rounded-lg px-3 py-2 text-yellow-400 cursor-pointer hover:bg-yellow-600 hover:text-yellow-200">
                         Danger Toast
                    </div></button>
                    <button @click="Info" ><div
                        class="border-2 border-blue-600 rounded-lg px-3 py-2 text-blue-400 cursor-pointer hover:bg-blue-600 hover:text-blue-200">
                        Info Toast
                    </div></button>  
                    <button @click="Succses" > <div
                        class="border-2 border-green-600 rounded-lg px-3 py-2 text-green-400 cursor-pointer hover:bg-green-600 hover:text-green-200">
                        Succses Toast
                    </div></button>
                    <button @click="Error" ><div
                        class="border-2 border-red-600 rounded-lg px-3 py-2 text-red-400 cursor-pointer hover:bg-red-600 hover:text-red-200">
                        Error Toast
                    </div></button>


                </div>
            </div>
        </div>
    </div>


    <router-view class="p-24"></router-view>
</template>

<script>
export default {
  data() {
    return {
      myString: "Button"
      
    };
  },
  methods: {
    Succses() {
      this.myString = "Succses";
    },
    Error() {
      this.myString = "Error";
    },
    Warning() {
      this.myString = "Warning";
    },
    Info() {
      this.myString = "Info";
    },
    Buutton() {
      this.myString = "Button";
    },

  }
};

</script>

<style lang="scss">
#app {
    @apply h-screen bg-gray-50;
}

nav {
    a.active {
        &::after {
            @apply block w-full bg-green-500;
            content: '';
            height: 1.5px;
        }
    }
}
</style>
