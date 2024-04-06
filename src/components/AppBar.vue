<script setup lang="ts">
import { appWindow } from '@tauri-apps/api/window';
import {VscChromeMinimize, VscChromeMaximize, VscChromeClose}  from "vue3-icons/vsc";

    const handleMinimize = () => {
        appWindow.minimize()
    }

    const handleToggleMaximize = () => {
        appWindow.toggleMaximize()
    }

    const handleClose = () => {
        appWindow.close()
    }
</script>

<template>
    <div className="app_bar" data-tauri-drag-region>
        <div className="title">Tauri Template</div>

        <div className="window_buttons">
        <button @click="handleMinimize">
            <VscChromeMinimize />
        </button>
        <button @click="handleToggleMaximize">
            <VscChromeMaximize />
        </button>
        <button @click="handleClose">
            <VscChromeClose />
        </button>
        </div>
    </div>
</template>

<style scoped>
    .app_bar {
   width: 100%;
   height: 45px;
   border-bottom: 1px solid rgba(255, 255, 255, 0.05);

   position: relative;

   display: flex;
   align-items: center;
   justify-content: space-between;

   .title {
      padding-left: 15px;

      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;

      user-select: none;
      pointer-events: none;

      font-size: 0.9rem;
   }

   .window_buttons {
      height: 45px;
      width: calc(45px * 3);

      display: flex;
      align-items: center;
      justify-content: flex-end;

      button {
         width: 45px;
         height: 45px;

         display: flex;
         align-items: center;
         justify-content: center;

         background-color: transparent;
         border: none;
         outline: none;

         cursor: pointer;
         transition: all 0.2s ease-in-out;

         svg {
            color: rgba(255, 255, 255, 0.5);
            transition: all 0.2s ease-in-out;

            font-size: 0.9rem;
         }

         &:hover {
            background-color: rgba(255, 255, 255, 0.05);
            svg {
               color: #fff;
            }
         }

         &:last-child:hover {
            background-color: rgb(255, 38, 38);
         }
      }
   }
}
</style>