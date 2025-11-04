<script setup lang="ts">
const cards = ref([
    {
    title: 'Red Dead Redemption 2',
    description: 'Red Dead Redemption 2 (RDR2) is an action-adventure game set in an open-world representation of the American West in 1899, focusing on outlaw Arthur Morgan and the Van der Linde gang.',
    icon: "i-material-symbols-award-star-outline-rounded",
    image: {
      path: '/Rdr2.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Dying Light 2: Stay Human',
    icon: "i-material-symbols-award-star-outline-rounded",
    description: 'Dying Light 2: Stay Human is a first-person action RPG set in a post-apocalyptic open world where players navigate a city overrun by zombies and hostile factions.',
    image: {
      path: '/DyingLight2.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Dying Light 1',
    description: 'Dying Light is a first-person action survival game set in a zombie-infested, open-world city called Harran.',
    image: {
      path: '/DyingLight1.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Horizon: Forbidden West',
    description: 'Horizon Forbidden West is an action RPG set in a post-apocalyptic America where the player controls the protagonist Aloy as she journeys to a dangerous region known as the Forbidden West to confront new threats.',
    image: {
      path: '/HorizonForbiddenWest.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Horizon: Zero Dawn',
    icon: "i-material-symbols-award-star-outline-rounded",
    description: 'Horizon Zero Dawn is an action role-playing game set in a post-apocalyptic world where humanity has regressed to tribal societies and giant, animalistic machines roam the land.',
    image: {
      path: '/HorizonZeroDawn.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Days Gone',
    description: 'Days Gone is an action-adventure survival-horror game where players control Deacon St. John, a former outlaw and now a drifter and bounty hunter, in a post-apocalyptic open world.',
    image: {
      path: '/DaysGone.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Last Of Us: Part 2',
    description: 'The Last of Us Part II is an action-adventure game developed by Naughty Dog that continues the story of The Last of Us.',
    image: {
      path: '/LastOfUs2.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Last Of Us: Part 1',
    description: 'The Last of Us Part I is a remake of the 2013 action-adventure game where a smuggler named Joel is tasked with escorting a teenage girl, Ellie, across a post-apocalyptic United States.',
    image: {
      path: '/LastOfUs1.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Ghost Of Tsushima',
    description: 'Ghost of Tsushima is an action-adventure video game where players control Jin Sakai, a samurai fighting to protect the island of Tsushima during the 1274 Mongol invasion of Japan. ',
    image: {
      path: '/GhostOfTsushima.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Severed Steel',
    icon: "i-material-symbols-award-star-outline-rounded",
    description: 'Severed Steel is a fast-paced, single-player first-person shooter (FPS) with a focus on fluid movement, destructible environments, and a "bullet time" mechanic.',
    image: {
      path: '/SeveredSteel.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'PUBG: BattleGrounds',
    description: 'PUBG: Battlegrounds is a player-vs-player battle royale shooter where up to 100 players parachute onto a large map, scavenging for weapons and gear to fight until only one player or team remains.',
    image: {
      path: '/PUBG.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Counter Strike 2',
    description: 'CS2, or Counter-Strike 2, is a free-to-play, multiplayer tactical first-person shooter developed by Valve, replacing Global Offensive on the Source 2 engine.',
    image: {
      path: '/CS2.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Fall Guys: Ultimate Knockout',
    description: 'Fall Guys is a free-to-play, massively multiplayer party royale game where up to 32 players compete in a series of chaotic obstacle courses and mini-games until only one remains. ',
    image: {
      path: '/FG.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Contraband Police',
    description: 'Contraband Police" is a game where players act as a border guard in a fictional 1980s communist country called Acaristan.',
    image: {
      path: '/ContrabandPolice.jpg',
      width: 363,
      height: 152
    }
  },
  {
    title: 'Palworld',
    description: 'Palworld is a multiplayer, open-world survival crafting game where players collect and befriend creatures called "Pals" to use for various tasks.',
    image: {
      path: '/Palworld.jpg',
      width: 363,
      height: 152
    }
  },
])
</script>

<template>
<UContainer>
  <UPageGrid>
    <UPageCard
      v-for="(card, index) in cards"
      :key="index"
      v-bind="card"
    >
      <UColorModeImage
        v-if="card.image"
        :light="`${card.image.path}`"
        :dark="`${card.image.path}`"
        :width="card.image.width"
        :height="card.image.height"
        :alt="card.title"
        loading="lazy"
        class="w-full"
      />
    </UPageCard>
  </UPageGrid>
</UContainer>
</template>

