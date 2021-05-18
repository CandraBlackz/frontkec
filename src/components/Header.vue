<template>
    <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark" style="border-top: 2px solid rgb(54, 60, 228);">
        <div class="container-fluid">
            <router-link :to="{name: 'home'}" class="navbar-brand"> KECAMATAN LOLAYAN
            </router-link>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarCollapse"
                aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarCollapse">
                <ul class="navbar-nav mr-auto mb-2 mb-md-0">
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            INFORMASI
                        </a>
                        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <router-link :to="{name: 'post'}" class="dropdown-item"><img src="assets/images/svg/newspaper.svg" class="rounded" style="width: 20px"> Berita</router-link>
                        <router-link :to="{name: 'event'}" class="dropdown-item"><img src="assets/images/svg/calendar.svg" class="rounded" style="width: 20px"> Agenda</router-link>
                        </div>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            GALERI
                        </a>
                        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <router-link :to="{name: 'photo'}" class="dropdown-item"><img src="assets/images/svg/photo.svg" class="rounded" style="width: 20px"> Foto</router-link>
                        <router-link :to="{name: 'video'}" class="dropdown-item"><img src="assets/images/svg/video-camera.svg" class="rounded" style="width: 20px"> Video</router-link>
                        </div>
                    </li>
                    <li class="nav-item">
                        <router-link :to="{name: 'contact'}" class="nav-link"> KONTAK</router-link>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'Header'
    }
</script>