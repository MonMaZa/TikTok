<template>
    <div
        id="SideNavMain"
        :class="route.fullPath === '/' ? 'lg:w-[310px]' : 'lg:w-[220px]'"
        class="fixed z-20 bg-white pt-[70px] h-full lg:border-r-0 border-r w-[75px] overflow-auto"
    >
        <div class="lg:w-full w-[55px] mx-auto">
            <nuxt-link to="/">
                <MenuItem iconString="For You" colorString="#f02c56" sizeString="30" />
            </nuxt-link>
            <MenuItem iconString="Following" colorString="#000" sizeString="27" />
            <MenuItem iconString="LIVE" colorString="#000" sizeString="27" />

        </div>
    </div>
</template>

<script setup>
    const route = useRoute()
</script>