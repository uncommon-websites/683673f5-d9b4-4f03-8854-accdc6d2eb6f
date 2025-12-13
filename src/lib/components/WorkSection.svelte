<script lang="ts">
  const features = [
    {
      title: "Hybrid ELO Ranking",
      desc: "Sophisticated MMR/ELO system that learns from actual gameplay, even for players with zero match history.",
      bg: "bg-black",
      img: "/generated/image-padel-players-celebrating-after-winning--1765587968881-2.webp",
      dark: true
    },
    {
      title: "Tournament Management",
      desc: "Run single elimination, double elimination, Swiss system, or hybrid formats with ease.",
      bg: "bg-gray-100",
      img: "/generated/image-padel-tournament-bracket-display-on-a-sc-1765587966308-1.webp",
      dark: false
    },
    {
      title: "Club Dashboard",
      desc: "Manage members, track engagement, and organize recurring tournaments from one central hub.",
      bg: "bg-white",
      img: "/generated/image-padel-club-manager-working-on-tablet-at--1765587971396-3.webp",
      dark: false
    },
    {
      title: "Balanced Matches",
      desc: "Solve the level mismatch problem with intelligent player pairing based on real performance data.",
      bg: "bg-gray-900",
      img: "/generated/image-padel-doubles-match-with-evenly-matched--1765587976476-5.webp",
      dark: true
    },
    {
      title: "Community Building",
      desc: "Create sticky, long-term communities with recurring engagement, not just one-off events.",
      bg: "bg-gray-50",
      img: "/generated/image-group-of-diverse-padel-players-of-differ-1765587973965-4.webp",
      dark: false,
      full: true
    },
    {
      title: "Brand Partnerships",
      desc: "Enable sponsor integration and brand activations at your events with built-in marketing tools.",
      bg: "bg-white",
      img: "/generated/image-padel-tournament-event-with-multiple-cou-1765587979103-6.webp",
      dark: false
    },
    {
      title: "Real-Time Updates",
      desc: "Players and spectators stay informed with live tournament brackets and match notifications.",
      bg: "bg-gray-100",
      img: "/generated/image-padel-tennis-players-competing-in-an-int-1765587963093-0.webp",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">The most versatile tournament platform in padel.</span> Combining social play with sophisticated competitive ranking to keep your community engaged and coming back.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each features as feature}
      <div class="group cursor-pointer {feature.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${feature.bg} mb-4 ${feature.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if feature.img}
             <img src={feature.img} alt={feature.title} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${feature.dark ? 'text-white' : 'text-black'}`}>{feature.title}</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{feature.title}</h3>
        <p class="text-sm text-gray-600">{feature.desc}</p>
      </div>
    {/each}
  </div>
</section>
