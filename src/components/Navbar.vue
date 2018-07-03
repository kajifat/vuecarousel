<template>
  <nav class="navigation">
      <div class="navigation__inner">
        <ul class="navigation__list">
          <li class="navigation__item"><a class="navigation__link" href="#">Home</a></li>
          <li class="navigation__item"><a class="navigation__link" href="#">About Us</a></li>
          <li class="navigation__item"><a class="navigation__link" href="#">Contact Us</a></li>
        </ul>
      </div>
    </nav>
</template>

<script>
export default {
  name: "Navbar",
  data () {
    return {}
  }
}
</script>

<style>
.navigation {
  width: 100%;
  max-width: 920px;
  position: fixed;
  border-bottom: 1px solid #ccc;
  background: #fff;
  height: 50px;
  z-index: 1;
}
.navigation__inner {
  display: flex;
  height: 50px;
  margin: 0 auto;
  overflow: hidden;
}

.navigation__link {
  display: block;
  padding-right: 40px;
  font-size: 14px;
  line-height: 50px;
  text-decoration: none;
  color: #000;
  cursor: pointer;
}
.navigation__link:hover {
  text-decoration: underline;
}

.navigation__list {
  display: flex;
  flex-wrap: wrap;
  margin: 0;
  padding: 0;
  list-style: none;
  background: #fff;
}
</style>

