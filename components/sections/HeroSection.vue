<script setup>
import { ref } from 'vue'
const navIsOpen = ref(false)
const navItems = [
    {
        id: 1,
        text: "Portfolio",
        href: "/",
    },
    {
        id: 2,
        text: "Products",
        href: "#",
    },
    {
        id: 3,
        text: "Services",
        href: "#",
    },
    {
        id: 4,
        text: "Company",
        href: "#",
    }
]
 
function toggleNavbar() {
    navIsOpen.value = !navIsOpen.value
    document.body.classList.toggle("overflow-y-auto")
}
</script>
<template>
    <section bg="gray-1 dark:gray-9" py="32 sm:36 lg:40"
        class="overflow-hidden h-100dvh min-h-max flex items-center relative">
        <div class="absolute top-0 left-0 -translate-x-54% -translate-y-70% w-2/5 rd-full aspect-square bg-emerald-6/70
            backdrop-filter blur-3xl op-50"></div>
        <div class="absolute bottom-0 right-0 translate-x-54% translate-y-70% w-2/5 rd-full aspect-square bg-emerald-6/70
            backdrop-filter blur-3xl op-50"></div>
        <div class="absolute min-w-300px w-48% md-w-2/5 aspect-square rd-full bg-gradient-to-r from-emerald-4/5 right-0
            -translate-y-40% translate-x-40% top-0">
            <div class="inset-10% rd-full bg-gradient-to-l from-emerald-4/20">
                <div class="absolute inset-20% rd-full bg-gradient-to-l from-emerald-400/30"></div>
            </div>
        </div>
        <div class="absolute min-w-300px w-48% md:w-2/5 aspect-square rd-full bg-gradient-to-l from-emerald-4/5 left-0
            translate-y-40% -translate-x-40% bottom-0">
            <div class="inset-10% rd-full bg-gradient-to-r from-emerald-4/40">
                <div class="absolute inset-20% rd-full bg-gradient-to-r from-emerald-4/50"></div>
            </div>
        </div>
        <div px="5 sm:10 md:12 lg:5" class="mx-auto lg-max-w-7xl w-full">
            <div class="text-center flex flex-col items-center space-y-10">
                <span text="gray-7 dark:gray-3"
                    class="border border-gray-5 px3 py0.5 rd-full bg-gray-50 dark:bg-gray-950 bg-op-50">
                    Creativity in mind
                </span>
                <h1 text="4xl md:5xl lg:6xl/tight xl:7xl/tight gray-9 dark:white" class="font-bold max-w-4xl capitalize">
                    We inspire Growth for your business brand
                </h1>
                <p text="base gray-7 dark:gray-3 center" class="max-w-xl">
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Similique deleniti earum, qui odio,
                    dolorum labore incidunt ad ab porro, provident excepturi molestiae corporis molestias nam accusamus.
                </p>
                <div class="flex justify-center">
                    <a href="#" class="px8 h12 rd-full flex items-center gap-x-3 bg-emerald-7 text-white hover-bg-op-80">
                        Let's talk
                        <span i-carbon-arrow-right flex text-xl></span>
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>