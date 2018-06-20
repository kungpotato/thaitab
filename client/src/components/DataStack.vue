<template>
  <div class="container">
    <div class="row">
      <div class="col-md-8">
        <span class="head-data">สถานที่ท่องเที่ยวและประเพณีไทย</span><hr/>
        <div class="row">
          <div class="col-md-4">
            <img class="img-fit" src="http://img.painaidii.com/images/20150330_3_1427698222_987521.jpg" alt="น้ำตก">
          </div>
          <div class="col-md-8">
            <b>title kungpotato</b>
            <p>
              Lorem ipsum dolor sit amet, mei augue malorum scaevola no, ut vim possim aliquando.
              An sententiae honestatis scriptorem eos, novum dissentias nam an. Nam latine malorum sensibus at,
              ei sea rebum partem comprehensam, nominavi deleniti ius ut. Per habeo perpetua ad,
              te eam nostro dissentias, iudico impetus ornatus ad vix. An modus mnesarchum ullamcorper nec.
            </p>
          </div>
        </div><hr/>
      </div>
      <div class="col-md-4">
        <recom-room/>
      </div>
    </div>
  </div>
</template>

<script>
import Recommend from './Recommend'

export default {
  name: 'data-list',
  components: {
    'recom-room': Recommend
  }
}
</script>
