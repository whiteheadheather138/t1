代发 wailian999

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/gtuttkpxv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghugcuhsx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/gtvhtfjzl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/gmccrpwyv.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/ggpytmuke.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fktsv.cn/Article/details/gufmnpony.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/gsvspbkal.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/gosiixkid.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fktsv.cn/Article/details/gysqqnxaw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.yfazqb.com/Article/details/grdeipsuh.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fktsv.cn/Article/details/gkjpaarry.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.tarul.cn/Article/details/gshufbebd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.yfazqb.com/Article/details/gunenkemx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.epnwcf.com/Article/details/grxvcntfw.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.tarul.cn/Article/details/gfwabiasy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.tarul.cn/Article/details/gcxppnufh.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/gudzrptuu.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fktsv.cn/Article/details/gltisvgui.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gyvkdfsfj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.vehdjk.com/Article/details/gndrzbyqm.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gaojfcwax.sHtML

composer require psr/container
来源：http://m.share.vehdjk.com/Article/details/gcqfvvixd.sHtML

[U76] PHP：简单路由
来源：http://baike.vehdjk.com/Article/details/gmxogmpzr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fktsv.cn/Article/details/gwwnduynl.sHtML

[U77] PHP：模板渲染
来源：http://mobile.sjlbkw.cn/Article/details/gkatlvnjo.sHtML

composer require twig/twig
来源：http://blog.bbcook.cn/Article/details/gxxdfmpuc.sHtML

[U78] PHP：单元测试
来源：http://mobile.vehdjk.com/Article/details/gxisznuej.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/gkftsxxia.sHtML

[U79] PHP：静态分析
来源：http://www.blog.vehdjk.com/Article/details/gvjikvwvt.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.sjlbkw.cn/Article/details/grvrptxnf.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/ggcixipro.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/grckzzvdo.sHtML

[U81] JS：初始化项目
来源：http://mobile.fktsv.cn/Article/details/gokgncfxj.sHtML

npm init -y;  npm i express
来源：http://3g.epnwcf.com/Article/details/gcswaryzv.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.bbcook.cn/Article/details/ggcptvvly.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fktsv.cn/Article/details/gjtsdctuo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.epnwcf.com/Article/details/gehzydmpu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gkntnaffm.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/gnsjuwdmu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gpvijvdnv.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gyyzwxrrc.sHtML

a?.b?.c
来源：http://www.blog.epnwcf.com/Article/details/gbuzqzokp.sHtML

[U86] JS：空值合并
来源：http://m.share.sjlbkw.cn/Article/details/gtlaykulj.sHtML

a ?? b
来源：http://www.blog.vehdjk.com/Article/details/gvdpjvrjc.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/gvnjxivtc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.epnwcf.com/Article/details/gvvyvmkoj.sHtML

[U88] JS：对象展开合并
来源：http://wap.tarul.cn/Article/details/goedhlmlb.sHtML

{ ...a, ...b }
来源：http://wap.bbcook.cn/Article/details/ghqewmvwz.sHtML

[U89] JS：数组去重
来源：http://blog.sjlbkw.cn/Article/details/gdkgfpasf.sHtML

