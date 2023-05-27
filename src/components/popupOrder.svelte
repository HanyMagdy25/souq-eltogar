<script>
  import { fly } from "svelte/transition";
</script>

<div
  in:fly={{ y: -10, duration: 500 }}
  out:fly={{ y: -10, duration: 500 }}
  class="bg-white p-4 rounded-md sm:w-11/12 md:w-4/5 lg:w-9/12"
>
  <!-- Start Top  -->
  <div
    class="flex flex-col gap-4 sm:flex-row justify-between pb-2 border-b border-solid border-[#ddd]"
  >
    <div class="flex gap-4 sm:gap-8 justify-between">
      <div>
        <h3 class="font-semibold text-sm sm:text-base text-dark opacity-80">
          كود الطلب
        </h3>
        <h3 class="font-bold text-dark text-sm sm:text-base">31478549321</h3>
      </div>
      <div>
        <h3 class="font-semibold text-sm sm:text-base text-dark opacity-80">
          اسم العميل
        </h3>
        <h3 class="font-bold text-dark text-sm sm:text-base">Hany</h3>
      </div>
      <div>
        <h3 class="font-semibold text-sm sm:text-base text-dark opacity-80">
          رقم الموبايل
        </h3>
        <h3 class="font-bold text-dark text-sm sm:text-base">01112994482</h3>
      </div>
    </div>
    <div class="flex items-center gap-3 justify-between">
      <h3 class="font-semibold text-dark opacity-70">حالة الطلب</h3>
      <div
        class="bg-red-500 text-white rounded-3xl px-5 py-1 text-sm font-semibold"
      >
        التاجر ألغى الطلب
      </div>
    </div>
  </div>

  <div class="flex justify-between py-4">
    <h2 class="font-bold text-dark text-2xl">المنتجات</h2>
  </div>

  <table class="w-full text-center border border-solid border-[#ddd]">
    <thead>
      <tr>
        <th />
        <th class="py-3 font-semibold text-dark text-sm sm:text-base opacity-80"
          >اسم المنتج</th
        >
        <th class="py-3 font-semibold text-dark text-sm sm:text-base opacity-80">عدد القطع</th
        >
        <th class="py-3 font-semibold text-dark text-sm sm:text-base opacity-80">السعر</th>
      </tr>
    </thead>

    <tbody>
      <tr class="bg-gray-100 border-b border-solid border-gray-300">
        <td class="py-5 flex justify-center items-center min-width-3rem">
          <img
            src="https://res.cloudinary.com/dia1kfg4m/image/upload/v1670573442/Rectangle_3_a1sxid.png"
            alt="product"
            class="w-12 h-12 rounded-full shadow-sm shadow-slate-600"
          />
        </td>
        <td class="text-sm opacity-90 font-bold text-dark sm:text-base px-2"
          >عرض 2 قطع مع الخصم من شركة يوتيوب</td
        >
        <td class="text-sm opacity-90 font-bold text-dark sm:text-base">6</td>
        <td class="text-sm opacity-90 font-bold text-dark sm:text-base">130 جنيه مصرى</td>
      </tr>
      <tr class="bg-gray-100 border-b border-solid border-gray-300">
        <td class="py-5 flex justify-center items-center min-width-3rem">
          <img
            src="https://res.cloudinary.com/dia1kfg4m/image/upload/v1670573442/Rectangle_3_a1sxid.png"
            alt="product"
            class="w-12 h-12 rounded-full shadow-sm shadow-slate-600"
          />
        </td>
        <td class="text-sm opacity-90 font-bold text-dark sm:text-base px-2"
          >عرض 6 قطع مع الخصم من شركة يوتيوب</td
        >
        <td class="text-sm opacity-90 font-bold text-dark sm:text-base">2</td>
        <td class="text-sm opacity-90 font-bold text-dark sm:text-base">650 جنيه مصرى</td>
      </tr>
     
    </tbody>
  </table>

  <p class="my-5 opacity-70 font-semibold text-sm text-dark">
    اذا واجهتك اي مشاكل من فضلك انتظر حتي نقوم بإعادة النظر في طلب سيادتكم، و يمكنكم ايضا ارسال رسالة الي مدير اعمالك للمساعدة
  </p>
</div>
