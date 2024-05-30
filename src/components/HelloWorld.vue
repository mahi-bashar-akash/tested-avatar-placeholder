<template>

  <div class="intro-wrapper-header">
    <div class="side-face">
      <img :src="`/svg/justify-left.svg`" class="sidebar-toggle" alt="justify-left" @click="sidebarToggle()">
      <img :src="`/svg/smie.svg`" class="smile" alt="smile">
    </div>
    <a href="https://github.com/mahibashardeveloper/avatar-placeholder" class="github-link">
      Code view on github
    </a>
  </div>
  <div class="intro-wrapper">
    <div class="sidebar" :class="{'active' : sidebarIsActive}">
      <div class="sidebar-hidden-close">
        <img :src="`/svg/close.svg`" class="sidebar-close" alt="close" @click="sidebarToggle()">
      </div>
      <div class="sidebar-title">
        Overview
      </div>
      <a href="#introduction" class="sidebar-link" @click="sidebarToggle()">
        Introduction
      </a>
      <a href="#install" class="sidebar-link" @click="sidebarToggle()">
        Install
      </a>
      <div class="sidebar-title">
        Properties
      </div>
      <a href="#getting-started" class="sidebar-link" @click="sidebarToggle()">
        Getting started
      </a>
      <a href="#avatar-photo" class="sidebar-link" @click="sidebarToggle()">
        Avatar Photo
      </a>
      <a href="#avatar-name" class="sidebar-link" @click="sidebarToggle()">
        Avatar Name
      </a>
      <a href="#avatar-size" class="sidebar-link" @click="sidebarToggle()">
        Avatar Size
      </a>
      <a href="#background-color" class="sidebar-link" @click="sidebarToggle()">
        Avatar Background Color
      </a>
      <a href="#text-color" class="sidebar-link" @click="sidebarToggle()">
        Avatar Text Color
      </a>
      <a href="#border-radius" class="sidebar-link" @click="sidebarToggle()">
        Avatar Border Radius
      </a>
    </div>
    <div class="content">

      <div id="introduction">
        <div class="content-title">Introduction</div>
        <p class="content-paragraph">
          The complete documentation reference of the AvatarPlaceHolder Library, a JavaScript library made for displaying avatar as name which can be one, two or three words.
        </p>
      </div>

      <div id="install">
        <div class="content-title">Install</div>
        <p class="content-paragraph">The quickest way to implement AvatarPlaceHolder is to use the hosted version on npm package</p>
        <div class="bg-light pt-3">
        <pre>

          npm i avatar-placeholder-package

        </pre>
        </div>
      </div>

      <div id="getting-started">
        <div class="content-title">Getting Started</div>
        <p class="content-paragraph">
          Apply this code into your vue template
        </p>
        <div class="bg-light">
        <pre>
          {{preCode}}
        </pre>
        </div>
      </div>

      <div id="avatar-photo">
        <div class="content-title">Avatar Photo</div>

        <pre class="py-1">
        props: <br>
        avatar: {<br>
          type: String,<br>
          default: null,<br>
        }<br>
      </pre>

        <div class="bg-light pt-1 mt-2">
        <pre>
          {{preCodeAvatar}}
        </pre>
        </div>

      </div>

      <div id="avatar-name">
        <div class="content-title">Avatar Name</div>

        <pre class="py-1">
        props: <br>
        name: {<br>
          type: String,<br>
          required: true,<br>
        }<br>
      </pre>

        <div class="bg-light pt-1 mt-2">
        <pre>
          {{preCodeAvatarName}}
        </pre>
        </div>

        <div class="mt-2">
          <div class="mb-2">Preview</div>
          <AvatarPlaceHolder name="Olivia Mia Maeve" size="size-64" background-color="bg-blue" text-color="text-white" radius="rounded-none"/>
        </div>
      </div>

      <div id="avatar-size">
        <div class="content-title">Avatar Size</div>

        <div class="pe-3">
          <ul>
            <li class="py-1">Size 32 --- .size-32</li>
            <li class="py-1">Size 64 --- .size-64</li>
            <li class="py-1">Size 128 --- .size-128</li>
            <li class="py-1">Size 256 --- .size-256</li>
          </ul>
        </div>

        <pre class="py-1">
        props: <br>
        size: {<br>
          type: String,<br>
          default: 'size-32',<br>
        }<br>
      </pre>

        <div class="bg-light pt-1 mt-2">
        <pre>
          {{preCodeAvatarSize}}
        </pre>
        </div>

        <div class="mt-2">
          <div class="mb-2">Preview</div>
          <AvatarPlaceHolder name="Olivia Mia Maeve" size="size-64" background-color="bg-blue" text-color="text-white" radius="rounded-none"/>
        </div>
      </div>

      <div id="background-color">
        <div class="content-title">Background Color</div>
        <p class="content-paragraph">
          you can use this code. But if you don't need of those code you can custom create background-color
        </p>
        <div class="pe-3">
          <ul class="list-flex">
            <li class="list-data py-1">bg-blue</li>
            <li class="list-data py-1">bg-indigo</li>
            <li class="list-data py-1">bg-purple</li>
            <li class="list-data py-1">bg-pink</li>
            <li class="list-data py-1">bg-red</li>
            <li class="list-data py-1">bg-orange</li>
            <li class="list-data py-1">bg-yellow</li>
            <li class="list-data py-1">bg-green</li>
            <li class="list-data py-1">bg-teal</li>
            <li class="list-data py-1">bg-cyan</li>
            <li class="list-data py-1">bg-light</li>
            <li class="list-data py-1">bg-white</li>
            <li class="list-data py-1">bg-dark</li>
            <li class="list-data py-1">bg-subtle-blue</li>
            <li class="list-data py-1">bg-subtle-indigo</li>
            <li class="list-data py-1">bg-subtle-purple</li>
            <li class="list-data py-1">bg-subtle-pink</li>
            <li class="list-data py-1">bg-subtle-red</li>
            <li class="list-data py-1">bg-subtle-orange</li>
            <li class="list-data py-1">bg-subtle-yellow</li>
            <li class="list-data py-1">bg-subtle-green</li>
            <li class="list-data py-1">bg-subtle-teal</li>
            <li class="list-data py-1">bg-subtle-cyan</li>
            <li class="list-data py-1">bg-subtle-dark</li>
          </ul>
        </div>
        <pre class="py-1">
        props: <br>
        backgroundColor: {<br>
          type: String,<br>
          default: 'bg-blue',<br>
        }<br>
      </pre>
        <div class="bg-light pt-1 mt-2">
        <pre>
          {{preCodeAvatarBackgroundColor}}
        </pre>
        </div>

        <div class="mt-2">
          <div class="mb-2">Preview</div>
          <AvatarPlaceHolder name="Olivia Mia Maeve" size="size-64" background-color="bg-blue" text-color="text-white" radius="rounded-none"/>
        </div>
      </div>

      <div id="text-color">
        <div class="content-title">Text Color</div>

        <p class="content-paragraph">
          you can use this code. But if you don't need of those code you can custom create color
        </p>
        <div class="pe-3">
          <ul class="list-flex">
            <li class="list-data py-1">text-blue</li>
            <li class="list-data py-1">text-indigo</li>
            <li class="list-data py-1">text-purple</li>
            <li class="list-data py-1">text-pink</li>
            <li class="list-data py-1">text-red</li>
            <li class="list-data py-1">text-orange</li>
            <li class="list-data py-1">text-yellow</li>
            <li class="list-data py-1">text-green</li>
            <li class="list-data py-1">text-teal</li>
            <li class="list-data py-1">text-cyan</li>
            <li class="list-data py-1">text-light</li>
            <li class="list-data py-1">text-white</li>
            <li class="list-data py-1">text-dark</li>
          </ul>
        </div>
        <pre class="py-1">
        props: <br>
        textColor: {<br>
          type: String,<br>
          default: 'text-blue',<br>
        }<br>
      </pre>
        <div class="bg-light pt-1 mt-2">
        <pre>
          {{preCodeAvatarTextColor}}
        </pre>
        </div>

        <div class="mt-2">
          <div class="mb-2">Preview</div>
          <AvatarPlaceHolder name="Olivia Mia Maeve" size="size-64" background-color="bg-blue" text-color="text-white" radius="rounded-none"/>
        </div>
      </div>

      <div id="border-radius">
        <div class="content-title">Border Radius</div>

        <p class="content-paragraph">
          you can use this code. But if you don't need of those code you can custom create border-radius
        </p>
        <div class="pe-3">
          <ul class="list-flex">
            <li class="list-data py-1">rounded-none</li>
            <li class="list-data py-1">rounded-circle</li>
          </ul>
        </div>
        <pre class="py-1">
        props: <br>
        radius: {<br>
          type: String,<br>
          default: 'rounded-none',<br>
        }<br>
      </pre>
        <div class="bg-light pt-1 mt-2">
        <pre>
          {{preCodeAvatarRadius}}
        </pre>
        </div>

        <div class="mt-2">
          <div class="mb-2">Preview</div>
          <AvatarPlaceHolder name="Olivia Mia Maeve" size="size-64" background-color="bg-blue" text-color="text-white" radius="rounded-circle"/>
        </div>
      </div>

    </div>
  </div>

