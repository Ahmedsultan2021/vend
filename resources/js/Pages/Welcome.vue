<script setup>
import { Head, Link } from '@inertiajs/vue3';

defineProps({
    canLogin: {
        type: Boolean,
    },
    canRegister: {
        type: Boolean,
    },
    laravelVersion: {
        type: String,
        required: true,
    },
    phpVersion: {
        type: String,
        required: true,
    },
});


function pepsi() {
    fetch('https://testv-a9639-default-rtdb.europe-west1.firebasedatabase.app/test.json', {
        method: 'PATCH',
        body: JSON.stringify({ pepsi: 1 }),
        headers: {
            'Content-Type': 'application/json'
        }
    })
}
function cola() {
    fetch('https://testv-a9639-default-rtdb.europe-west1.firebasedatabase.app/test.json', {
        method: 'PATCH',
        body: JSON.stringify({ cola: 1 }),
        headers: {
            'Content-Type': 'application/json'
        }
    })
}
function sup() {
    fetch('https://testv-a9639-default-rtdb.europe-west1.firebasedatabase.app/test.json', {
        method: 'PATCH',
        body: JSON.stringify({ "7up": 1 }),
        headers: {
            'Content-Type': 'application/json'
        }
    })
}


</script>

<template>

    <Head title="Welcome" />
    <header class="container mx-auto flex w-full items-center justify-between py-4 px-6">
        <a href="#">
            <div class="w-full text-center text-lg font-extrabold sm:w-fit sm:text-left">
                <span class="text-violet-500">Unique</span>
                <span class="dark:text-slate-400">Fund</span>
            </div>
        </a>
        <nav class="hidden bg-white text-base dark:bg-slate-900 sm:block">
            <ul class="flex items-center space-x-2">
                <li class="group relative">
                    <a class="block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                        href="/">
                        Home
                    </a>
                </li>
                <li class="group relative">
                    <a class="block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                        href="#">
                        Solutions
                    </a>
                    <ul
                        class="invisible absolute z-30 space-y-2 rounded-lg border border-slate-50 bg-white p-4 opacity-0 shadow-xl transition-opacity delay-75 ease-in-out group-hover:visible group-hover:opacity-100 dark:border-slate-800 dark:bg-slate-900">
                        <li>
                            <a class="undefined block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                                href="#">
                                Business Line of Credit
                            </a>
                        </li>
                        <li>
                            <a class="undefined block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                                href="#">
                                SBA Loan
                            </a>
                        </li>
                        <li>
                            <a class="undefined block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                                href="#">
                                Revenue Based Financing
                            </a>
                        </li>
                        <li>
                            <a class="undefined block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                                href="#">
                                Invoice Factoring
                            </a>
                        </li>
                    </ul>
                </li>
                <li class="group relative">
                    <a class="block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                        href="/about">
                        About
                    </a>
                </li>
                <li class="group relative">
                    <a class="block whitespace-nowrap px-2 py-2 text-sm text-slate-900 no-underline transition hover:text-slate-900 dark:text-slate-50 dark:hover:text-slate-50"
                        href="/contact">
                        Contact
                    </a>
                </li>
            </ul>
        </nav>
        <button class="block text-slate-400 hover:text-slate-900 dark:hover:text-slate-50 sm:hidden"
            title="Open navigation menu">
            <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em">
                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M4 6h16M4 12h16M4 18h16"></path>
            </svg>
        </button>
        <nav
            class="fixed -right-2/3 top-0 z-20 h-full w-2/3 transform overflow-y-auto bg-white py-4 text-base transition dark:bg-slate-900 sm:hidden">
            <ul class="flex flex-col space-y-2">
                <li class="text-right">
                    <button class="px-6 py-2 text-slate-400 hover:text-slate-900 dark:hover:text-slate-50">
                        <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em">
                            <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2" d="M5 12h14m-4 4l4-4m-4-4l4 4"></path>
                        </svg>
                    </button>
                </li>
                <li class="group relative w-full overflow-x-visible text-right">
                    <a class="mx-4 block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                        href="/">
                        Home
                    </a>
                </li>
                <li class="group relative w-full overflow-x-visible text-right">
                    <a class="mx-4 block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                        href="#">
                        Solutions
                    </a>
                    <ul
                        class="h-0 space-y-2 overflow-y-hidden bg-slate-50 px-4 py-0 transition-all delay-75 ease-in-out group-hover:h-full group-hover:py-4 dark:bg-slate-800">
                        <li>
                            <a class="undefined block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                                href="#">
                                Business Line of Credit
                            </a>
                        </li>
                        <li>
                            <a class="undefined block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                                href="#">
                                SBA Loan
                            </a>
                        </li>
                        <li>
                            <a class="undefined block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                                href="#">
                                Revenue Based Financing
                            </a>
                        </li>
                        <li>
                            <a class="undefined block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                                href="#">
                                Invoice Factoring
                            </a>
                        </li>
                    </ul>
                </li>
                <li class="group relative w-full overflow-x-visible text-right">
                    <a class="mx-4 block whitespace-nowrap px-2 py-2 text-sm text-slate-400 no-underline transition hover:text-slate-900 dark:hover:text-slate-50"
                        href="/about">
                        About
                    </a>
                </li>
                <li class="group relative w-full overflow-x-visible text-right">
                    <a class="mx-4 block whitespace-nowrap px-2 py-2 text-sm text-slate-900 no-underline transition hover:text-slate-900 dark:text-slate-50 dark:hover:text-slate-50"
                        href="/contact">
                        Contact
                    </a>
                </li>
            </ul>
        </nav>
    </header>
    <section
        class="grid grid-cols-1 lg:grid-cols-3 items-center justify-center gap-10 bg-slate-50 py-12 px-6 dark:bg-slate-900 md:grid-cols-2">
        <div @click="pepsi" 
            class="block cursor-pointer  rounded-lg bg-white text-surface shadow-secondary-1 dark:bg-surface-dark dark:text-white justify-center">
            <div class="relative overflow-hidden bg-cover bg-no-repeat">
                <img class="rounded-t-lg" src="images/pepsi.png" style="height: 300px;" alt="" />
            </div>
            <div class="p-6">
                <p class="text-base text-center">
                   pepsi
                </p>
            </div>
        </div>
        <div

        @click="cola"
        class="block cursor-pointer  rounded-lg bg-white text-surface shadow-secondary-1 dark:bg-surface-dark dark:text-white">
            <div class="relative overflow-hidden bg-cover bg-no-repeat">
                <img class="rounded-t-lg" src="images/cola.png" style="height: 300px" alt="" />
            </div>
            <div class="p-6">
                <p class="text-base text-center">
                   cola
                </p>
            </div>
        </div>
        <div

        @click="sup"
        
        class="block rounded-lg cursor-pointer bg-white text-surface shadow-secondary-1 dark:bg-surface-dark dark:text-white">
            <div class="relative overflow-hidden bg-cover bg-no-repeat">
                <img class="rounded-t-lg" src="images/7up.png" style="height: 300px" alt="" />
            </div>
            <div class="p-6">
                <p class="text-base text-center">
                   7up
                </p>
            </div>
        </div>
    </section>
    <section class="container mx-auto px-8 py-28 sm:px-12">
        <h1 class="sm:mb-18 mb-24 w-full text-center text-4xl font-bold dark:text-slate-50 sm:mx-auto sm:w-4/5">
            Your favorite cafe in town
        </h1>
        <div class="grid grid-cols-2 gap-4 md:grid-cols-3">
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2">
                        <path d="M12 18h.01m-2.838-2.828a4 4 0 0 1 5.656 0m-8.485-2.829a8 8 0 0 1 11.314 0"></path>
                        <path d="M3.515 9.515c4.686-4.687 12.284-4.687 17 0"></path>
                    </g>
                </svg>
                <div class="mt-3 text-sm font-semibold">Working space</div>
            </div>
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2">
                        <path d="M12 18h.01m-2.838-2.828a4 4 0 0 1 5.656 0m-8.485-2.829a8 8 0 0 1 11.314 0"></path>
                        <path d="M3.515 9.515c4.686-4.687 12.284-4.687 17 0"></path>
                    </g>
                </svg>
                <div class="mt-3 text-sm font-semibold">Affordable price</div>
            </div>
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2">
                        <path d="M12 18h.01m-2.838-2.828a4 4 0 0 1 5.656 0m-8.485-2.829a8 8 0 0 1 11.314 0"></path>
                        <path d="M3.515 9.515c4.686-4.687 12.284-4.687 17 0"></path>
                    </g>
                </svg>
                <div class="mt-3 text-sm font-semibold">High speed internet</div>
            </div>
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2"
                        d="M3 14a1 1 0 0 1 1-1h16a1 1 0 0 1 1 1v2a1 1 0 0 1-1 1H4a1 1 0 0 1-1-1zm5-1v4m8-12v.5a2 2 0 0 0 2 2a2 2 0 0 1 2 2v.5">
                    </path>
                </svg>
                <div class="mt-3 text-sm font-semibold">Smoking area</div>
            </div>
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2">
                        <path d="M20 6v12a2 2 0 0 1-2 2H8a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2zM10 16h6">
                        </path>
                        <path d="M11 11a2 2 0 1 0 4 0a2 2 0 1 0-4 0M4 8h3m-3 4h3m-3 4h3"></path>
                    </g>
                </svg>
                <div class="mt-3 text-sm font-semibold">Meeting room</div>
            </div>
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2">
                        <path d="M4 6a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2z"></path>
                        <path d="M9 16V8h4a2 2 0 0 1 0 4H9"></path>
                    </g>
                </svg>
                <div class="mt-3 text-sm font-semibold">Huge parking lot</div>
            </div>
        </div>
    </section>
    <section class="container mx-auto px-8 py-28 sm:px-12">
        <h1 class="sm:mb-18 mb-24 w-full text-center text-4xl font-extrabold dark:text-slate-50 sm:mx-auto sm:w-4/5">
            We provide
            <span class="text-violet-500">variety of choices</span>

            for any kind of situations
        </h1>
        <div class="grid grid-cols-2 gap-4 md:grid-cols-4">
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-white py-5 px-6 text-center text-slate-800 shadow-lg shadow-slate-200 transition dark:bg-slate-700 dark:text-slate-200 dark:shadow-slate-700">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2"
                        d="M3 8a3 3 0 0 1 3-3h12a3 3 0 0 1 3 3v8a3 3 0 0 1-3 3H6a3 3 0 0 1-3-3zm0 2h18M7 15h.01M11 15h2">
                    </path>
                </svg>
                <div class="mt-3 text-sm font-semibold">Business Line of Credit</div>
            </div>
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2" d="M3 21h18M3 10h18M5 6l7-3l7 3M4 10v11m16-11v11M8 14v3m4-3v3m4-3v3"></path>
                </svg>
                <div class="mt-3 text-sm font-semibold">SBA Loan</div>
            </div>
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2">
                        <path d="M9 5H7a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V7a2 2 0 0 0-2-2h-2"></path>
                        <path
                            d="M9 5a2 2 0 0 1 2-2h2a2 2 0 0 1 2 2v0a2 2 0 0 1-2 2h-2a2 2 0 0 1-2-2zm5 6h-2.5a1.5 1.5 0 0 0 0 3h1a1.5 1.5 0 0 1 0 3H10m2 0v1m0-8v1">
                        </path>
                    </g>
                </svg>
                <div class="mt-3 text-sm font-semibold">Revenue Based Financing</div>
            </div>
            <div
                class="flex cursor-pointer flex-col items-center justify-start rounded-lg bg-slate-50 py-5 px-6 text-center text-slate-800 shadow-slate-200 transition hover:bg-white hover:shadow-lg hover:shadow-slate-200 dark:bg-slate-800 dark:text-slate-200 dark:shadow-slate-700 dark:hover:shadow-slate-800">
                <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                    class="h-8 w-8">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2">
                        <path d="M14 3v4a1 1 0 0 0 1 1h4"></path>
                        <path d="M17 21H7a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h7l5 5v11a2 2 0 0 1-2 2zM9 7h1m-1 6h6m-2 4h2">
                        </path>
                    </g>
                </svg>
                <div class="mt-3 text-sm font-semibold">Invoice Factoring</div>
            </div>
        </div>
        <div class="mt-8 grid grid-cols-1 items-center gap-4 rounded-lg bg-violet-500 py-12 px-14 md:grid-cols-2">
            <div class="text-center md:text-left">
                <div class="text-4xl font-extrabold text-white">
                    Business Line
                    <br />
                    of Credit
                </div>
                <div class="mt-2 text-sm text-violet-100">
                    Pay interest only on what you use
                </div>
                <ul class="mt-6 mb-8 text-sm text-violet-100 md:mb-0">
                    <li class="flex items-center justify-center md:justify-start">
                        <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                            class="mr-3">
                            <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2" d="m5 12l5 5L20 7"></path>
                        </svg>
                        High credit limit
                    </li>
                    <li class="flex items-center justify-center md:justify-start">
                        <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                            class="mr-3">
                            <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2" d="m5 12l5 5L20 7"></path>
                        </svg>
                        Fast disbursement, anytime
                    </li>
                </ul>
            </div>
            <form class="flex flex-col md:ml-8">
                <input class="mb-4 rounded-md px-4 py-3 font-light" min="0" placeholder="How much do you need?"
                    type="number" />
                <button
                    class="flex items-center justify-center rounded-md bg-violet-900 px-4 py-3 font-semibold text-white shadow-md shadow-violet-700 transition hover:bg-slate-900"
                    type="submit">
                    <svg preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" width="1.2em" height="1.2em"
                        class="mr-2">
                        <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                            stroke-width="2" d="M3 10a7 7 0 1 0 14 0a7 7 0 1 0-14 0m18 11l-6-6"></path>
                    </svg>
                    Find the best limit
                </button>
            </form>
        </div>
    </section>
    <!-- <section class="container mx-auto px-12 py-28">
        <h1 class="mb-24 w-full text-center text-4xl font-extrabold dark:text-slate-50 md:mx-auto md:mb-24 md:w-4/5">
            Our
            <span class="text-violet-500">happy customers</span>
        </h1>
        <div class="flex flex-col space-y-6 md:flex-row md:space-y-0">
            <div
                class="flex w-full flex-col justify-between rounded-lg bg-white py-8 px-6 text-center text-slate-800 shadow-lg shadow-slate-200 transition dark:bg-slate-800 dark:shadow-slate-800">
                <div class="w-full text-center text-sm">
                    <img alt="Hanging out with friends" class="mx-auto mb-8 h-20 w-20" src="/images/avatar-1.png" />
                    <p class="mb-6 leading-relaxed text-slate-500 dark:text-slate-400">
                        They helped me to quickly and easily compare my options, and I was
                        able to secure the financing I needed to grow my business.
                    </p>
                    <div class="font-semibold text-slate-600">John Doe</div>
                    <div class="text-xs text-slate-400">Crispy Creamy Crepes</div>
                </div>
            </div>
            <div
                class="z-10 flex w-full flex-col justify-between rounded-lg bg-white py-8 px-6 text-center text-slate-800 shadow-lg shadow-slate-200 transition dark:bg-slate-800 dark:shadow-slate-800 md:scale-y-110 md:scale-x-110">
                <div class="w-full text-center text-sm">
                    <img alt="Hanging out with friends" class="mx-auto mb-8 h-20 w-20" src="/images/avatar-1.png" />
                    <p class="mb-6 leading-relaxed text-slate-500 dark:text-slate-400">
                        This team was knowledgeable and helpful, walking me through the
                        process and finding a financing solution that fit my business
                        perfectly.
                    </p>
                    <div class="font-semibold text-slate-600">Peter Smith</div>
                    <div class="text-xs text-slate-400">Chick Chicken</div>
                </div>
            </div>
            <div
                class="flex w-full flex-col justify-between rounded-lg bg-white py-8 px-6 text-center text-slate-800 shadow-lg shadow-slate-200 transition dark:bg-slate-800 dark:shadow-slate-800">
                <div class="w-full text-center text-sm">
                    <img alt="Hanging out with friends" class="mx-auto mb-8 h-20 w-20" src="/images/avatar-1.png" />
                    <p class="mb-6 leading-relaxed text-slate-500 dark:text-slate-400">
                        Thanks to their guidance, I was able to secure the financing I needed
                        to get my business off the ground.
                    </p>
                    <div class="font-semibold text-slate-600">Jane Brown</div>
                    <div class="text-xs text-slate-400">Pizzy Pizza</div>
                </div>
            </div>
        </div>
    </section> -->
    <footer class="mt-28 bg-slate-50 dark:bg-black">
        <div
            class="container mx-auto flex flex-col items-start space-y-12 px-8 pb-8 pt-12 md:flex-row md:space-y-0 md:space-x-12 md:px-12">
            <div class="flex w-full flex-col space-y-4 text-center md:w-2/5 md:text-left">
                <div class="w-full text-lg font-extrabold md:w-fit md:text-left">
                    <span class="text-violet-500">Unique</span>
                    <span class="dark:text-slate-400">Fund</span>
                </div>
                <p class="text-sm text-slate-600">
                    UniqueFund provides access to fast and reliable financing solutions for
                    SMEs.
                </p>
            </div>
            <div class="w-full text-center text-slate-600 md:w-1/5 md:text-left">
                <div class="text-sm font-semibold">Company</div>
                <ul class="text-sm">
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            About
                        </a>
                    </li>
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Terms of Service
                        </a>
                    </li>
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Privacy Policy
                        </a>
                    </li>
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Cookie Policy
                        </a>
                    </li>
                </ul>
            </div>
            <div class="w-full text-center text-slate-600 md:w-1/5 md:text-left">
                <div class="text-sm font-semibold">Solutions</div>
                <ul class="text-sm">
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Business Line of Credit
                        </a>
                    </li>
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            SBA Loan
                        </a>
                    </li>
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Revenue Based Financing
                        </a>
                    </li>
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Invoice Factoring
                        </a>
                    </li>
                </ul>
            </div>
            <div class="w-full text-center text-slate-600 md:w-1/5 md:text-left">
                <div class="text-sm font-semibold text-slate-600">Partnership</div>
                <ul class="text-sm">
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Loan Partner
                        </a>
                    </li>
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Affiliate
                        </a>
                    </li>
                    <li class="pt-3">
                        <a class="underline decoration-transparent underline-offset-4 transition hover:decoration-slate-700"
                            href="#" rel="noopener noreferrer" target="_blank">
                            Brand Guideline
                        </a>
                    </li>
                </ul>
            </div>
        </div>
        <div
            class="container mx-auto border-t border-slate-200 p-8 text-center text-sm text-slate-600 dark:border-slate-900 md:flex-row md:px-12">
            ©

            2023

            UniqueFund. All rights reserved.
        </div>
    </footer>
</template>

<style>
.bg-dots-darker {
    background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(0,0,0,0.07)'/%3E%3C/svg%3E");
}

@media (prefers-color-scheme: dark) {
    .dark\:bg-dots-lighter {
        background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(255,255,255,0.07)'/%3E%3C/svg%3E");
    }
}
</style>
