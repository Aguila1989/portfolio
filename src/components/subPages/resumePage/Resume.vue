<script>
import ResumeCard from "@/components/subPages/resumePage/ResumeCard.vue";
import ResumeCardExpanded from "@/components/subPages/resumePage/resumeCardExpanded.vue";

export default {
  name: "Resume",
  components: { ResumeCardExpanded, ResumeCard }
};
</script>

<template>
  <div class="resume-page">
    <h1>Resume</h1>
    <div class="resume-containers">
      <ResumeCard class="talents" title="TALENTS AND SKILLS" list="Javascript<br>HTML<br>CSS<br>VUE<br>JAVA<br>C#"/>
      <ResumeCard class="languages" title="LANGUAGES"
                  list="Dutch: Native language<br>Spanish: Good<br>English: Good<br>French: Moderate<br/>"/>
      <ResumeCardExpanded class="education" title="EDUCATION" :sections="[
          { title: 'Howest Bruges 2022 - Present', text: 'Bachelor in Applied Informatics' },
          { title: 'Syntra West Kortrijk 2014-2016', text: 'Accounting (first 2 years)' },
          { title: 'Mariawende Bruges 2001-2008', text: 'Secondary Education, STW' }
          ]"/>
      <ResumeCardExpanded class="experience" title="EXPERIENCE" :sections="[
          { title: 'STP: 28/02/2022-24/06/2022', text: 'Production and Quality Coordinator' },
          { title: 'Gsnel: 01/08/2018-11/08/2019', text: 'Truck Driver C' },
          { title: 'Sandwich Shop Merlijn: 16/11/2016-11/03/2019', text: 'Business Owner' },
          { title: 'Bivit: 31/01/2011-31/12/2016', text: '-Warehouse Manager/Logistics Manager' },
          { title: 'Jules: 10/2010-01/2011', text: 'Salesperson/Cashier' },
          { title: 'Colruyt: 10/2008-09/2010', text: 'Temporary Non-food Supervisor' }
          ]"/>
      <ResumeCard class="license" title="DRIVERS LICENSE" list="Drivers License Category B and C"/>
      <ResumeCard class="cv" title="DOWNLOAD CV" list="<a href='/src/assets/files/CV%20Demeulenaere%20Kevin%20Nederlands.pdf' target='_blank'>Download Dutch CV</a>
                                                      <br><a href='/src/assets/files/CV%20Demeulenaere%20Kevin%20Engels.pdf' target='_blank'>Download English CV</a>"/>
    </div>
  </div>
</template>

<style scoped>

h1 {
  font-family: 'Playwrite GB S', sans-serif;
  margin-top: 5rem;
  text-align: center;
}

.resume-containers {
  opacity: 0.8;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 2rem;
  padding: 2rem;
}

.resume-containers > * {
  flex: 1 1 45%;
  max-width: 45%;
}

@media (max-width: 768px) {
  .resume-containers {
    flex-direction: column;
    padding: 1rem;
  }

  .resume-containers > * {
    flex: 1 1 100%;
    max-width: 100%;
  }
}


.talents {
  background-color: #d0e7f5;
}

.languages {
  background-color: #d4edda;
}

.education {
  background-color: #f8d7da;
}

.experience {
  background-color: #fff3cd;
}

.license {
  background-color: #d6d8f5;
}

.cv {
  background-color: #fce4ec;
}

</style>
