<template>
  <div class="profile col-md-3">
    <div class="d-flex align-items-center flex-column">
      <div class="col-md-10">
        <img src="https://i.pinimg.com/originals/df/ef/52/dfef52bc718c0e35ded5ad5eb80da4bb.jpg"
          class="col-md-12 p-0 custom-div rounded" alt="">
        <p class="py-4 text-name">Budiono Siregar</p>
        <p class="text-desc">{{ dataDesc }}</p>
        <ul class="list-group list-unstyled " :class="{'contactMore' : dataContact.length > 3}">
          <li class="list-contact list-group-item-action" v-for="(item, index) in dataContact" >
            {{ item }}
          </li>
        </ul>
      </div>
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
        dataDesc: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus, inventore.',
        dataContact: ['armandnur10@gmail.com', 'mannd_10', 'armandnur10@outlook.com', 'armandnur10@outlook.com']
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
<style scoped>

  .profile {
    /* padding-top: 5rem; */
    letter-spacing: .25rem;
    font-family: 'Nunito Sans', sans-serif;
  }

  .list-contact {
    padding: .25rem!important;
    margin: .25rem 0!important;
    letter-spacing: 0px;
    border: 1px solid gray;
    border-radius: .25rem;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }

  .fw-bold {
    font-weight: 800;
  }

  .profile .text-name {
    font-weight: 800;
    font-size: 2.5rem;
  }

  .custom-div {
    max-height: 40vh;
  }

</style>
