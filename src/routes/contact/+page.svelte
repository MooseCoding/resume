<script>
    import ContactCard from "$lib/main/ContactCard.svelte";
    import { page } from '$app/stores';
</script>

<div class="bg-gradient-to-b from-pink-500 to-pink-700 min-h-screen py-10 px-6 text-white flex flex-col items-center">
    <h1 class="text-6xl font-bold text-pink-200 text-center py-4">Contact Me</h1>

    <ContactCard
        name="Topher Fontana"
        username="MooseCoding"
        title="Starting Fullstack Web Developer, Roboticist"
        email="topherfontana@gmail.com"
        phone="+1 (239) 789-0196"
        github="https://github.com/MooseCoding"
        youtube="https://youtube.com/@moosecoding1221?si=iQxVmvwuftlgzGUO"
        website="{$page.url}"
        cardClass="bg-pink-600 bg-opacity-80 hover:bg-opacity-100 hover:shadow-lg transform hover:scale-105 transition duration-300 ease-in-out text-white rounded-lg p-8 shadow-md max-w-md"
    />
</div>