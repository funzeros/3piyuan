<template>
    <div class="bg">
        <img :src="showBg.src" :alt="showBg.alt">
    </div>
</template>
<script>
import bg1 from '@/assets/bg/BG1.jpg';

export default {
    name:"bg",
    data() {
        return {
            img:[
                {id:"3001",src:bg1,alt:"背景1-沙滩"},
                {id:"3002",src:"",alt:""}
            ],
            bgNum:0,
        }
    },
    computed: {
        showBg(){
            return this.img[this.bgNum];
        }
    },
}
</script>
<style scoped>
    .bg{

    }
</style>