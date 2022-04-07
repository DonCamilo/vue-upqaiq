<template>
  <form>
    <label>Email</label>
    <input type="email" required v-model="email" />
    <label>Password</label>
    <input type="password" required v-model="password" />
      <label>Role:</label>
    <select v-model="role">
      <option value="developer">WEB Developer</option>
      <option value="designer">WEB Designer</option>
    </select>
    <label> Skills</"label">

    <div class="terms">
    <input type="checkbox" v-model="terms" required>
    <label>Accept terms and coditions. </label>
  </div>
  <div>
    <input type="checkbox" value="shaun" v-model="names">
    <label>shan</label>
  <div>
  <div>
    <input type="checkbox" value="mario" v-model="names">
    <label>mario</label>
  <div>
  <div>
    <input type="checkbox" value="yoshi" v-model="names">
    <label>yoshi</label>
  <div>
  
  
 

    
    </select>
  </form>
  <p>Email: {{ email }}</p>
  <p>Password: {{ password }}</p>
  <p>Role: {{ role }}</p>
  <P> Terms accepted: {{ terms }}</p>
  <p> Names: {{""}} </p>
</template>
<script>
export default {
  data() {
    return {
      email: '',
      password: '',
      role:'',
      terms: false,
      names: [],
      tempSkill: '',
      skills: [], 

      

    };
  },
};
</script>
<style>
form {
  max-width: 420px;
  margin: 30px auto;
  background: white;
  text-align: left;
  padding: 40px;
  border-radius: 10px;
}
label {
  color: #aaa;
  display: inline-block;
  margin: 25px 0 15px;
  font-size: 0.6em;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
}
input,
select {
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border-top: none;
  border-left: none;
  border-right: none;
  border-bottom: 1xp solid #ddd;
  color: #555;
}
input[type='checkbox'] {
  display: inline-block;
  width: 16px;
  margin: 0 10px 0 0;
  position: relative;
  top: 2px;
}
.pill {
  display: inline-block;
  margin: 20px 10px 0 0;
  padding: 6px 12px;
  background: #eee;
  border-radius: 20px;
  font-size: 12px;
  letter-spacing: 1px;
  font-weight: bold;
  color: #777;
  cursor: pointer;
}
button {
  background: #0b6dff;
  border: 0;
  padding: 10px 20px;
  color: white;
  border-radius: 20px;
}
.submit {
  text-align: center;
}
.error {
  color: #ff0062;
  margin-top: 10px;
  font-size: 0.8em;
  font-weight: bold;
}
</style>
