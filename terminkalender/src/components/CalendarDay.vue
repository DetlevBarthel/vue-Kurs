<template>
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
</template>
<script>
export default {
    name:'CalendarDay',
    props:['day']
}
</script>