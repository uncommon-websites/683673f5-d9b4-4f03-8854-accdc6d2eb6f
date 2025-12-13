<script lang="ts">
  const photos = [
    {
      title: "Real-Time Rankings",
      desc: "Watch your ranking evolve with every match. Our ELO system provides instant feedback and motivates continuous improvement.",
      img: "/generated/image-padel-players-celebrating-after-winning--1765587968881-2.webp"
    },
    {
      title: "Seamless Organization",
      desc: "Club managers get powerful tools to schedule, manage, and track tournaments without the administrative headache.",
      img: "/generated/image-close-up-of-padel-racket-and-ball-on-cou-1765587981751-7.webp"
    },
    {
      title: "Community Growth",
      desc: "Transform casual players into engaged community members with competitive structure that keeps them coming back.",
      img: "/generated/image-padel-tennis-players-competing-in-an-int-1765587963093-0.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">Built for club managers. Loved by players.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      SocialPadel solves the unbalanced match problem that plagues recreational padel. Our intelligent ranking system ensures fair competition while our flexible tournament formats keep your community engaged and growing.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
