<template>
  <div id="app">

    <CalenderWeek />
    <div id="calender-week">
      <div class="container-fluid mt-5">
        <div class="row">
          <div class="col-12">
            <div class="card-group">
              <!-- Tage -->
              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Montag</strong>
                </div>
                <div class="card-body">
                  <div>1</div>
                  <div class="alert alert-success text-center">
                    <div>Müll rausbringen</div>
                    <div>
                      <i class="fas fa-edit mr-2"></i>
                      <i class="far fa-trash-alt"></i>
                    </div>
                  </div>
                </div>
              </div>

              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Dienstag</strong>
                </div>
                <div class="card-body">
                  <div>1</div>
                </div>
              </div>

              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Mittwoch</strong>
                </div>
                <div class="card-body">
                  <div>1</div>
                </div>
              </div>

              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Donnerstag</strong>
                </div>
                <div class="card-body">
                  <div>1</div>
                </div>
              </div>

              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Freitag</strong>
                </div>
                <div class="card-body">
                  <div>1</div>
                  <div class="alert alert-success text-center">
                    <div>Müll rausbringen</div>
                    <div>
                      <i class="fas fa-edit mr-2"></i>
                      <i class="far fa-trash-alt"></i>
                    </div>
                  </div>
                </div>
              </div>

              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Samstag</strong>
                </div>
                <div class="card-body">
                  <div>1</div>
                </div>
              </div>

              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Sonntag</strong>
                </div>
                <div class="card-body">
                  <div>1</div>
                  <div class="alert alert-primary text-center">
                    <div>Grillen mit freunden</div>
                    <div>
                      <i class="fas fa-edit mr-2"></i>
                      <i class="far fa-trash-alt"></i>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="calender-entry">
      <div class="container mt-5">
        <div class="row">
          <div class="col-6 offset-3">
            <div class="card">
              <div class="card-header text-center bg-vue ">
                <h5>Neuer Termin für: <strong> Dienstag</strong></h5>
              </div>
              <div class="card-body">
                <input 
                type="text"
                class="form-control"
                placeholder="Neuer Termin"
                >
                <div class="mt-3 text-center">
                <span 
                v-for="(color,index) in ['primary','success', 'info', 'warning', 'danger']"
                :key="index"
                class="alert mr-2 square alert-primary"
                :class="['alert-'+color]"
                style="cursor: pointer;"
                ></span>
                </div>
                <hr>
                <button class="btn bg-vue2 btn-block">Eintragen</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CalenderWeek from "./components/CalenderWeek"
export default {
  name: 'App',
  components: {
    CalenderWeek
  }
}
</script>

<script>
export default {
  name: "App",
};
</script>
<style scoped>
.bg-vue {
  background-color: rgb(52, 73, 94);
  color: white;
}
.bg-vue2 {
  background-color: rgb(65,184, 131);
  color: white;
}
.square{
  width:40px;
  height: 40px
}
</style>
