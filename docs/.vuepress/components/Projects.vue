<style>
.projects-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 100vh;
  margin-top: 24px;
}


.card.purple {
  background: linear-gradient(135deg, #CE9FFC 0%,#7367F0 100%);
}

.card.green {
  background: linear-gradient(150deg, #39ef74, #4600f1 100%);
}

.card.blue {
  background: linear-gradient(135deg, #13f1fc 0%,#0470dc 100%);
}

.card.magenta {
  background: linear-gradient(135deg, #FF57B9 0%,#A704FD 100%);
}

.card.orange {
  background:linear-gradient(135deg, #fad961 0%,#f76b1c 100%);
}

.card.sun {
  background:linear-gradient(135deg, #fcdf8a 0%,#f38381 100%);
}

.card.red {
  background:linear-gradient(135deg, #F5515F 0%,#A1051D 100%);
}

.card.cyan {
  background:linear-gradient(135deg, #0FF0B3 0%,#036ED9 100%);
}

.card.bull {
background: rgb(104,175,223);
background: linear-gradient(90deg, rgba(104,175,223,1) 50%, rgba(0,191,255,1) 100%);

}

.card {
  width: 300px;
  box-sizing: border-box;
  padding: 2em;
  border-radius: 10px;
  color: white;
  box-shadow: 5px 5px 10px #ccc;
  margin-right: 1em;
  margin-bottom: 1em;
  filter: grayscale(40%);
}

.card:hover {
  filter: grayscale(0%);
}

.card > a {
  color: #FFFFFF;
  text-decoration: none;
}

.card > a > button:hover {
  color: #1DA1F2;
  cursor:pointer;
}

button {
  text-transform: uppercase;
  width: 150px;
  display: block;
  margin: 0 auto;
  border-radius: 10px;
  padding: 1em;
  background: white;
  border: none;
  font-weight: bold;
  margin-top: 4em;
}

.project-cards {

}

.ui-list {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.project-cards > ul {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

</style>

<template>
  <div class="projects-section">
    <p>
      Sometimes I like to create some personal projects to learn new technologies and be updated and give my bit to the community.
    </p>
    <p>
      When I started working with node, I was working on an existing application, so I was always curious about how I could create a service from scratch, so guess what? I made my own! I leave it below if you want to take a look at it and if you want to contact me to give me feedback or talk about it you know where I am!
    </p>

    <div class="project-cards">
      <ul class="ui-list">
        <li>
          <div class="card purple">
            <h2>Node Todo Application</h2>
            <p>
              Typescript Node Application with some concepts I'm learning like Dependency Injection, Error handler, Logger with Request Id and more!
            </p>
            <p>
              <div class="stack">
                <ul class="ui-list">
                  <li>
                    <img src="../../icons/typescript.svg" alt="typescript">
                  </li>
                  <li>
                    <img src="../../icons/nodejs.svg" alt="node">
                  </li>
                  <li>
                    <img src="../../icons/mongodb.svg" alt="mongo">
                  </li>
                  <li>
                    <img src="../../icons/docker.svg" alt="docker">
                  </li>
                </ul>
              </div>
            </p>
            <a target="_blank" rel="noopener noreferrer" href="https://github.com/AlbertHernandez/todo-node">
              <button>
                Visit
              </button>
            </a>
          </div>
        </li>

          <li>
            <div class="card bull">
              <h2>Bull Bus</h2>
              <p>
                Library that exposes an async event bus using Bull with redis. Useful when we want to work with an event-bus in a project but we don't want to use external providers like kafka or PubSub.
              </p>
              <p>
                <div class="stack">
                  <ul class="ui-list">
                    <li>
                      <img src="../../icons/typescript.svg" alt="typescript">
                    </li>
                    <li>
                      <img src="../../icons/nodejs.svg" alt="node">
                    </li>
                  </ul>
                </div>
              </p>
              <a target="_blank" rel="noopener noreferrer" href="https://github.com/AlbertHernandez/bull-bus">
                <button>
                  Visit
                </button>
              </a>
            </div>
          </li>
      </ul>

    </div>

    <p>
      Some time ago I discovered the github actions, I started to use them in many projects and I also made some of my own, they are not much but I am glad that there are people who see them useful and are using them.
    </p>

    <div class="project-cards">
      <ul class="ui-list">
        <li>
          <div class="card green">
            <h2>Branch Name Action</h2>
            <p>
              Check if the branch name is following a convention name
            </p>
            <p>
              <div class="stack">
                <ul class="ui-list">
                  <li>
                    <img src="../../icons/javascript.svg" alt="javascript">
                  </li>
                  <li>
                    <img src="../../icons/docker.svg" alt="docker">
                  </li>
                  <li>
                    <img src="../../icons/npm.svg" alt="docker">
                  </li>
                </ul>
              </div>
            </p>
            <a target="_blank" rel="noopener noreferrer" href="https://github.com/AlbertHernandez/branch-name-action">
              <button>
                Visit
              </button>
            </a>
          </div>
        </li>

        <li>
          <div class="card blue">
            <h2>Assign Me</h2>
            <p>
              Automatically adds you to the assignees in the pull request
            </p>
            <p>
            <div class="stack">
              <ul class="ui-list">
                <li>
                  <img src="../../icons/javascript.svg" alt="javascript">
                </li>
                <li>
                  <img src="../../icons/docker.svg" alt="docker">
                </li>
                <li>
                  <img src="../../icons/npm.svg" alt="docker">
                </li>
              </ul>
            </div>
            </p>
            <a target="_blank" rel="noopener noreferrer" href="https://github.com/AlbertHernandez/assign-me">
              <button>
                Visit
              </button>
            </a>
          </div>
        </li>

        <li>
          <div class="card magenta">
            <h2>Working Label Action</h2>
            <p>
              Add labels depending if the pull request is ready to review
            </p>
            <p>
            <div class="stack">
              <ul class="ui-list">
                <li>
                  <img src="../../icons/javascript.svg" alt="javascript">
                </li>
                <li>
                  <img src="../../icons/docker.svg" alt="docker">
                </li>
                <li>
                  <img src="../../icons/npm.svg" alt="docker">
                </li>
              </ul>
            </div>
            </p>
            <a target="_blank" rel="noopener noreferrer" href="https://github.com/AlbertHernandez/working-label-action">
              <button>
                Visit
              </button>
            </a>
          </div>
        </li>

        <li>
          <div class="card orange">
            <h2>Is Ready Action</h2>
            <p>
              Check if the Pull Request is Ready to be Merged in the main branch.
            </p>
            <p>
            <div class="stack">
              <ul class="ui-list">
                <li>
                  <img src="../../icons/javascript.svg" alt="javascript">
                </li>
                <li>
                  <img src="../../icons/docker.svg" alt="docker">
                </li>
                <li>
                  <img src="../../icons/npm.svg" alt="docker">
                </li>
              </ul>
            </div>
            </p>
            <a target="_blank" rel="noopener noreferrer" href="https://github.com/AlbertHernandez/is-ready-action">
              <button>
                Visit
              </button>
            </a>
          </div>
        </li>
      </ul>

    </div>

    <p>
      I am a big fan of the Insomnia application, for me it is the best client to make REST requests to services. And you know the best thing? You can create your own plugins so I couldn't resist to make some!
    </p>

    <div class="project-cards">
      <ul class="ui-list">
        <li>
          <div class="card red">
            <h2>Ocean Light Theme</h2>
            <p>
              Light theme for Insomnia
            </p>
            <p>
            <div class="stack">
              <ul class="ui-list">
                <li>
                  <img src="../../icons/javascript.svg" alt="javascript">
                </li>
                <li>
                  <img src="../../icons/npm.svg" alt="docker">
                </li>
              </ul>
            </div>
            </p>
            <a target="_blank" rel="noopener noreferrer" href="https://insomnia.rest/plugins/insomnia-plugin-ocean-light-theme">
              <button>
                Visit
              </button>
            </a>
          </div>
        </li>

        <li>
          <div class="card cyan">
            <h2>Ocean Dark Theme</h2>
            <p>
              Dark theme for Insomnia
            </p>
            <p>
            <div class="stack">
              <ul class="ui-list">
                <li>
                  <img src="../../icons/javascript.svg" alt="javascript">
                </li>
                <li>
                  <img src="../../icons/npm.svg" alt="docker">
                </li>
              </ul>
            </div>
            </p>
            <a target="_blank" rel="noopener noreferrer" href="https://insomnia.rest/plugins/insomnia-plugin-ocean-dark-theme">
              <button>
                Visit
              </button>
            </a>
          </div>
        </li>
      </ul>

    </div>
  </div>
</template>

<script>
export default {
  name: "Projects",
};
</script>
