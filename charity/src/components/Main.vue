<template>
    <main>
        <FirstSection/>
        <Jumbotron :listItems= "listItems" />
        <Gallery/>
        <Articles/>
        <SecondJumbotron/>
    </main>
</template>

<script>
import FirstSection from '@/components/First_section.vue'
import Jumbotron from '@/components/Jumbotron.vue'
import Gallery from '@/components/Gallery.vue'
import Articles from '@/components/Articles.vue'
import SecondJumbotron from '@/components/Second_jumbotron.vue'
export default {
    name: 'Main',
    components: {
        FirstSection,
        Jumbotron,
        Gallery,
        Articles,
        SecondJumbotron
    },
    data(){
        return{
            listItems: [
          {
            icon: '<i class="fas fa-tint"></i>',
            message: 'Clean Water'
          },
          {
            icon: '<i class="fas fa-stethoscope"></i>',
            message: 'Vaccinations'
          },
          {
            icon: '<i class="fas fa-graduation-cap"></i>',
            message: 'Education'
          },
          {
            icon: '<i class="fab fa-pagelines"></i>',
            message: 'Farming'
          }

        ]
        }
    }
}
</script>

<style lang="scss" scoped>
    main{
        
        
    }
</style>