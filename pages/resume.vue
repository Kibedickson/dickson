<template>
  <div class="md:flex md:flex-row md:gap-10">
    <div class="md:w-1/4">
      <h1 class="text-center font-semibold text-2xl md:hidden">
        Web Developer
      </h1>
      <div
        class="block rounded-full shadow-xl mx-auto h-48 w-48 bg-cover bg-center mt-4 avatar-sm"
      ></div>
      <h2 class="text-center font-semibold text-2xl mt-4">
        Dickson Kibe
      </h2>
      <h3
        class="text-center font-bold hidden md:block text-sm uppercase text-gray-500"
      >
        Web Developer
      </h3>
      <info-list class="mt-12" />
      <div class="mt-12">
        <button
          class="bg-blue-500 text-white active:bg-blue-600 font-bold uppercase text-xs px-6 py-4 rounded-lg shadow hover:shadow-md outline-none focus:outline-none"
          type="button"
          style="transition: all 0.15s ease"
        >
          Download Resume
        </button>
      </div>
    </div>
    <div class="md:w-3/3">
      <h2 class="hidden md:block md:mt-4 font-semibold text-2xl">
        Professional Summary
      </h2>
      <professional-summary class="mt-8 md:mt-5" />
      <h2 class="mt-12 font-semibold text-2xl">
        Work Experience
      </h2>
      <work-experience>
        <template v-slot:designation>
          Web Developer
        </template>
        <template v-slot:company>
          Wise and Agile Solutions
        </template>
        <template v-slot:location>
          Nairobi
        </template>
        <template v-slot:type>
          Full Time
        </template>
        <template v-slot:duration>
          December, 2020 - present
        </template>
      </work-experience>
      <work-experience>
        <template v-slot:designation>
          Freelance Web Developer
        </template>
        <template v-slot:company>
          Freelance
        </template>
        <template v-slot:location>
          Kisumu, Maseno
        </template>
        <template v-slot:type>
          Full Time
        </template>
        <template v-slot:duration>
          January, 2019 - November, 2020
        </template>
      </work-experience>

      <h2 class="mt-12 font-semibold text-2xl">
        Education
      </h2>
      <education>
        <template v-slot:degree>
          Bachelor of Science, Computer Science -
          <!--          <span class="text-gray-600 font-black">63.73%</span>-->
        </template>
        <template v-slot:institute>
          Maseno University
        </template>
        <template v-slot:duration>
          2016 - 2020
        </template>
      </education>
      <education>
        <template v-slot:degree>
          High School
          <span class="text-gray-600 font-black">A- (76)</span>
        </template>
        <template v-slot:institute>
          Muhoho High School
        </template>
        <template v-slot:duration>
          2012 - 2015
        </template>
      </education>
    </div>
  </div>
</template>

<script>
import InfoList from '@/components/InfoList';
import Education from '@/components/Education';
import WorkExperience from '@/components/WorkExperience';
import ProfessionalSummary from '@/components/ProfessionalSummary';

export default {
  components: {
    InfoList,
    Education,
    WorkExperience,
    ProfessionalSummary,
  },
};
</script>
