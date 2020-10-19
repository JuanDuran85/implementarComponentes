<template>
  <div class="container">
      <div class="row">
          <div class="col-12 col-sm-12 col-md-6 col-lg-4 col-xl-4">
            <div class="card">
                <img :src="urlImg" class="card-img-top" alt="img1">
                <div class="card-body">
                    <h5 class="card-title">Card title</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
            </div>
          </div>
          <div class="col-12 col-sm-12 col-md-6 col-lg-4 col-xl-4">
            <div class="card">
                <img :src="urlImg" class="card-img-top" alt="img1">
                <div class="card-body">
                    <h5 class="card-title">Card title</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
            </div>
          </div>
          <div class="col-12 col-sm-12 col-md-6 col-lg-4 col-xl-4">
            <div class="card">
                <img :src="urlImg" class="card-img-top" alt="img1">
                <div class="card-body">
                    <h5 class="card-title">Card title</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
            </div>
          </div>
          <div class="col-12 col-sm-12 col-md-6 col-lg-4 col-xl-4">
            <div class="card">
                <img :src="urlImg" class="card-img-top" alt="img1">
                <div class="card-body">
                    <h5 class="card-title">Card title</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
            </div>
          </div>
          <div class="col-12 col-sm-12 col-md-6 col-lg-4 col-xl-4">
            <div class="card">
                <img :src="urlImg" class="card-img-top" alt="img1">
                <div class="card-body">
                    <h5 class="card-title">Card title</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
            </div>
          </div>
          <div class="col-12 col-sm-12 col-md-6 col-lg-4 col-xl-4">
            <div class="card">
                <img :src="urlImg" class="card-img-top" alt="img1">
                <div class="card-body">
                    <h5 class="card-title">Card title</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
            </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Cards',
    props: {
/*         urlImg: {
            type: String,
            required: true,
            default: "https://picsum.photos/seed/picsum/200/300"
        }, */
        dataCards: {
            type: Array,
            required: true
        }
    }
}
</script>

<style>

</style>