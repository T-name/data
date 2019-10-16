<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <title>网课代看</title>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=Edge,chrome=1">
    <meta name="renderer" content="webkit">
    <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
    <link rel="stylesheet" href="https://cdnjs.loli.net/ajax/libs/mdui/0.4.3/css/mdui.min.css">
    <script src="https://cdnjs.loli.net/ajax/libs/mdui/0.4.3/js/mdui.min.js"></script>
    <style>
        body {
            background-color: #FFFFFF;
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 56 28' width='56' height='28'%3E%3Cpath fill='%23EDF1F6' fill-opacity='1' d='M56 26v2h-7.75c2.3-1.27 4.94-2 7.75-2zm-26 2a2 2 0 1 0-4 0h-4.09A25.98 25.98 0 0 0 0 16v-2c.67 0 1.34.02 2 .07V14a2 2 0 0 0-2-2v-2a4 4 0 0 1 3.98 3.6 28.09 28.09 0 0 1 2.8-3.86A8 8 0 0 0 0 6V4a9.99 9.99 0 0 1 8.17 4.23c.94-.95 1.96-1.83 3.03-2.63A13.98 13.98 0 0 0 0 0h7.75c2 1.1 3.73 2.63 5.1 4.45 1.12-.72 2.3-1.37 3.53-1.93A20.1 20.1 0 0 0 14.28 0h2.7c.45.56.88 1.14 1.29 1.74 1.3-.48 2.63-.87 4-1.15-.11-.2-.23-.4-.36-.59H26v.07a28.4 28.4 0 0 1 4 0V0h4.09l-.37.59c1.38.28 2.72.67 4.01 1.15.4-.6.84-1.18 1.3-1.74h2.69a20.1 20.1 0 0 0-2.1 2.52c1.23.56 2.41 1.2 3.54 1.93A16.08 16.08 0 0 1 48.25 0H56c-4.58 0-8.65 2.2-11.2 5.6 1.07.8 2.09 1.68 3.03 2.63A9.99 9.99 0 0 1 56 4v2a8 8 0 0 0-6.77 3.74c1.03 1.2 1.97 2.5 2.79 3.86A4 4 0 0 1 56 10v2a2 2 0 0 0-2 2.07 28.4 28.4 0 0 1 2-.07v2c-9.2 0-17.3 4.78-21.91 12H30zM7.75 28H0v-2c2.81 0 5.46.73 7.75 2zM56 20v2c-5.6 0-10.65 2.3-14.28 6h-2.7c4.04-4.89 10.15-8 16.98-8zm-39.03 8h-2.69C10.65 24.3 5.6 22 0 22v-2c6.83 0 12.94 3.11 16.97 8zm15.01-.4a28.09 28.09 0 0 1 2.8-3.86 8 8 0 0 0-13.55 0c1.03 1.2 1.97 2.5 2.79 3.86a4 4 0 0 1 7.96 0zm14.29-11.86c1.3-.48 2.63-.87 4-1.15a25.99 25.99 0 0 0-44.55 0c1.38.28 2.72.67 4.01 1.15a21.98 21.98 0 0 1 36.54 0zm-5.43 2.71c1.13-.72 2.3-1.37 3.54-1.93a19.98 19.98 0 0 0-32.76 0c1.23.56 2.41 1.2 3.54 1.93a15.98 15.98 0 0 1 25.68 0zm-4.67 3.78c.94-.95 1.96-1.83 3.03-2.63a13.98 13.98 0 0 0-22.4 0c1.07.8 2.09 1.68 3.03 2.63a9.99 9.99 0 0 1 16.34 0z'%3E%3C/path%3E%3C/svg%3E");
        }

        .mdui-col-xs-3 .mdui-select {
            float: right;
        }
    </style>
</head>
<body class="mdui-theme-primary-indigo mdui-theme-accent-red mdui-appbar-with-toolbar">

<header class="mdui-appbar mdui-appbar-fixed">
    <div class="mdui-toolbar mdui-color-theme">
        <a class="mdui-btn mdui-btn-icon" mdui-drawer="{target: '#left-drawer', swipe: true}"><i
                class="mdui-icon material-icons">menu</i></a>
        <a class="mdui-typo-title">网课代看</a>
        <div class="mdui-toolbar-spacer"></div>
    </div>
</header>

<div class="mdui-drawer mdui-drawer-close" id="left-drawer">
    <ul class="mdui-list" mdui-collapse="{accordion: true}" style="margin-bottom: 76px;">
        <li class="mdui-list-item mdui-ripple" mdui-dialog="{target: '#info'}">
            <i class="mdui-list-item-icon mdui-icon material-icons">info</i>
            <div class="mdui-list-item-content">关于</div>
        </li>
        <li class="mdui-divider"></li>
        <div class="mdui-m-l-2 mdui-typo mdui-text-color-theme-disabled">
            <p>V 1.0</p>
        </div>
    </ul>
</div>

<div class="mdui-dialog" id="info">
    <div class="mdui-dialog-title">关于</div>
    <div class="mdui-dialog-content">MDUI前端框架<br/>by：小嵩</div>
    <div class="mdui-dialog-actions">
        <button class="mdui-btn mdui-ripple" mdui-dialog-confirm>确定</button>
    </div>
</div>

<div class="mdui-container mdui-m-y-5" style="max-width: 840px">
    <div class="mdui-card">

        <!-- 卡片头部，包含头像、标题、副标题 -->
        <div  class="mdui-card-header">

            <img class="mdui-card-header-avatar" src="https://i.loli.net/2019/10/16/clD9YTWoVnqFMRH.jpg"/>
            <div class="mdui-card-header-title">小嵩</div>
            <div class="mdui-card-header-subtitle">1874434844</div>
        </div>

        <!-- 卡片的媒体内容，可以包含图片、视频等媒体内容，以及标题、副标题 -->
        <div class="mdui-card-media">

            <img src="https://i.loli.net/2019/10/16/fGBOb16I8uvDFli.jpg"/>


            <!-- 卡片中可以包含一个或多个菜单按钮 -->
<!--            <div class="mdui-card-menu">-->
<!--                <button class="mdui-btn mdui-btn-icon mdui-text-color-white"><i class="mdui-icon material-icons">share</i></button>-->
<!--            </div>-->
        </div>

        <!-- 卡片的标题和副标题 -->
        <div class="mdui-card-primary">
            <div class="mdui-card-primary-title">网课 代看</div>
            <div class="mdui-card-primary-subtitle">超星学习通 智慧树 等等</div>
        </div>

        <!-- 卡片的内容 -->
        <div class="mdui-card-content">要代看的同学可以联系我们哦，5台电脑，3台服务器时刻在线待刷哦。
        </div>

        <!-- 卡片的按钮 -->
        <div class="mdui-card-actions">
            <button  class="mdui-btn mdui-ripple" onclick="mdui.alert('请使用QQ扫描二维码联系我们')">联系我们</button>
<!--            <button class="mdui-btn mdui-ripple"></button>-->
<!--            <button class="mdui-btn mdui-btn-icon mdui-float-right"><i class="mdui-icon material-icons">expand_more</i></button>-->
<!--      -->
       </div>

    </div>
</div>
</body>

</html>
