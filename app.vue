<template>
  <div>
    <FormKit
        type="text"
        label="Username"
        name="username"
        help="Pick a new username"
        validation="required|matches:/^@[a-zA-Z]+$/|length:5"
        value="@useFormkit"
        prefix-icon="avatarMan"
        inner-class="mycustom-inner"
    >
      <template #label="context">
        {{ context.label }}
        ?
        <span>{{ context.help }}</span>
      </template>
      <template #help></template>
    </FormKit>
    <FormKit type="select"/>
    <FormKit type="textarea"/>
  </div>
</template>
