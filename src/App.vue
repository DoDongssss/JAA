<script lang="ts">
import { defineComponent } from 'vue'
import { RouterLink, RouterView } from 'vue-router'
import index from '../src/views/index.vue'
import about from '../src/views/about.vue'
import skills from '../src/views/skills.vue'
import project from '../src/views/project.vue'
import contact from '../src/views/contact.vue'
import foot from '../src/components/footer.vue'

export default defineComponent({
    components: {
      index,
      about,
      skills,
      project,
      contact,
      foot
      
    },
    setup () {
        return {}
    }
})
</script>

<template>
  <index/>
  <about/>
  <skills/>
  <project/>
  <contact/>
  <foot /> 

  <el-backtop :bottom="55">
    <div class="abs-center flex-col">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="h-[20px] fill-[#00ADB5]">
        <path d="M96 256H128V512H0V352H32V320H64V288H96V256zM512 352V512H384V256H416V288H448V320H480V352H512zM320 64H352V448H320V416H192V448H160V64H192V32H224V0H288V32H320V64zM288 128H224V192H288V128z"/>
      </svg>
      <!-- <span class="font-bold text-[7px] color-222831">TOP</span> -->
    </div>
  </el-backtop>
</template>

<style scoped>
  .el-backtop{
    display: flex;
    height: 50px!important;
    width: 50px!important;
    border: 3px solid #00ADB5;
  }
  .el-backtop svg{
    animation: racket-animation 1.5s linear infinite;
  }
  .el-backtop:hover svg{
    animation: racket-animation .5s ease-in infinite;
  }

  @keyframes racket-animation {
    0%,100%{
      transform: translateY(3px);
    }
    50%{
      transform: translateY(-3px);
    }
  }
</style>