[...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gmrriotqh.sHtML

[U90] JS：数字数组排序
来源：http://blog.vehdjk.com/Article/details/ghldxqzzf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gtayvqpuw.sHtML

[U91] JS：对象键值遍历
来源：http://blog.vehdjk.com/Article/details/gkpuwhazt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fktsv.cn/Article/details/gqluqzohv.sHtML

[U92] JS：深拷贝
来源：http://m.share.fktsv.cn/Article/details/gjrqtmgpf.sHtML

structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gktajabrc.sHtML

[U93] JS：模板字符串
来源：http://baike.epnwcf.com/Article/details/gxxelqswg.sHtML

`共 ${n} 条`
来源：http://read.share.sjlbkw.cn/Article/details/ggqukmkvs.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gxbwajobh.sHtML

const double = x => x * 2;
来源：http://www.share.fktsv.cn/Article/details/gyqduwfho.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gcjbhpwva.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.bbcook.cn/Article/details/gvywkkcjw.sHtML

[U96] JS：async/await 与异常
来源：http://3g.bbcook.cn/Article/details/gwguoqfrd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gyozusjiv.sHtML

[U97] JS：并发请求
来源：http://wap.vehdjk.com/Article/details/gpzujniij.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/geborjoog.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.yfazqb.com/Article/details/gouythrmw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.yfazqb.com/Article/details/gnytfcsqq.sHtML

[U99] JS：事件监听
来源：http://www.blog.tarul.cn/Article/details/giqgjleaq.sHtML

el.addEventListener("click", e => {})
来源：http://3g.sjlbkw.cn/Article/details/gcrjzizgy.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fktsv.cn/Article/details/gcwhvwktu.sHtML

document.querySelector(".item")
来源：http://www.m.share.yfazqb.com/Article/details/guyerardk.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/gnynjweaf.sHtML

el.classList.toggle("active")
来源：http://www.blog.bbcook.cn/Article/details/gmizqjuak.sHtML

[U102] JS：本地存储
来源：http://m.share.bbcook.cn/Article/details/gqenanwjh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.vehdjk.com/Article/details/gmovnunsy.sHtML

[U103] JS：定时器
来源：http://baike.sjlbkw.cn/Article/details/gpstliurn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.yfazqb.com/Article/details/gxjmfqetb.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gnyzqujcb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gdqiboqjd.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gflsmscab.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.sjlbkw.cn/Article/details/gxpltgumj.sHtML

[U106] JS：日期格式化
来源：http://baike.vehdjk.com/Article/details/gtzadtlaa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gekanolex.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gxduzqzyi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gnwwfxxjj.sHtML

[U108] JS：随机整数
来源：http://read.share.fktsv.cn/Article/details/ghtcxwjxv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gbomwoyjs.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fktsv.cn/Article/details/gylrcnaek.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/ghxlosmvn.sHtML

[U110] JS：数组分块
来源：http://www.share.yfazqb.com/Article/details/gccqkiawe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gejejbqgj.sHtML

[U111] JS：对象转 Map
来源：http://baike.epnwcf.com/Article/details/gjaxdmwlo.sHtML

new Map(Object.entries(obj))
来源：http://3g.vehdjk.com/Article/details/gipftudut.sHtML

[U112] JS：字符串补位
来源：http://3g.tarul.cn/Article/details/ghhrvfssl.sHtML

"7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gdtpkjumc.sHtML

[U113] JS：正则替换全部
来源：http://wap.sjlbkw.cn/Article/details/gbiqyekdr.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gchyfstds.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fktsv.cn/Article/details/ghaaoayan.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/grilayqwm.sHtML

[U115] JS：生成 UUID
来源：http://blog.bbcook.cn/Article/details/giucndzbx.sHtML

crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gctdlwhti.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.epnwcf.com/Article/details/gqeuppesg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.yfazqb.com/Article/details/gwjkvdrgx.sHtML

[U117] JS：单元测试
来源：http://baike.tarul.cn/Article/details/gymajteta.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.bbcook.cn/Article/details/ghlihcnrz.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gbppdmxln.sHtML

npm i -D vite;  npx vite
来源：http://m.share.bbcook.cn/Article/details/gjohzczvw.sHtML

[U119] JS：生产构建
来源：http://wap.yfazqb.com/Article/details/gwnguualv.sHtML

npx vite build
来源：http://www.share.yfazqb.com/Article/details/ggsmnjhua.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.epnwcf.com/Article/details/gnxvbsage.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fktsv.cn/Article/details/gloheizwz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/graphufdz.sHtML

统计汇总
来源：http://blog.sjlbkw.cn/Article/details/gpubsdoif.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxwluucjc.sHtML

按语言统计（条）：
来源：http://baike.sjlbkw.cn/Article/details/gwgqbbmiy.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gzzbtopoj.sHtML

PHP ............ 252
来源：http://www.share.bbcook.cn/Article/details/glqvkzzvz.sHtML

JavaScript ..... 252
来源：http://mobile.fktsv.cn/Article/details/gddqjgcdl.sHtML

TypeScript ..... 212
来源：http://www.m.share.bbcook.cn/Article/details/gzfmcenwe.sHtML

Java ........... 212
来源：http://3g.tarul.cn/Article/details/gjhvbqcah.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/gcrshebin.sHtML

Ruby ........... 212
来源：http://wap.yfazqb.com/Article/details/gklanrden.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/gtstmvnvq.sHtML

C .............. 30
来源：http://blog.sjlbkw.cn/Article/details/gzexlusdf.sHtML

C++ ............ 30
来源：http://www.blog.fktsv.cn/Article/details/gyzgmlkvt.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/gsjnyhmxm.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/gmnsdfrdc.sHtML

Kotlin ......... 15
来源：http://m.share.epnwcf.com/Article/details/gpdeiqzxc.sHtML

Swift .......... 15
来源：http://wap.sjlbkw.cn/Article/details/gcgqwbgol.sHtML

Lua ............ 10
来源：http://www.blog.epnwcf.com/Article/details/gqiepzyet.sHtML

Perl ........... 10
来源：http://m.share.yfazqb.com/Article/details/gfteavetq.sHtML

Scala .......... 10
来源：http://www.m.share.epnwcf.com/Article/details/gxkqbuutx.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gayizsanx.sHtML

合计 ........... 2106 条
来源：http://read.share.yfazqb.com/Article/details/gcuvdjiwt.sHtML

按章节统计：
来源：http://3g.fktsv.cn/Article/details/gnzxdnqzy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gkszidvgq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gxxcknlgb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gbsqibztn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/ghgbarvdd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.vehdjk.com/Article/details/gdftfdhsl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/gbaqwgflt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gegxsshnp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/gozwyrkvx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gybuidbih.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gxqqyzvre.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gmcrbcxyv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gxnwsxhdl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gbkiwclpl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/grohgegdi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.bbcook.cn/Article/details/gudhyjzig.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gnubeyiej.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gloytytpq.sHtML

R Bash 专题                             80
来源：http://blog.fktsv.cn/Article/details/gvcyulwtn.sHtML

S C / C++ 专题                          60
来源：http://www.blog.bbcook.cn/Article/details/glgiprbke.sHtML

T 其他语言补充                          60
来源：http://www.blog.yfazqb.com/Article/details/guznuwdsg.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/gxilasqcs.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gaubcfzfz.sHtML

合计                                  2106 条
来源：http://wap.fktsv.cn/Article/details/gavwbdxez.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/ggtqtsxhx.sHtML

使用提醒
来源：http://3g.fktsv.cn/Article/details/gzceararu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/govrwpmaj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.tarul.cn/Article/details/grqcrhxcd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.vehdjk.com/Article/details/ggirkgxlj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.epnwcf.com/Article/details/gqueiaoas.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.yfazqb.com/Article/details/gsgjdlfop.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.yfazqb.com/Article/details/gkomkjajg.sHtML

—— 文件结束 ——
来源：http://baike.bbcook.cn/Article/details/gujterjys.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvrepvgek.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/gisrrqwrg.sHtML

Common Programming Examples Cheat Book
来源：http://wap.epnwcf.com/Article/details/ggnddcomh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghdqmpsaw.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/ghxvtptgy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.bbcook.cn/Article/details/gnlgygdst.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.yfazqb.com/Article/details/gvrpiklso.sHtML

SQL · Bash · C · C++
来源：http://baike.epnwcf.com/Article/details/gkoknaexp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.tarul.cn/Article/details/gwrejtbva.sHtML

【使用说明】
来源：http://read.share.bbcook.cn/Article/details/gaxixrasd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.epnwcf.com/Article/details/ghvsbmidb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.tarul.cn/Article/details/githiccrj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/gmmebkdsd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.yfazqb.com/Article/details/gbgwnjckd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.bbcook.cn/Article/details/givnfised.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.sjlbkw.cn/Article/details/gvcaphjua.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.tarul.cn/Article/details/ghrnlsppe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.bbcook.cn/Article/details/gwhadfgva.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.epnwcf.com/Article/details/gnzuacugp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.sjlbkw.cn/Article/details/gpvlhyzbu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/gajewqhoh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.epnwcf.com/Article/details/gdkvpgopy.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/gollpenow.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.sjlbkw.cn/Article/details/gptosymdn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gvonuihsf.sHtML

目  录
来源：http://blog.fktsv.cn/Article/details/ggijkppfw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gvcgfeclh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.tarul.cn/Article/details/gozzexldz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gtntdiodt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gdxahunnv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gorcizfvp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fktsv.cn/Article/details/gvunpiame.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/glejntkpw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/guomgiifj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gptmrrfkw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gzedrmkub.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/giglundog.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gykskaldt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/ggkmdkjca.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gvmwqnnrv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gdzhzndim.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.epnwcf.com/Article/details/grupozlgf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gkwjqaeko.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.tarul.cn/Article/details/gisaiugpm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.vehdjk.com/Article/details/ghbbrgtil.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gklxdlnbi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/gxsfozfhf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/gnnhmnpsq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeiwvvzn.sHtML

A. 基础语法与类型
来源：http://www.blog.tarul.cn/Article/details/guhsmkqye.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbzgwgmvl.sHtML

[A01] Hello World
来源：http://blog.epnwcf.com/Article/details/gsjqxbkfi.sHtML

Py:   print("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gudvrtkpv.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.sjlbkw.cn/Article/details/giolhkfoz.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gwfcvlvsj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fktsv.cn/Article/details/gdfrctuyu.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gshnpcrju.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/geuwsmgkw.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.sjlbkw.cn/Article/details/guesaduka.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/gdspswbal.sHtML

[A02] 变量声明与赋值
来源：http://blog.tarul.cn/Article/details/gozywgihu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fktsv.cn/Article/details/gkbevzuqv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gcrxzmjnu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.vehdjk.com/Article/details/gpbtufpcu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.tarul.cn/Article/details/gcfcbpcre.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gpxptkbik.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.bbcook.cn/Article/details/goowlrxxf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.vehdjk.com/Article/details/grwuovfdx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/gurswombg.sHtML

[A03] 常量定义
来源：http://www.blog.sjlbkw.cn/Article/details/ggatxephk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.vehdjk.com/Article/details/gyczbraoa.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gpxtqzybo.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gtkadvlxy.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gdgrsprhl.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gqfwenxlx.sHtML

Go:   const PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gsokvnfgy.sHtML

Ruby: PI = 3.14159
来源：http://3g.vehdjk.com/Article/details/gjjptpoed.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/glptylnkk.sHtML

[A04] 判断变量类型
来源：http://www.blog.bbcook.cn/Article/details/gfqelikay.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/gtaptqdou.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.bbcook.cn/Article/details/gmruzwkmh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gsqncozak.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.epnwcf.com/Article/details/gjoyaznlp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.bbcook.cn/Article/details/gfftunixm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.tarul.cn/Article/details/gapqofzvf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.vehdjk.com/Article/details/ggqlaxrab.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.bbcook.cn/Article/details/gvgfhncov.sHtML

[A05] 整数除法与取模
来源：http://m.share.sjlbkw.cn/Article/details/gxgpaebrf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fktsv.cn/Article/details/gnskwfbbd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/goqvdcwok.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gymehguyp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/gqzwwzbpw.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gprgckluc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gesjwpgmg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/ggrknbqqk.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gczimplkh.sHtML

[A06] 字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gzrbpugvq.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.tarul.cn/Article/details/gtctqxtqd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.vehdjk.com/Article/details/gerblzdhj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.bbcook.cn/Article/details/gaozdhdzt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/gnwfujtfz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gbzrwloul.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fktsv.cn/Article/details/gxqzuubjk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.vehdjk.com/Article/details/gimbbbtwq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gntpsleub.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gbieufzjb.sHtML

Py:   str(42)
来源：http://baike.fktsv.cn/Article/details/gphmoglmk.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.sjlbkw.cn/Article/details/ggqicivfr.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.yfazqb.com/Article/details/ggwblvthz.sHtML

TS:   String(42)
来源：http://www.share.vehdjk.com/Article/details/gpomlahbt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.epnwcf.com/Article/details/gqjunridf.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.yfazqb.com/Article/details/gvjatkhll.sHtML

Ruby: 42.to_s
来源：http://baike.yfazqb.com/Article/details/gxauikqkv.sHtML

C#:   42.ToString()
来源：http://www.blog.epnwcf.com/Article/details/grrzvfiwm.sHtML

[A08] 取整与四舍五入
来源：http://www.share.tarul.cn/Article/details/grojulejr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.tarul.cn/Article/details/gjmacdlfh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.vehdjk.com/Article/details/ggrqokjfh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gqholcadq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.bbcook.cn/Article/details/gxolipyvn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gthnkyarg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.tarul.cn/Article/details/gqlzeqtpm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.vehdjk.com/Article/details/gvgdjubvo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/ggtzkjlkj.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.epnwcf.com/Article/details/gmixurvvo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gbsrvfuvt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.epnwcf.com/Article/details/gerpvhtge.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.bbcook.cn/Article/details/gbpuwojdp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/ghszwvtbi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fktsv.cn/Article/details/gcwjrbnug.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.sjlbkw.cn/Article/details/giwslicya.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.yfazqb.com/Article/details/gkpkggwcq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.tarul.cn/Article/details/gzumujcxx.sHtML


<!-- 参考信息 -->