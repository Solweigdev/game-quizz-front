<template>
<div v-for="person in props.persons">
  <span v-text="person.name"></span>
  <span v-text="person.age"></span>

  <button v-on:click="display('name')">Display Name</button>
  <button v-on:click="display('age')">Display Age</button>
</div>
  <Label>First Name</Label>
  <Input id="firstName"/>
</template>

<script setup lang="ts">
// Types
import type Person from "@/types/person";
import type PersonProperty from "@/types/personType";
// Label
import Label from "@/components/label.vue";
import Input from "@/components/Input.vue";

  const props = defineProps<{
    persons: Person[]
  }>()

  const display = (property: PersonProperty) => {
    props.persons.forEach((person: Person) => {
      console.log(person[property])
    })
  }

</script>
