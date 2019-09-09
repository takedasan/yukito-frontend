<template>
  <el-container>
    <el-header height="30px" style="background-color: rgb(238, 241, 246)">
      Yukito
    </el-header>
    <el-container>
      <el-aside width="200px">
        <el-menu :router="true">
          <div style="margin-top: 10px;margin-bottom: 10px">
            <i class="el-icon-location"></i>
            <span>契約社員</span>
          </div>
          <el-menu-item index="/person/list" :route="{ path: `/person/list` }">
            契約社員一覧
          </el-menu-item>
          <el-menu-item index="/person/edit" :route="{ path: `/person/edit` }">
            契約社員編集
          </el-menu-item>
          <div style="margin-top: 10px;margin-bottom: 10px">
            <i class="el-icon-location"></i>
            <span>契約</span>
          </div>
          <el-menu-item index="2-1">契約一覧</el-menu-item>
          <el-menu-item index="2-2">契約編集</el-menu-item>
          <div style="margin-top: 10px;margin-bottom: 10px">
            <i class="el-icon-location"></i>
            <span>労働時間</span>
          </div>
          <el-menu-item index="3-1">労働時間一覧</el-menu-item>
          <el-menu-item index="3-2">労働時間編集</el-menu-item>
          <div style="margin-top: 10px;margin-bottom: 10px">
            <i class="el-icon-location"></i>
            <span>支払い</span>
          </div>
          <el-menu-item index="4-1">支払い一覧</el-menu-item>
          <el-menu-item index="4-2">支払い編集</el-menu-item>
        </el-menu>
      </el-aside>
      <el-main style="padding-top:0px">
        <nuxt />
      </el-main>
    </el-container>
  </el-container>
</template>
