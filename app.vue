<template>
  <div
  class="bg-repeat bg-cover w-full h-full font-sans"
  style="background-image: url(/bg.jpg)"
>
  <div class="flex items-center justify-center h-full">
    <div
      class="max-w-[800px] relative z-20 shadow-lg after:content-[' '] after:z-[-1] after:h-full after:bg-slate-100 after:border after:border-slate-200 after:absolute after:left-2.5 after:right-2.5 after:top-0 after:mt-2 after:rounded"
    >
      <div class="bg-white border border-slate-200 p-6 rounded">
        <!-- Start Screen -->
        <section class="flex flex-col items-center gap-6">
          <img src="/bruno.svg" class="w-64 h-64 rounded-full" />
          <h1 class="text-center font-bold text-2xl">
            Finance Chatbot Advisor
          </h1>
          <form class="flex flex-col gap-2 w-full">
            <input
              type="text"
              placeholder="Your name"
              class="w-full transition p-2 text-sm border border-slate-300/60 shadow-sm placeholder:text-slate-400/90 focus:ring-4 focus:ring-primary focus:ring-opacity-20 focus:border-primary focus:border-opacity-40 pr-16 rounded-xl"
            />
            <small class="text-slate-500 italic">
              Please provide a name so we can knows who is talkin.
            </small>
            <button
              type="submit"
              class="transition w-full bg-blue-950 text-slate-300 font-medium py-2 px-3 rounded hover:bg-opacity-90"
            >
              Start a New Chat
            </button>
            <button
              type="button"
              class="transition w-full bg-slate-200 text-slate-600 font-medium py-2 px-3 rounded hover:bg-opacity-90"
            >
              Continue Previous Chat
            </button>
          </form>
        </section>

        <!-- Chat Screen -->
        <section class="flex flex-col min-w-[520px] w-full">
          <!-- Customer Support Agent -->
          <div class="flex items-center gap-3.5 pb-4 border-b border-dashed">
            <div>
              <div
                class="w-12 h-12 overflow-hidden rounded-full image-fit border-2 border-slate-200/70"
              >
                <img src="/bruno.svg" />
              </div>
            </div>
            <div>
              <div class="font-medium truncate max-w-[9rem] md:max-w-none">
                Chatbot
              </div>
              <div
                class="text-slate-500 mt-0.5 truncate max-w-[9rem] md:max-w-none"
              >
                Customer Support Agent
              </div>
            </div>
          </div>

          <!-- Messages -->
          <div
            class="flex flex-col gap-3.5 py-5 px-3 overflow-y-scroll max-h-[400px]"
          >
            <!-- To flip message use "flex-row-reverse" -->
            <div class="flex items-end gap-3">
              <!-- Profile Image -->
              <img
                class="block w-12 h-12 overflow-hidden rounded-full border-2 border-slate-200/70"
                src="/bruno.svg"
              />
              <!-- Text Image -->
              <!-- <div
                class="flex uppercase items-center justify-center text-xl text-center text-white font-bold bg-gradient-to-t from-sky-500 to-emerald-500 w-12 h-12 overflow-hidden rounded-full border-2 border-slate-200/70"
              >
                js
              </div> -->
              <!-- Main Content -->
              <div
                class="w-3/5 flex flex-col gap-2 border px-4 pt-3 pb-4 rounded-xl bg-slate-50/80 border-slate-200/80"
              >
                <!-- Message Content -->
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Duis mollis massa in lacus vulputate scelerisque. Duis
                  ultrices est in faucibus porttitor.
                </div>
                <!-- Time -->
                <div class="text-xs text-slate-500/70">11:15 AM</div>
              </div>
            </div>
            <div class="flex flex-row-reverse items-end gap-3">
              <!-- Profile Image -->
              <div
                class="flex uppercase items-center justify-center text-xl text-center text-white font-bold bg-gradient-to-t from-sky-500 to-emerald-500 w-12 h-12 overflow-hidden rounded-full border-2 border-slate-200/70"
                src="/bruno.svg"
              >
                js
              </div>
              <!-- Main Content -->
              <div
                class="w-3/5 flex flex-col gap-2 border px-4 pt-3 pb-4 rounded-l-xl rounded-tl-xl bg-slate-50/80 border-slate-200/80"
              >
                <!-- Message Content -->
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Duis mollis massa in lacus vulputate scelerisque. Duis
                  ultrices est in faucibus porttitor.
                </div>
                <!-- Time -->
                <div class="text-xs text-slate-500/70">11:15 AM</div>
              </div>
            </div>
            <div class="flex items-end gap-3">
              <!-- Profile Image -->
              <!-- Text Image -->
              <!-- <div
                class="flex uppercase items-center justify-center text-xl text-center text-white font-bold bg-gradient-to-t from-sky-500 to-emerald-500 w-12 h-12 overflow-hidden rounded-full border-2 border-slate-200/70"
              >
                js
              </div> -->
              <img
                class="block w-12 h-12 overflow-hidden rounded-full border-2 border-slate-200/70"
                src="/bruno.svg"
              />
              <!-- Main Content -->
              <!-- To flip bubble, change "rounded-r-xl" to "rounded-l-xl" -->
              <div
                class="w-3/5 flex flex-col gap-2 border px-4 pt-3 pb-4 rounded-r-xl rounded-tl-xl bg-slate-50/80 border-slate-200/80"
              >
                <!-- Message Content -->
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Duis mollis massa in lacus vulputate scelerisque. Duis
                  ultrices est in faucibus porttitor.
                </div>
                <!-- Time -->
                <div class="text-xs text-slate-500/70">11:15 AM</div>
              </div>
            </div>
          </div>
          <form class="relative">
            <textarea
              class="transition p-4 w-full text-sm border border-slate-300/60 shadow-sm placeholder:text-slate-400/90 focus:ring-4 focus:ring-primary focus:ring-opacity-20 focus:border-primary focus:border-opacity-40 pr-16 rounded-xl resize-none"
              placeholder="Enter your message..."
            ></textarea>
            <button
              type="submit"
              class="absolute top-2 right-2 h-10 w-10 flex items-center justify-center bg-gradient-to-t from-sky-500 to-emerald-500 rounded-full text-white"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="16"
                height="16"
                fill="currentColor"
                class="bi bi-send"
                viewBox="0 0 16 16"
              >
                <path
                  d="M15.854.146a.5.5 0 0 1 .11.54l-5.819 14.547a.75.75 0 0 1-1.329.124l-3.178-4.995L.643 7.184a.75.75 0 0 1 .124-1.33L15.314.037a.5.5 0 0 1 .54.11ZM6.636 10.07l2.761 4.338L14.13 2.576zm6.787-8.201L1.591 6.602l4.339 2.76z"
                />
              </svg>
            </button>
          </form>
        </section>
      </div>
    </div>
  </div>
</div>
</template>
