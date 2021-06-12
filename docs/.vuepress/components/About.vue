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
      <h2> Hi There, I'm Albert! <img src="https://raw.githubusercontent.com/ABSphreak/ABSphreak/master/gifs/Hi.gif" width="30px"></h2>

      <p>
        I'm a Software Engineer 🚀 from Spain 🇪🇸, currently working 👨🏻‍💻 at <em><a href="https://www.coverwallet.com/">Coverwallet, an Aon Company</a></em>.
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
</script>