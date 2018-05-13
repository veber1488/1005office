<template>
  <div class="app-container documentation-container">
   <!-- <div class="empty-cases-header"><h2 style="display: flex; justify-content: center; align-items: center; letter-spacing: 0.2em; margin-left: 20px">Empty Cases</h2></div>  -->
    <div class="empty-cases-header"><h2 style="letter-spacing: 0.2em; margin-left: 20px">Empty Cases</h2><div> <transition name="bounce"><el-button v-if="checked || checked1 || checked2 || checked3 || checked4 || checked5 || checked6 || checked7" style=" margin-right: 20px" type="success">Description</el-button></transition><el-button style=" margin-right: 20px;" type="primary">View all</el-button></div>
    </div> 
    <section class="card">
      <div class="card--content" @click="checked = !checked" v-bind:class="{ active: isChecked }"><div class="card-header"><h3 class="card-header-item card-header-item1">CaseType1</h3> <el-checkbox class="card-header-item2" v-model="checked" size="medium"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_disk_array_scsi.svg" width="190" height="auto" alt="image description" class="card--content-img"></div>
      <div class="card--content" @click="checked1 = !checked1"><div class="card-header"><h3 class="card-header-item card-header-item1">CaseType2</h3> <el-checkbox class="card-header-item2" v-model="checked1"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_disk_array_scsi.svg" width="190" height="auto" alt="image description" class="card--content-img"></div>
      <div class="card--content" @click="checked2 = !checked2"><div class="card-header"><h3 class="card-header-item card-header-item1">CaseType3</h3> <el-checkbox class="card-header-item2" v-model="checked2"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_disk_array_scsi.svg" width="190" height="auto" alt="image description" class="card--content-img"></div>
      <div class="card--content" @click="checked3 = !checked3"><div class="card-header"><h3 class="card-header-item card-header-item1">CaseType4</h3> <el-checkbox class="card-header-item2" v-model="checked3"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_disk_array_scsi.svg" width="190" height="auto" alt="image description" class="card--content-img"></div>
      <div class="card--content" @click="checked4 = !checked4"><div class="card-header"><h3 class="card-header-item card-header-item1">CaseType5</h3> <el-checkbox class="card-header-item2" v-model="checked4"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_disk_array_scsi.svg" width="190" height="auto" alt="image description" class="card--content-img"></div>
      <div class="card--content" @click="checked5 = !checked5"><div class="card-header"><h3 class="card-header-item card-header-item1">CaseType6</h3> <el-checkbox class="card-header-item2" v-model="checked5"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_disk_array_scsi.svg" width="190" height="auto" alt="image description" class="card--content-img"></div>
      <div class="card--content" @click="checked6 = !checked6"><div class="card-header"><h3 class="card-header-item card-header-item1">CaseType7</h3> <el-checkbox class="card-header-item2" v-model="checked6"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_disk_array_scsi.svg" width="190" height="auto" alt="image description" class="card--content-img"></div>
      <div class="card--content" @click="checked7 = !checked7"><div class="card-header"><h3 class="card-header-item card-header-item1">CaseType8</h3> <el-checkbox class="card-header-item2" v-model="checked7"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_disk_array_scsi.svg" width="190" height="auto" alt="image description" class="card--content-img"></div>
     
      
    </section>
   <div class="empty-cases-header"><h2 style="letter-spacing: 0.2em; margin-left: 20px">User's Library</h2> <div><transition name="bounce"><el-button v-if="checkedDev1 || checkedDev2 || checkedDev3 || checkedDev4 || checkedDev5 || checkedDev6 || checkedDev7 || checkedDev8" style=" margin-right: 20px" type="success">Description</el-button></transition><el-button style=" margin-right: 20px;" type="primary">View all</el-button></div>
    </div> 
    <section class="card">
       <div class="card--content" @click="checkedDev1 = !checkedDev1"><div class="card-header"><h3 class="card-header-item card-header-item1">DevType1</h3><el-checkbox class="card-header-item2" v-model="checkedDev1"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_controller.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedDev2 = !checkedDev2"><div class="card-header"><h3 class="card-header-item card-header-item1">DevType2</h3><el-checkbox class="card-header-item2" v-model="checkedDev2"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_controller.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedDev3 = !checkedDev3"><div class="card-header"><h3 class="card-header-item card-header-item1">DevType3</h3><el-checkbox class="card-header-item2" v-model="checkedDev3"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_controller.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedDev4 = !checkedDev4"><div class="card-header"><h3 class="card-header-item card-header-item1">DevType4</h3><el-checkbox class="card-header-item2" v-model="checkedDev4"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_controller.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedDev5 = !checkedDev5"><div class="card-header"><h3 class="card-header-item card-header-item1">DevType5</h3><el-checkbox class="card-header-item2" v-model="checkedDev5"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_controller.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedDev6 = !checkedDev6"><div class="card-header"><h3 class="card-header-item card-header-item1">DevType6</h3><el-checkbox class="card-header-item2" v-model="checkedDev6"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_controller.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedDev7 = !checkedDev7"><div class="card-header"><h3 class="card-header-item card-header-item1">DevType7</h3><el-checkbox class="card-header-item2" v-model="checkedDev7"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_controller.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedDev8 = !checkedDev8"><div class="card-header"><h3 class="card-header-item card-header-item1">DevType8</h3><el-checkbox class="card-header-item2" v-model="checkedDev8"></el-checkbox></div>
      <img src="/src/views/netOffConfig/san_controller.svg" width="190" height="auto" alt="image description"></div>
    </section>
    <div class="empty-cases-header"><h2 style="letter-spacing: 0.2em; margin-left: 20px">УПАСК</h2> <div><transition name="bounce"><el-button v-if="checkedUp1 || checkedUp2 || checkedUp3 || checkedUp4 || checkedUp5 || checkedUp6 || checkedUp7 || checkedUp8" style=" margin-right: 20px;" type="success">Description</el-button></transition>
    <el-button style=" margin-right: 20px;" type="primary">View all</el-button></div>
    </div> 
    <section class="card">
      <div class="card--content" @click="checkedUp1 = !checkedUp1"><div class="card-header"><h3 class="card-header-item card-header-item1">Type1</h3><el-checkbox class="card-header-item2" v-model="checkedUp1"></el-checkbox></div>
      <img src="/src/views/netOffConfig/sata_disk_array.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedUp2 = !checkedUp2"><div class="card-header"><h3 class="card-header-item card-header-item1">Type2</h3><el-checkbox class="card-header-item2" v-model="checkedUp2"></el-checkbox></div>
      <img src="/src/views/netOffConfig/sata_disk_array.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedUp3 = !checkedUp3"><div class="card-header"><h3 class="card-header-item card-header-item1">Type3</h3><el-checkbox class="card-header-item2" v-model="checkedUp3"></el-checkbox></div>
      <img src="/src/views/netOffConfig/sata_disk_array.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedUp4 = !checkedUp4"><div class="card-header"><h3 class="card-header-item card-header-item1">Type4</h3><el-checkbox class="card-header-item2" v-model="checkedUp4"></el-checkbox></div>
      <img src="/src/views/netOffConfig/sata_disk_array.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedUp5 = !checkedUp5"><div class="card-header"><h3 class="card-header-item card-header-item1">Type5</h3><el-checkbox class="card-header-item2" v-model="checkedUp5"></el-checkbox></div>
      <img src="/src/views/netOffConfig/sata_disk_array.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedUp6 = !checkedUp6"><div class="card-header"><h3 class="card-header-item card-header-item1">Type6</h3><el-checkbox class="card-header-item2" v-model="checkedUp6"></el-checkbox></div>
      <img src="/src/views/netOffConfig/sata_disk_array.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedUp7 = !checkedUp7"><div class="card-header"><h3 class="card-header-item card-header-item1">Type7</h3><el-checkbox class="card-header-item2" v-model="checkedUp7"></el-checkbox></div>
      <img src="/src/views/netOffConfig/sata_disk_array.svg" width="190" height="auto" alt="image description"></div>
      <div class="card--content" @click="checkedUp8 = !checkedUp8"><div class="card-header"><h3 class="card-header-item card-header-item1">Type8</h3><el-checkbox class="card-header-item2" v-model="checkedUp8"></el-checkbox></div>
      <img src="/src/views/netOffConfig/sata_disk_array.svg" width="190" height="auto" alt="image description"></div>
    </section>
  </div>
