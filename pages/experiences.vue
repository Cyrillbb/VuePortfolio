<template>
  <div class="experiences">
    <app-card>
      <template #card-header> Hello header </template>
      <template #card-body>
        I'm a Front-end developer with experience in building web applications
        and websites. <br />
        I specialize in JavaScript/TypeScript and Vue.js (2 and 3). Also have a
        bit of experience in react.js, php and node.js.
      </template>
    </app-card>

    <app-card>
      <template #card-header> Preferred tech-stack </template>
      <template #card-body>
        <ul>
          <li>Vue.js (vue 2 and vue 3), vuex, vue-router, vue-cli.</li>
          <li>TypeScript</li>
          <li>HTML, CSS, SCSS, Bootstrap, PrimeFaces</li>
          <li>Docker</li>
          <li>Php, node.js</li>
        </ul>
      </template>
    </app-card>

    <app-card>
      <template #card-header>Experience</template>
      <div>Front-end developer at chain pharmacy "Vita" (vitaexpress.ru)</div>

      <template #card-body>
        <ul>
          <li>
            Developed a pharmacy chain e-commerce customer-facing website as a
            member of a 7-person team.
          </li>
          <li>
            Created a library of ui-components (inputs, modals, form validation
            logic etc.) as member of 2-person team.
          </li>
          <li>Created several promotion landing-pages.</li>
          <li>
            Implemented front-end logic along with 3rd-party software
            integrations for a custmer-facing project.
          </li>
          <li>
            Refactored several old modules with modern front-end technologies
            and practices.
          </li>
          <li>
            Created UI for several internal projects as a member of a 3-person
            team.
          </li>
        </ul>
      </template>
    </app-card>
  </div>
</template>

<style>
.experiences ul {
  font-size: 17px;
}
</style>
