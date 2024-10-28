<script>
    import ProjectCard from '$lib/main/ProjectCard.svelte';
</script>

<div class="bg-gradient-to-b from-purple-900 to-gray-700 min-h-screen py-10 px-6 text-white">
    <h1 class="text-6xl font-bold text-purple-200 text-center py-4">Notable Projects</h1>

    <div class="flex flex-col items-center space-y-8">
        <ProjectCard 
            title="Congressional App Challenge"
            description="3 teammates and I made a fullstack web application that tracks crucial weather alerts, provides a forum, has a learning aspect through a game and more. It was made using NextJS (React), Deno, and SQLite. Click the card for the YouTube video."
            cardClass="bg-purple-500 hover:bg-purple-600 hover:shadow-lg transform hover:scale-105 transition duration-300 ease-in-out text-white rounded-lg p-6 shadow-md max-w-md"
            url="https://youtu.be/ZIquQqs5_bw?si=-Q-deeWhU0SU_hMk"
        />

        <ProjectCard 
            title="jEdison Knights Robot Captain"
            description="I was the robot captain for my FIRST Tech Challenge team. I was mostly involved with the programming side and was our coding expert for most of my first 2 years. I also did CAD and assembly, and contributed to the notebook and portfolio that showcase our team and our community involvement. Click to access our LinkTree!"
            cardClass="bg-purple-500 hover:bg-purple-600 hover:shadow-lg transform hover:scale-105 transition duration-300 ease-in-out text-white rounded-lg p-6 shadow-md max-w-md"
            url="https://linktr.ee/jedisonknights23571?utm_source=linktree_profile_share&ltsid=78f1c401-3bdb-442f-87e4-1e7a05bee428"
        />
    </div>
</div>