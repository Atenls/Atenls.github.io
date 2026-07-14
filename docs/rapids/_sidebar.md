<!-- rapids/_sidebar.md -->
<style>
.sidebar .sidebar-nav > ul > li {
    margin: 8px 0 8px 0;
    padding: 4px 0 4px 8px;
    box-shadow: 0 0 6px rgb(81 62 96 / 20%);
    border-radius: 1em 0 0 1em;
}

.sidebar .sidebar-nav > ul > li > ul > li {
    margin: 4px 0;
}

.app-sub-sidebar {
    line-height: 1.625;
}

.app-sub-sidebar li {
    position: relative;
    padding-left: 1.25em;
    margin: 2px 0;

    &::before { 
        content: "";
        position: absolute;
        left: 4px;
        top: 12px;
        transform: translateY(-50%);
        width: 4px;
        height: 2px;
        background: rgb(180, 180, 180, 0.5);
        border-radius: 2px;
    }

    &:hover::before {
        content: "";
        background: rgb(73, 119, 172);
        height: 4px;
    }
}

.app-sub-sidebar li a:hover {
    color: rgb(73, 119, 172);
}

.sidebar .sidebar-nav > ul > li > a {
    position: relative;
    padding-left: 1.25em;

    &::before {
      content: "";
      position: absolute;
      left: 4px;
      top: 16px;
      transform: translateY(-50%);
      width: 5px;
      height: 18px;
      background: rgb(180, 180, 180, 0.5);
      border-radius: 4px;
    }

    &:hover::before {
      content: "";
      background: rgb(73, 119, 172);
    }
}

.test {
    color: rgb(142, 37, 184);
}

.sidebartitle {
    font-size: 1.5em;
    font-weight: 600;
    color: transparent; 
    background: linear-gradient(135deg, rgb(64, 132, 209), rgb(177, 33, 196)) text;
    text-shadow: 0 0 1px rgba(29, 59, 99, 0.2);
    margin: 1em auto;
    width: fit-content;
}

.sidebarsubtitle {
    font-size: 1.25em;
    font-weight: 600;
    text-shadow: 0 0 1px rgba(29, 59, 99, 0.2);
    margin: 1em auto;
    width: fit-content;
}

</style>


<p class="sidebartitle">Rapids - 「激流」</p>

* [首页](rapids/rapids)
* [更新记录](rapids/updatelogs)
* [设计](rapids/design)
* [副本流程](rapids/dungeon)
* [副本图鉴](rapids/dungeonlist)
* [副本机制](rapids/dungeonmechanics)
* [怪物信息](rapids/mobsinfo)
* [材料图鉴](rapids/materials)
* [套装属性](rapids/setattributes)
* [Rapids 服务条款](rapids/terms)

<p style="margin-top: -1.5em; margin-bottom: 1.5em; display: block; border-radius: 0 0 0 2.5em; box-shadow: 0 6px 8px rgba(29, 59, 99, 0.2);">
&nbsp;
</p>
