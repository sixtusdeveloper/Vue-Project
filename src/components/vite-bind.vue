<!-- Very important notes: -->
<!-- Directives are special tokens in the markup that tell the library to do something to a DOM element. -->
<!-- The v-bind directive is used to bind an attribute to an expression. -->

<template>
    <div>
      <p v-bind:title="message">
        Hover your mouse over me for a few seconds
        to see my dynamically bound title!
      </p>
    </div>
  </template>