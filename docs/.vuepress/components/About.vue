<style>
.about-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-top: -38.8px;
  min-height: 100vh;
}

.name {
  font-size: 3rem;
  font-weight: bold;
}

.lastname {
  color: #1DA1F2;
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

.social-icons-container > ul > li.youtube > a > img {
  margin-top: -3px
}

</style>

<template>
  <div class="about-section">
    <div class="introduction">
      <h2> Hi There, I'm
        <div class="name">
          <span class="firstname">Albert</span>
          <span class="lastname">Hernandez</span>
          <img src="https://raw.githubusercontent.com/ABSphreak/ABSphreak/master/gifs/Hi.gif" width="32px">
        </div>

      </h2>


      <p>
        I'm a Software Engineer 🚀 from Spain 🇪🇸, currently working 👨🏻‍💻 at <em><a href="https://www.coverwallet.com/" target="_blank" rel="noopener noreferrer">Coverwallet, an Aon Company</a></em>.
        <br>
        I'm a passionate learner who loves the code ☕︎. You'll always find me learning something new.
      </p>
      <p>
         Also, I have started a <em><a href="https://www.youtube.com/channel/UCrjQ8NCnBBI4M3CZlkua8CQ" target="_blank" rel="noopener noreferrer">youtube channel</a></em> where I create tutorials about Web Technologies like Node, Javascript... I love sharing knowledge, it's the best way to grow 🚀
      </p>
      <p>
        Beside's programming, I love Apple 🍎, watching Netflix 📺 and delicious food 🌯 🍱.
      </p>
    </div>

    <div class="social-icons-container">
      <ul class="ui-list social-networks">
        <li>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/AlbertHernandez">
            <img src="../../icons/github.svg" alt="github">
          </a>
        </li>
        <li>
          <a target="_blank" rel="noopener noreferrer" href="https://www.linkedin.com/in/albert-hernandez-pellicer/">
            <img src="../../icons/linkedin.svg" alt="linkedin">
          </a>
        </li>
        <li>
          <a target="_blank" rel="noopener noreferrer" href="https://medium.com/@AlbertHernandezDev">
            <img src="../../icons/medium.svg" alt="medium">
          </a>
        </li>
        <li>
          <a target="_blank" rel="noopener noreferrer" href="mailto:alberthernandezdev@gmail.com">
            <img src="../../icons/gmail.svg" alt="mail">
          </a>
        </li>
        <li class="youtube">
          <a target="_blank" rel="noopener noreferrer" href="https://www.youtube.com/channel/UCrjQ8NCnBBI4M3CZlkua8CQ">
            <img src="../../icons/youtube.svg" alt="youtube">
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
