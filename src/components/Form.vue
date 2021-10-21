<template>
  <div>
    <pre>
      {{ JSON.stringify(formValues, null, 2) }}
    </pre>
    <form>
      <p>Employee Form</p>
      <hr />
      <div>
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="formValues.name" />
      </div>
      <div>
        <label for="profile">Profile Summary:</label>
        <textarea
          type="text"
          id="profile"
          v-model="formValues.profileSummary"
        />
      </div>
      <div>
        <label for="job-location">Job Location</label>
        <select id="job-location" multiple v-model="formValues.jobLocation">
          <option value="Delhi">Delhi</option>
          <option value="Haryana">Haryana</option>
          <option value="Punjab">Punjab</option>
        </select>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      formValues: {
        name: "",
        profileSummary: "",
        jobLocation: [],
      },
    };
  },
};
</script>