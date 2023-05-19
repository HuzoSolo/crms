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
                    <!-- charts -->
                    <li>
                        <div class="btn customside btnbox">
                            <i class="fa-solid fa-graduation-cap btnico pt-2"></i>
                            <!-- <span>Dersler</span> -->
                        </div>
                    </li>
                    <!-- profile -->
                    <li>
                        <div class="btn customside btnbox">
                            <i class="fa-solid fa-user btnico pt-2"></i>
                            <!-- <span>kullanıcı</span> -->
                        </div>
                    </li>

                    <!-- applications -->
                    <li>
                        <div class="btn customside btnbox">
                            <i class="fa-solid fa-puzzle-piece btnico pt-2"></i>
                            <!-- <span>yoklama</span> -->
                        </div>
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

<style lang="scss" scoped>


</style>