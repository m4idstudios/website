<script setup>
useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
  ],
  link: [
    { rel: 'icon', href: '/favicon.ico' }
  ],
  htmlAttrs: {
    lang: 'en'
  }
})

const title = 'M4id Studios'
const description = 'A hobby studio team, bringing minecraft mods and servers, plus other games, with a promised priority of user experience and quality to the best of our ability!'

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  ogImage: 'https://cdn.discordapp.com/attachments/1449244199223431250/1547011014246010990/logo-full.png?ex=6af39ac7&is=6af24947&hm=74ae306f30703031414a33cb90825eb3f5aabeefd019ce5ab2563965860af325&',
  twitterCard: 'summary_large_image'
})
</script>

<template>
  <UApp>
    <UCard class="mc-panel">
      <h1>
        Work In Progress Website
      </h1>

      <p>
        Can't be bothered to make the website, and plus I don't really have anything to put on it anyway. Stay tuned! <3
      </p>
    </UCard>
    <!--    <UHeader>
          <template #left>
            <NuxtLink
              to="/"
              class="focus-visible:outline-3 outline-primary/25 rounded-md p-1 -ms-1"
            >
              <AppLogo class="w-auto h-6 shrink-0" />
            </NuxtLink>

            <TemplateMenu />
          </template>

          <template #right>
            <UColorModeButton />

            <UButton
              to="https://github.com/nuxt-ui-templates/starter"
              target="_blank"
              icon="i-simple-icons-github"
              aria-label="GitHub"
              color="neutral"
              variant="ghost"
            />
          </template>
        </UHeader>-->

    <UMain>
      <NuxtPage />
    </UMain>

<!--    <USeparator class="mc-divider"/>-->

    <UFooter>
      <template #left>
        <p class="text-sm text-muted">
          M4id Studios, All Rights Reserved • © {{ new Date().getFullYear() }}
        </p>
      </template>

      <template #right>
        <p class="text-sm text-muted">
          Made by DoctorM4id • Developed on Nuxt
        </p>
      </template>

<!--      <template #right>
        <UButton
          to="https://github.com/m4idstudios"
          target="_blank"
          icon="i-simple-icons-github"
          aria-label="GitHub"
          color="neutral"
          variant="ghost"
        />
      </template>-->
    </UFooter>
  </UApp>
</template>
