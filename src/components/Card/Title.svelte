<script>
  let className = "";
  export {className as class};
  export let hover = true;
  export let title = "";
  export let subheader = "";
  export let avatar = "";

  export let wrapperClasses = "flex px-4 py-2 items-center";
</script>

<div class="{className} {wrapperClasses}">
  <div>
    <img
      class="rounded-full"
      width="44"
      height="44"
      src={avatar}
      alt="avatar"
      class:hidden={!avatar} />
  </div>
  <div class="pl-4 py-2">
    <div class:hidden={!title} class="font-medium text-lg">{title}</div>
    <div class="text-sm text-gray-600 pt-0" class:hidden={!subheader}>
      {subheader}
    </div>
  </div>
</div>
