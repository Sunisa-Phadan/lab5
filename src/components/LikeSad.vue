<script setup>
    import { ref } from 'vue';
const like = ref(0);
const sad = ref(0);

function likeClick(){
  like.value++;
}

function sadClick(){
  sad.value++;
} 
</script>

<template>
    <div class="container">
      <div class="row g-3 ">
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card" style="width: 20rem;">
            <img class="card-img-top" src="https://pbs.twimg.com/media/EryyxEkVcAAjxqm.jpg" alt="Card image cap">
            <div class="card-body">
              <h5 class="card-title">ดอกกุหลาบสีน้ำเงิน</h5>
              <p class="card-text">หมายถึง "รักที่เป็นไปได้ ดอกไม้แห่งความสมหวัง ดอกไม้แห่งความสุข" และความในใจอันหนักแน่นว่า "อดทนต่อความรัก และรอคอยอย่างมั่นคง"</p>
                <div class="btn-group">
                    <button @click="likeClick">Like</button>&nbsp;
                    {{ like }} &nbsp;
                    <button @click="sadClick">Sad</button>
                    &nbsp;  {{ sad }} &emsp;  &#160;
                      <div><small class="text-muted"> 9 mins </small>&nbsp; &nbsp;&#160;
                      <i class="bi bi-hand-thumbs-up"></i> &nbsp; &#160;
                      <i class="bi bi-heartbreak-fill"></i>
                      </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
        
</template>
