<!-- docs/_sidebar.md -->
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

.sidebartitle {
    font-size: 1.5em;
    font-weight: 600;
    color: transparent; 
    background: linear-gradient(135deg, oklch(0.9029 0.0419 213.12), oklch(0.7706 0.1283 190), oklch(0.6471 0.1727 265.46)) text;
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


<p class="sidebartitle">「DP IV 官方文档」</p>

* [首页](pages/README)
* [更新日志](pages/updatelogs)
* [赞助相关](pages/sponsor.md)
* [Tempest](pages/tempest)
* [交易所指南](pages/market)
* [每日副本](pages/每日副本)
* [存储相关](pages/storage)

<p style="margin-top: -1.5em; margin-bottom: 1.5em; display: block; border-radius: 0 0 0 2.5em; box-shadow: 0 6px 8px rgba(29, 59, 99, 0.2);">
&nbsp;
</p>

<p class="sidebarsubtitle">「玩家攻略」</p>

* [指令大全](pages/指令大全)
* [(g1)生存指北](pages/g1)
* [(g2)天泽岛引导](pages/g2)



<p style="margin-top: -1.5em; margin-bottom: 1.5em; display: block; border-radius: 0 0 0 2.5em; box-shadow: 0 6px 8px rgba(29, 59, 99, 0.2);">
&nbsp;
</p>

<p class="sidebarsubtitle">「附录」</p>

* [如何为WIKI贡献?](pages/CONTRIBUTING)
* [设计规范](pages/DESIGNCODE)