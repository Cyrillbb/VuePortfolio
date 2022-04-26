<template>
  <div class="app-tag-cloud card">
    <ul class="cloud" role="navigation" aria-label="Webdev word cloud">
      <li v-for="(item, index) in tagsArr" :key="index">
        <a href="#" :data-weight="item.weight">{{ item.name }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "AppTagCloud",

  data() {
    return {
      tagsArr: [
        {
          name: "HTML5",
          weight: 5,
        },
        {
          name: "CSS3",
          weight: 4,
        },
        {
          name: "SCSS",
          weight: 5,
        },
        {
          name: "JavaScript",
          weight: 8,
        },
        {
          name: "React",
          weight: 10,
        },
        {
          name: "Express",
          weight: 1,
        },
        {
          name: "Jest",
          weight: 2,
        },
        {
          name: "Socket.io",
          weight: 3,
        },
        {
          name: "Responsive",
          weight: 6,
        },
        {
          name: "Ajax",
          weight: 10,
        },
        {
          name: "Vue",
          weight: 9,
        },
        {
          name: "Vuex",
          weight: 8,
        },
        {
          name: "TypeScript",
          weight: 6,
        },
        {
          name: "docker",
          weight: 4,
        },
        {
          name: "Git",
          weight: 3,
        },
        {
          name: "Linux",
          weight: 5,
        },
        {
          name: "PHP",
          weight: 2,
        },
        {
          name: "Vue-router",
          weight: 6,
        },
      ],
    };
  },
};
</script>

<style>
.app-tag-cloud {
  display: flex;
  align-items: center;
  justify-content: center;
}

ul.cloud {
  list-style: none;
  padding-left: 0;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  line-height: 2.75rem;
  width: 450px;
}

ul.cloud a {
  --size: 4;
  --color: #ff9e64;
  color: var(--color);
  font-size: calc(var(--size) * 0.25rem + 0.5rem);
  display: block;
  padding: 0.125rem 0.25rem;
  position: relative;
  text-decoration: none;
  transition: all 0.25s;
}

ul.cloud a[data-weight="1"] {
  --size: 1;
}
ul.cloud a[data-weight="2"] {
  --size: 2;
}
ul.cloud a[data-weight="3"] {
  --size: 3;
}
ul.cloud a[data-weight="4"] {
  --size: 4;
}
ul.cloud a[data-weight="5"] {
  --size: 6;
}
ul.cloud a[data-weight="6"] {
  --size: 8;
}
ul.cloud a[data-weight="7"] {
  --size: 10;
}
ul.cloud a[data-weight="8"] {
  --size: 13;
}
ul.cloud a[data-weight="9"] {
  --size: 16;
}

ul[data-show-value] a::after {
  content: " (" attr(data-weight) ")";
  font-size: 1rem;
}

ul.cloud li:nth-child(2n + 1) a {
  --color: #9ece6a;
}
ul.cloud li:nth-child(3n + 1) a {
  --color: #7aa2f7;
}
ul.cloud li:nth-child(4n + 1) a {
  --color: #f7768e;
}

ul.cloud a:focus {
  outline: 1px dashed;
}

ul.cloud a::before {
  content: "";
  position: absolute;
  top: 0;
  left: 50%;
  width: 0;
  height: 100%;
  background: var(--color);
  transform: translate(-50%, 0);
  opacity: 0.15;
  transition: all 0.25s;
}

ul.cloud a:hover {
  scale: 1.3;
  z-index: 10;
  /* font-size: 25px; */
  transition: all 0.25s;
}

@media (prefers-reduced-motion) {
  ul.cloud * {
    transition: none !important;
  }
}

@keyframes blick {
  100% {
    left: 125%;
  }
}
</style>