<script setup>
    const bgNav = 'bg-white'
    const color = 'text-black'
</script>

<template>
    <nav class="navbar navbar-expand-lg navbar-light fixed-top" :class="bgNav">
        <div class="container">
            <a class="navbar-brand" :class="color" style="font-size: 24px; font-weight: 700;" href="#">Sajid.</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse my-2" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item m-2">
                        <a class="nav-link active" aria-current="page" href="#hero">Home</a>
                    </li>
                    <li class="nav-item dropdown m-2">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            Dropdown
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li><a class="dropdown-item" href="#">Action</a></li>
                            <li><a class="dropdown-item" href="#">Another action</a></li>
                            <li><hr class="dropdown-divider"></li>
                            <li><a class="dropdown-item" href="#">Something else here</a></li>
                        </ul>
                    </li>
                    <li class="nav-item m-2">
                        <a class="nav-link" aria-current="page" href="#features">Features</a>
                    </li>
                    <li class="nav-item m-2">
                        <a class="nav-link" aria-current="page" href="#pricing">Pricing</a>
                    </li>
                    <li class="nav-item m-2">
                        <a class="nav-link" aria-current="page" href="#feedback">Testimonial</a>
                    </li>
                    <li class="nav-item m-2">
                        <a class="nav-link" aria-current="page" href="#about">About</a>
                    </li>
                    <li class="nav-item m-2">
                        <a class="nav-link" aria-current="page" href="#contact">Contact</a>
                    </li>
                </ul>
                <form class="d-flex">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <!-- <a class="nav-link active" aria-current="page" href="#">Sign In</a> -->
                            <button class="btn btn-ligh">Sign In</button>
                        </li>
                        <li class="nav-item">
                            <!-- <a class="nav-link active" aria-current="page" href="#">Register</a> -->
                            <button class="btn btn-primary">Register</button>
                        </li>
                    </ul>
                </form>
            </div>
        </div>
    </nav>
</template>