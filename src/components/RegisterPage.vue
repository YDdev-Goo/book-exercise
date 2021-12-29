<template>
  <div>
    <form @submit.prevent="submitForm">
      <div class="form-group">
        <input
          type="text"
          class="form-contool"
          id="username"
          v-model="form.username"
        />
      </div>
      <div class="form-group">
        <input
          type="email"
          id="emailAddress"
          class="form-control"
          v-model="form.emailAddress"
        />
      </div>
      <div class="form-group">
        <input
          type="password"
          id="password"
          class="form-control"
          v-model="form.password"
        />
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: 'RegisterPage',
  data: function () {
    return {
      form: {
        username: '',
        emailAddress: '',
        password: ''
      }
    }
  },
  methods: {
    submitForm() {}
  }
}
</script>

<style lang="scss" scoped></style>
