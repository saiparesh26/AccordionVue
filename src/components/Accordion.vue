<template>
    <article class="message">
        <div class="message-header">
            <div class="level">
                <div class="level-left">
                    <div class="level-item">
                        <p class="subtitle is-6 has-text-white">BillingDocumentLine</p>
                    </div>
                </div>
                <div class="level-right" style="margin-left: 150px">
                    <div class="level-item">
                        <a @click="onShow"> <i id = "mainIcon" class="fas fa-plus"></i> </a>
                    </div>
                </div>
            </div>
            
        </div>
        <div class="message-body" v-if="open">
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
                        <p>Pipelines Direct linked</p>
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
            <div class="level">
                <div class="level-left">
                    <div class="level-item">
                        <p>Attributes(5)</p>
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
            open: true
        }
    },
    methods: {
        onShow: function(){
            this.open = !this.open;
            let mainIcon = document.getElementById('mainIcon');
            if(!this.open){
                mainIcon.classList.remove('fa-mius');
                mainIcon.classList.add('fa-plus');
            }
            if(this.open){
                mainIcon.classList.add('fa-minus');
                mainIcon.classList.remove('fa-plus');
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