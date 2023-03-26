<script>
  import { Img, Heading, P } from 'flowbite-svelte';
  import { News, HeroHeader, HeroBody } from 'flowbite-svelte-blocks';
  import { Button } from 'flowbite-svelte';
  import { ArrowRight, VideoCamera } from 'svelte-heros';
</script>

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


<div class="mr-auto place-self-center lg:col-span-7">
  <HeroHeader
    h1Class="max-w-2xl mb-4 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl dark:text-white"
    pClass="max-w-2xl mb-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400"
  >
    <svelte:fragment slot="h1">Payments tool for software companies</svelte:fragment>
    <svelte:fragment slot="paragraph">
      From checkout to global sales tax compliance, companies around the world use Flowbite to
      simplify their payment stack.
    </svelte:fragment>
    <a href="/"
      ><button size="xl" color="red" class="inline-flex items-center justify-center mr-3">
        Get started<ArrowRight size="18" class="ml-2 -mr-1" />
      </button>
    </a>
    <a href="/"
      ><button color="light" size="xl" class="inline-flex items-center justify-center">
        Speak to Sales
      </button>
    </a>
  </HeroHeader>
</div>
<div class="hidden lg:mt-0 lg:col-span-5 lg:flex">
  <img
    src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/hero/phone-mockup.png"
    alt="mockup"
  />
</div>


</main>