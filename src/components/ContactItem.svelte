<script>
    export let iconClass;
    export let text;
    export let href;
    export let iconColor;
  </script>
  
  <div class="flex items-center space-x-4">
    <i class={`fa-xl ${iconClass} ${iconColor} icon w-6`}></i>
    <a
      class="text-slate-950 dark:text-gray-300 hover:text-gray-900 dark:hover:text-gray-100 transition-colors"
      href={href}
    >
      {text}
    </a>
  </div>
  