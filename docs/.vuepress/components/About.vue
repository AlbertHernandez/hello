<style>
.about-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 100vh;
}

.introduction {
  margin-top: 40px;
  font-weight: bold;
}

.name {
  font-size: 3rem;
  font-weight: bold;
}

.lastname {
  color: #0086EB;
}

.section {
  min-height: 100vh;
}

.icon {
  width: 30px;
  height: 30px;
}

.social-icons-container {
  margin-top: 64px;
}

.social-networks {
  display: flex;
  justify-content: flex-start;
}

.ui-list {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.social-networks > li > a {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 50px;
  width: 50px;
  background-color: #495057;
  border-radius: 100%;
  margin-right: 16px;
}

.social-networks > li > a:hover {
  background-color: #0086EB;
}

</style>

<template>
  <div class="about-section section">
    <div class="name">
      <span class="firstname">ALBERT</span>
      <span class="lastname">HERNANDEZ</span>
    </div>

    <div class="introduction">
      <p>
        I'm a
        <span
            class="typing"
            data-period="2000"
            style="color: #1DA1F2; font-weight: bold"
            data-rotate='[ " Frontend ", " Backend ", " Fullstack " ]'>
            </span>
        Developer. I'm a passionate learner who loves the code.
      </p>
      <p>
        You'll always find me learning something new.
      </p>
    </div>

    <div class="social-icons-container">
      <ul class="ui-list social-networks">
        <li>
          <a href="https://github.com/AlbertHernandez">
            <img class="icon" src="../../icons/github.svg" alt="github-icon">
          </a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/albert-hernandez-pellicer/">
            <img class="icon" src="../../icons/linkedin-x.svg" alt="linkedin-icon">
          </a>
        </li>
        <li>
          <a href="https://medium.com/@AlbertHernandezDev">
            <img class="icon" src="../../icons/medium-x.svg" alt="medium-icon">
          </a>
        </li>
        <li>
          <a href="mailto:alberthernandezdev@gmail.com">
            <img class="icon" src="../../icons/round-mail-outline.svg" alt="mail-icon">
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Introduction",
};

var TxtRotate = function(el, toRotate, period) {
  this.toRotate = toRotate;
  this.el = el;
  this.loopNum = 0;
  this.period = parseInt(period, 10) || 2000;
  this.txt = '';
  this.tick();
  this.isDeleting = false;
};

TxtRotate.prototype.tick = function() {
  var i = this.loopNum % this.toRotate.length;
  var fullTxt = this.toRotate[i];

  if (this.isDeleting) {
    this.txt = fullTxt.substring(0, this.txt.length - 1);
  } else {
    this.txt = fullTxt.substring(0, this.txt.length + 1);
  }

  this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

  var that = this;
  var delta = 300 - Math.random() * 100;

  if (this.isDeleting) { delta /= 2; }

  if (!this.isDeleting && this.txt === fullTxt) {
    delta = this.period;
    this.isDeleting = true;
  } else if (this.isDeleting && this.txt === '') {
    this.isDeleting = false;
    this.loopNum++;
    delta = 500;
  }

  setTimeout(function() {
    that.tick();
  }, delta);
};

window.onload = function() {
  var elements = document.getElementsByClassName('typing');
  for (var i=0; i<elements.length; i++) {
    var toRotate = elements[i].getAttribute('data-rotate');
    var period = elements[i].getAttribute('data-period');
    if (toRotate) {
      new TxtRotate(elements[i], JSON.parse(toRotate), period);
    }
  }
  // INJECT CSS
  var css = document.createElement("style");
  css.type = "text/css";
  css.innerHTML = ".typing > .wrap { border-right: 0.08em solid #666 }";
  document.body.appendChild(css);
};
</script>