<template>
  <header>
    <div class="container">
      <div class="row row--4">
          <h1 class="logo col">
            <span class="visually-hidden">BriteCore</span>
            <a href="#">
              <img src="../assets/images/logo.png" alt="BriteCore" />
              <i class="ion-arrow-down-b"></i>
            </a>
          </h1>
        <nav class="navbar col-three-fourths">
          <h2 class="visually-hidden">BriteCore Navbar</h2>
          <ul class="navbar__list list list--inline">
            <li class="navbar__item">
              <a href="" class="navbar__link">
                <i class="ion-umbrella"></i> Polices
              </a>
            </li>
            <li class="navbar__item">
              <a href="" class="navbar__link">
                <i class="ion-flash"></i> Claims
              </a>
            </li>
            <li class="navbar__item">
              <a href="" class="navbar__link">
                <i class="ion-person"></i> Contacts
              </a>
            </li>
            <li class="navbar__item">
              <a href="" class="navbar__link">
                <i class="ion-pie-graph"></i> Data
              </a>
            </li>
            <li class="navbar__item navbar__item--active">
              <a href="" class="navbar__link">
                <i class="ion-ios-book"></i> Lines
              </a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>
