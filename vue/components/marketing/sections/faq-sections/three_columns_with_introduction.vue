<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <section aria-labelledby="faq-heading" class="bg-white">
    <div class="max-2xl mx-auto py-16 px-4 sm:py-24 sm:px-6 lg:max-w-7xl lg:px-8">
      <div class="max-w-xl">
        <h2 id="faq-heading" class="text-2xl font-bold tracking-tight text-gray-900">Frequently asked questions</h2>
        <p class="mt-4 text-base text-gray-500">Questions. Frequently asked ones. Plus our answers. That's how FAQs work. If you can't find what you're looking for, you can always <a href="#" class="font-medium text-indigo-600 hover:text-indigo-500">send us an email</a> with your enquiry.</p>
      </div>

      <dl class="mt-12 grid grid-cols-1 gap-y-10 sm:mt-16 md:grid-cols-2 md:gap-x-6 lg:grid-cols-3">
        <div v-for="faq in faqs" :key="faq.id">
          <dt class="text-base font-medium text-gray-900">{{ faq.question }}</dt>
          <dd class="mt-3 text-sm text-gray-500">{{ faq.answer }}</dd>
        </div>
      </dl>
    </div>
  </section>
</template>

<script setup>
const faqs = [
  {
    id: 1,
    question: "What's the best thing about Switzerland?",
    answer:
      "I don't know, but the flag is a big plus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cupiditate laboriosam fugiat.",
  },
  // More questions...
]
</script>