<script>
    /**
     * @desc    Toggles the mobile menu
     */
    function toggleMenu() {
        console.log('toggle menu');
        const menu = document.querySelector('#menu');
        if (menu) {
            menu.classList.toggle('hidden');
        }
    }
</script>

<header>
    <nav class="flex flex-wrap items-center justify-between w-full py-4 md:py-0 px-4 text-lg text-white bg-gray-900">
        <div>
            <a href="/" class="flex flex-wrap items-center justify-between">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-6 w-6 mr-1">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M12 12.75c1.148 0 2.278.08 3.383.237 1.037.146 1.866.966 1.866 2.013 0 3.728-2.35 6.75-5.25 6.75S6.75 18.728 6.75 15c0-1.046.83-1.867 1.866-2.013A24.204 24.204 0 0112 12.75zm0 0c2.883 0 5.647.508 8.207 1.44a23.91 23.91 0 01-1.152 6.06M12 12.75c-2.883 0-5.647.508-8.208 1.44.125 2.104.52 4.136 1.153 6.06M12 12.75a2.25 2.25 0 002.248-2.354M12 12.75a2.25 2.25 0 01-2.248-2.354M12 8.25c.995 0 1.971-.08 2.922-.236.403-.066.74-.358.795-.762a3.778 3.778 0 00-.399-2.25M12 8.25c-.995 0-1.97-.08-2.922-.236-.402-.066-.74-.358-.795-.762a3.734 3.734 0 01.4-2.253M12 8.25a2.25 2.25 0 00-2.248 2.146M12 8.25a2.25 2.25 0 012.248 2.146M8.683 5a6.032 6.032 0 01-1.155-1.002c.07-.63.27-1.222.574-1.747m.581 2.749A3.75 3.75 0 0115.318 5m0 0c.427-.283.815-.62 1.155-.999a4.471 4.471 0 00-.575-1.752M4.921 6a24.048 24.048 0 00-.392 3.314c1.668.546 3.416.914 5.223 1.082M19.08 6c.205 1.08.337 2.187.392 3.314a23.882 23.882 0 01-5.223 1.082" />
                </svg>
                <h5>responsive navbar</h5>
            </a>
        </div>
        <!-- svelte-ignore a11y_click_events_have_key_events -->
        
        <div class="hidden w-full md:flex md:items-center md:w-auto" id="menu">
            <ul class="pt-4 text-base text-white md:flex md:justify-between md:pt-0">
                <li><a href="/" class="md:p-4 py-2 block hover:text-purple-400" on:click={() => toggleMenu()}>Home</a></li>
                <li><a href="/" class="md:p-4 py-2 block hover:text-purple-400" on:click={() => toggleMenu()}>Contact</a></li>
                <li><a href="/" class="md:p-4 py-2 block hover:text-purple-400" on:click={() => toggleMenu()}>Sign Up</a></li>
            </ul>
        </div>
    </nav>
</header>

<style></style>