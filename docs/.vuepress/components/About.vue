<style>
.about-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 100vh;
}

.introduction {
  margin-top: 40px;
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
  margin-top: 32px;
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

.social-icons-container > ul > li {
  margin-right: 32px;
}

.social-icons-container > ul > li > a > img {
  width: 32px;
}

</style>

<template>
  <div class="about-section">
<!--    <div class="name">-->
<!--      <span class="firstname">ALBERT</span>-->
<!--      <span class="lastname">HERNANDEZ</span>-->
<!--    </div>-->

    <div class="introduction">
      <h2> Hi There, I'm Albert! <img src="https://raw.githubusercontent.com/ABSphreak/ABSphreak/master/gifs/Hi.gif" width="30px"></h2>

      <p>
        I'm a Software Engineer 🚀 from Spain 🇪🇸, currently working 👨🏻‍💻 at <em><a href="https://www.coverwallet.com/" target="_blank" rel="noopener noreferrer">Coverwallet, an Aon Company</a></em>.
      </p>
      <p>
        I'm a passionate learner who loves the code ☕︎. You'll always find me learning something new.
      </p>
      <p>
        Beside's programming, I love Apple 🍎, watching Netflix 📺 and delicious food 🌯 🍱.
      </p>
    </div>

    <div class="social-icons-container">
      <ul class="ui-list social-networks">
        <li>
          <a href="https://github.com/AlbertHernandez">
            <img src="../../icons/github.svg" alt="mongo">
          </a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/albert-hernandez-pellicer/">
            <img src="../../icons/linkedin.svg" alt="mongo">
          </a>
        </li>
        <li>
          <a href="https://medium.com/@AlbertHernandezDev">
            <img src="../../icons/medium.svg" alt="mongo">
          </a>
        </li>
        <li>
          <a href="mailto:alberthernandezdev@gmail.com">
            <img src="../../icons/gmail.svg" alt="mongo">
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import GithubIcon from 'vue-material-design-icons/GitHub.vue';
import LinkedinIcon from 'vue-material-design-icons/Linkedin.vue';
import EmailIcon from 'vue-material-design-icons/Email.vue';
import BookopenIcon from 'vue-material-design-icons/BookOpen.vue';

export default {
  name: "Introduction",
};
</script>