<script>
    export let name;
    export let title1;
    export let title2;
    export let imgSrc;
  </script>
  
  <div class="flex flex-col items-center bg-slate-900 dark:bg-gray-700 px-6 py-8 sm:px-10 sm:py-12 rounded-t-lg">
    <img
      alt={name}
      class="rounded-full mb-4"
      height={96}
      src={imgSrc}
      style={{
        aspectRatio: "96/96",
        objectFit: "cover",
      }}
      width={96}
    />
    <h1 class="fira text-2xl font-semibold text-gray-100 mb-2">
      <span class="fira text-violet-400">{name}</span>_
    </h1>
    <p class="fira text-gray-300 text-sm">{title1}</p>
    <p class="fira text-gray-300 text-sm">{title2}</p>
  </div>
  