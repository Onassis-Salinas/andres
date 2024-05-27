<script>
    import { ArrowRightOutline } from "flowbite-svelte-icons";
    import { AccordionItem, Accordion } from "flowbite-svelte";
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from "flowbite-svelte";
    import { Contact } from "flowbite-svelte-blocks";
    import { Label, Input, Textarea, Button } from "flowbite-svelte";
    import { Section, HeroHeader, FeatureDefault, FeatureItem } from "flowbite-svelte-blocks";
    import { ChartPieSolid, LandmarkSolid, BriefcaseSolid, DollarOutline, RocketSolid, CogOutline } from "flowbite-svelte-icons";

    let name = "";
    let message = "";
</script>

<Navbar>
    <NavBrand href="/">
        <!-- <img src="/images/flowbite-svelte-icon-logo.svg" class="me-3 h-6 sm:h-9" alt="Flowbite Logo" /> -->
        <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">PET EAT</span>
    </NavBrand>
    <NavHamburger />
    <NavUl>
        <NavLi href="#">Inicio</NavLi>
        <NavLi href="#about">Acerca de</NavLi>
        <NavLi href="#faqs">FAQs</NavLi>
        <NavLi href="#contacto">Contacto</NavLi>
    </NavUl>
</Navbar>

<Section name="heroDefault" sectionClass="max-w-5xl mx-auto min-h-lvh flex justify-center items-center">
    <HeroHeader>
        <svelte:fragment slot="h1">Nutrición de primera pata</svelte:fragment>
        <svelte:fragment slot="paragraph">En PET EAT nos dedicamos a ofrecer a tus queridas mascotas una nutrición excepcional, elaborada con ingredientes de la más alta calidad y diseñada para promover su salud y bienestar en cada etapa de sus vidas.</svelte:fragment>
    </HeroHeader>

    <div class="flex flex-col mb-8 lg:mb-16 space-y-4 sm:flex-row sm:justify-center sm:space-y-0 sm:space-x-4">
        <a href="#about">
            <Button size="lg" color="red">
                Conocer mas <ArrowRightOutline size="md" class="ml-2 -mr-1" />
            </Button>
        </a>
        <a href="#contacto">
            <Button size="lg" color="light">Contactanos</Button>
        </a>
    </div>
</Section>

<div id="about"></div>

<Section name="feature" sectionClass="max-w-5xl mx-auto min-h-lvh flex justify-center items-center">
    <HeroHeader class="max-w-screen-md mb-8 lg:mb-16" h2Class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white" pClass="text-gray-500 sm:text-xl dark:text-gray-400">
        <svelte:fragment slot="h2">Nutrición personalizada para tus mascotas</svelte:fragment>
        <svelte:fragment slot="paragraph">En Pet Eat, nuestro objetivo es proporcionar alimentos saludables y de calidad humana para las mascotas en México. Realizamos evaluaciones individuales para determinar las porciones exactas y el tipo de alimento adecuado para tu mascota, considerando su peso, tamaño y edad.</svelte:fragment>
    </HeroHeader>
    <FeatureDefault>
        <FeatureItem>
            <svelte:fragment slot="icon"><ChartPieSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Personalización</svelte:fragment>
            <svelte:fragment slot="paragraph">Adaptamos las cantidades y tipo de alimento según las necesidades específicas de tu mascota, garantizando una nutrición óptima.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><ChartPieSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Calidad</svelte:fragment>
            <svelte:fragment slot="paragraph">Nuestro compromiso es ofrecer alimentos para mascotas con estándares de calidad equiparables a los alimentos para consumo humano, utilizando ingredientes frescos y de alta calidad.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><ChartPieSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Salud</svelte:fragment>
            <svelte:fragment slot="paragraph">Promovemos una alimentación saludable para las mascotas, con atención veterinaria especializada y guía nutricional.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><ChartPieSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Entregas a domicilio</svelte:fragment>
            <svelte:fragment slot="paragraph">Facilitamos tu vida con entregas a domicilio de alimentos frescos y empacados de forma segura, según tu frecuencia de compra.</svelte:fragment>
        </FeatureItem>
        <FeatureItem>
            <svelte:fragment slot="icon"><ChartPieSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
            <svelte:fragment slot="h3">Precios flexibles</svelte:fragment>
            <svelte:fragment slot="paragraph">Ofrecemos precios variables según las características del alimento, asegurando opciones accesibles para todos.</svelte:fragment>
        </FeatureItem>
    </FeatureDefault>
