代发 wailian999

[U55] PHP：match 表达式
来源：http://ufd.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qgj.zhixingplan.top

[U56] PHP：命名参数
来源：http://gbr.gogol.net.cn

f(a: 1, b: 2)
来源：http://vjm.hfpthk.cn

[U57] PHP：字符串插值
来源：http://sli.pengpengdd.cyou

"值: {$a}"
来源：http://sec.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://sls.yfazqb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://okt.sufxvd.cn

[U59] PHP：自定义排序
来源：http://kmn.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jwh.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://vzq.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dcv.zhijiandao.cn

[U61] PHP：正则
来源：http://whb.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mzc.dashuyun.cn

[U62] PHP：日期对象
来源：http://dlb.yj20258888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://phs.guowangkeji.top

[U63] PHP：文件读写
来源：http://abq.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mtp.fehbvm.com

[U64] PHP：目录遍历
来源：http://ytt.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://tqn.iojbl.cn

[U65] PHP：会话
来源：http://ezt.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vkl.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://txo.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rwr.ivvv.top

[U67] PHP：处理文件上传
来源：http://dla.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ecx.shuidangran.top

[U68] PHP：PDO 连接
来源：http://ddi.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xyg.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://arl.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cvm.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://kch.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jzo.316326.xyz

[U71] PHP：抛出异常
来源：http://xpt.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://cmg.yongpay.top

[U72] PHP：写错误日志
来源：http://hox.jiagoushi.top

error_log("失败: " . $e->getMessage());
来源：http://icu.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://jbz.yonumen.top

parse_ini_file("config.ini", true)
来源：http://swu.havefunace.top

[U74] PHP：读取环境变量
来源：http://sej.zycfv.cn

getenv("APP_ENV") ?: "production"
来源：http://vdt.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://cgd.hywenlv.cn

composer require psr/container
来源：http://gtq.gzhubu.top

[U76] PHP：简单路由
来源：http://jed.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vag.hfpthk.cn

[U77] PHP：模板渲染
来源：http://lsu.zycfv.cn

composer require twig/twig
来源：http://oea.meibo888.top

[U78] PHP：单元测试
来源：http://fzs.zdqjudy.top

composer require --dev phpunit/phpunit
来源：http://ikx.ybcxt.top

[U79] PHP：静态分析
来源：http://msx.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://qvl.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://piq.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xno.fzhhl.top

[U81] JS：初始化项目
来源：http://obd.tian-w.cn

npm init -y;  npm i express
来源：http://sxh.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://vby.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bos.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://wnf.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ltf.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://xht.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rni.birdmap.top

[U85] JS：可选链
来源：http://isa.cucudq.cn

a?.b?.c
来源：http://ixd.haohaochexian.top

[U86] JS：空值合并
来源：http://tqx.ydjk.org.cn

a ?? b
来源：http://wlq.ctjpmb.com

[U87] JS：解构默认值
来源：http://ygd.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://cvk.hywenlv.cn

[U88] JS：对象展开合并
来源：http://iip.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://ygx.bjfxy.top

[U89] JS：数组去重
来源：http://psy.tanke756.top

[...new Set(arr)]
来源：http://nle.52xcode.cn

[U90] JS：数字数组排序
来源：http://wrv.havefunace.top

[...arr].sort((a, b) => a - b)
来源：http://dsg.yonumen.top

[U91] JS：对象键值遍历
来源：http://aoe.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jbj.c1oappe.top

[U92] JS：深拷贝
来源：http://xmy.yfazqb.com

structuredClone(obj)
来源：http://knn.hesvh.cn

[U93] JS：模板字符串
来源：http://utk.svipenyu.cn

`共 ${n} 条`
来源：http://brm.xuanzx.com

[U94] JS：箭头函数
来源：http://fhf.tianlin.xyz

const double = x => x * 2;
来源：http://dxb.aizwys.cn

[U95] JS：Promise 包装
来源：http://qfu.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://gti.yj20258888.top

[U96] JS：async/await 与异常
来源：http://ncg.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cws.xziqi.cn

[U97] JS：并发请求
来源：http://vsl.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ixq.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://xct.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hlz.smart0.xyz

[U99] JS：事件监听
来源：http://ivt.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://ysj.xziqi.cn

