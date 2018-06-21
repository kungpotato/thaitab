<template>
  <div class='container'>
    <div class='row side-padding'>
      <div class='col-md-12 bg-option'>
        <b-form class="form-center" inline>
          <b>ตัวเลือกการค้นหา :</b><b-form-select class="mb-2 mr-sm-2 mb-sm-0" v-model='selected' :options='options'/>
          <b-form-input class="mb-2 mr-sm-2 mb-sm-0" type="text" placeholder="ใส่การค้นหา"></b-form-input>
          <b-button variant="dark">ค้นหา</b-button>
        </b-form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'page-option',
  data () {
    return {
      selected: null,
      options: [
        { value: null, text: 'ค้นหาตามชื่อที่เกี่ยวข้อง' },
        { text: 'ค้นหาตามชื่อภูมิภาค' },
        { text: 'ค้นหาตามชื่อจังหวัด' }
      ]
    }
  }
}
</script>
