<template>
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="contact">

      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          Contact Me &nbsp;
          <div class="h-[1px] w-32 bg-amber-200 md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
        <div class="flex justify-center">
          <img class="w-12/12 rounded-full mb-3 fadein-up"
            src="@/assets/foto.jpg" alt="Fotoku">
        </div>
        <div class="md:w-6/12">
		<div class="contact-info">
			<div class="info-item">
			<i class="fa fa-envelope"></i>
			<span>Nama		: {{ nama }}</span>
			</div>
			<div class="info-item">
			<i class="fa fa-envelope"></i>
			<span>Email		: {{ email }}</span>
			</div>
			<div class="info-item">
			<i class="fa fa-phone"></i>
			<span>Phone		: {{ phone }}</span>
			</div>
			<div class="info-item">
			<i class="fa fa-map-marker"></i>
			<span>Address&nbsp;: {{ address }}</span>
			</div>
		</div>
        </div>

      </section>

    </article>
  </div>

</template>

<script>
export default {
  data() {
    return {
      nama		: 'Yudya Hastriawan Sukma',
      email		: 'yudyasukma2@gmail.com',
      phone		: '089-530-583-955 (WA)',
      address		: 'Griya Taman Asri Blok HG-8 Tawangsari, Kec. Taman, Kab. Sidoarjo, Jawa Timur 61257'
    };
  }
};
</script>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}
</style>