[U100] JS：DOM 查询
来源：http://tmu.haohaochexian.top

document.querySelector(".item")
来源：http://qgf.xinyue.icu

[U101] JS：classList 操作
来源：http://ies.tian-w.cn

el.classList.toggle("active")
来源：http://wkn.dashuyun.cn

[U102] JS：本地存储
来源：http://hcy.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cze.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://yki.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iuv.xinyue.icu

[U104] JS：防抖
来源：http://bpw.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://elf.yj202588.top

[U105] JS：节流
来源：http://pyw.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jaz.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://vmk.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://puo.dianchejie.cn

[U107] JS：数字千分位
来源：http://jig.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hyi.shangyingyoupin.top

[U108] JS：随机整数
来源：http://goq.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ppp.feifeiyinyue.top

[U109] JS：数组分组
来源：http://trp.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://uet.jlsjyb.cn

[U110] JS：数组分块
来源：http://zpp.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bbd.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://dzj.jqgfzy.top

new Map(Object.entries(obj))
来源：http://yhl.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://doh.dianchejie.cn

"7".padStart(3, "0")
来源：http://tkq.shzxlz.cn

[U113] JS：正则替换全部
来源：http://zui.gzhubu.top

s.replaceAll("a", "b")
来源：http://dia.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://gxw.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://twp.52xcode.cn

[U115] JS：生成 UUID
来源：http://bcz.guannengcc.top

crypto.randomUUID()
来源：http://hfb.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://sho.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://srp.fktsv.cn

[U117] JS：单元测试
来源：http://bvh.hammf.cn

npm i -D vitest;  npx vitest
来源：http://qwr.epnwcf.com

[U118] JS：开发服务器
来源：http://cyq.9152youxi.cn

npm i -D vite;  npx vite
来源：http://ckk.fzhhl.top

[U119] JS：生产构建
来源：http://vso.nanxuanxn.top

npx vite build
来源：http://vmb.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://zlc.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://ewn.kuanghao11.cn

================================================================================
来源：http://wol.uphjek.com

统计汇总
来源：http://zte.zycfv.cn

================================================================================
来源：http://zhe.aibaodan.cn

按语言统计（条）：
来源：http://rpj.nanxinkj.top

Python ......... 252
来源：http://dnh.uphjek.com

PHP ............ 252
来源：http://swj.yongpay.top

JavaScript ..... 252
来源：http://yay.sufxvd.cn

TypeScript ..... 212
来源：http://vwd.jqgufenzy.top

Java ........... 212
来源：http://jjb.jqgfzy.top

Go ............. 212
来源：http://osz.hysaishi.cn

Ruby ........... 212
来源：http://lgm.aibaodan.cn

C# ............. 212
来源：http://iyt.aibaodan.cn

C .............. 30
来源：http://dvw.fktsv.cn

C++ ............ 30
来源：http://wyn.mhx1999.top

SQL ............ 90
来源：http://bso.ivvv.top

Bash ........... 80
来源：http://ahg.hammf.cn

Kotlin ......... 15
来源：http://szr.fzhhl.top

Swift .......... 15
来源：http://nsk.ywan-chungtsiang.top

Lua ............ 10
来源：http://lya.jinqigfzy.top

Perl ........... 10
来源：http://cra.wangdashe.top

Scala .......... 10
来源：http://tws.9152youxi.cn

------------------------------------
来源：http://fyq.sufxvd.cn

合计 ........... 2106 条
来源：http://ybr.tian-w.cn

按章节统计：
来源：http://qho.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jre.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eti.yj20258888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eyq.gaohongyu789.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eup.dashuyun.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dki.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ftn.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lfw.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rrs.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ldr.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://adh.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pfg.chenzaomai.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ivo.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gsd.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yac.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://obl.xylfe.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ybs.cdnleiting.top

Q SQL 专题                              90
来源：http://cba.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://ebe.52xcode.cn

S C / C++ 专题                          60
来源：http://mmz.havefunace.top

T 其他语言补充                          60
来源：http://aht.jiagoushi.top

U 高频实用片段                         120
来源：http://pak.xziqi.cn

------------------------------------
来源：http://duc.yj20258888.top

合计                                  2106 条
来源：http://qgu.smart0.xyz

