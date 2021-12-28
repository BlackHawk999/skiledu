<template>
  <div :class="['sidebar', { open: active }]">
    <div class="wrapper">
      <div class="close-icon" @click="active = !active">
        <img src="@/assets/images/close.svg" alt="" />
      </div>
      <div class="sidebar-reg">
        <a class="log right" href="">Log in</a>
        <a class="log" href="">Sign Up</a>
      </div>

      <div class="titles">
        <h5 v-for="(item, idx) in items" :key="idx">{{ item.title }}</h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Sidebar",
  data() {
    return {
      items: [
        { title: "Home" },
        { title: "Carrers" },
        { title: "Blog" },
        { title: "About Us" },
      ],
    };
  },
  props: {
    active: {
      type: Boolean,
    },
  },
};
</script>

<style lang="scss" scoped>
.sidebar {
  background-color: #fff2e1;
  position: fixed;
  left: 0;
  right: 0;
  min-height: 100vh;
  display: none;
  transform: translateX(100%);
  transition: all 0.4s;
  z-index: 100;

  &.open {
    transform: translateX(0);
  }

  .wrapper {
    display: flex;
    flex-direction: column;
    position: relative;
  }

  .sidebar-reg {
    display: flex;
    align-items: center;
    justify-content: center;
    padding-bottom: 10px;
    margin: 20px 0 20px 0;
    border-bottom: 1px solid #2f327d;

    .log {
      border: 1px solid #ffffff;
      background: #ffffff;
      box-shadow: 0px 20px 24px rgba(0, 0, 0, 0.03);
      border-radius: 80px;
      padding: 5px 30px;
      text-decoration: none;
      white-space: nowrap;

      &.right {
        margin-right: 35px;
      }

      &:hover {
        background: #2f327d;
        color: #ffffff;
      }
    }
  }

  .close-icon {
    position: absolute;
    left: 15px;
    top: 10px;
  }

  .titles {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    padding-right: 90px;

    h5 {
      font-weight: 500;
      font-size: 24px;
      line-height: 14px;
      color: #2f327d;
      margin-bottom: 35px;
      transition: 0.2s cubic-bezier(0.77, 0, 0.175, 1);
      cursor: pointer;

      &:hover {
        transform: translateX(10px);
      }
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .sidebar {
    display: none;
  }
}

@media screen and (max-width: 991.98px) {
  .sidebar {
    display: none;
  }
}
@media screen and (max-width: 767.98px) {
  .sidebar {
    display: block;
  }
}
</style>
