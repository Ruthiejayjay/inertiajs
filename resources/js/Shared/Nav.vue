<template>
  <nav class="ml-6">
    <ul class="flex space-x-6">
      <li>
        <NavLink href="/" :active="$page.component === 'Home'" >Home</NavLink>
      </li>
      <li>
        <NavLink href="/users" :active="$page.component === 'Users'" >Users</NavLink>
      </li>
      <li>
        <NavLink href="/settings" :active="$page.component === 'Settings'" >Settings</NavLink>
      </li>
      <li>
        <Link
          href="/logout"
          method="post"
          :data="{ foo: 'bar' }"
          as="button"
          class="text-black hover:underline"
          >Log out</Link
        >
      </li>
    </ul>
  </nav>
</template>

  <script setup>
import NavLink from "./NavLink"
import { Link } from "@inertiajs/inertia-vue3";
</script>
