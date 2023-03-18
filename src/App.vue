<script >
export default {
    data() {
        return {
            toggleBtn: true,
        }
    },
    methods: {
        toggleMenu(event) {
            this.toggleBtn = !this.toggleBtn;
        }
    },
    mounted() {
    },
}
</script>

<template>
    <!-- Header -->
    <header>
        <!-- container -->
        <div class="container mx-auto px-4">
            <nav class="flex justify-between items-center py-5">
                <div class="w-32 md:w-full z-20">
                    <img src="./assets/img/logo.png" alt="">
                </div>
                <ul class="z-20 text-xl fixed top-0 left-0 w-full h-screen flex flex-col justify-center items-center bg-gray-900 bg-opacity-90
                        md:bg-transparent md:h-auto md:flex-row md:justify-between md:static md:visible"
                    :class="{ invisible: toggleBtn }">
                    <li class="m-12 md:m-0">
                        <a class="text-white md:text-black hover:text-orange-500 trasition duration-300" href="#">Home</a>
                    </li>
                    <li class="m-12 md:m-0">
                        <a class="text-white md:text-black hover:text-orange-500 trasition duration-300"
                            href="#">Product</a>
                    </li>
                    <li class="m-12 md:m-0">
                        <a class="text-white md:text-black hover:text-orange-500 trasition duration-300" href="#">FAQ</a>
                    </li>
                    <li class="m-12 md:m-0">
                        <a class="text-white md:text-black hover:text-orange-500 trasition duration-300"
                            href="#">Contact</a>
                    </li>
                </ul>
                <!-- Menu button -->
                <div @click="toggleMenu" class="z-20 cursor-pointer md:hidden" :class="{ textwhite: !toggleBtn }">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-8 h-8 inline-block">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                    </svg>
                </div>
            </nav>
        </div>
    </header>

    <!-- Banner -->
    <section>
        <div class="banner
                w-full bg-no-repeat bg-cover relative h-620">
            <div class="absolute top-1/2 left-1/2 tranform -translate-x-1/2 -translate-y-1/2 z-10 text-white text-center">
                <!-- tag -->
                <p class="text-xl mb-5">Food app</p>
                <!-- title -->
                <h1 class="text-4xl mb-5 font-bold max-w-2xl md:leading-relaxed md:text-5xl">Why stay hungry when
                    you can order form Bella Onojie
                </h1>
                <!-- desc  -->
                <p class="text-xl mb-5 font-light">Download the bella onoje’s food app now on</p>
                <div class="flex justify-center">
                    <button
                        class="mx-4 border border-transparent bg-red-500 px-10 py-3 rounded-full hover:bg-transparent hover:border-white transition-all duration-300 ease-in">Playstore</button>
                    <button
                        class="mx-4 border border-white bg-transparent px-10 py-3 rounded-full hover:bg-red-500 hover:border-transparent  transition-all duration-300 ease-in">Appstore</button>
                </div>
            </div>
        </div>
    </section>

    <!-- App Image -->
    <section class="relative">
        <div class="absolute top-1/2 left-1/2 tranform -translate-x-2/3 -translate-y-1/4">
            <img class="max-w-none w-screen pl-20 md:w-auto " src="./assets/img/app-img.png" alt="phone app screen">
        </div>
    </section>

    <!-- App step -->
    <section class="pt-96 mt-28 sm:pt-40-c md:mt-0">
        <div class="container mx-auto px-4">
            <hr class="w-4/5 mx-auto h-0.5 bg-gray-200 md:w-2/5">
            <!-- title -->
            <h2 class="text-center text-4xl font-semibold py-10">How the app works</h2>

            <!-- step 1 -->
            <div class="flex flex-col justify-evenly py-10 md:flex-row ">
                <!-- img -->

                <img class="text-center mb-10" src="./assets/img/app-1.png" alt="app screen">

                <!-- text -->
                <div class="text-center md:text-left md:my-auto">
                    <!-- tag -->
                    <span class="text-red-500 font-semibold">
                        Create an account
                    </span>
                    <!--title  -->
                    <h2 class="text-4xl text-blue-900 font-bold max-w-md leading-relaxed py-5 ">Create/login to an existing
                        account to get started</h2>
                    <p class="text-xl text-gray-500 font-light max-w-sm mx-auto md:mx-0">An account is created with your
                        email
                        and a desired password</p>
                </div>
            </div>

            <!-- step 2 -->
            <div class="flex flex-col justify-evenly py-10 md:flex-row">
                <!-- img -->

                <img class="text-center mb-10 order-1 md:order-2" src="./assets/img/app-2.png" alt="app screen">

                <!-- text -->
                <div class="text-center md:text-left md:my-auto order-2 md:order-1">
                    <!-- tag -->
                    <span class="text-red-500 font-semibold">
                        Explore varieties
                    </span>
                    <!--title  -->
                    <h2 class="text-4xl text-blue-900 font-bold max-w-md leading-relaxed py-5 ">Shop for your favorites
                        meal as e dey hot.
                    </h2>
                    <p class="text-xl text-gray-500 font-light max-w-sm mx-auto md:mx-0">
                        An account is created with your email
                        and a desired password
                    </p>
                </div>
            </div>

            <!-- step 3 -->
            <div class="flex flex-col justify-evenly py-10 md:flex-row">
                <!-- img -->

                <img class="text-center mb-10" src="./assets/img/app-3.png" alt="app screen">

                <!-- text -->
                <div class="text-center md:text-left md:my-auto">
                    <!-- tag -->
                    <span class="text-red-500 font-semibold">
                        Checkout
                    </span>
                    <!--title  -->
                    <h2 class="text-4xl text-blue-900 font-bold max-w-md leading-relaxed py-5 ">When you done check out
                        and get it delivered.
                    </h2>
                    <p class="text-xl text-gray-500 font-light max-w-sm mx-auto md:mx-0">
                        When you done check out and get it
                        delivered with ease.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Download -->
    <section>
        <!-- background -->
        <div class="download relative w-full h-620 bg-no-repeat bg-cover">
            <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-center text-white z-10">
                <!-- title -->
                <h1 class="text-4xl mb-5 max-w-2xl md:leading-relaxed md:text-5xl">Download the app now</h1>
                <!-- desc -->
                <p class="text-xl mb-5">Available on your favorite store. Start your premium experience now</p>
                <!-- button -->
                <div class="flex justify-center">
                    <button
                        class="mx-4 border border-transparent bg-red-500 px-10 py-3 rounded-full hover:bg-transparent hover:border-white transition-all duration-300 ease-in">Playstore</button>
                    <button
                        class="mx-4 border border-white bg-transparent px-10 py-3 rounded-full hover:bg-red-500 hover:border-transparent  transition-all duration-300 ease-in">Appstore</button>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container mx-auto px-4 ">
            <div class="flex flex-col md:flex-row justify-center items-center py-5">
                <div class="w-32 md:w-full">
                    <img src="./assets/img/logo.png" alt="">
                </div>
                <div class="flex items-center mt-5 text-gray-500">
                    <!-- phone -->
                    <a href="#" class="flex mx-4">
                        <!-- icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="w-6 h-6 text-red-500 mr-4">
                            <path fill-rule="evenodd"
                                d="M2 3.5A1.5 1.5 0 013.5 2h1.148a1.5 1.5 0 011.465 1.175l.716 3.223a1.5 1.5 0 01-1.052 1.767l-.933.267c-.41.117-.643.555-.48.95a11.542 11.542 0 006.254 6.254c.395.163.833-.07.95-.48l.267-.933a1.5 1.5 0 011.767-1.052l3.223.716A1.5 1.5 0 0118 15.352V16.5a1.5 1.5 0 01-1.5 1.5H15c-1.149 0-2.263-.15-3.326-.43A13.022 13.022 0 012.43 8.326 13.019 13.019 0 012 5V3.5z"
                                clip-rule="evenodd" />
                        </svg>
                        <p>0912345678</p>
                    </a>
                    <!-- email -->
                    <a href="mailto:info@me.com" class="flex mx-4">
                        <!-- icon -->
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="w-6 h-6 text-red-500 mr-4">
                            <path d="M3 4a2 2 0 00-2 2v1.161l8.441 4.221a1.25 1.25 0 001.118 0L19 7.162V6a2 2 0 00-2-2H3z" />
                            <path
                                d="M19 8.839l-7.77 3.885a2.75 2.75 0 01-2.46 0L1 8.839V14a2 2 0 002 2h14a2 2 0 002-2V8.839z" />
                        </svg>
                        <!-- address -->
                        <p>info@me.com</p>
                    </a>
                </div>
            </div><!-- logo -->
            
            <!-- copy -->
            <div class="text-center text-sm text-gray-500 mb-4">
                <p>Copy &copy; 2023 Bella Onojie</p>
            </div>
        </div>

    </footer>
</template>

<style scoped>
.textwhite {
    color: white;
}

.download {
    background-image: url('./assets/img/download.png');
}

.banner {
    background-image: url('./assets/img/banner.png');
}</style>
