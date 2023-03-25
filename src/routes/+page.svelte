<script>
  import { Img, Heading, P } from 'flowbite-svelte';
  import {
    TeamWrapper,
    TeamHeader,
    TeamBody,
    TeamItem,
    Facebook,
    Github,
    Twitter
  } from 'flowbite-svelte-blocks';
	import Helo from '../components/Helo.svelte';
  let members = [
    {
      href: '/',
      src: 'https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/bonnie-green.png',
      alt: 'Bonnie Green',
      name: 'Bonnie Green',
      jobTitle: 'CEO & Web Developer',
      description: 'Bonnie drives the technical strategy of the flowbite platform and brand.'
    },
    {
      href: '/',
      src: 'https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/jese-leos.png',
      alt: 'Jese Leos',
      name: 'Jese Leos',
      jobTitle: 'CTO',
      description: 'Jese drives the technical strategy of the flowbite platform and brand.'
    },
    {
      href: '/',
      src: 'https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/michael-gouch.png',
      alt: 'Michael Gouch',
      name: 'Michael Gouch',
      jobTitle: 'Senior Front-end Developer',
      description: 'Michael drives the technical strategy of the flowbite platform and brand'
    },
    {
      href: '/',
      src: 'https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/sofia-mcguire.png',
      alt: 'Lana Byrd',
      name: 'Lana Byrd',
      jobTitle: 'Marketing & Sale',
      description: 'Lana drives the technical strategy of the flowbite platform and brand.'
    }
  ];
</script>

<Helo />

<main class="lg:px-40">
  <Heading class="p-8" tag="h1" customSize="text-3xl">WikiSafari</Heading>

<P class="px-8 py-4" >
  <p >Testing the typewriter effect</p>

  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
  labore et dolore magna aliqua. Amet cursus sit amet dictum sit. Quis enim lobortis scelerisque
  fermentum dui faucibus in. Mattis vulputate enim nulla aliquet porttitor lacus luctus accumsan.
  Ipsum dolor sit amet consectetur adipiscing elit. Euismod nisi porta lorem mollis aliquam ut
  porttitor. Tortor consequat id porta nibh. Tortor condimentum lacinia quis vel eros donec ac odio.
  Elementum sagittis vitae et leo duis ut diam quam nulla. Vel turpis nunc eget lorem.
</P>
<P class="px-8 py-4">
  Aliquet porttitor lacus luctus accumsan. Ac orci phasellus egestas tellus rutrum tellus. Non odio
  euismod lacinia at quis risus sed. Nam libero justo laoreet sit amet cursus sit amet. Arcu odio ut
  sem nulla pharetra diam sit amet nisl. Vulputate mi sit amet mauris commodo quis imperdiet.
  Malesuada nunc vel risus commodo viverra. Eget nulla facilisi etiam dignissim diam quis enim. Hac
  habitasse platea dictumst quisque. Ultrices gravida dictum fusce ut placerat orci nulla
  pellentesque dignissim.
</P>
<P class="px-8 py-4">
  Nec feugiat in fermentum posuere urna nec tincidunt praesent. Nulla pharetra diam sit amet nisl
  suscipit adipiscing bibendum est. Eu turpis egestas pretium aenean pharetra magna. Ultricies lacus
  sed turpis tincidunt id. Urna nec tincidunt praesent semper feugiat nibh. Aliquam etiam erat velit
  scelerisque in dictum non consectetur. Suspendisse in est ante in nibh mauris cursus mattis
  molestie. Facilisi nullam vehicula ipsum a. Tellus pellentesque eu tincidunt tortor aliquam nulla
  facilisi. Libero justo laoreet sit amet cursus sit amet.
</P>
<P class="px-8 py-4">
  Nec feugiat in fermentum posuere urna nec tincidunt praesent. Nulla pharetra diam sit amet nisl
  suscipit adipiscing bibendum est. Eu turpis egestas pretium aenean pharetra magna. Ultricies lacus
  sed turpis tincidunt id. Urna nec tincidunt praesent semper feugiat nibh. Aliquam etiam erat velit
  scelerisque in dictum non consectetur. Suspendisse in est ante in nibh mauris cursus mattis
  molestie. Facilisi nullam vehicula ipsum a. Tellus pellentesque eu tincidunt tortor aliquam nulla
  facilisi. Libero justo laoreet sit amet cursus sit amet.
</P>
<P class="px-8 py-4">
  Nec feugiat in fermentum posuere urna nec tincidunt praesent. Nulla pharetra diam sit amet nisl
  suscipit adipiscing bibendum est. Eu turpis egestas pretium aenean pharetra magna. Ultricies lacus
  sed turpis tincidunt id. Urna nec tincidunt praesent semper feugiat nibh. Aliquam etiam erat velit
  scelerisque in dictum non consectetur. Suspendisse in est ante in nibh mauris cursus mattis
  molestie. Facilisi nullam vehicula ipsum a. Tellus pellentesque eu tincidunt tortor aliquam nulla
  facilisi. Libero justo laoreet sit amet cursus sit amet.
</P>
<P class="px-8 py-4">
  Nec feugiat in fermentum posuere urna nec tincidunt praesent. Nulla pharetra diam sit amet nisl
  suscipit adipiscing bibendum est. Eu turpis egestas pretium aenean pharetra magna. Ultricies lacus
  sed turpis tincidunt id. Urna nec tincidunt praesent semper feugiat nibh. Aliquam etiam erat velit
  scelerisque in dictum non consectetur. Suspendisse in est ante in nibh mauris cursus mattis
  molestie. Facilisi nullam vehicula ipsum a. Tellus pellentesque eu tincidunt tortor aliquam nulla
  facilisi. Libero justo laoreet sit amet cursus sit amet.
</P>

<TeamWrapper>
  <TeamHeader>
    <svelte:fragment slot="label">Our Team</svelte:fragment>
    <p class="font-light text-gray-500 lg:mb-16 sm:text-xl dark:text-gray-400">
      Explore the whole collection of open-source web components and elements built with the
      utility classes from Tailwind
    </p>
  </TeamHeader>
  <TeamBody>
    {#each members as { href, src, alt, name, jobTitle, description }}
      <TeamItem {href} {src} {alt} {name} {jobTitle}>
        <p class="mt-3 mb-4 font-light text-gray-500 dark:text-gray-400">
          {description}
        </p>
        <svelte:fragment slot="social">
          <Facebook href="/" />
          <Github href="/" />
          <Twitter href="/" />
        </svelte:fragment>
      </TeamItem>
    {/each}
  </TeamBody>
</TeamWrapper>

</main>