<template>
<header id="header">
   <i class="fa fa-list mobile-nav-toggle d-xl-none"></i>
    <div class="d-flex flex-column">

      <div class="profile">
        <img src="https://i.postimg.cc/htbQPnYV/rsz-img-20220228-wa0028.jpg" alt="" class="img-fluid rounded-circle">
        <h1 class="text-light"><a href="#">Emihle Cebisa</a></h1>
        <div class="social-links mt-3 text-center">
          <a href="https://github.com/CebisaE/" target="_blank" class="google-plus"><i class="fab fa-github"></i></a>
          <a href="https://codepen.io/cebisae"  target="_blank" class="google-plus"><i class="fab fa-codepen"></i></a>
          <a href="https://www.linkedin.com/in/emihle-cebisa-60292b223" target="_blank" class="linkedin"><i class="fab fa-linkedin-in"></i></a>
        </div>
      </div>

      <nav id="navbar" class="nav-menu navbar mobile-nav-active">
        <ul>
          <li><a href="#hero" class="nav-link scrollto active"><i class="fa fa-home"></i> <span>Home</span></a></li>
          <li><a href="#about" class="nav-link scrollto"><i class="fa fa-user"></i> <span>About</span></a></li>
          <li><a href="#resume" class="nav-link scrollto"><i class="fa fa-file"></i> <span>Resume</span></a></li>
          <li><a href="#projects" class="nav-link scrollto"><i class="fa fa-book"></i> <span>Projects</span></a></li>
          <li><a href="#testimonials" class="nav-link scrollto"><i class="fa fa-server"></i> <span>Testimonials</span></a></li>
          <li><a href="#contact" class="nav-link scrollto"><i class="fa fa-envelope"></i> <span>Contact</span></a></li>
        </ul>
      </nav>
      <!-- <b-button v-b-toggle.sidebar-variant>Toggle Sidebar</b-button> -->
    <!-- <b-sidebar id="sidebar-variant" title="Sidebar" bg-variant="dark" text-variant="light" shadow>
      <div class="px-3 py-2">
        <p>
          Cras mattis consectetur purus sit amet fermentum. Cras justo odio, dapibus ac facilisis
          in, egestas eget quam. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.
        </p>
        <b-img src="https://picsum.photos/500/500/?image=54" fluid thumbnail></b-img>
      </div>
    </b-sidebar> -->
    </div>
  </header>

</template>

<script>
export default {
  methods:{
    function() {
  "use strict";

  /**
   * Easy selector helper function
   */
  const select = (el, all = false) => {
    el = el.trim()
    if (all) {
      return [...document.querySelectorAll(el)]
    } else {
      return document.querySelector(el)
    }
  }

  /**
   * Easy event listener function
   */
  const on = (type, el, listener, all = false) => {
    let selectEl = select(el, all)
    if (selectEl) {
      if (all) {
        selectEl.forEach(e => e.addEventListener(type, listener))
      } else {
        selectEl.addEventListener(type, listener)
      }
    }
  }

  /**
   * Easy on scroll event listener 
   */
  const onscroll = (el, listener) => {
    el.addEventListener('scroll', listener)
  }

  /**
   * Navbar links active state on scroll
   */
  let navbarlinks = select('#navbar .scrollto', true)
  const navbarlinksActive = () => {
    let position = window.scrollY + 200
    navbarlinks.forEach(navbarlink => {
      if (!navbarlink.hash) return
      let section = select(navbarlink.hash)
      if (!section) return
      if (position >= section.offsetTop && position <= (section.offsetTop + section.offsetHeight)) {
        navbarlink.classList.add('active')
      } else {
        navbarlink.classList.remove('active')
      }
    })
  }
  window.addEventListener('load', navbarlinksActive)
  onscroll(document, navbarlinksActive)

  /**
   * Scrolls to an element with header offset
   */
  const scrollto = (el) => {
    let elementPos = select(el).offsetTop
    window.scrollTo({
      top: elementPos,
      behavior: 'smooth'
    })
  }

  /**
   * Back to top button
   */
  let backtotop = select('.back-to-top')
  if (backtotop) {
    const toggleBacktotop = () => {
      if (window.scrollY > 100) {
        backtotop.classList.add('active')
      } else {
        backtotop.classList.remove('active')
      }
    }
    window.addEventListener('load', toggleBacktotop)
    onscroll(document, toggleBacktotop)
  }

  /**
   * Mobile nav toggle
   */
  on('click', '.mobile-nav-toggle', function(e) {
    select('body').classList.toggle('mobile-nav-active')
    this.classList.toggle('fa-list')
    this.classList.toggle('fa-x')
  })

  /**
   * Scrool with ofset on links with a class name .scrollto
   */
  on('click', '.scrollto', function(e) {
    if (select(this.hash)) {
      e.preventDefault()

      let body = select('body')
      if (body.classList.contains('mobile-nav-active')) {
        body.classList.remove('mobile-nav-active')
        let navbarToggle = select('.mobile-nav-toggle')
        navbarToggle.classList.toggle('bi-list')
        navbarToggle.classList.toggle('bi-x')
      }
      scrollto(this.hash)
    }
  }, true)

  /**
   * Scroll with ofset on page load with hash links in the url
   */
  window.addEventListener('load', () => {
    if (window.location.hash) {
      if (select(window.location.hash)) {
        scrollto(window.location.hash)
      }
    }
  });
  }
  }
}
</script>

