<template>
  <div class="col-md-9 info row m-0 p-0">
    <div class="col-md-4">
      <div class="d-flex justify-content-between align-items-center">
        <p class="text-title mb-5">Experience</p>
        <a class="text-mini mb-5">See All</a>
      </div>
      <ul class="list-group list-unstyled ">
        <li v-for="(item, index) in dataExperience" :key="index" v-if="index < 3">
          <p class="text-mini">{{ item.date }}</p>
          <p class="text-subtitle">{{ item.title }}</p>
          <p class="text-mini">{{ item.location }}</p>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <div class="d-flex justify-content-between align-items-center">
        <p class="text-title mb-5">Education</p>
        <a class="text-mini mb-5">See All</a>
      </div>
      <ul class="list-group list-unstyled ">
        <li v-for="(item, index) in dataEducation" :key="index" v-if="index < 3">
          <p class="text-mini">{{ item.date }}</p>
          <p class="text-subtitle">{{ item.title }}</p>
          <p class="text-mini">{{ item.location }}</p>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <div class="d-flex justify-content-between align-items-center">
        <p class="text-title mb-5">Skill</p>
        <a class="text-mini mb-5">See All</a>
      </div>
      <ul class="list-group ">
        <li class="text-mini my-1" v-for="item in dataSkill" >
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
  export default {
    name: '',
    components: {

    },
    mixins: [],
    props: {

    },
    data() {
      return {
        dataExperience: [{
            date: "October 1'st 2022",
            title: "Google Developer Group Participant",
            location: "Indosat Tower"
          },
          {
            date: "October 1'st 2022",
            title: "Google Developer Group Participant",
            location: "Indosat Tower"
          },
          {
            date: "October 1'st 2022",
            title: "Google Developer Group Participant",
            location: "Indosat Tower"
          },
          {
            date: "October 1'st 2022",
            title: "Google Developer Group Participant",
            location: "Indosat Tower"
          },
          {
            date: "October 1'st 2022",
            title: "Google Developer Group Participant",
            location: "Indosat Tower"
          },

        ],
        dataEducation: [{
            date: "May 1st 2020 - June 23th 2024",
            title: "SMK IDN",
            location: "West Java"
          },
          {
            date: "May 1st 2020 - June 23th 2024",
            title: "SMK IDN",
            location: "West Java"
          },
          {
            date: "May 1st 2020 - June 23th 2024",
            title: "SMK IDN",
            location: "West Java"
          },
        ],
        dataSkill: [
          'HTML', 'CSS', 'JavaScript', 'React.js', 'Vue.js', 'Angular',
          'Java', 'Kotlin', 'XML', 'Android Studio', 'SQLite',
          'Dart', 'Flutter SDK', 'Material Design', 'Firebase'
        ]
      }
    },
    computed: {

    },
    watch: {

    },
    mounted() {

    },
    methods: {

    }
  };

</script>
<style>
  .info .text-title {
    font-weight: 700;
    font-size: 2.5rem;
  }

  .info .text-subtitle {
    font-weight: 700;
    font-size: 1.5rem;
  }

  .info .text-mini {
    font-weight: 500;
    font-size: 1rem;
    color: gray;
  }

</style>
