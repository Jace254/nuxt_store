<script setup lang="ts">
import { Input } from '@/components/ui/input'
import { Button } from '@/components/ui/button'
import { Label } from '@/components/ui/label'
</script>

<template>
  <form>
    <div py8 px5 bg-faded b rounded-lg border-base shadow-sm>
      <h1 pb pt text-lg font-bold text-center>
        Login to your account
      </h1>
      <div flex flex-col gap-2 md:w="360px" w="300px">
        <Input id="email" type="email" placeholder="Email" />

        <Input id="password" type="password" placeholder="Password" />

        <Button class="mt-6" variant="default">
          Sign In
        </Button>
        <Button class="mt-3" variant="link">
          <NuxtLink to="/register">
            Register
          </NuxtLink>
        </Button>
      </div>
    </div>
  </form>
</template>
