<template>
  <div>
    <b-navbar toggleable="md" type="dark" variant="info">
        <div class="container">
            <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
            <img class="logo" src="../assets/images/banners/logo.svg">
            <b-collapse is-nav id="nav_collapse">
                <b-navbar-nav>
                    <b-nav-item href="#"><b>หน้าแรก</b></b-nav-item>
                    <b-nav-item href="#"><b>ที่พัก</b></b-nav-item>
                    <b-nav-item href="#"><b>ยอดนิยม</b></b-nav-item>
                    <b-nav-item href="#"><b>โปรโมชัน</b></b-nav-item>
                    <b-nav-item href="#"><b>ติดต่อเรา</b></b-nav-item>
                </b-navbar-nav>
            </b-collapse>
        </div>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'navbar',
  data () {
    return {}
  }
}
