<template lang="pug">
  div.app(ref="app")
    router-view

</template>

<script >
export default {
  name: "app",
  mounted() {},
  methods: {}
};
</script>

<style lang="scss">
@import "src/components/common/scss/base.scss";
#app {
  color: $font-color;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100%;
  background-color: #282c34;
  &::-webkit-scrollbar {
    width: 5px;
    height: 16px;
    background-color: black;
    opacity: 1;
  }
  &::-webkit-scrollbar-track {
    -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
    border-radius: 10px;
    // background-color: #f5f5f5;
  }
  &::-webkit-scrollbar-thumb {
    border-radius: 10px;
    -webkit-box-shadow: inset 0 0 6px rgba(54, 54, 54, 0.3);
    background-color: red;
  }
}
html {
  height: 100%;
  z-index: -1;
  background: rgba(255, 255, 255, 1);
  font-family: "Source Sans Pro", "Helvetica Neue", Helvetica, Arial, sans-serif;
  // background: rgba(0,0,0,.5);
  
}
.v-note-wrapper {
  height: 820px !important;
  
}
.popup-dropdown{
  background: rgba(0, 0, 0, .9)!important;
}
body {
  letter-spacing: 1px;
  background: #32373d!important;
  opacity: 1;
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
  // filter: blur(0.8px);
  // margin: -30px;
  position: absolute;
  height: 100%;
  width: 100%;
  z-index: -1;
  
}
.ivu-input {
  height: 33px !important;
  padding-left: 7px !important;
  padding-top: 0 !important;
  padding-bottom: 0 !important;
  padding-right: 0 !important;
  border: 0 !important;
  background: black !important;
  // border-top-left-radius: 4px;
  // border-bottom-left-radius: 4px;
  // border-top-right-radius: 0 !important;
  // border-bottom-right-radius: 0 !important;
  color: white;
  outline-color: rgba(255, 255, 255, 0);
  border: 0 !important;
  transition: background-color 0.25s linear;
  caret-color: red;
  &::placeholder {
    color: #777;
  }
  &:hover {
    background-color: hsla(0, 0%, 57%, 0.4);
  }
}
.ivu-upload {
  height: 33px !important;
  padding-left: 0 !important;
  padding-top: 0 !important;
  padding-bottom: 0 !important;
  padding-right: 0 !important;
  border-left: 0 solid gray !important;
  border-right: 0 solid gray !important;
  border-top: 0 !important;
  border-bottom: 0 !important;
  background: black !important;
  border-top-right-radius: 0 !important;
  border-bottom-right-radius: 0 !important;
  border-top-left-radius: 0 !important;
  border-bottom-left-radius: 0 !important;
  div {
    padding: 0 0 0 0 !important;
  }
  .ivu-icon-ios-cloud-upload {
    font-size: 20px !important;
    line-height: 33px !important;
  }
}
// iview page
.ivu-page-item{
  width: 30px!important;
  height: 28px!important;
  background: black!important;
  border: none!important;
  line-height: 28px!important;
  // border-radius: 3px!important;
}
.ivu-page-item-jump-next{
  border: none!important;
  line-height: 28px!important;
  width: 28px!important;
  height: 28px!important;
}
.ivu-page-item-jump-prev{
  border: none!important;
  line-height: 28px!important;
  width: 28px!important;
  height: 28px!important;
}
.ivu-page-prev{
  width: 28px!important;
  height: 28px!important;
  background: black!important;
  border: none!important;
  line-height: 28px!important;
}
.ivu-page-next{
  width: 28px!important;
  height: 28px!important;
  background: black!important;
  border: none!important;
  line-height: 28px!important;
}
body,
h1,
h2,
h3,
h4,
p {
  padding: 0;
  margin: 0;
}
h4 {
  font-size: 14px;
}
// markdown
.v-note-op{
  background: #282c34!important;

}
.op-icon:hover{
background: rgba(0,0,0,.3)!important;
color: gray!important;
}
.divarea-wrapper{
  background: rgba(0,0,0,.85);
}
.auto-textarea-input{
background: rgba(0,0,0,0);
color: white!important;
}
.mu-list{
  background: rgba(0,0,0,.9)!important;
  padding: 0!important;
}
.mu-item {
    min-height: 33px!important;
    display: flex;
    padding: 7px 14px!important;
    color: rgba(0, 0, 0, 0.87);
    position: relative;
}
.mu-item-title{
  color: white!important;
  line-height: 30px!important;
  font-size: 14px!important;

}
.v-note-wrapper.fullscreen{
  top: 33px!important;
  height: 100%!important;
}
.v-note-wrapper{
  height:calc(100vh - 230px)!important;
}

.op-icon.selected{
  background: rgba(0,0,0,.3)!important;
  color: gray!important;
}
.op-icon{
  color: gray!important;
}
.auto-textarea-input.no-resize{
  background: rgba(0,0,0,0)!important;
}
.dropdown {
    display: inline-block!important;
    cursor: pointer;
    height: 28px;
    width: 28px;
    font-size: 15px;
    color: rgb(117, 117, 117);
    text-align: center;
    line-height: 1;
    background: #282c34!important;
    margin: 0px !important;
    padding: 4.5px 6px 0px 3.5px !important;
    border-radius: 5px !important;
    border: none!important;
    outline: none !important;
}
// iview-msg
.ivu-message-notice-content{
  background: rgba(0, 0, 0, .9)!important;
  color: rgba(255, 255, 255, .8);
  margin-top: 20px!important;
}

// 切图组件背景
.cropper-bg{
  background-image: none!important;
}
.cropper-modal {
    background-color: #32373d;
    opacity: .5;
}
</style>