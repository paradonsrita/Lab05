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
    <div>
      <h3>title</h3>
      <div class="col">
          <div class="card shadow-sm">
            <svg class="bd-placeholder-img card-img-top" width="100%" height="225" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Placeholder: Thumbnail" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="#55595c"></rect><text x="50%" y="50%" fill="#eceeef" dy=".3em">Thumbnail</text></svg>
            <div class="card-body">
              <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
              <div class="d-flex justify-content-between align-items-center">
                <div class="btn-group">
                  <button @click="likeClick"><i class="bi bi-star-fill"></i></button>
                  like = {{ like }}
                  <button @click="sadClick"><i class="bi bi-emoji-frown-fill"></i></button>
                  
                    <p>. .</p>
                    
                  sad = {{ sad }}

                </div>
                <small class="text-muted">9 mins</small>
              </div>
            </div>
          </div>
        </div>
     
        
     
    </div>
   
</template>

