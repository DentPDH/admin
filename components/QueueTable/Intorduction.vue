<template>
  <div class="">
    <h4 class="">การทำงานของระบบจองคิว</h4>
    <ol class="">
      <li class="">เลือกวันที่ (สามารถเลือกวันล่วงหน้าได้)</li>
      <li class="">สร้างช่วงเวลาของแต่ละวัน (Timeslots)</li>
      <li class="">กำหนดจำนวนที่เปิดรับในช่วงเวลานั้น</li>
    </ol>
    <hr />

    <h4 class="">การลบวันที่ (REMOVE DATE)</h4>
    <ul class="">
      <li class="">
        การลบตารางtimeslots ของทั้งวันนั้นจะต้องยังไม่มีการจองเข้า ถึงจะลบได้
        (ยอดจองคิวต้องเท่ากับ 0)
      </li>
    </ul>
    <hr />

    <h4 class="">การแก้ไข timeslot (EDIT)</h4>
    <h6 class="card-subtitle">
      หลังจากสร้างเสร็จสมบูรณ์แล้ว สามารถแก้ไขได้ที่หน้า ตารางเวลา
      แล้วทำการเลือกวัน
    </h6>
    <ol class="">
      <li class="">
        แก้ไขจำนวนเปิดรับใหม่ สามารถปรับเพิ่มหรือลดได้ <br />
        แต่ต้องไม่น้อยกว่าตัวเลขที่มียอดจองมาแล้ว
      </li>
      <li class="">
        การลบ timeslot ช่วงเวลานั้นๆ ต้องไม่มีการจองมาก่อน ( คิวจองเป็น 0 )
        ถึงจะสามารถลบได้ <br />(หากมีคนจองมาแล้วและต้องการลบ timeslot นั้น
        ให้แก้ไขโดยการ ปรับตัวเลขเปิดรับจอง มาเท่ากับจำนวนคนจองแล้ว จะทำให้
        timeslot นั้นไม่สามารถจองเพิ่มได้อีกเนื่องจากเต็มแล้ว)
      </li>
      <li class="">
        ในกรณีที่ต้องการปิดไม่รับจองของวันนั้นๆ ให้ปรับmode เป็น OFF
      </li>
    </ol>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>