</Section>

<div id="faqs"></div>

<section class="max-w-5xl mx-auto min-h-lvh flex justify-center items-center gap-5 flex-col">
    <HeroHeader class="mb-8 lg:mb-16" h2Class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white" pClass="text-gray-500 sm:text-xl dark:text-gray-400">
        <svelte:fragment slot="h2">Preguntas Frecuentes</svelte:fragment>
        <svelte:fragment slot="paragraph">Aquí encontrarás respuestas a las preguntas más comunes sobre Pet Eat y nuestros productos.</svelte:fragment>
    </HeroHeader>
    <Accordion class="w-full">
        <AccordionItem>
            <span slot="header">¿Cómo funciona la evaluación de la cantidad de alimento?</span>
            <p class="mb-2 text-gray-500 dark:text-gray-400">En Pet Eat realizamos una evaluación personalizada de tu mascota, teniendo en cuenta su peso, tamaño y edad para determinar las porciones adecuadas de alimento que necesita consumir diariamente.</p>
        </AccordionItem>
        <AccordionItem>
            <span slot="header">¿Qué tipo de ingredientes utilizan en sus alimentos?</span>
            <p class="mb-2 text-gray-500 dark:text-gray-400">Nuestros alimentos están elaborados con ingredientes de calidad humana, frescos y de alta calidad, garantizando una nutrición óptima para tu mascota.</p>
        </AccordionItem>
        <AccordionItem>
            <span slot="header">¿Cuál es la frecuencia de las entregas a domicilio?</span>
            <p class="mb-2 text-gray-500 dark:text-gray-400">La frecuencia de las entregas a domicilio puede ser semanal, quincenal o mensual, según tus preferencias. La opción mensual es la más recomendada.</p>
        </AccordionItem>
        <AccordionItem>
            <span slot="header">¿Ofrecen atención veterinaria especializada?</span>
            <p class="mb-2 text-gray-500 dark:text-gray-400">Sí, en Pet Eat contamos con atención veterinaria especializada para brindarte asesoramiento y cuidados adicionales para tu mascota.</p>
        </AccordionItem>
        <AccordionItem>
            <span slot="header">¿Cómo puedo empezar a comprar sus productos?</span>
            <p class="mb-2 text-gray-500 dark:text-gray-400">Puedes comenzar a comprar nuestros productos simplemente seleccionando los alimentos deseados y realizando tu pedido en nuestra página web. ¡Es fácil y conveniente!</p>
        </AccordionItem>
    </Accordion>
</section>

<div id="contacto"></div>
<Section id="contacto" name="contact" sectionClass="max-w-5xl mx-auto min-h-lvh flex justify-center items-center">
    <Contact>
        <svelte:fragment slot="h2">Contactanos</svelte:fragment>
        <svelte:fragment slot="paragraph">¿Listo para darle a tu mascota la alimentación que se merece? Contáctanos ahora para realizar tu pedido.</svelte:fragment>
        <form class="space-y-8">
            <div>
                <Label for="subject" class="block mb-2">Tu nombre</Label>
                <Input  bind:value={name} id="subject" name="subject" placeholder="" required />
            </div>
            <div>
                <Textarea bind:value={message} id="subject" name="subject" placeholder="Tu mensaje..." label="Your message" />
            </div>
            <a href={`mailto:bladimir.leyva@uabc.edu.mx?subject=Mensaje de ${name}&body=${message}`}>
                <Button>Mandar correo</Button>
            </a>
            <a href={`https://wa.me/526645613973?text=Mensaje de: ${name} -- ${message}`}>
                <Button>Mandar whatsapp</Button>
            </a>
        </form>
    </Contact>
</Section>