</template>
<script>
import DropdownMenu from '@/components/Share/dropdownMenu'

export default {
  name: 'addDevice',
  components: { DropdownMenu },
  data() {
    return {
     checked: true,
     checked1: false,
     checked2: false,
     checked3: false,
     checked4: false,
     checked5: false,
     checked6: false,
     checked7: false,
     checked8: false,
     checkedDev1: false,
     checkedDev2: false,
     checkedDev3: false,
     checkedDev4: false,
     checkedDev5: false,
     checkedDev6: false,
     checkedDev7: false,
     checkedDev8: false,
     checkedUp1: false,
     checkedUp2: false,
     checkedUp3: false,
     checkedUp4: false,
     checkedUp5: false,
     checkedUp6: false,
     checkedUp7: false,
     checkedUp8: false,
     isChecked: false,
    ischeckedBorder: true

    }
  },
computed: {
  checkChecked: function() {
    if (this.checked = true) {

    }
  }
}
}
</script>

<style rel="stylesheet/scss" lang="scss" scoped>
.documentation-container {
  margin: 0px;
  .document-btn {
    float: left;
    margin-left: 50px;
    // vertical-align: middle;
    display: block;
    cursor: pointer;
    background: black;
    color: white;
    height: 60px;
    width: 200px;
    line-height: 60px;
    font-size: 20px;
    text-align: center;
  }
}

.card {
  display: flex;
  min-width: 100%;
  min-height: 200px;
  overflow-x: auto;
  background-color: #bdc3c7;
  border: 2px solid #34495e;
  justify-content: space-between;
  cursor: pointer;
}

.isChekedBorder {
  border: 2px solid red;
}

.card-header {
  display: flex;
  justify-content: space-between;
}

.card-header::-webkit-scrollbar {
  display: none;
}

.card-header-item1 {
  flex: 4;
}
.card-header-item2 {
  flex: 1;
}

.card::-webkit-scrollbar {
  display: none;
}
.card--content {
  background-color: #fff;
  min-width: 200px;
  margin: 5px;
  padding: 5px;
  color: #34495e;
  justify-content: space-around;
  border: #34495e;
  display: flex;
  flex-direction: column;
}
.card--content-img {
  align-items: center;
}

.empty-cases-header {
  display: flex;
  min-width: 100%;
  min-height: 3em;
  overflow-x: auto;
  background-color: #34495e;
  color: #ecf0f1;
  align-items: center;
  justify-content: space-between;
}
.users-library-header {
  display: flex;
  min-width: 100%;
  min-height: 3em;
  overflow-x: auto;
  background-color: #34495e;
  color: #ecf0f1;
  align-items: center;
  justify-content: space-between;
}

.bounce-enter-active {
  animation: bounce-in .8s;
}
.bounce-leave-active {
  animation: bounce-in .4s reverse;
}
@keyframes bounce-in {
  0% {
    transform: scale(0);
  }
  50% {
    transform: scale(2);
  }
  100% {
    transform: scale(1);
  }
}

// 

</style>