--------------------------------------------------------------------------------
来源：http://wgk.andypj.xyz

使用提醒
来源：http://zsc.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://fkp.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://djz.cheryme.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://asw.guowangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wyg.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pjo.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pfb.epnwcf.com

—— 文件结束 ——
来源：http://olu.yuxming.cn

================================================================================
来源：http://zny.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://nyz.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://iaz.jqgufenzy.top

================================================================================
来源：http://cjp.aizwys.cn

【收录内容】
来源：http://adt.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://rzp.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bby.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://sss.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dpr.shanyushiyangkeji.top

【使用说明】
来源：http://vge.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qmm.sweek.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://npf.ydzc1.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rzy.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://svk.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://brw.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qht.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qhz.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eiv.chenlongwang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sje.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tnp.shangyingyoupin.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rgn.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vhr.fktsv.cn

【文件统计】
来源：http://wmd.shanyushiyangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gjx.yj202588.top

--------------------------------------------------------------------------------
来源：http://ufh.fengsongda.top

目  录
来源：http://ejc.epnwcf.com

--------------------------------------------------------------------------------
来源：http://mkq.hnqzz.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hwc.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ptj.sxryk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ide.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sdo.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qpr.hesvh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rhz.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ptq.vehdjk.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cyg.cqqwz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qdt.yonumen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gvd.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bss.yfazqb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tnu.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://agp.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://auh.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sdz.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wkn.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://thp.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://blv.snrcjt.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://grd.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://osh.gaohongyu789.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cce.fehbvm.com

================================================================================
来源：http://mwn.daria6918.cn

A. 基础语法与类型
来源：http://czn.yj202588.top

================================================================================
来源：http://oda.tarul.cn

[A01] Hello World
来源：http://dfg.pengpengdd.cyou

Py:   print("Hello, World!")
来源：http://sdb.jinqigufen.top

PHP:  echo "Hello, World!";
来源：http://fls.ybcxt.top

JS:   console.log("Hello, World!");
来源：http://sgy.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://apy.ivvv.top

Java: System.out.println("Hello, World!");
来源：http://ocf.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://vrd.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://kiz.9152youxi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pkc.tianlin.xyz

[A02] 变量声明与赋值
来源：http://tjo.jqgufenzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cot.tarul.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ayd.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://awa.svipenyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vqw.cqqwz.cn

Java: String name = "Alex"; int age = 20;
来源：http://lty.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://yhx.gogol.net.cn

Ruby: name = "Alex"; age = 20
来源：http://bno.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://jsu.nanxuanxn.top

[A03] 常量定义
来源：http://ive.vqdsnc.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ktf.tarul.cn

PHP:  const PI = 3.14159;
来源：http://dua.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://qgo.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://uje.tian-w.cn

Java: static final double PI = 3.14159;
来源：http://iqu.0kj1m.cn

Go:   const PI = 3.14159
来源：http://xyv.fzhhl.top

Ruby: PI = 3.14159
来源：http://ndn.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://blc.cashguo.top

[A04] 判断变量类型
来源：http://siq.nanxinkj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rfj.xuetiantiany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fsd.zhiwuduotai.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nyo.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://fnz.ybcxt.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lvk.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://rdh.dianchejie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tea.zycfv.cn

C#:   x.GetType().Name; x is int
来源：http://syp.quarkkingdee.top

[A05] 整数除法与取模
来源：http://qcd.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dac.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zwx.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vwm.iojbl.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://czx.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://cny.52xcode.cn

Go:   7 / 2; 7 % 2
来源：http://hqq.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://egz.tanke756.top

C#:   7 / 2; 7 % 2
来源：http://rpv.yfazqb.com

[A06] 字符串转数字
来源：http://vyc.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://anf.yongpay.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rau.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jik.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://idp.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ofg.vehdjk.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sbw.yongpay.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rzl.tianlin.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dbg.yj20258.top

[A07] 数字转字符串
来源：http://bpe.snrcjt.cn

Py:   str(42)
来源：http://zfl.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://fbv.yongpay.top

JS:   String(42); (42).toString()
来源：http://dok.aibaodan.cn

TS:   String(42)
来源：http://ikx.haohaochexian.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hky.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://msx.yfazqb.com


<!-- 参考信息 -->