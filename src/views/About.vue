<template>
  <b-list-group>
    <b-list-group-item class="gr-item">
      <div class="d-flex flex-row bd-highlight justify-content-center">
        <div class="p-2 bd-highlight">
          <b-img
            class="avatar"
            :src="require(`@/assets/img/avatar.jpg`)"
          ></b-img>
        </div>
        <div class="p-2 bd-highlight">
          <h1 class="text-white mb-1">{{ infor.name }}</h1>
          <h5 class="text-white">
            {{ infor.description }}
          </h5>
        </div>
      </div>
    </b-list-group-item>
    <div v-for="item in socials" :key="item.name">
      <a :href="[item.link]" class="gr-item list-group-item" button>
        <div class="container">
          <img
            class="img-social"
            :src="require(`@/assets/img/icon/${item.image}`)"
            alt=""
          />
          <span class="text-white ml-2"> {{ item.name }}</span>
        </div>
      </a>
    </div>
  </b-list-group>
</template>

<script>
export default {
  created() {
    document.title = "Quang Truong Profile";
  },
  data() {
    return {
      infor: {
        name: "Quang Trường",
        description: "✌️ Xin chào✌️",
      },
      socials: [
        {
          name: "facebook",
          link: "https://fb.me/truongnq2k",
          image: "facebook.png",
        },
        {
          name: "gitlab",
          link: "https://gitlab.com/truongnq2k",
          image: "gitlab.png",
        },
        {
          name: "github",
          link: "https://github.com/truongnq2k",
          image: "github.png",
        },
        {
          name: "zalo",
          link: "https://zalo.me/0352918986",
          image: "zalo.png",
        },
        { name: "phone", link: "tel:0352918986", image: "phone.png" },
        {
          name: "gmail",
          link: "mailto:truongnq2k@gmail.com",
          image: "gmail.png",
        },
      ],
    };
  },
};
</script>

<style scoped>
.gr-item {
  padding: 0.5em 1.8em;
}
.gr-item .avatar {
  border-radius: 999px;
  height: 8em;
  width: 8em;
}
.img-social {
  border-radius: 999px;
  height: 4rem;
}
.list-group-item {
  background-color: rgb(30, 30, 30);
}
a {
  color: inherit;
  text-decoration: inherit;
  font-weight: bold;
  font-size: 2rem;
  border: 2px solid black;
}
.flex {
  display: flex;
}
</style>