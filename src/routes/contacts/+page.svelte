<script>
  import Profile from '../../components/Profile.svelte';
  import ContactItem from '../../components/ContactItem.svelte';
</script>


<div class="flex flex-col items-center min-h-[100vh] p-6 sm:p-10 bg-slate-950">
  <div class="max-w-md w-full bg-slate-300 rounded-lg shadow-lg">
    <Profile
      name="rkkm"
      title1="DevOps Engineer"
      title2="Java/Kotlin developer"
      imgSrc="../images/avatar1.webp"
    />
    <div class="px-6 py-8 sm:px-10 sm:py-12 space-y-6 bg-slate-400 rounded-b-lg">
      <ContactItem
        iconClass="fa-brands fa-telegram"
        iconColor="text-blue-500"
        text="@realkkm"
        href="https://t.me/realkkm"
      />
      <ContactItem
        iconClass="fa-brands fa-discord"
        iconColor="text-indigo-500"
        text="@rkkm"
        href="https://discord.com/users/346562964729626629"
      />
      <ContactItem
        iconClass="fa-brands fa-twitch"
        iconColor="text-purple-500"
        text="@rkkm_"
        href="https://www.twitch.tv/rkkm_"
      />
      <ContactItem
        iconClass="fa-brands fa-github"
        iconColor="text-gray-700 dark:text-gray-300"
        text="@realkarmakun"
        href="https://github.com/realkarmakun"
      />
    </div>
  </div>
</div>