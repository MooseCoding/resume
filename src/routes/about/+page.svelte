<script>
	function monthsSince(date) {
  const now = new Date();
  const startDate = new Date(date);
  
  // Calculate the difference in months
  let months = (now.getFullYear() - startDate.getFullYear()) * 12;
  months += now.getMonth() - startDate.getMonth();

  return months;
}

let mType = monthsSince('2024-06-01');
let mC = monthsSince('2022-08-01');
let mCpp = monthsSince('2023-09-01');
let mJ = monthsSince('2023-08-16'); 
let mP = monthsSince('2021-02-11'); 
let mS = monthsSince('2024-9-30');

</script>

<div class="bg-gradient-to-b from-blue-900 to-gray-800 text-white min-h-screen flex flex-col items-center py-8 px-4">
    <div class="text-center space-y-6">
        <h1 class="text-4xl font-bold text-blue-300">About Me</h1>
        <p class="text-lg text-gray-300">I'm Topher (aka MooseCoding), a roboticist and starting to venture into web development.</p>
        <h2 class="text-2xl font-semibold text-blue-300 mt-8">Some of my programming language knowledge</h2>
        <ul class="text-lg text-gray-200 space-y-2">
            <li>TypeScript: {mType} months</li>
            <li>C: {mC} months</li>
            <li>C++: {mCpp} months</li>
            <li>Java: {mJ} months</li>
            <li>Python: {mP} months</li>
            <li>Svelte: {mS} months</li>
        </ul>
    </div>
</div>