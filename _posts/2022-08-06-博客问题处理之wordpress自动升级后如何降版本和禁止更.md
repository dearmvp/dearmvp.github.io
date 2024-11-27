---
layout: post
title: 博客问题处理之wordpress自动升级后如何降版本和禁止更新
date: 2022-08-06 00:03
author: wangms
comments: true
categories: [wordpress, 文章, 随笔]
---
<h2>一、问题和处理过程</h2>
<p>今天浏览网站首页发现显示样式有所变化，主要体现在首页文章列表摘要信息显示的长度过长</p>
<p><img src="https://img.wangms.com/blog/1659423783332-618dd898-d724-45da-91a5-690f1dd02dc1.png" alt="img" /></p>
<p>WordPress 版本回退插件 WP Downgrade</p>
<p><img src="https://img.wangms.com/blog/1659423863850-7683cfb2-54fc-4a3a-b44c-3fbdab2a64cc.png" alt="img" /></p>
<p>使用起来比较简单，红框是重点操作步骤  </p>
<p>WordPress Target Version 填入想要回退到的版本点击保存更改，如果填写的版本可以识别成功，会出现黄色框的提示。如下</p>
<blockquote>
<p>In order to perform the upgrade/downgrade to WP 5.9.3 please go to Update Core.</p>
<p>Up-/Downgrade Core</p>
</blockquote>
<p><img src="https://img.wangms.com/blog/1659423962252-f4302150-6c15-40e9-b005-0242432c60b2.png" alt="img" /></p>
<p>直接点击Up-/Downgrade Core按钮后会跳到仪表盘更新页面。</p>
<p><img src="https://img.wangms.com/blog/1659424152643-5d4c1f89-534d-4fc5-adac-2277e1591dba.png" alt="img" /></p>
<p>不出意外的话会安装成功（此插件有回退版本失败的可能，网站数据重要的话，需提前备份），直接跳到了对应版本宣传页面。</p>
<p><img src="https://img.wangms.com/blog/1659424451306-8dc02ce1-a69d-4a46-887c-794e414a6e03.png" alt="img" /></p>
<p>再次访问首页发现也会到最初合理样子，网站内容按摘要的形式显示出来，看起来比上面异常页面要舒服些。</p>
<p><img src="https://img.wangms.com/blog/1659424502918-cc079aa6-f3d0-482d-b032-c3d73af6d1ba.png" alt="img" /></p>
<h2>二、如何避免自动更新</h2>
<p>禁止更新</p>
<p>网站根目录找到wp-config.php文件在最下方添加如下代码</p>
<blockquote>
<p>/*<em> 关闭WordPress自动更新升级 </em>/</p>
<p>define('AUTOMATIC_UPDATER_DISABLED', true);</p>
</blockquote>
<h2>三、wordpress版本库</h2>
<p>WordPress 版本库列表 <a href="https://cn.wordpress.org/download/releases/">https://cn.wordpress.org/download/releases/</a></p>
<p>我是按着版本库恢复到了5.9.3 的版本后页面显示正常了</p>
