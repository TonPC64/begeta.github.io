<template>
  <div class="pd-10px">
    <h1>Justify Self</h1>
    <div>เป็น Atomic Class ที่ใช้เพื่อระบุการจัดวางของตัว Flex Item เอง ใช้ Justify Self เพื่อจัดในแกน Main-Axis</div>

    <h3>Property</h3>
    <table-atomic :data="property" ></table-atomic>

    <h3>Value</h3>
    <table-atomic :data="value" type="value"></table-atomic>

    <h3>Responsive <span class="cl-success">YES</span></h3>
    <responsive/>

    <h3>Hover <span class="cl-danger">NO</span></h3>
  </div>
</template>

<script>
import TableAtomic from '@/components/TableAtomic'
import Responsive from '@/components/Responsive'

export default {
  components: {
    TableAtomic,
    Responsive
  },
  data () {
    return {
      property: [
        ['Class', 'jtf-s-[value]-[responsive]'],
        ['Property', 'justify-self']
      ],
      value: [
        [
          'Class',
          'start',
          'end',
          'left',
          'right',
          'flex-start',
          'flex-end',
          'self-start',
          'self-end',
          'strecth'
        ],
        [
          'Value Description',
          'สำหรับ "start"',
          'สำหรับ "end"',
          'สำหรับ "left"',
          'สำหรับ "right"',
          'สำหรับ "flex-start"',
          'สำหรับ "flex-end"',
          'สำหรับ "self-start"',
          'สำหรับ "self-end"',
          'สำหรับ "strecth"'
        ]  
      ]
    }
  }
}
</script>

