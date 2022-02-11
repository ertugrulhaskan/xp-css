<template>
  <div class="lg:hidden h-screen px-10 pt-10 blue-screen">
    <p>A problem has been detected and windows has been shut down to prevent damage to your computer.</p>
    <p>If this is the first time you've seen this Stop error screen, restart your computer. If this screen appears again, follow these steps:</p>
    <p>Check to be sure you have adequate disk space. If a driver is identified in the Stop message, disable the driver or check with the manufacturer for driver updates. Try changing video adapters.</p>
    <p>Check with your hardware vendor for any BIOS updates. Disable BIOS memory options such as caching or shadowing. If you need to use Safe Mode to remove or disable components, restart your computer, press F8 to select Advanced Startup options, and then select Safe Mode.</p>
    <p>Technical information:</p>
    <p>*** STOP: 0x0000007e (0x80000003, 0x805c49b8, 0xf7a172b4, 0xf7a16fb0)</p>
  </div>
  <div class="hidden lg:grid lg:grid-rows-6 lg:h-full">
    <div class="row-span-1 bar-top"></div>
    <section class="row-span-4">
      <div class="container mx-auto h-full flex justify-center max-w-5xl bg-xp">
        <div class="w-6/12 pr-10 flex justify-end items-center">
          <div class="relative">
            <div class="w-60">
              <the-logo></the-logo>
            </div>
            <p class="absolute bottom-4">To begin, click your user name</p>
          </div>
        </div>
        <div class="divider"></div>
        <div class="w-6/12 pl-10 flex justify-start items-center">
          <div class="p-2 rounded-md bg-xpDarkBlue w-full max-w-sm user-wrapper">
            <div class="flex">
              <figure class="w-12 h-12 mr-3 rounded-[4px] border-2 border-yellow-300">
                <img
                  src="https://picsum.photos/42"
                  alt="User Image"
                  class="object-cover w-full h-full"
                />
              </figure>
              <div class="relative w-full max-w-[70%]">
                <h2>Alex</h2>
                <form class="absolute" action="#">
                  <label for="txtPassword" class="text-xs">Type your password</label>
                  <div class="flex">
                    <div class="flex items-center">
                      <input
                        type="password"
                        name="txtPassword"
                        class="h-[31px] rounded-md outline-none text-black px-2 text-xl"
                        id="txtPassword"
                      />
                      <button class="rounded-md w-8 overflow-hidden ml-2">
                        <img
                          src="@/assets/images/system-login.jpg"
                          alt="Login"
                          class="object-none w-8 h-8"
                        />
                      </button>
                    </div>
                  </div>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <div class="row-span-1 bar-bottom">
      <div class="container mx-auto max-w-5xl h-full">
        <div class="flex justify-between items-center h-full">
          <div class="flex items-center">
            <button class="rounded-md w-8 overflow-hidden mr-2">
              <img
                src="@/assets/images/system-shutdown.jpg"
                alt="Logout"
                class="object-none w-8 h-8"
              />
            </button>
            <span>Turn off computer</span>
          </div>
          <div>
            <p>After you log on, you can add or change accounts.</p>
            <p>Just go to Control Panel and click User Accounts.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TheLogo from "@/components/TheLogo.vue";
export default {
  name: "HomeView",
  components: { TheLogo }
};
</script>
