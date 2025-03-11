<template>
  <div class="container">
    <div>User Login</div>
    <div style="width: 100%">
      <div style="width: 100%; float: auto">
        <form
          id="loginForm"
          @submit.prevent="login"
          style="
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 10px;
            background-color: #f9f9f9;
            margin: 0 auto;
            max-width: 400px;
            display: flex;
            flex-direction: column;
            align-items: center;
          "
        >
          <div style="margin-bottom: 15px">
            <input
              type="email"
              id="email"
              v-model="email"
              placeholder="user@email.com"
              style="width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 5px"
            />
          </div>
          <div style="margin-bottom: 15px">
            <input
              type="password"
              id="password"
              v-model="password"
              placeholder="Password"
              style="width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 5px"
            />
          </div>
          <button
            type="submit"
            class="btn btn-primary"
            style="
              width: 100%;
              padding: 10px;
              border: none;
              border-radius: 5px;
              background-color: #007bff;
              color: white;
            "
          >
            Login
          </button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'userLogin',
}
</script>
