<script setup>

function onToggleMenu() {
    const name = document.getElementById('ion-icon').getAttribute('name')
    if(name  === 'menu'){
        document.getElementById('ion-icon').setAttribute('name', 'close')
    }else{
        document.getElementById('ion-icon').setAttribute('name', 'menu')
    }

    const nav = document.getElementById('nav-links')

nav.classList.toggle('!top-[9%]')


}



</script>


<template>
    <header class="">
        <nav
        id="nav"
        class="flex justify-around items-center w-[92%] mx-auto">
            <div class="">
                <img src="/Group.png" alt="">
            </div>
            <div 
            id="nav-links"
            class="md:static  absolute md:min-h-fit min-h-[30vh] md:bg-white bg-black -top-[100%] md:w-auto w-full flex md:flex-row flex-col items-center md:justify-around px-5 md:flex-1">
                <ul class="flex md:flex-row flex-col items-center md:items-center gap-[4vw] gap-8 pt-10 md:pt-0">
                    <li class=" font-extrabold uppercase md:text-black text-white"><a href="#">programmes & workshops</a></li>
                    <li class=" font-extrabold uppercase md:text-black text-white"><a href="#">how to get here</a></li>
                </ul>
                <div class="mt-[30px] md:mt-0 mx-auto md:mx-0 ">
                <button class="bg-red-600 px-5 py-2 flex text-white items-center font-extrabold uppercase">Register Now <img class="mx-2" src="/Vector%20(1).png" alt=""> </button>
            </div>
            </div>
            <div class="flex items-center md:hidden ">
                
                <ion-icon @click="onToggleMenu()"
                id="ion-icon"
                name="menu"></ion-icon>
            </div>

        </nav>
    </header>
</template>