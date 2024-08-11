<script setup>
const features = [
  {
    title: "RAG Implementations",
    description:
      "Developing AI systems that combine large language models (LLMs) with retrieval mechanisms to provide accurate, contextually relevant information.",
    icon: "bx:bxs-briefcase",
  },
  {
    title: "Natural Language Processing (NLP)",
    description:
      "Creating applications for sentiment analysis, chatbots, text summarization, and translation.",
    icon: "bx:bxs-window-alt",
  },
  {
    title: "Audio & Vision",
    description:
      "Building AI solutions for voice & image recognition, object detection, facial recognition, and more.",
    icon: "bx:bxs-data",
  },
  {
    title: "Integrated AI Solutions",
    description:
      "We don’t just build powerful AI models; we also ensure they are seamlessly integrated into your business processes with custom visualizations and front-end interfaces.",
    icon: "bx:bxs-bot",
  },
  {
    title: "End-to-End Delivery",
    description:
      "From backend AI implementation to the front-end user experience, we deliver fully integrated solutions that are ready to deploy and scale..",
    icon: "bx:bxs-file-find",
  },
  {
    title: "Data Sovereignty and Protection",
    description:
      "We ensure that your data remains secure, fully under your control, and compliant with the highest standards of privacy and data governance. That's why we primarily work with self-hosted, open-source large language models (LLMs) and dedicated vector databases.",
    icon: "bx:bxs-user",
  },
];
</script>

<template>
  <div class="mt-16 md:mt-0">
    <h2 class="text-4xl lg:text-5xl font-bold lg:tracking-tight !leading-[1.2]">
      From concept to reality, we transform your ideas into solutions.
    </h2>
    <p class="text-lg mt-4 text-slate-600">
      Your requirements, our expertise – together, we create custom AI solutions. 
    </p>
  </div>

  <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16">
    <div v-for="item of features" class="flex gap-4 items-start">
      <div class="mt-1 bg-black rounded-full p-2 w-8 h-8 shrink-0">
        <Icon class="text-white" :name="item.icon" />
      </div>
      <div>
        <h3 class="font-semibold text-lg">{{ item.title }}</h3>
        <p class="text-slate-500 mt-2 leading-relaxed">
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>
