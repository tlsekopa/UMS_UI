<template>
  <div>
    <div>
      <form action="http://127.0.0.1:3001/user" method="post" v-if="user">
      <h2>USER DETAILS</h2>
      <input type="text" name="username" placeholder="Username">&nbsp;
      <input type="text" name="password" placeholder="Password">&nbsp;
      <input type="text" name="activity" placeholder="Activity">&nbsp;
      <input type="text" name="avatar" placeholder="Avatar">&nbsp;
      <input type="text" name="actrole" placeholder="Role">&nbsp;
      <input type="submit" value="submit">
    </form>
    <form action="http://127.0.0.1:3001/person" method="post" v-else-if="person">
      <h2>PERSONAL DETAILS</h2>
      <input type="text" name="firstname" placeholder="First Name">&nbsp;
      <input type="text" name="lastname" placeholder="Last Name">&nbsp;
      <input type="text" name="age" placeholder="Age">&nbsp;
      <input type="text" name="gender" placeholder="Gender">&nbsp;
      <input type="submit" value="submit">
    </form>
    <form action="http://127.0.0.1:3001/contact" method="post" v-else>
      <h2>CONTACT DETAILS</h2>
      <input type="text" name="cellphone" placeholder="Cellphone">&nbsp;
      <input type="text" name="email" placeholder="E-Mail">&nbsp;
      <input type="text" name="facebook" placeholder="Facebook">&nbsp;
      <input type="text" name="twitter" placeholder="Twitter">&nbsp;
      <input type="text" name="tiktok" placeholder="TikTok">&nbsp;
      <input type="text" name="linkedin" placeholder="Linkedin">&nbsp;
      <input type="submit" value="submit">
    </form>
    </div>
    <div>
      <form action="http://127.0.0.1:3001/signin" method="post" v-if="signin">
      <h2>SIGN IN</h2>
      <input type="text" name="username" placeholder="USER NAME">
      <input type="text" name="password" placeholder="PASSWORD">
      <input type="submit" value="submit">
    </form>
    </div>
    
  </div> 
</template>
<script>
  export default {
    data: () => ({
      user: false,
      contact: false,
      person: false,
      signin: false
      
    }),

    methods: {
      
    },
  }
</script>