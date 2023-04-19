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
    border-radius: var(--hris-radius-2);
    color: var(--hris-white);
    padding: 15px 32px;
    text-align: center;
    text-decoration: var(--hris-text-decoration-none);
    font-size: var(--hris-text-sm-medium-font-size);
    font-weight: var(--hris-font-weights-kanit-3);
    line-height: var(--hris-text-sm-medium-line-height);
  }
  .button :hover{
    background-color: var(--hris-primary-hover);
  }
  .button :active{
    background-color: var(--hris-primary-active);
  }
  </style> 