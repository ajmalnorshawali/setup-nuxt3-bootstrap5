# TUTORIAL 3: NUXT VIEWS

# STEP 1
- Create **app/components/AppHeader.vue**
- Copy and paste the following code
```
<template>
<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
        <NuxtLink class="navbar-brand" href="#">Navbar</NuxtLink>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item">
                    <NuxtLink to="/" class="nav-link">Home</NuxtLink>
                </li>
            </ul>
        </div>
    </div>
</nav>
</template>
```

# STEP 2
- Create **app/components/AppFooter.vue**
- Copy and paste the following code
```
<template>
<div class="bg-dark py-3">
    <p class="text-center text-white mb-0">Design by <b>AJMAL NS</b></p>
</div>
</template>
```

## STEP 3
- Create **app/layouts/default.vue**
- Copy and paste the following code
```
<script setup lang="ts"></script>

<template>
<AppHeader />
    <slot />
<AppFooter />
</template>
```

## STEP 4
- Create **app/pages/index.vue**
- Copy and paste the following code
```
<template>
<h1 class="text-center">HOME PAGE</h1>
</template>
```

## STEP 5
- Open file **_app.vue_**
- Copy and paste the following code
```
<script setup lang="ts"></script>

<template>
<NuxtLayout>
    <NuxtPage />
</NuxtLayout>
</template>
```

## STEP 6
- Save and run
```
npm run dev
```

#
[<< Prev](https://code.cloud-connect.asia/ajmalnorshawali/setup-nuxt3-bootstrap5/-/blob/main/Tutorial%202:%20Install%20Bootstrap%205.md)
