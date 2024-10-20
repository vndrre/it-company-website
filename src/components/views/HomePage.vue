<script setup>
    import { Headset, Lightbulb, Goal } from 'lucide-vue-next';
    import Planning from '../Planning.vue';
import Expertice from '../Expertice.vue';
import Testimonials from '../Testimonials.vue';
import Footer from '../Footer.vue';
import Leaders from '../Leaders.vue';
import Contact from '../Contact.vue';
</script>

<template>
    <div class="grid place-items-center px-[100px] py-[50px] font-main">
        <div class="flex items-center gap-[100px]">
            <div class="grid grid-cols-1 gap-3">
                <p class="text-[#FF3E54] text-[24px] font-bold">\ We Are Here \</p>
                <h1 class="text-[48px] text-[#0E1F51] font-bold">
                    Better Insights For <br/>
                    Business Growth
                </h1>
                <a href="/" class="bg-[#FF3E54] hover:bg-[#f13a4f] duration-100 text-white rounded-md p-3 font-semibold ml-2 text-center mr-[250px]">
                    View More
                </a>
            </div>

            <div>
                <img src="/src/assets/landing-image.png" alt="">
            </div>
        </div>
    </div>

    <section class="bg-[#F7F7F7] px-[50px] py-[100px]">
        <div class="grid place-items-center">
            <div class="flex items-center gap-10">
                <div>
                    <img src="/src/assets/Mask group.png" alt="">
                </div>

                <div class="grid gap-5">
                    <div class="grid grid-cols-1">
                        <p class="text-[#FF3E54] text-[24px] font-bold">\ About us \</p>
                        <h1 class="text-[40px] font-bold text-[#0E1F51]">
                            One of the Fastest Way to <br/>
                            Business Growth
                        </h1>
                    </div>

                    <div>
                        <p class="text-[16px]">
                            It is a long established fact that a reader will be distracted by the <br>
                            readable content of a page when looking at its layout. The point of <br>
                            using Lorem Ipsum is that it has a more-or-less normal distribution <br>
                            of letters, as opposed
                        </p>
                    </div>

                    <div class="bg-white rounded-md p-2">
                        <div class="flex items-center gap-5">
                            <div class="bg-[#F7F7F7] rounded-md p-4">
                                <Headset class="text-[#FF3E54]"/>
                            </div>

                            <div class="grid grid-cols-1">
                                <h1 class="text-[#0E1F51] text-[20px] font-bold">Get Instant Professional Advice</h1>
                                <p class="text-[16px]">Ready to Help : <span class="text-[#FF3E54] font-bold">+1 356 678 7897</span> </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section>
        <Planning />
    </section>

    <section class="bg-[#F7F7F7] px-[50px] py-[100px]">
        <div class="grid place-items-center">
            <div class="flex items-center gap-10">
                <div>
                    <img src="/src/assets/Mask group2.png" alt="">
                </div>

                <div class="grid gap-5">
                    <div class="grid grid-cols-1">
                        <p class="text-[#FF3E54] text-[24px] font-bold">\ What We DO \</p>
                        <h1 class="text-[40px] font-bold text-[#0E1F51]">
                            We Develop Product That <br>
                            People Love to Use.
                        </h1>
                    </div>

                    <div>
                        <p class="text-[16px]">
                            It is a long established fact that a reader will be distracted by the <br>
                            readable content of a page when looking at its layout. The point of <br>
                            using Lorem Ipsum is that it has a more-or-less normal distribution <br>
                            of letters, as opposed
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-5">
                        <div class="bg-white rounded-md py-4 px-5">
                            <div class="flex items-center gap-5">
                                <div class="bg-[#FF3E54] bg-opacity-15 rounded-md p-4">
                                    <Lightbulb class="text-[#FF3E54]"/>
                                </div>

                                <div class="grid grid-cols-1">
                                    <h1 class="text-[#FF3E54] font-bold text-[16px]">Our Vision</h1>
                                    <p class="text-[#0E1F51] text-[14px] font-medium">
                                        It is a long esta <br>
                                        -blished fact that
                                    </p>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-md py-4 px-5">
                            <div class="flex items-center gap-5">
                                <div class="bg-[#FF3E54] bg-opacity-15 rounded-md p-4">
                                    <Goal class="text-[#FF3E54]"/>
                                </div>

                                <div class="grid grid-cols-1">
                                    <h1 class="text-[#FF3E54] font-bold text-[16px]">Our Goal</h1>
                                    <p class="text-[#0E1F51] text-[14px] font-medium">
                                        It is a long esta <br>
                                        -blished fact that
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="mt-3">
                        <a href="/" class="bg-[#FF3E54] hover:bg-[#f13a4f] duration-100 text-white rounded-md py-3 px-6">View More</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section>
        <Expertice />
    </section>

    <section>
        <!-- Our Leaders section -->
        <Leaders />
    </section>

    <section>
        <Testimonials />
    </section>

    <section>
        <!-- Blog section -->
    </section>

    <section>
        <!-- Get in touch section -->
    </section>

    <section>
        <Footer />
    </section>
</template>
