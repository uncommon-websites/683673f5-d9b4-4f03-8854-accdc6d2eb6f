<script lang="ts">
  const stats = [
    {
      label: "$2B Market",
      desc: "Starting with padel clubs, SocialPadel captures the massive $2 billion racquet sports market. Our dynamic ELO ranking and hybrid tournament formats position us to scale across the entire competitive recreational sports ecosystem.",
      img: "/generated/image-padel-tournament-event-with-multiple-cou-1765587979103-6.webp"
    },
    {
      label: "4 Tournament Formats",
      desc: "The most versatile tournament platform in padel. Support for single elimination, double elimination, Swiss system, and hybrid formats (Swiss rounds + playoffs). No other platform offers this flexibility.",
      img: "/generated/image-padel-tournament-bracket-display-on-a-sc-1765587966308-1.webp"
    },
    {
      label: "AI-Powered Development",
      desc: "Built with cutting-edge AI assistance, our sophisticated backend handles complex ELO calculations and tournament logistics. The system learns and adapts, providing accurate rankings even for players with zero match history.",
      img: "/generated/image-padel-club-manager-working-on-tablet-at--1765587971396-3.webp"
    },
    {
      label: "Club-First Approach",
      desc: "Designed for recurring engagement, not one-off events. Our club-focused model builds sticky, long-term communities with multiple revenue streams: subscriptions, event fees, and brand partnerships.",
      img: "/generated/image-group-of-diverse-padel-players-of-differ-1765587973965-4.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      The numbers behind SocialPadel. Market opportunity, technical capabilities, and competitive advantages.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
