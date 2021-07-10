<template>
  <nav class="navbar navbar-expand-md navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Ableton Live</a>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Live</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Push</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Shop</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Packs</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Help</a>
          </li>
          <li class="nav-item dropdown"></li>
        </ul>
        <form class="d-flex">
          <a class="nav-link active" aria-current="page" href="#"
            >Try Live for free</a
          >
        </form>
      </div>
    </div>
  </nav>
  <div class="container">
    <div class="background"></div>
    <div class="display-3 margin-top">Hello! this is made by Bootstrap</div>
    <figcaption class="blockquote-footer">
      Someone famous in Source Title
    </figcaption>
  </div>
  <div class="container">
    <div class="row">
      <div class="col-12 col-lg-4 colleft ">
        <img
          class="img-1"
          src="https://images.pexels.com/photos/3756766/pexels-photo-3756766.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
          alt=""
        />
      </div>
      <div class="col-12 col-lg-4 colleft ">
        <img
          class="img-3"
          src="https://images.unsplash.com/photo-1511379938547-c1f69419868d?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
          alt=""
        />
      </div>
      <div class="col-12 col-lg-4 colleft ">
        <img
          class="img-2"
          src="https://images.unsplash.com/photo-1503832725-c34828469568?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=754&q=80"
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<style scoped>
.img-1 {
  width: 100%;
  height: 400px;
  object-fit: cover;
  transform: scaleX(-1);
  margin-bottom: 10px;
}
.img-2 {
  width: 100%;
  height: 300px;
  object-fit: cover;
  margin-bottom: 10px;
}

.img-3 {
  width: 100%;
  object-fit: cover;
  margin-bottom: 10px;
  transform: translate(60px, 0px);
}

@media (min-width: 768px) {
  .img-3 {
    transform: translate(60px, 200px);
  }
}
.margin-top {
  margin: 30px 0;
}
.background {
  position: fixed;
  z-index: -1;
  top: 0;
  left: 0;
  height: 50vh;
  width: 50vw;
  background-color: yellow;
}
.nav-item {
  margin-left: 20px;
}
</style>
