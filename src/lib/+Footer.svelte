<script>
//   import { Youtube, HelpCircle, Instagram } from 'lucide-svelte'; // Note: lucide-svelte uses different icon names
</script>

<footer class="mx-10 bg-gray-1000 text-white rounded-lg px-6 w-auto py-8 md:px-12 border border-gray-900">
  <div class="max-w-8xl mx-auto">
    <!-- Main footer content -->
    <div class="flex flex-col md:flex-row justify-between gap-8">
      <!-- Logo section -->
      <div class="mb-6 md:mb-0">
        <div class="flex items-center">
          <div class="h-10 w-10 bg-purple-600 rounded flex items-center justify-center mr-2">
            <div class="h-6 w-6 bg-black rotate-45"></div>
          </div>
          <span class="text-purple-500 text-xl font-bold">NO HESI</span>
        </div>
      </div>

      <!-- Navigation columns - responsive grid -->
      <div class="grid grid-cols-2 md:grid-cols-3 gap-8">
        <!-- Column 1 -->
        <div>
          <ul class="space-y-3">
            <li>
              <a href="/about" class="hover:text-purple-400">
                About Us
              </a>
            </li>
            <li>
              <a href="/contacts" class="hover:text-purple-400">
                Contacts
              </a>
            </li>
          </ul>
        </div>

        <!-- Column 2 -->
        <div>
          <ul class="space-y-3">
            <li>
              <a href="/get-started" class="hover:text-purple-400">
                Get started
              </a>
            </li>
            <li>
              <a href="/subscription" class="hover:text-purple-400">
                Subscription
              </a>
            </li>
            <li>
              <a href="/servers" class="hover:text-purple-400">
                Servers
              </a>
            </li>
            <li>
              <a href="/leaderboard" class="hover:text-purple-400">
                Leaderboard
              </a>
            </li>
          </ul>
        </div>

        <!-- Column 3 -->
        <div>
          <ul class="space-y-3">
            <li>
              <a href="/privacy" class="hover:text-purple-400">
                Privacy Policy
              </a>
            </li>
            <li>
              <a href="/terms" class="hover:text-purple-400">
                Terms Of Use
              </a>
            </li>
            <li>
              <a href="/refund" class="hover:text-purple-400">
                Refund Policy
              </a>
            </li>
            <li>
              <a href="/cookies" class="hover:text-purple-400">
                Cookie Policy
              </a>
            </li>
          </ul>
        </div>
      </div>

      <!-- Social media icons - shows at top on mobile, right side on desktop -->
      <div class="order-first md:order-last mb-6 md:mb-0">
        <div class="flex justify-end space-x-4">
          <a
            href="https://youtube.com"
            class="text-gray-400 hover:text-white"
          >
            <!-- <Youtube size={24} /> -->
          </a>
          <a
            href="https://discord.com"
            class="text-gray-400 hover:text-white"
          >
            <!-- <HelpCircle size={24} /> Note: questionSquare is HelpCircle in lucide-svelte -->
          </a>
          <a
            href="https://instagram.com"
            class="text-gray-400 hover:text-white"
          >
            <!-- <Instagram size={24} /> -->
          </a>
          <a
            href="https://tiktok.com"
            class="text-gray-400 hover:text-white"
          >
            <span class="font-bold text-xl">␥</span>
          </a>
        </div>
      </div>
    </div>

    <!-- Copyright -->
    <div class="mt-12 pt-4 border-t border-gray-800">
      <p class="text-sm text-gray-500">
        NoHesi™ 2024. All rights reserved.
      </p>
    </div>
  </div>
</footer>

<style>
  /* If you need to add any custom styles */
  .bg-gray-1000 {
    background-color: #111;
  }
  a {
    transition: color 0.2s ease;
  }
</style>