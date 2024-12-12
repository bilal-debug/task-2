<script setup>
import { ref } from "vue";

const name=ref("")
const email=ref("")
const mobilephone=ref("")
const options=ref("")
const options1=ref("")
const options2=ref("")
const education=ref("")
const click=ref("")
const click1=ref("")
const click2=ref("")
const click3=ref("")

const error=ref("")
const errorm=ref("")
const errorm1=ref("")
const errorm2=ref("")
const errorm3=ref("")
const errorm4=ref("")
const errorm5=ref("")
const errorm6=ref("")

function submission(e) {
    e.preventDefault()
   
    
    if (name.value==="") {
        
        
        error.value='please fill this field'
        
    }
    else{
        error.value=''
    }
    if (email.value==="") {
        
        
        errorm.value='please fill this field'
        
    }
    else{
        errorm.value=''
    }
    if (mobilephone.value==="") {
        
        
        errorm1.value='please fill this field'
        
    }
    else{
        errorm1.value=''
    }
    if (options.value==="") {
        
        
        errorm2.value='please fill this field'
        
    }
    else{
        errorm2.value=''
    }
    if (options1.value==="") {
        
        
        errorm3.value='please fill this field'
        
    }
    else{
        errorm3.value=''
    }
    if (education.value==="") {
        
        
        errorm4.value='please fill this field'
        
    }
    else{
        errorm4.value=''
    }
    if (options2.value==="") {
        
        
        errorm5.value='please fill this field'
        
    }
    else{
        errorm5.value=''
    }
    if (click.value==="" && click1.value==="" && click2.value==="" && click3.value==="") {
        
        
        errorm6.value='please fill this field'
        
    }
    else{
        errorm6.value=''
    }
   
    
}


</script>
<template>
    <div class="">
        <div class=" ">
            <h1 class=" uppercase text-red-600  text-6xl font-extrabold text-center mt-2 mb-[-13px] md:text-[200px] md:pt-[100px] md:ml-6">
                register
            </h1>
            <h2 class=" uppercase text-black  text-6xl font-extrabold text-center mx-[180px] md:text-[170px] md:text-end md:mt-[-40px] ">
                Now
            </h2>
        </div>
        <div class="mt-5 mx-9 md:text-e">
            <p class=" text-center  text-[12px] md:text-[22px] md:mx-auto md:w-[50%] md:text-end ">Register to join <span class="font-bold">SIT Open House 2025, 8th - 9th February 2025,</span> SIT Punggol Campus, 1 Punggol Coast Road.</p>
        </div>
        <div class=" md:bg-[url('/tickets.png')] bg-contain bg-end bg-no-repeat  "
        
        style="background-position: 0 100%" 
        >
            <form action="" class="mx-9 mt-9 md:mx-[350px] ">
                <h2 class="font-bold mb-3 md:text-[32px]">Enter your Details</h2>
                <div class="mb-4">
                    <label for="" class="font-bold text-[16px] "> Full Name*</label><br>
                    <input class="w-[70%]  outline outline-1 outline-gray-400 mt-2 md:outline-2 md:outline-black md:p-3 md:w-[100%] " id="name"  type="text" v-model="name">
                    <p v-if="error" style="color: red; font-size: large;">{{error }}</p>
                </div>
                <div class="mb-4">
                    <label for="" class="font-bold text-[16px] " > Email*</label><br>
                    <input class="w-[70%]  outline outline-1 outline-gray-400 mt-2 md:outline-2 md:outline-black md:p-3 md:w-[100%] " id="email"  type="email" v-model="email">
                    <p v-if="errorm" style="color: red; font-size: large;">{{errorm }}</p>
                </div>
                <div class="mb-4">
                    <label for="" class="font-bold text-[16px] "> Mobile Phone*</label><br>
                    <input class="w-[70%]  outline outline-1 outline-gray-400 mt-2 md:outline-2 md:outline-black md:p-3 md:w-[100%] " id="mobilephone"  type="tel" v-model="mobilephone">
                    <p v-if="errorm1" style="color: red; font-size: large;">{{errorm1 }}</p>
                </div>
                <div class="">
    <label for="options" class="font-bold text-[16px] ">Last Qualification Attained*
    </label>
    <select 
      id="options" 
      class="w-[70%] px-4 py-2 outline outline-1 outline-gray-400 mt-2 md:outline-2 md:outline-black md:p-3 md:w-[100%]" v-model="options">
      <option value="" disabled selected>Choose an option</option>
      <option value="option1">B.com</option>
      <option value="option2">M.com</option>
      <option value="option3">Phd</option>
    </select>
    <p v-if="errorm2" style="color: red; font-size: large;">{{errorm2 }}</p>
  </div>

  <div class="flex items-center mt-2 mb-3">
    <div class="">
    <label for="options" class="font-bold text-[16px] ">Current Institution*
    </label>
    <select 
      id="options1" 
      class="w-[80%] px-4 py-2 outline outline-1 outline-gray-400 md:outline-2 md:outline-black mt-2 md:p-3 md:w-[90%]" v-model="options1">
      <option value="" disabled selected>Choose an option</option>
      <option value="option11">UCP</option>
      <option value="option22">VUAS</option>
      <option value="option33">ITP</option>
    </select>
    <p v-if="errorm3" style="color: red; font-size: large;">{{errorm3 }}</p>
  </div>
  <div>
    <div class="mb-4">
                    <label for="" class="font-bold text-[16px] "> Year of Education*</label><br>
                    <input class="w-[70%]  outline outline-1 outline-gray-400 mt-2 md:outline-2 md:outline-black md:p-3 md:w-[100%] " id="education"  type="number" placeholder="YYYY" v-model="education">
                    <p v-if="errorm4" style="color: red; font-size: large;">{{errorm4 }}</p>
                </div>
  </div>
  </div>

  <div class="">
    <label for="options" class="font-bold text-[16px] ">Current Institution*
    </label>
    <select 
      id="options2" 
      class="w-[80%] px-4 py-2 outline outline-1 outline-gray-400 mt-2 md:outline-2 md:outline-black md:p-3 md:w-[100%]" v-model="options2">
      <option value="" disabled selected>Choose an option</option>
      <option value="option1">BSCS</option>
      <option value="option2">MCS</option>
      <option value="option3">PHD</option>
    </select>
    <p v-if="errorm5" style="color: red; font-size: large;">{{errorm5 }}</p>
  </div>