</template>

<script>

import AvatarPlaceHolder from "avatar-placeholder-package";
import 'avatar-placeholder-package/dist/avatar-placeholder-package.css'

export default {
  components: {AvatarPlaceHolder},
  data() {
    return {
      sidebarIsActive: false,
      preCode: `
        <template>

            <AvatarPlaceHolder/>

        </template>

          <!-- apply this code inside of script -->

          import AvatarPlaceHolder from "avatar-placeholder-package";
          import 'avatar-placeholder-package/dist/avatar-placeholder-package.css'

          export default {
              components: {AvatarPlaceHolder}
          }

      `,
      preCodeAvatar: `<AvatarPlaceHolder avatar="avatar.png"/>`,
      preCodeAvatarName: `<AvatarPlaceHolder name="Olivia Mia Maeve"/>`,
      preCodeAvatarSize: `<AvatarPlaceHolder size="size-64"/>`,
      preCodeAvatarBackgroundColor: `<AvatarPlaceHolder background-color="bg-blue"/>`,
      preCodeAvatarTextColor: `<AvatarPlaceHolder text-color="text-blue"/>`,
      preCodeAvatarRadius: `<AvatarPlaceHolder radius="rounded-circle"/>`,
    }
  },
  mounted() {

  },
  methods: {

    sidebarToggle() {
      this.sidebarIsActive = !this.sidebarIsActive
    }

  }
}

</script>

<style>
@import '../css/wrapper.css';
</style>