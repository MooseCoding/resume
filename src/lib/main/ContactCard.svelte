<script>
    export let name = "Your Name";
    export let username = "Username";
    export let title = "Your Title"; // e.g., "Software Engineer"
    export let email = "your.email@example.com";
    export let phone = "+123 456 7890";
    export let linkedin = "";
    export let github = "https://github.com/yourusername";
    export let youtube = "https://youtube.com/yourusername";
    export let website = "https://yourwebsite.com";
  </script>
  
  <div class="bg-pink-400 p-6 rounded-lg shadow-lg max-w-xs mx-auto text-center space-y-4">
    <h2 class="text-2xl font-bold text-gray-800">{name}</h2>
    <h3 class="text-xl text-gray-900">{username}</h3>
    <p class="text-gray-900">{title}</p>
  
    <div class="flex flex-col items-center space-y-2">
      <a href={`mailto:${email}`} class="text-gray-800 hover:text-blue-500">
        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="w-5 h-5 inline mr-2" viewBox="0 0 24 24">
          <path d="M12 13.065l-11-7.065h22l-11 7.065zm11-8.065h-22v16h22v-16z"/>
        </svg>
        {email}
      </a>
  
      <a href={`tel:${phone}`} class="text-gray-800 hover:text-green-500">
        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="w-5 h-5 inline mr-2" viewBox="0 0 24 24">
          <path d="M17.707 16.293l-2.121 2.121c-.293.293-.678.439-1.061.439s-.768-.146-1.061-.439l-1.414-1.414c-1.171-.195-2.343-.488-3.486-1.03s-2.091-1.397-3.071-2.377-1.751-2.006-2.377-3.071c-.543-1.144-.835-2.315-1.03-3.486l-1.414-1.414c-.293-.293-.439-.678-.439-1.061s.146-.768.439-1.061l2.121-2.121c.586-.586 1.535-.586 2.121 0l2.121 2.121c.586.586.586 1.535 0 2.121l-1.414 1.414c.151.806.383 1.603.707 2.378s.812 1.518 1.374 2.08 1.314 1.046 2.08 1.374c.775.324 1.572.556 2.378.707l1.414-1.414c.586-.586 1.535-.586 2.121 0l2.121 2.121c.586.586.586 1.535 0 2.121z"/>
        </svg>
        {phone}
      </a>
    </div>
  
    <div class="flex justify-center space-x-4">
      {#if linkedin}
        <a href={linkedin} target="_blank" rel="noopener noreferrer" class="text-blue-700 hover:text-blue-900">
          <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="w-6 h-6" viewBox="0 0 24 24">
            <path d="M19 3h-14c-1.104 0-2 .896-2 2v14c0 1.104.896 2 2 2h14c1.104 0 2-.896 2-2v-14c0-1.104-.896-2-2-2zm-11 14h-2v-8h2v8zm-1-9c-.553 0-1-.447-1-1s.447-1 1-1 1 .447 1 1-.447 1-1 1zm10 9h-2v-4c0-1.105-.895-2-2-2s-2 .895-2 2v4h-2v-8h2v1.025c.586-.769 1.445-1.025 2.5-1.025 2.207 0 3.5 1.343 3.5 3v5z"/>
          </svg>
        </a>
      {/if}
  
      {#if github}
        <a href={github} target="_blank" rel="noopener noreferrer" class="text-gray-800 hover:text-gray-600">
          <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="w-6 h-6" viewBox="0 0 24 24">
            <path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.387.6.113.82-.258.82-.577v-2.17c-3.338.724-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.757-1.333-1.757-1.087-.744.083-.729.083-.729 1.205.085 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.304 3.495.997.108-.776.418-1.304.76-1.604-2.665-.3-5.467-1.334-5.467-5.931 0-1.312.469-2.381 1.236-3.22-.124-.302-.536-1.521.116-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.984-.398 3.006-.403 1.022.005 2.049.137 3.006.403 2.293-1.552 3.299-1.23 3.299-1.23.653 1.655.242 2.874.118 3.176.77.839 1.236 1.908 1.236 3.22 0 4.61-2.807 5.625-5.479 5.921.43.37.823 1.102.823 2.222v3.293c0 .322.216.694.825.576 4.765-1.587 8.2-6.084 8.2-11.387 0-6.627-5.373-12-12-12z"/>
          </svg>
        </a>
      {/if}
  
    {#if youtube}
      <a href={youtube} target="_blank" rel="noopener noreferrer" class="text-red-600 hover:text-red-800">
        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="w-6 h-6" viewBox="0 0 24 24">
          <path d="M23.498 6.186c-.336-1.25-1.317-2.207-2.538-2.436-2.054-.338-10.254-.338-10.254-.338s-8.196 0-10.254.338c-1.221.229-2.202 1.186-2.538 2.436C.002 7.472 0 12 0 12s.002 4.528.707 5.814c.336 1.25 1.317 2.207 2.538 2.436 2.054.338 10.254.338 10.254.338s8.2 0 10.254-.338c1.221-.229 2.202-1.186 2.538-2.436C24 16.528 24 12 24 12s-.002-4.528-.502-5.814zm-14.831 7.166v-6.386l6.182 3.193-6.182 3.193z"/>
        </svg>
      </a>
    {/if}
  
      {#if website}
        <a href={website} target="_blank" rel="noopener noreferrer" class="text-gray-700 hover:text-gray-900">
          <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="w-6 h-6" viewBox="0 0 24 24">
            <path d="M12 0c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm0 22c-5.514 0-10-4.486-10-10s4.486-10 10-10 10 4.486 10 10-4.486 10-10 10zm0-18c-4.411 0-8 3.589-8 8 0 4.411 3.589 8 8 8s8-3.589 8-8c0-4.411-3.589-8-8-8zm1 13h-2v-6h2v6zm0-8h-2v-2h2v2z"/>
          </svg>
        </a>
      {/if}
    </div>
  </div>