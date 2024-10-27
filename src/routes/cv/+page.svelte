<script>
  import SkillCategory from '../../components/SkillCategory.svelte';

  let skillCategories = [
    {
      category: "Platforms",
      skills: [
        { name: "Linux" },
        { name: "SSH" },
        { name: "Ansible" },
        { name: "Docker" },
        { name: "Kubernetes" },
        { name: "Helm" }
      ]
    },
    {
      category: "Software",
      skills: [
        { name: "nginx" },
        { name: "PosgreSQL" },
        { name: "MYSQL (MariaDB)" },
        { name: "Redis" },
        { name: "git" },
        { name: "ClickHouse" },
        { name: "Kafka" }
      ]
    },
    {
      category: "CI/CD",
      skills: [
        { name: "Gitlab CI/CD" },
        { name: "Github Actions" },
        { name: "Prometheus" },
        { name: "Grafana" },
        { name: "Loki" },
        { name: "SigNoz" },
        { name: "InfluxDB" },
        { name: "telegraf" }
      ]
    },
    {
      category: "Languages",
      skills: [
        { name: "Java" },
        { name: "Kotlin" },
        { name: "Python" },
        { name: "JavaScript" }
      ]
    }
  ];
</script>

 <div class="max-w-4xl mx-auto p-4">
    <!-- Header -->
    <header class="flex items-center justify-between">
      <div>
        <h1 class="text-4xl font-bold">Pavel Konstantinov</h1>
        <h2 class="text-xl">DevOps Engineer, Java/Kotlin developer</h2>
        <h2 class="text-xl">Residence: Omsk, Russia, UTC+6</h2>
      </div>
      <img src={"../images/avatar1.webp"} alt="Profile" class="w-32 h-32 rounded-full object-cover"/>
    </header>
  
    <!-- Experience -->
    <section class="mt-8">
      <h3 class="text-2xl font-semibold">Experience</h3>
      <ol class="mt-2 relative border-s border-gray-200 dark:border-gray-700">            
        <li class="mb-10 ms-4">
            <div class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"></div>
            <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Since February 2020 to August 2024</time>
            <h3 class="text-lg font-semibold dark:text-white">DevOps-engineer at RustMe</h3>
            <p class="mb-4 text-base font-normal text-gray-200 dark:text-gray-400">My responsobilites are creating and maintaining critical infrastructure for <strong class="text-violet-400">game servers</strong> as well as for development critical resources. Basicly monitoring, setting up new servers, networking, handling CI/CD and any kind of automation.</p>
            <a href="https://rustme.net" class="inline-flex items-center px-4 py-2 text-sm font-medium text-gray-900 bg-white border border-gray-200 rounded-lg hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:outline-none focus:ring-gray-100 focus:text-blue-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700 dark:focus:ring-gray-700">Check the server out, it's pretty cool &rarr;</a>
        </li>
        <li class="mb-10 ms-4">
          <div class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"></div>
          <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Since August 2024 to Now</time>
          <h3 class="text-lg font-semibold dark:text-white">DevOps-engineer at Raffeisein Bank</h3>
      </li>
    </ol>
    </section>
    <!-- Education -->
    <section class="mt-8">
      <h3 class="text-2xl font-semibold">Education</h3>
      <div class="mt-2">
        <h4 class="text-xl font-medium">Dostoevsky Omsk State University, Russia</h4>
        <p>2018 - 2024 | Computer Security Specialist Degree</p>
      </div>
    </section>
  
    <section class="mt-8">
      <h3 class="text-2xl font-semibold">Skills</h3>
      <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 mt-4 text-center">
        {#each skillCategories as { category, skills }}
          <SkillCategory {category} {skills} />
        {/each}
      </div>
    </section>
  </div>

