<template>
  <Layout>
    <h1>About us</h1>
    <p>Quienes somos nosotros... algo de texto Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsam nam beatae ut reiciendis perferendis tempora blanditiis nisi error illo aliquam, nihil iure itaque, odit iste, assumenda eaque iusto laudantium vitae.</p>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Exercitationem officia quia quis a sint consectetur, culpa iusto dolor. Minima eveniet laudantium neque recusandae sint saepe rem rerum blanditiis maiores assumenda.</p>
    <div class="magazine">
      <g-image class="dogs" src="~/images/dogs.jpg" width="500" />
      <div class="magazine-content">
        <h2 class="subtitle">Quien es Manuela?</h2>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Esse unde dolores error accusantium cumque, ut voluptatem assumenda. Nostrum, amet non, quasi consequuntur nesciunt perspiciatis molestiae, libero sit vero vel et.</p>
      </div>
    </div>

    <p>Algo mas?</p>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "About us"
  }
};
</script>

<style>
.magazine {
  display: flex;
}
.magazine-content {
  padding: 0 2rem;
}
.dogs {
  object-fit: cover;
}
h1,
h2,
h3,
p {
  margin-bottom: 20px;
}
.subtitle {
  font-weight: 900;
}
</style>

