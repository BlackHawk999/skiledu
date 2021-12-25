<template>
  <div class="header">
    <div class="container">
      <Navbar />
      <div class="header-wrapper">
        <div class="header-title">
          <h1>Studying <span>Online is now much easier</span></h1>
          <p>
            Skilline is an interesting platform that will teach you in more an
            interactive way
          </p>
          <div class="header-btns">
            <button class="join">Join for free</button>
            <button class="play">
              <svg
                width="24"
                height="28"
                viewBox="0 0 24 28"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M22.5751 12.8097C23.2212 13.1983 23.2212 14.135 22.5751 14.5236L1.51538 27.1891C0.848878 27.5899 5.91205e-07 27.1099 6.25202e-07 26.3321L1.73245e-06 1.00123C1.76645e-06 0.223477 0.848877 -0.256572 1.51538 0.14427L22.5751 12.8097Z"
                  fill="#23BDEE"
                />
              </svg>
            </button>
            <p>Watch how it works</p>
          </div>
        </div>
        <div class="header-infos">
          <div class="count">
            <div class="count-icon">
              <svg
                version="1.1"
                id="Layer_1"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                x="0px"
                y="0px"
                width="512px"
                height="512px"
                viewBox="0 0 512 512"
                enable-background="new 0 0 512 512"
                xml:space="preserve"
              >
                <g>
                  <path
                    d="M446.562,98H429v15.058C429,126.271,418.629,137,405.415,137h-0.36C391.841,137,381,126.271,381,113.058V98H137v15.058
		C137,126.271,125.9,137,112.686,137h-0.361C99.11,137,88,126.271,88,113.058V98H65.439C46.419,98,31,113.372,31,132.392v303.061
		C31,454.473,46.419,470,65.439,470h381.123c19.02,0,34.438-15.527,34.438-34.548V132.392C481,113.372,465.581,98,446.562,98z
		 M445,402.562c0,19.02-15.419,34.438-34.439,34.438H102.439C83.419,437,68,421.581,68,402.562V206.438
		C68,187.418,83.419,172,102.439,172h308.121C429.581,172,445,187.418,445,206.438V402.562z"
                  />
                  <path
                    d="M112.5,128.947c10.144,0,18.5-8.223,18.5-18.367V60.07c0-10.145-8.356-18.367-18.5-18.367S94,49.926,94,60.07v50.51
		C94,120.725,102.356,128.947,112.5,128.947z"
                  />
                  <path
                    d="M405.5,128.947c10.144,0,18.5-8.224,18.5-18.367V60.07c0-10.145-8.356-18.367-18.5-18.367
		c-10.143,0-18.5,8.223-18.5,18.367v50.51C387,120.724,395.357,128.947,405.5,128.947z"
                  />
                  <path
                    d="M412,207h-14v31h-60v-31h-14v31h-62v-31h-14v31h-60v-31h-14v31h-61v-31H99v31h-8v13h8v62h-8v14h8v58h-8v13h8v22h14v-22h61
		v22h14v-22h60v22h14v-22h62v22h14v-22h60v22h14v-22h8v-13h-8v-58h8v-14h-8v-62h8v-13h-8V207z M174,385h-61v-58h61V385z M174,313
		h-61v-62h61V313z M248,385h-60v-58h60V385z M248,313h-60v-62h60V313z M324,385h-62v-58h62V385z M324,313h-62v-62h62V313z M398,385
		h-60v-58h60V385z M398,313h-60v-62h60V313z"
                  />
                </g>
              </svg>
            </div>
            <div class="count-text">
              <h5>250k</h5>
              <p>Assisted Students</p>
            </div>
          </div>
          <div class="master-class">
            <div class="class-img">
              <img src="@/assets/images/class-img.jpg" alt="" />
            </div>
            <div class="class-text">
              <h5>User Experience Class</h5>
              <p>Today at 12.00 PM</p>
              <button>Join Now</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
export default {
  name: "Header",
  components: {
    Navbar,
  },
};
</script>

<style lang="scss" scoped>
.header {
  background-image: url("../assets/images/header-bc.png");

  &-wrapper {
    display: flex;
  }

  .header-title {
    h1 {
      font-family: Popp;
      font-style: normal;
      font-weight: bold;
      font-size: 54px;
      line-height: 81px;
      color: #f48c06;
    }
    span {
      color: #2f327d;
    }

    p {
      font-family: Nun;
      font-style: normal;
      font-weight: normal;
      font-size: 24px;
      line-height: 160%;
      color: #464646;
    }
  }

  .header-btns {
    display: flex;
    align-items: center;

    .join {
      color: #ffffff;
      background: #f48c06;
      font-family: Popp;
      font-style: normal;
      font-weight: 600;
      font-size: 24px;
      line-height: 36px;
      padding: 22px 38px;
      border: none;
      border-radius: 80px;
      cursor: pointer;
    }

    .play {
      width: 80px;
      height: 80px;
      background: #ffffff;
      box-shadow: 2px 20px 60px rgba(61, 155, 185, 0.1);
      margin: 0 32px 0 40px;
      padding: 24px 22px 24px 24px;
      border: none;
      border-radius: 50%;
      cursor: pointer;
      transition: 0.3s all;

      &:hover {
        transform: scale(1.1);
      }
    }
  }

  &-infos {
    display: flex;
    flex-direction: column;

    .count {
      display: flex;
      background: rgba(255, 255, 255, 0.8);
      backdrop-filter: blur(20px);
      border-radius: 20px;
      padding: 15px 28px;
    }

    .count-icon {
      width: 50px;
      height: 50px;
      margin-right: 32px;

      svg {
        width: 100%;
        height: 100%;
      }
    }

    .count-text {
      display: flex;
      flex-direction: column;

      h5 {
        color: #595959;
        font-family: Nun;
        font-style: normal;
        font-weight: bold;
        font-size: 24px;
        line-height: 180%;
      }

      p {
        color: #545567;
        font-family: Nun;
        font-style: normal;
        font-weight: 600;
        font-size: 20px;
        line-height: 180%;
      }
    }

    .master-class {
      display: flex;
      background: rgba(255, 255, 255, 0.8);
      backdrop-filter: blur(20px);
      border-radius: 20px;
      padding: 15px 28px;
    }

    .class-img {
      width: 56px;
      height: 56px;
      margin-right: 23px;
      border-radius: 50%;
      overflow: hidden;

      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }

    .class-text {
      display: flex;
      flex-direction: column;

      h5 {
        font-family: Nun;
        font-style: normal;
        font-weight: bold;
        font-size: 24px;
        line-height: 180%;
        color: #595959;
      }

      p {
        font-family: Nun;
        font-style: normal;
        font-weight: 600;
        font-size: 20px;
        color: #545567;
        margin: 10px 0 20px 0;
      }

      button {
        color: #ffffff;
        background: #d8587e;
        font-family: Nun;
        font-style: normal;
        font-weight: bold;
        font-size: 20px;
        line-height: 27px;
        border: none;
        border-radius: 50px;
        padding: 12px 47px;
      }
    }
  }
}
</style>
