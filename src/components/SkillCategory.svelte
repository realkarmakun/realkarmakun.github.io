<!-- SkillCategory.svelte -->
<script>
    import SkillTag from './SkillTag.svelte';
    export let category;
    export let skills = [];
  </script>
  
  <div class="bg-slate-950 p-4 rounded-lg">
    <h4 class="text-xl font-bold mb-2">{category}</h4>
    <div class="flex flex-wrap gap-2 justify-center">
      {#each skills as skill}
        <SkillTag name={skill.name} />
      {/each}
    </div>
  </div>