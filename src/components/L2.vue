<template>
    <article class="message">
        <div class="message-header">
            <div class="level">
                <div class="level-left">
                    <div class="level-item">
                        <p class="subtitle is-6 has-text-white">Downstream Objects L2</p>
                    </div>
                </div>
                <div class="level-right" style="margin-left: 125px">
                    <div class="level-item">
                        <a @click="onShowL2"> <i id = "mainIconL2" class="fas fa-plus"></i> </a>
                    </div>
                </div>
            </div>
            
        </div>
        <div class="message-body" v-if="openL2">
             <div class="level">
                <div class="level-left">
                    <div class="level-item">
                        <p>File Type Generated</p>
                    </div>
                </div>
                <div class="level-right" >
                    <div class="level-item">
                        <a> <i class="fas fa-plus"></i> </a>
                    </div>
                </div>
            </div>
            
            <div class="level">
                <div class="level-left">
                    <div class="level-item">
                        <p>Notebook</p>
                    </div>
                </div>
                <div class="level-right" >
                    <div class="level-item">
                        <a> <i class="fas fa-plus"></i> </a>
                    </div>
                </div>
            </div>
            
        </div>
</article>
</template>

<script>
import 'bulma/css/bulma.css'
export default {
    data: function(){
        return {
            openL2: false
        }
    },
    methods: {
        onShowL2: function(){
            this.openL2 = !this.openL2;
            let mainIconL2 = document.getElementById('mainIconL2');
            if(!this.openL2){
                mainIconL2.classList.remove('fa-mius');
                mainIconL2.classList.add('fa-plus');
            }
            if(this.openL2){
                mainIconL2.classList.add('fa-minus');
                mainIconL2.classList.remove('fa-plus');
            }
        }
    }
}
</script>

<style scoped>
    .message{
        width: 350px;
    }
</style>