<style>
#header {
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  width: 300px;
  transition: all ease-in-out 0.5s;
  z-index: 9997;
  transition: all 0.5s;
  padding: 0 15px;
  background: #040b14;
  overflow-y: auto;
}
#header .profile img {
  margin: 15px auto;
  display: block;
  width: 120px;
  border: 8px solid #2c2f3f;
}
#header .profile h1 {
  font-size: 24px;
  margin: 0;
  padding: 0;
  font-weight: 600;
  -moz-text-align-last: center;
  text-align-last: center;
  font-family: "Poppins", sans-serif;
}
#header .profile h1 a, #header .profile h1 a:hover {
  color: #fff;
  text-decoration: none;
}
#header .profile .social-links a {
  font-size: 18px;
  display: inline-block;
  background: #212431;
  color: #fff;
  line-height: 1;
  padding: 8px 0;
  margin-right: 4px;
  border-radius: 50%;
  text-align: center;
  width: 36px;
  height: 36px;
  transition: 0.3s;
}
#header .profile .social-links a:hover {
  background: #149ddd;
  color: #fff;
  text-decoration: none;
}

#main {
  margin-left: 300px;
}

@media (max-width: 1199px) {
  #header {
    left: -300px;
  }

  #main {
    margin-left: 0;
  }
}
/* Desktop Navigation */
.nav-menu {
  padding: 30px 0 0 0;
}
.nav-menu * {
  margin: 0;
  padding: 0;
  list-style: none;
}
.nav-menu > ul > li {
  position: relative;
  white-space: nowrap;
}
.nav-menu a, .nav-menu a:focus {
  display: flex;
  align-items: center;
  color: #a8a9b4;
  padding: 12px 15px;
  margin-bottom: 8px;
  transition: 0.3s;
  font-size: 15px;
}
.nav-menu a i, .nav-menu a:focus i {
  font-size: 24px;
  padding-right: 8px;
  color: #6f7180;
}
.nav-menu a:hover, .nav-menu .active, .nav-menu .active:focus, .nav-menu li:hover > a {
  text-decoration: none;
  color: #fff;
}
.nav-menu a:hover i, .nav-menu .active i, .nav-menu .active:focus i, .nav-menu li:hover > a i {
  color: #149ddd;
}

/* Mobile Navigation */
.mobile-nav-toggle {
  position: fixed;
  right: 15px;
  top: 15px;
  z-index: 9998;
  border: 0;
  font-size: 24px;
  transition: all 0.4s;
  outline: none !important;
  background-color: #149ddd;
  color: #fff;
  width: 40px;
  height: 40px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  line-height: 0;
  border-radius: 50px;
  cursor: pointer;
}

.mobile-nav-active {
  overflow: hidden;
}
.mobile-nav-active #header {
  left: 0;
}


</style>