<style>
.job-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 100vh;
}

.job {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.position {
  font-weight: bold;
  color: #1DA1F2;
}

.time {
  margin-left: auto;
}

.description {

}

.company {
  font-weight: bold;
  font-size: 24px;
  font-family: 'Saira Extra Condensed', sans-serif;
}

.coverwallet-title {
  margin-top: 8px;
}

.ui-list {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.stack {
  margin-top: 24px;
}

.stack > ul {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.stack > ul > li {
  margin-right: 32px;
}

.stack > ul > li > img {
  width: 32px;
}

</style>

<template>
  <div class="job-section">
    <timeline>
      <timeline-title>
        <img
            src="https://images.assets-landingi.com/h3sfIxbQ/coverwallet_icon_blue.png"
            class="icon-heart"
            slot="others"
        />
        <div class="company coverwallet-title">
          CoverWallet, an Aon company
        </div>
      </timeline-title>

      <timeline-item bg-color="#9dd8e0">
        <div class="job">
          <div class="position"> Software Engineer </div>
          <div class="time"> March 2021 - Present </div>
          <div class="stack">
            <ul class="ui-list">
              <li>
                <img src="../../icons/nodejs.svg" alt="node">
              </li>
              <li>
                <img src="../../icons/redis.svg" alt="redis">
              </li>
              <li>
                <img src="../../icons/mongodb.svg" alt="mongo">
              </li>
              <li>
                <img src="../../icons/postgresql.svg" alt="postgresql">
              </li>
              <li>
                <img src="../../icons/docker.svg" alt="docker">
              </li>
              <li>
                <img src="../../icons/npm.svg" alt="npm">
              </li>
              <li>
                <img src="../../icons/nestjs.svg" alt="npm">
              </li>
            </ul>
          </div>
        </div>
      </timeline-item>

      <timeline-item bg-color="#fd7878">
        <div class="job">
          <div class="position"> Junior FullStack Frontend Software Engineer </div>
          <div class="time"> October 2019 - March 2021 </div>
          <div class="description">
            <p>
              Together with some node developers, we have created multiple microservices that have
              become core projects of the company. Some of them are systems of recommendations of
              actions to our agents, system of assignments of agents to customers who enter the
              platform, system of synchronization between different consumers and providers...
            </p>

            <p>
              For all these microservices I have been leading the part of the UI where we offer
              real time information of all of them. I have also participated in the node services
              themselves, working closely with the Product team, SalesForce and Node developers
              for adapting all our services to new requirements in a scalable way.
            </p>

            <p>
              To carry out all these services we have used technologies like React and Redux
              at the client, and for the backend Node with Koa. We have also used Postgres,
              Mongo and Redis as database, all depending on the project itself.
            </p>
          </div>
          <div class="stack">
            <ul class="ui-list">
              <li>
                <img src="../../icons/nodejs.svg" alt="node">
              </li>
              <li>
                <img src="../../icons/redis.svg" alt="redis">
              </li>
              <li>
                <img src="../../icons/mongodb.svg" alt="mongo">
              </li>
              <li>
                <img src="../../icons/postgresql.svg" alt="postgresql">
              </li>
              <li>
                <img src="../../icons/docker.svg" alt="docker">
              </li>
              <li>
                <img src="../../icons/html-five.svg" alt="html">
              </li>
              <li>
                <img src="../../icons/redux.svg" alt="redux">
              </li>
              <li>
                <img src="../../icons/sass-alt.svg" alt="sass">
              </li>
              <li>
                <img src="../../icons/npm.svg" alt="npm">
              </li>
            </ul>
          </div>
        </div>
      </timeline-item>

      <timeline-item bg-color="#3ad49f">
        <div class="job">
          <div class="position"> Junior Frontend Software Engineer </div>
          <div class="time"> July 2019 - October 2019 </div>
          <div class="description">
            <p>
              I worked on an existing frontend project. My tasks included fixing bugs, creating new
              features defined by the product team, integrating third party services and participating
              in team code reviews.
            </p>
          </div>
          <div class="stack">
            <ul class="ui-list">
              <li>
                <img src="../../icons/html-five.svg" alt="html">
              </li>
              <li>
                <img src="../../icons/redux.svg" alt="redux">
              </li>
              <li>
                <img src="../../icons/sass-alt.svg" alt="sass">
              </li>
              <li>
                <img src="../../icons/npm.svg" alt="npm">
              </li>
            </ul>
          </div>
        </div>
      </timeline-item>

      <timeline-item bg-color="#ffd129">
        <div class="job">
          <div class="position"> Internship </div>
          <div class="time"> Feb 2019 - July 2019 </div>
          <div class="description">
            <p>
              I worked in the frontend team with some very talented engineers, here I learned how to produce
              software in a clean and scalable way, that would allow us to reuse our solutions in an easy way.
            </p>
          </div>
          <div class="stack">
            <ul class="ui-list">
              <li>
                <img src="../../icons/html-five.svg" alt="html">
              </li>
              <li>
                <img src="../../icons/redux.svg" alt="redux">
              </li>
              <li>
                <img src="../../icons/sass-alt.svg" alt="sass">
              </li>
              <li>
                <img src="../../icons/npm.svg" alt="npm">
              </li>
            </ul>
          </div>
        </div>
      </timeline-item>
    </timeline>
  </div>
</template>

<script>
import { Timeline, TimelineItem, TimelineTitle } from 'vue-cute-timeline'

export default {
  components: {
    Timeline,
    TimelineItem,
    TimelineTitle
  }
}
</script>