<script>
  import { lazyLoad } from "$lib/utils/lazyLoad";
  import decision from "$lib/assets/decision.svg"
  import analysis from "$lib/assets/analysis.svg"
  import user_check from "$lib/assets/user_check.svg"
  import insight from "$lib/assets/insight.svg"

  let contentArray = [
    {
        heading: "User Behavior",
        text: "Unlock deep insights into user behavior, tracking every click and interaction to understand your audience like never before.",
        image:user_check
        
    },
    {
        heading: "Sharper Analysis",
        text: "Harness the power of sharper analysis to refine your strategies, ensuring precision and clarity in your data interpretations.",
        image:analysis

    },
    {
        heading: "Product Insights",
        text: "Gain actionable product insights to optimize features, enhance user experience, and drive innovation with data at your fingertips.",
        image:insight
    },
    {
        heading: "Data-Driven Decisions",
        text: "Empower your business with data-driven decisions, turning raw data into strategic actions for sustained growth.",
        image:decision
    }
];

</script>

{#each contentArray as content}
<div class="card z-10 lg:w-80 lg:p-6 p-12 m-4 lg:m-auto duration-300 gap-3 bg-slate-50 border-2 border-gray-100">
  <img use:lazyLoad={content.image} class="w-8 left-4 top-8 inline" alt="">
  <div class="items-center text-pretty text-left">
    <div class=" inline text-left text-xl font-semibold">{content.heading}</div>
    <p class="mt-2">{content.text}</p>
  </div>
</div>
  {/each}