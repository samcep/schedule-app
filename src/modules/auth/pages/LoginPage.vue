<script setup lang="ts">
import GoogleIcon from '../icons/GoogleIcon.vue'
</script>

<template>
  <div class="card bg-base-100 w-full max-w-sm shrink-0 shadow-2xl">
    <form class="card-body">
      <h1 class="text-2xl xl:text-3xl font-extrabold text-center">Sign In</h1>
      <div class="form-control">
        <label class="label">
          <span class="label-text">Email</span>
        </label>
        <input type="email" placeholder="email" class="input input-bordered" required />
      </div>
      <div class="form-control">
        <label class="label">
          <span class="label-text">Password</span>
        </label>
        <input type="password" placeholder="password" class="input input-bordered" required />
        <label class="label">
          <a href="#" class="label-text-alt link link-hover">Forgot password?</a>
        </label>
      </div>
      <div class="form-control mt-6">
        <button class="btn btn-primary">Login</button>
      </div>

      <div class="flex w-full flex-col">
        <div class="divider">or</div>
      </div>

      <div class="form-control">
        <button class="btn btn-neutral"><GoogleIcon></GoogleIcon>Sign in with Google</button>
      </div>
      <div class="form-contorl mt-6">
        <label class="label">
          <RouterLink :to="{ name: 'register' }" class="label-text-alt link link-hover"
            >Don't have an account? Sign up</RouterLink
          >
        </label>
      </div>
    </form>
  </div>
</template>
