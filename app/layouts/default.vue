<template>
  <el-container>
    <el-header>Yukito</el-header>
    <el-container>
      <el-aside style="background-color: rgb(238, 241, 246)" width="200px">
        <el-menu :router="true">
          <div style="margin-top: 10px;margin-bottom: 10px">
            <i class="el-icon-location"></i>
            <span>契約管理業務</span>
          </div>
          <el-menu-item index="/person/list" :route="{ path: `/person/list` }">
            契約一覧
          </el-menu-item>
          <el-menu-item index="/person/edit" :route="{ path: `/person/edit` }">
            契約編集
          </el-menu-item>
          <div style="margin-top: 10px;margin-bottom: 10px">
            <i class="el-icon-location"></i>
            <span>労働時間管理業務</span>
          </div>
          <el-menu-item index="1-1">労働時間一覧</el-menu-item>
          <el-menu-item index="1-2">労働時間編集</el-menu-item>
          <div style="margin-top: 10px;margin-bottom: 10px">
            <i class="el-icon-location"></i>
            <span>支払い管理業務</span>
          </div>
          <el-menu-item index="1-1">支払い一覧</el-menu-item>
          <el-menu-item index="1-2">支払い編集</el-menu-item>
        </el-menu>
      </el-aside>
      <el-main style="padding-top:0px">
        <nuxt />
      </el-main>
    </el-container>
  </el-container>
</template>
