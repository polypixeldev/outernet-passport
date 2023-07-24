<script>
  const guilds = [
    "🔬 The Lab",
    "🍳 The Cookhouse",
    "🛠️ The Hardware Shack",
    "🥾 Hike Club",
    "📻 The Orpheus Show",
    "☕ Café Orpheus",
    "🎾 Outernet Sports",
    "🥖 Bakery @ Café Orpheus",
    "📞 SussyTel",
    "📶 OuterLAN",
    "🧶 Crochet Club",
    "🎵 Rickrolls & Fun",
    "🔨 Public Works",
    "☁ Outernet Web Services",
    "🎫 Outernet Passport",
    "🕺 Dance Off",
    "✈️ Radio Controlled",
    "⚔️ Dueling",
    "💡 Debates & Trivia",
    "📻 Outernet Radio (W2H)",
    "🌌 Outernet Space Agency",
    "🎬 Film & Movies",
    "🧘‍♀️ Orpheus Legion",
    "🔫 Splash Ops",
    "♻️ Eco-Pioneers",
  ];

  const colors = [
    "red-600",
    "greenish",
    "purple",
    "brownish",
    "lightblue",
    "green",
    "yellow",
  ];

  const fullGuilds = [...guilds, ...guilds, ...guilds, ...guilds];
</script>

<div
  class="fixed -left-20 -top-16 -z-10 flex w-[250%] flex-row flex-wrap items-center justify-start overflow-hidden bg-white blur-sm dark:bg-black md:w-[150%]"
>
  {#each fullGuilds as guild}
    <div class="m-2 rounded-md bg-zinc-100 p-5 dark:bg-neutral-800">
      <p
        class={`text-2xl font-black md:text-3xl lg:text-4xl text-${
          colors[Math.round(Math.random() * (colors.length - 1))]
        }`}
      >
        {guild}
      </p>
    </div>
  {/each}
</div>
<div class="flex h-full w-full flex-col items-center justify-center font-inter">
  <div
    class="mx-3 flex flex-col items-center justify-center rounded-md bg-blue-500 px-3 py-8 text-white shadow-md shadow-black md:px-10 md:py-16"
  >
    <p class="text-center text-xl font-semibold md:text-2xl lg:text-3xl">
      Login to access your Outernet Passport!
    </p>
    <button
      class="mt-10 rounded-md bg-blue-800 p-5 text-lg font-extrabold md:text-xl lg:text-2xl"
      >Login with OuterLAN Identity</button
    >
  </div>
</div>
