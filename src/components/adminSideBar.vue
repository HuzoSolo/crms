<template>
    <div class="sideBar">
        <div class="logo">
                <a href="#" class="logobox ">

                    <img src="/src/assets/img/crms-transparent-logo.png" alt="" class="logo">

                </a>
            </div>

            <!-- tabs -->
            <div class="tabs">
                <ul class="menu">

                    <!-- courses -->
                    <li>
                        <a href="#courses" class="btn customside btnbox">
                            <i class="fa-solid fa-graduation-cap btnico pt-2"></i>
                            <!-- <span>Dersler</span> -->
                        </a>
                    </li>
                    <!-- teachers -->
                    <li>
                        <a href="#teachers" class="btn customside btnbox">
                            <i class="fa-solid fa-chalkboard-user btnico pt-2"></i>
                            <!-- <span>eğitmenler</span> -->
                        </a>
                    </li>

                    <!-- students -->
                    <li>
                        <a href="#students" class="btn customside btnbox">
                            <i class="fa-sharp fa-solid fa-user-graduate btnico pt-2"></i>
                            <!-- <span>öğrenciler</span> -->
                        </a>
                    </li>


                    <!-- payments -->
                    <li>
                        <a href="#payments" class="btn customside btnbox">
                            <i class="fa-solid fa-money-check-dollar btnico pt-2"></i>
                            <!-- <span>yoklama</span> -->
                        </a>
                    </li>

                    <!-- settings -->
                    <li>
                        <div class="btn customside btnbox">
                            <i class="fa-solid fa-gear btnico pt-2"></i>
                            <!-- <span>ayarlar</span> -->
                        </div>
                    </li>

                </ul>
            </div>
            <!-- close button -->
            <div class="clsbtn">
                <ul class="">
                    <li>
                        <div class="closebtn btn-group dropup">
                            <a href="">
                                <button class="btn customside" type="button" data-bs-toggle="dropdown"
                                    aria-expanded="false">
                                    <i class="fa-solid fa-power-off btnico pt-2"></i>
                                </button>
                                <ul class="dropdown-menu text-center">
                                    <li class="opt">Profile</li>
                                    <hr>
                                    <li class="opt">Settings</li>
                                    <hr>
                                    <li class="opt">Log out</li>
                                </ul>
                            </a>
                        </div>
                    </li>
                </ul>

            </div>
    </div>
</template>

<script>
export default {
}
</script>

<style>


</style>