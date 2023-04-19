<template>
    <div>
      <button class="button">{{ text }}</button>
    </div>
  </template>
  <script>
  export default {
    name: 'Button',
    props: {
      text: {
        type: String,
        required: true,
        default: 'Button',
      },
    },
  };
  </script>
  <style scoped>
  .button {
    background-color: var(--hris-primary-primary);
    border: none;
    border-radius: 8px;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
  }
  .button :hover{
    background-color: var(--hris-primary-hover);
  }
  .button :active{
    background-color: var(--hris-primary-active);
  }
  </style> 