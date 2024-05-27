<script>
    import { News, HeroBody } from "flowbite-svelte-blocks";
    import { ArrowRightOutline } from "flowbite-svelte-icons";
    import { AccordionItem, Accordion } from "flowbite-svelte";
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from "flowbite-svelte";
    import { Contact } from "flowbite-svelte-blocks";
    import { Label, Input, Textarea, Button } from "flowbite-svelte";
    import { Section, HeroHeader, FeatureDefault, FeatureItem } from "flowbite-svelte-blocks";
    import { ChartPieSolid, LandmarkSolid, BriefcaseSolid, DollarOutline, RocketSolid, CogOutline } from "flowbite-svelte-icons";
</script>

<Navbar>
    <NavBrand href="/">
        <img src="/images/flowbite-svelte-icon-logo.svg" class="me-3 h-6 sm:h-9" alt="Flowbite Logo" />
        <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Flowbite</span>
    </NavBrand>
    <NavHamburger />
    <NavUl>
        <NavLi href="/">Home</NavLi>
        <NavLi href="/about">About</NavLi>
        <NavLi href="/docs/components/navbar">Navbar</NavLi>
        <NavLi href="/pricing">Pricing</NavLi>
        <NavLi href="/contact">Contact</NavLi>
    </NavUl>
</Navbar>

<Section name="heroDefault" sectionClass="max-w-5xl mx-auto min-h-lvh flex justify-center items-center">
    <HeroHeader>
        <svelte:fragment slot="h1">We invest in the world’s potential</svelte:fragment>
        <svelte:fragment slot="paragraph">Here at Flowbite we focus on markets where technology, innovation, and capital can unlock long-term value and drive economic growth.</svelte:fragment>
    </HeroHeader>

    <div class="flex flex-col mb-8 lg:mb-16 space-y-4 sm:flex-row sm:justify-center sm:space-y-0 sm:space-x-4">
        <a href="/">
            <Button size="lg" color="red">
                Learn more <ArrowRightOutline size="md" class="ml-2 -mr-1" />
            </Button>
        </a>
        <a href="/">
            <Button size="lg" color="light">Watch video</Button>
        </a>
    </div>
</Section>

<Section name="feature" sectionClass="max-w-5xl mx-auto min-h-lvh flex justify-center items-center">
    <HeroHeader class="max-w-screen-md mb-8 lg:mb-16" h2Class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white" pClass="text-gray-500 sm:text-xl dark:text-gray-400">
        <svelte:fragment slot="h2">Designed for business teams like yours</svelte:fragment>
        <svelte:fragment slot="paragraph">Here at Flowbite we focus on markets where technology, innovation, and capital can unlock long-term value and drive economic growth.</svelte:fragment>
    </HeroHeader>
    <FeatureDefault>
        <FeatureItem>
            <svelte:fragment slot="icon"><ChartPieSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Marketing</svelte:fragment>
            <svelte:fragment slot="paragraph">Plan it, create it, launch it. Collaborate seamlessly with all the organization and hit your marketing goals every month with our marketing plan.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><LandmarkSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Legal</svelte:fragment>
            <svelte:fragment slot="paragraph">Protect your organization, devices and stay compliant with our structured workflows and custom permissions made for you.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><BriefcaseSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Business Automation</svelte:fragment>
            <svelte:fragment slot="paragraph">Auto-assign tasks, send Slack messages, and much more. Now power up with hundreds of new templates to help you get started.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><DollarOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Finance</svelte:fragment>
            <svelte:fragment slot="paragraph">Audit-proof software built for critical financial operations like month-end close and quarterly budgeting.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><RocketSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Enterprise Design</svelte:fragment>
            <svelte:fragment slot="paragraph">Craft beautiful, delightful experiences for both marketing and product with real cross-company collaboration.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><CogOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Operations</svelte:fragment>
            <svelte:fragment slot="paragraph">Keep your company’s lights on with customizable, iterative, and structured workflows built for all efficient teams and individual.</svelte:fragment>
        </FeatureItem>
    </FeatureDefault>
</Section>

<section class="max-w-5xl mx-auto min-h-lvh flex justify-center items-center gap-5 flex-col">
    <HeroHeader class="mb-8 lg:mb-16" h2Class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white" pClass="text-gray-500 sm:text-xl dark:text-gray-400">
        <svelte:fragment slot="h2">Designed for business teams like yours</svelte:fragment>
        <svelte:fragment slot="paragraph">Here at Flowbite we focus on markets where technology, innovation, and capital can unlock long-term value and drive economic growth.</svelte:fragment>
    </HeroHeader>
    <Accordion class="w-full">
        <AccordionItem>
            <span slot="header">My Header 1</span>
            <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
            <p class="text-gray-500 dark:text-gray-400">
                Check out this guide to learn how to <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> get started </a>
                and start developing websites even faster with components on top of Tailwind CSS.
            </p>
        </AccordionItem>
        <AccordionItem>
            <span slot="header">My Header 2</span>
            <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
            <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
            <p class="mb-2 text-gray-500 dark:text-gray-400">Learn more about these technologies:</p>
            <ul class="list-disc ps-5 dark:text-gray-400 text-gray-500">
                <li>
                    <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> Lorem ipsum </a>
                </li>
                <li>
                    <a href="https://tailwindui.com/" rel="noreferrer" target="_blank" class="text-blue-600 dark:text-blue-500 hover:underline"> Tailwind UI </a>
                </li>
            </ul>
        </AccordionItem>
    </Accordion>
</section>
<Section name="contact" sectionClass="max-w-5xl mx-auto min-h-lvh flex justify-center items-center">
    <Contact>
        <svelte:fragment slot="h2">Contact Us</svelte:fragment>
        <svelte:fragment slot="paragraph">Got a technical issue? Want to send feedback about a beta feature? Need details about our Business plan? Let us know.</svelte:fragment>
        <form class="space-y-8">
            <div>
                <Label for="email" class="block mb-2">Your email</Label>
                <Input id="email" name="email" placeholder="name@flowbite.com" required />
            </div>
            <div>
                <Label for="subject" class="block mb-2">Subject</Label>
                <Input id="subject" name="subject" placeholder="Let us know how we can help you" required />
            </div>
            <div>
                <Textarea id="subject" name="subject" placeholder="Leave a comment..." label="Your message" />
            </div>
            <Button>Send message</Button>
        </form>
    </Contact>
</Section>