<div class="font-bold mt-9">
    <p>Which programme or workshop are you most interested in attending at the Open House? You may select more than one.
    </p>
</div>
<div class="mb-4 grid  mt-4 ">
                 
                    <label for=""><input  class="mx-1 items-center  " id="click"  type="checkbox" v-model="click">Business, Communication and Design</label>
                    <label for=""><input  class="mx-1 items-center  " id="click1"  type="checkbox" v-model="click1">Engineering</label>
                    <label for=""><input  class="mx-1 items-center  " id="click2"  type="checkbox" v-model="click2">Food, Chemical and Biotechnology</label>
                    <label for=""><input  class="mx-1 items-center  " id="click3"  type="checkbox" v-model="click3">Health and Social Sciences</label>
                    <p v-if="errorm6" style="color: red; font-size: large;">{{errorm6 }}</p>
                </div>
                <div class="bg-black px-5 pt-5 pb-5 ">
                    <h3 class="text-white font-bold">Personal Data Consent*</h3>
                    <div class="text-white flex">
                       

                        <div><label for=""><input  class="mx-1 items-center  " id="nae"  type="checkbox"></label></div>
                        <div>By clicking submit, you agree that SIT (and its service providers and agents) may collect, use, disclose and/or process your personal data:<br><br>

                            1. to send you information related to the topics of interest and the types of emails you have selected above, which may include information on degree programmes and upcoming courses, seminars, events, resources and/or surveys by SIT and/or its Overseas University partners;
 and for analysis.

 <br><br>2. We look forward to journeying with you on your path of lifelong learning. You can manage your preferences or unsubscribe at any time through the links provided in our communications. To learn more about how SIT protects your personal data, you may refer to SIT’s Personal Data Protection Policy here.</div>
                    </div>

                </div>
                <div class="flex justify-end">
                <button @click="(e)=>submission(e)" class="bg-red-600 flex items-center px-4 py-2 mt-7 ">
                    <div class="uppercase text-white">
                        submit
                    </div>
                    <div>
                        <img class="mx-2 w-2" src="C:\Users\ThinkPad-L440\Downloads\Vector (1).png" alt="">
                    </div>
                </button> </div>

  
            </form>
        </div>
    </div>
</template>


