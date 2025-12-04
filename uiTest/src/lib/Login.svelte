<script lang="ts">
  import { FloatingLabelInput, Button } from "flowbite-svelte";
  let size = $state("1.25rem");
</script>

<div
  class="flex flex-col justify-center items-center w-full h-screen dark:bg-gray-900"
>
  <div class="w-75 p-3">
    <p class="text-3xl font-bold text-center mb-5 dark:text-white">Log in</p>
    <form class="flex flex-col gap-4" action="/">
      <FloatingLabelInput
        variant="outlined"
        name="username"
        id="username"
        type="text">Username</FloatingLabelInput
      >
      <FloatingLabelInput
        variant="outlined"
        name="password"
        id="password"
        type="passsword">Password</FloatingLabelInput
      >
      <a href="#" class="base text-primary-500">Froget Password ?</a>
      <Button type="submit">Continue</Button>
    </form>
    <div class="flex flex-row gap-3 justify-center items-center my-4">
      <hr class="w-25 text-gray-400" />
      <p class="small px-2 text-gray-400">or</p>
      <hr class="w-25 text-gray-400" />
    </div>
    <Button color="light" class="w-full mb-5"
      ><iconify-icon
        icon="flat-color-icons:google"
        width={size}
        height={size}
        class="me-3"
      ></iconify-icon>Login With Google</Button
    >
    <Button color="light" class="w-full mb-2"
      ><iconify-icon
        icon="fluent:fingerprint-16-regular"
        width={size}
        height={size}
        class="me-3"
      ></iconify-icon>Login with Credentials</Button
    >
  </div>
  <p class="base text-gray-400">
    Don't Have An Account? <a href="#" class="text-primary-500">Create One</a>
  </p>
</div>
