<template>
    <q-card flat bordered class="my-card absolute-right q-pa-xl" style="overflow: auto;">
      <q-card-section>
        <span class="about-me"><strong>Resume</strong></span>
      </q-card-section>

      <q-card-section>
        <div class="row">
          <div class="col-7">
            <q-timeline color="secondary" :layout="myLayout">
              <q-timeline-entry heading>
                Education
              </q-timeline-entry>

              <q-timeline-entry title="Event Title" subtitle="February 22, 1986">
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et
                  dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
                  ex
                  ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                  fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                  deserunt
                  mollit anim id est laborum.
                </div>
              </q-timeline-entry>

              <q-timeline-entry title="Event Title" subtitle="February 21, 1986" icon="delete">
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et
                  dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
                  ex
                  ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                  fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
                  deserunt
                  mollit anim id est laborum.
                </div>
              </q-timeline-entry>

              <q-timeline-entry heading>
                November, 2017
              </q-timeline-entry>

              <q-timeline-entry title="Event Title" subtitle="February 22, 1986"
                avatar="https://cdn.quasar.dev/img/avatar2.jpg">
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit
                </div>
              </q-timeline-entry>

              <q-timeline-entry title="Event Title" subtitle="February 22, 1986">
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit
                </div>
              </q-timeline-entry>

              <q-timeline-entry title="Event Title" subtitle="February 22, 1986" color="orange" icon="done_all">
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit
                </div>
              </q-timeline-entry>

              <q-timeline-entry title="Event Title" subtitle="February 22, 1986">
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit
                </div>
              </q-timeline-entry>

              <q-timeline-entry title="Event Title" subtitle="February 22, 1986">
                <div>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit
                </div>
              </q-timeline-entry>
            </q-timeline>
          </div>
          <div class="col-1"></div>
          <div class="col-4 " style="font-size: 18px;">
            <div>
              <p class="text-h3 q-mt-md">Code skills</p>
            </div>
            <div class="q-mt-lg">
              <q-label class="q-ml-sm">Java</q-label>
              <q-linear-progress :value="progress" size="6px" rounded class="q-mb-md q-ml-sm progressBar" />
            </div>
            <div>
              <q-label class="q-ml-sm">Angular</q-label>
              <q-linear-progress :value="progress" size="6px" rounded class="q-mb-md q-ml-sm progressBar" />
            </div>
            <div>
              <q-label class="q-ml-sm">Vue.js</q-label>
              <q-linear-progress :value="progress" size="6px" rounded class="q-mb-md q-ml-sm progressBar" />
            </div>
            <div>
              <q-label class="q-ml-sm">Spring framework</q-label>
              <q-linear-progress :value="progress" size="6px" rounded class="q-mb-md q-ml-sm progressBar" />
            </div>
          </div>
        </div>
      </q-card-section>
    </q-card>
</template>

<script>
export default {
  name: 'Resume',
  data() {
    return {
      myLayout: 'dense',
      progress: 0.4
    }
  }
}
</script>

<style>
.my-card {
  background-color: rgb(34, 34, 34);
  height: 100%;
  border-radius: 40px;
  width: 70%;
}
.progressBar {
  color: rgb(68, 148, 136);
}
</style>
