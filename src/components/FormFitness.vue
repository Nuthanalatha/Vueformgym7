<template>
  <h1>CUTE FITNESS CENTER</h1>
  <form @submit.prevent="handleSubmit">
    <div class="mb-3">
      <label for="cutomerName">Name</label>
      <input
        type="text"
        class="form-control"
        id="exampleInputEmail1"
        placeholder="ENTER NAME"
        v-model="name"
      />
      />
    </div>
    <div class="mb-3">
      <label for="cutomerAge">Age</label>
      <input
        type="text"
        class="form-control"
        id="exampleInputPassword1"
        placeholder="ENTER AGE"
        v-model="age"
      />
    </div>
    <div>
      <label for="customerPackage"> Select your fitness package</label>

      <select id="customerPackage" v-model="selectedPackage">
        <option value="muscle">Muscle Building</option>
        <option value="crossfit">Cross fit training</option>
        <option value="zumba">Zumba</option>
      </select>
    </div>
    <div>
      <label for="customerPackageValidity"> Package Validity</label>

      <select id="customerPackageValidity" v-model="packageValidity">
        <option value="3month">3 Months</option>
        <option value="6month">6 Months</option>
        <option value="1year">1 Year</option>
      </select>
    </div>

    <div class="mb-3 form-check">
      <h3>How did you hear about us ?</h3>
      <input
        type="checkbox"
        id="exampleCheck1"
        value="friendrefrence"
        v-model="referer"
      />
      <label for="friendref">Friend Reference</label>
      <input
        type="checkbox"
        id="socialMediaRef"
        value="socialMediaRef"
        v-model="referer"
      />
      <label for="socialmedia">Social Media</label>
      <input type="checkbox" id="normal" value="normal" v-model="referer" />
      <label for="nonref">None</label>
    </div>
    <div>
      <h3>Which category you belong to ?</h3>
      <input
        type="radio"
        id="overweight"
        value="overweight"
        v-model="category"
      />
      <label for="overweight">Overweight</label>
      <input
        type="radio"
        id="underweight"
        value="underweight"
        v-model="category"
      />
      <label for="underweight">Underweight</label>
      <input type="radio" id="normal" value="normal" v-model="category" />
      <label for="normal">Normal</label>
    </div>
    <div>
      <input
        type="checkbox"
        id="confirmTerm"
        value="friendrefrence"
        v-model="confirm"
      />
      <label for="confirmTerm">Agree to trems ?</label>
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      age: "",
      selectedPackage: "",
      packageValidity: "",
      referer: [],
      category: null,
      confirm: false,
    };
  },
  methods: {
    handleSubmit() {
      console.log("name", this.name);
      console.log("age", this.age);
      console.log("selectedPackage", this.selectedPackage);
      console.log("packageValidity", this.packageValidity);
      console.log("referer", this.referer);
      console.log("category", this.category);
      console.log("confirm", this.confirm);
      (name = ""),
        (age = ""),
        (selectedPackage = ""),
        (packageValidity = ""),
        (referer = []),
        (category = null),
        (confirm = false);
    },
  },
};
</script>

<style></style>
