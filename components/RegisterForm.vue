<script setup lang="ts">
import { Input } from '@/components/ui/input'
import { Button } from '@/components/ui/button'
import { Label } from '@/components/ui/label'
</script>

<template>
  <form>
    <div py8 px5 bg-faded b rounded-lg border-base shadow-sm>
      <h1 pb pt text-lg font-bold text-center>
        Create an account
      </h1>
      <div flex flex-col gap-2 md:w="360px" w="300px">
        <div>
          <Label for="email">Email</Label>
          <Input id="email" type="email" placeholder="Email" />
        </div>

        <div>
          <Label for="password">Password</Label>
          <Input id="password" type="password" placeholder="Password" />
        </div>

        <div>
          <Label for="password">Repeat Password</Label>
          <Input id="password" type="password" placeholder="Repeat Password" />
        </div>

        <Button class="mt-6" variant="default">
          Create
        </Button>
        <Button class="mt-3" variant="link">
          <NuxtLink to="/">
            Login
          </NuxtLink>
        </Button>
      </div>
    </div>
  </form>
</template>
