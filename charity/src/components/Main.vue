<template>
    <main>
        <FirstSection/>
    </main>
</template>

<script>
import FirstSection from '@/components/First_section.vue'
export default {
    name: 'Main',
    components: {
        FirstSection
    }
}
</script>

<style lang="scss" scoped>
    main{
        
        height: 500vh;
        
    }
</style>