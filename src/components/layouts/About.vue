<template>
    <div>
        <div class="max-lg:mx-[50px]">
            <div class="flex flex-row max-lg:flex-col">
                <div v-motion-slide-visible-top class="basis-1/2 max-lg:w-full transition duration-700">
                    <img class="max-lg:mx-auto " src="../../assets/aboutus.png" alt="">
                </div>
                <div v-motion-slide-visible-bottom
                     class="basis-1/2  max-lg:grid max-lg:justify-items-center max-lg:mx-[50px] transition duration-700">
                    <div class="flex flex-col mt-72 max-xl:mt-64 max-lg:mt-0">
                        <div
                            class="flex flex-col text-5xl tracking-[-1%] space-y-2 text-[#331B3B] max-xl:text-4xl max-lg:text-3xl max-lg:grid max-lg:justify-items-center">
                            <p class="font-bold">{{ $t('about.first') }} </p>
                            <p class="relative font-light">{{ $t('about.second') }} <span
                                class="z-10 line__style__about relative ">{{ $t('about.third') }} </span></p>
                        </div>
                        <div
                            class="flex flex-col font-normal text-lg mt-5 mr-[59px] text-[rgba(51,27,59,0.66)] max-xl:text-base max-lg:mx-0  max-lg:grid max-lg:justify-items-center">
                            <p class="max-lg:w-[80%] max-lg:mx-0  max-sm:w-[120%]">Lorem Ipsum has been the industry's
                                standard dummy text
                                ever since the 1500s, when an unknown printer took a galley
                                of type and scrambled it to make a type specimen book.</p>
                            <p class="mt-2.5 max-lg:w-[80%] max-lg:mx-0 max-sm:w-[120%]">Lorem Ipsum has been the
                                industry's standard dummy text
                                ever since the 1500s, when an unknown printer took a galley
                                of type and scrambled it to make a type specimen book.</p>
                        </div>
                        <div class="max-lg:grid max-lg:justify-items-center">
                            <div
                                class="flex w-52 h-16 bg-[#331B3B] rounded-xl justify-center mt-9 cursor-pointer max-xl:w-48 max-xl:h-14 max-md:w-40 max-md:h-12 max-sm:w-32 max-sm:h-10">
                                <p class="flex self-center font-bold text-base text-white max-xl:text-sm max-sm:font-semibold uppercase">
                                    {{ $t('buttons.explore') }} </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "About"
}
</script>

<style scoped>
.line__style__about::before {
    content: '';
    position: absolute;
    height: 15%;
    width: 100%;
    background: #FDC221;
    bottom: 12%;
    z-index: -10;
}
</style>