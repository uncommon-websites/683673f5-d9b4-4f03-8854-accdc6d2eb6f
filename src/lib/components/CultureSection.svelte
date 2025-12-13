<script lang="ts">
  const cards = [
    {
      title: "Fair Competition",
      subtitle: "Every Match Matters",
      image: "/generated/image-padel-doubles-match-with-evenly-matched--1765587976476-5.webp"
    },
    {
      title: "Community First",
      subtitle: "Build Lasting Connections",
      image: "/generated/image-group-of-diverse-padel-players-of-differ-1765587973965-4.webp"
    },
    {
      title: "Professional Events",
      subtitle: "Tournament-Ready Platform",
      image: "/generated/image-padel-tournament-event-with-multiple-cou-1765587979103-6.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      More than just tournament software—SocialPadel creates competitive ecosystems where every player finds their level, every match is balanced, and every club builds a thriving community.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>→</span>
           <span>Engage</span>
        </div>
      </div>
    {/each}
  </div>
</section>
