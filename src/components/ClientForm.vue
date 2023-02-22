<template>
  <section class="hello container">
    <h1>{{ msg }}</h1>
    <form action="">
      <!-- <fieldset>
        <legend>CUSTOMER INFORMATION</legend> -->
      <div class="container-gr">
        <div class="column-position">
          <label for="name">Name </label>
          <input
            type="text"
            id="name"
            placeholder="Your first name.."
            class="input__3"
          />
        </div>
        <div class="column-position">
          <label for="phone">Phone </label>
          <input
            type="text"
            id="phone"
            placeholder="Your phone number"
            class="input__3"
          />
        </div>
        <div class="column-position">
          <label for="email">Email </label>
          <input
            type="email"
            id="email"
            placeholder="Your email"
            class="input__3"
          />
        </div>
      </div>
      <div class="column-position">
        <label for="problem">Problem </label>
        <input
          type="text"
          id="problem"
          placeholder="Your problem"
          class="input__3"
        />
      </div>
      <div class="column-position">
        <label for="message">Description </label>
        <textarea
          id="message"
          placeholder="Describe problem"
          name="message"
          class="input__3"
        >
        </textarea>
      </div>
      <button class="btn-form btn-red">Отправить</button>
      <!-- </fieldset> -->
    </form>
  </section>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
*,
*:before,
*:after {
  box-sizing: border-box;
}

label {
  margin-bottom: 6px;
}
.btn-form {
  border-radius: 6px;
  color: #fff;
  letter-spacing: 0.05em;
  padding: 13px 29px;
  width: 50%;
}
.btn-red {
  background: #aa2c18;
  border: 2px solid #aa2c18;
}
.btn-red:hover {
  background: #a30000;
}
.container {
  margin-left: 10%;
  margin-right: 10%;
  margin: 5%;
}
.container-gr {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 5%;
  margin-bottom: 20px;
}
.column-position {
  display: flex;
  flex-direction: column;
  // margin-top: 10px;
  margin-bottom: 10px;
  text-align: left;
}
.input__3 {
  border: solid 1px #000000;
  padding: 10px;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
@media screen and (max-width: 768px) {
  .container-gr {
    grid-template-columns: 1fr;
  }
}
</style>
