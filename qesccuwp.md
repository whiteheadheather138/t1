代发 wailian999

[U63] PHP：文件读写
来源：http://bfn.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qqb.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://sia.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://kll.feifeiyinyue.top

[U65] PHP：会话
来源：http://rwe.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gat.tarul.cn

[U66] PHP：设置 Cookie
来源：http://gjx.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iiz.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://jee.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://voe.tianlin.xyz

[U68] PHP：PDO 连接
来源：http://lfw.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://npk.mhx1999.top

[U69] PHP：PDO 预处理
来源：http://pvc.jinyuanbaomall.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qbt.epnwcf.com

[U70] PHP：PDO 事务
来源：http://wpz.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kjq.zhixingplan.top

[U71] PHP：抛出异常
来源：http://xps.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://cap.yueranfly.top

[U72] PHP：写错误日志
来源：http://irf.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://toz.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://xvv.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://vqw.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://wlz.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://jql.ivvv.top

[U75] PHP：依赖注入
来源：http://uww.dianchejie.cn

composer require psr/container
来源：http://xhg.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://hdm.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iax.0kj1m.cn

[U77] PHP：模板渲染
来源：http://xwz.fanxiaobao.xyz

composer require twig/twig
来源：http://bkh.tarul.cn

[U78] PHP：单元测试
来源：http://tzz.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://jvj.yanxiufei.cn

[U79] PHP：静态分析
来源：http://apu.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://nbe.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://cum.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://ykh.yfazqb.com

[U81] JS：初始化项目
来源：http://ics.xuanzx.com

npm init -y;  npm i express
来源：http://qxe.zycfv.cn

[U82] JS：package.json 脚本
来源：http://mhp.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rah.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://yvv.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ltz.uphjek.com

[U84] JS：CommonJS 写法
来源：http://wdc.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wlk.hywenlv.cn

[U85] JS：可选链
来源：http://jhv.hywenlv.cn

a?.b?.c
来源：http://pmt.tanke756.top

[U86] JS：空值合并
来源：http://mcr.jinghuilouyu.cn

a ?? b
来源：http://bie.zdbjq.cn

[U87] JS：解构默认值
来源：http://hsm.shzxlz.cn

const { a = 1, b = 2 } = obj;
来源：http://csn.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://wsi.yueranfly.top

{ ...a, ...b }
来源：http://hpw.hongshengwenyu.top

[U89] JS：数组去重
来源：http://lmn.0kj1m.cn

[...new Set(arr)]
来源：http://hfl.guowangkeji.top

[U90] JS：数字数组排序
来源：http://mkx.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://upt.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://lgw.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zrq.fktsv.cn

[U92] JS：深拷贝
来源：http://ure.gaohongyu789.top

structuredClone(obj)
来源：http://cnc.vehdjk.com

[U93] JS：模板字符串
来源：http://kig.cdnleiting.top

`共 ${n} 条`
来源：http://npm.dianchejie.cn

[U94] JS：箭头函数
来源：http://rws.0kj1m.cn

const double = x => x * 2;
来源：http://mnw.cdnleiting.top

[U95] JS：Promise 包装
来源：http://jpc.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://mgu.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://sln.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uhj.yfazqb.com

[U97] JS：并发请求
来源：http://ixm.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cjz.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://vdl.hnqzz.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nqa.jinqigfzy.top

[U99] JS：事件监听
来源：http://otf.yvedp.cn

el.addEventListener("click", e => {})
来源：http://ouu.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://syj.gogol.net.cn

document.querySelector(".item")
来源：http://czg.jinqigufen.top

[U101] JS：classList 操作
来源：http://gzs.redwolf501.top

el.classList.toggle("active")
来源：http://nnc.yvedp.cn

[U102] JS：本地存储
来源：http://bxz.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://udj.cheryme.top

[U103] JS：定时器
来源：http://iha.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mxl.yj20258.top

[U104] JS：防抖
来源：http://yjm.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nak.shanyushiyangkeji.top

[U105] JS：节流
来源：http://xfe.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rri.andypj.xyz

[U106] JS：日期格式化
来源：http://izo.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ugz.jqgufenzy.top

[U107] JS：数字千分位
来源：http://rvj.jinghuilouyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aga.bjfxy.top

[U108] JS：随机整数
来源：http://eoo.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://emv.uphjek.com

[U109] JS：数组分组
来源：http://fpd.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://iad.gzhubu.top

[U110] JS：数组分块
来源：http://ink.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hrb.sufxvd.cn

[U111] JS：对象转 Map
来源：http://pdu.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://mtt.sjlbkw.cn

[U112] JS：字符串补位
来源：http://cdj.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://azq.jinqigufen.top

[U113] JS：正则替换全部
来源：http://iwr.yonumen.top

s.replaceAll("a", "b")
来源：http://wdp.yonumen.top

[U114] JS：JSON 深比较
来源：http://gce.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oeu.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://vlo.fanxiaobao.xyz

crypto.randomUUID()
来源：http://mcl.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://cgz.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://wrk.xinyue.icu

[U117] JS：单元测试
来源：http://ung.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://lyz.ivvv.top

[U118] JS：开发服务器
来源：http://guq.yuanzhike.top

npm i -D vite;  npx vite
来源：http://whr.andypj.xyz

[U119] JS：生产构建
来源：http://wjs.zhijiandao.cn

npx vite build
来源：http://euw.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://tdc.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://ixc.cheryme.top

================================================================================
来源：http://bbh.pengpengdd.cyou

统计汇总
来源：http://bsd.hnxiangtu.top

================================================================================
来源：http://dwx.jlsjyb.cn

按语言统计（条）：
来源：http://kgi.zhengqikj.top

Python ......... 252
来源：http://inr.wangshuangyany.cn

PHP ............ 252
来源：http://tei.yuxming.cn

JavaScript ..... 252
来源：http://hpk.c1oappe.top

TypeScript ..... 212
来源：http://byc.dashuyun.cn

Java ........... 212
来源：http://khp.xingfuxueyuan.xyz

Go ............. 212
来源：http://buq.tanke756.top

Ruby ........... 212
来源：http://eos.bjfxy.top

C# ............. 212
来源：http://slh.xingfuxueyuan.xyz

C .............. 30
来源：http://xvh.haohaochexian.top

C++ ............ 30
来源：http://ync.zycfv.cn

SQL ............ 90
来源：http://eka.fzhhl.top

Bash ........... 80
来源：http://uar.svipenyu.cn

Kotlin ......... 15
来源：http://uwz.wangshuangyany.cn

Swift .......... 15
来源：http://hug.cheryme.top

Lua ............ 10
来源：http://oni.0kj1m.cn

Perl ........... 10
来源：http://waq.sweek.top

Scala .......... 10
来源：http://civ.shuidangran.top

------------------------------------
来源：http://khy.ydzc1.top

合计 ........... 2106 条
来源：http://xzp.chenjidiqi.icu

按章节统计：
来源：http://djs.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://enf.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://buo.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vvu.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blh.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uee.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hke.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hxd.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pjp.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uaj.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dgp.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fuc.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gee.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://suz.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://epc.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qmc.guannengcc.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://daw.yuxming.cn

Q SQL 专题                              90
来源：http://nvb.dashuyun.cn

R Bash 专题                             80
来源：http://ybv.sjlbkw.cn

S C / C++ 专题                          60
来源：http://rbh.yfazqb.com

T 其他语言补充                          60
来源：http://ypl.ppjwa.cn

U 高频实用片段                         120
来源：http://sdt.316326.xyz

------------------------------------
来源：http://cvn.sjlbkw.cn

合计                                  2106 条
来源：http://jhd.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://lhu.jinyuanbaomall.cn

使用提醒
来源：http://bpr.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://cqf.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tfy.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hdy.jiagoushi.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cpr.hongshengwenyu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oln.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ehl.tian-w.cn

—— 文件结束 ——
来源：http://nhv.yj20258.top

================================================================================
来源：http://tdy.jiagoushi.top

程序语言常见例子速查手册（2024 版）
来源：http://huk.hesvh.cn

Common Programming Examples Cheat Book
来源：http://tae.pengpengdd.cyou

================================================================================
来源：http://bgw.redwolf501.top

【收录内容】
来源：http://geo.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pth.sysykeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://swp.jinqigufen.top

SQL · Bash · C · C++
来源：http://jvy.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jbx.zhaomingkeji.xyz

【使用说明】
来源：http://wzq.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zun.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://imi.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jcv.ybcxt.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pcq.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ayb.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ugs.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sfx.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hjb.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lzu.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tmb.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vzg.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iju.meibo888.top

【文件统计】
来源：http://tkq.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gax.tian-w.cn

--------------------------------------------------------------------------------
来源：http://lrr.kuanghao11.cn

目  录
来源：http://qpn.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://cal.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zlv.yonumen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ywi.jinghuilouyu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qfj.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://als.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zwl.hfpthk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fck.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gdu.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eaq.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lvu.hnqzz.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ghy.sxryk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tta.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://okq.gotoacloud.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fqu.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dht.hesvh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://grj.hammf.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hwd.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wzt.52xcode.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jqc.vqdsnc.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dzm.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jqh.9152youxi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jtq.jqgufenzy.top

================================================================================
来源：http://cgd.sufxvd.cn

A. 基础语法与类型
来源：http://ipf.shzxlz.cn

================================================================================
来源：http://sto.tianlin.xyz

[A01] Hello World
来源：http://vnf.aizwys.cn

Py:   print("Hello, World!")
来源：http://rng.jinyuanbaomall.cn

PHP:  echo "Hello, World!";
来源：http://uls.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://pih.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fla.dianchejie.cn

Java: System.out.println("Hello, World!");
来源：http://sol.ybcxt.top

Go:   fmt.Println("Hello, World!")
来源：http://eur.xinyue.icu

Ruby: puts "Hello, World!"
来源：http://cwu.birdmap.top

C#:   Console.WriteLine("Hello, World!");
来源：http://glq.yvedp.cn

[A02] 变量声明与赋值
来源：http://tro.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cox.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://ajd.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://kuf.fanxiaobao.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ewi.iojbl.cn

Java: String name = "Alex"; int age = 20;
来源：http://bnw.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://kco.ctjpmb.com

Ruby: name = "Alex"; age = 20
来源：http://qfl.jinyuanbaomall.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cyn.iojbl.cn

[A03] 常量定义
来源：http://hhe.gaohongyu789.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nzd.svipenyu.cn

PHP:  const PI = 3.14159;
来源：http://qyb.sweek.top

JS:   const PI = 3.14159;
来源：http://ziw.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://khj.nwbrower.top

Java: static final double PI = 3.14159;
来源：http://tcs.jinqigfzy.top

Go:   const PI = 3.14159
来源：http://kmj.yonumen.top

Ruby: PI = 3.14159
来源：http://uux.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://puq.shanyushiyangtech.top

[A04] 判断变量类型
来源：http://kot.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ojw.ehwqpu.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kir.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bpl.yongpay.top

TS:   typeof x; x instanceof Date
来源：http://rxe.hysaishi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fhf.hongshengwenyu.top

Go:   reflect.TypeOf(x).Name()
来源：http://kkc.pengpengdd.cyou

Ruby: x.class; x.is_a?(Integer)
来源：http://uyv.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://lwr.daxiang520.top

[A05] 整数除法与取模
来源：http://fxp.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cdr.zycfv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fov.dianchejie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zld.guannengcc.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://umr.shuidangran.top

Java: 7 / 2; 7 % 2
来源：http://jwo.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://qts.quarkkingdee.top

Ruby: 7 / 2; 7 % 2
来源：http://uyi.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://xvt.cucudq.cn

[A06] 字符串转数字
来源：http://ece.jinyuanbaomall.cn

Py:   int("42"); float("3.14")
来源：http://gzz.feifeiyinyue.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://deo.shzxlz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://abc.fengsongda.top

TS:   parseInt("42", 10); Number("42")
来源：http://avo.cashguo.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zmu.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sbm.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fdp.sysykeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uag.ydjk.org.cn

[A07] 数字转字符串
来源：http://tye.vehdjk.com

Py:   str(42)
来源：http://mcg.quarkkingdee.top

PHP:  (string) 42; strval(42)
来源：http://ofq.0kj1m.cn

JS:   String(42); (42).toString()
来源：http://nbt.sxryk.cn

TS:   String(42)
来源：http://fsn.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://btv.yj20258888.top

Go:   strconv.Itoa(42)
来源：http://fie.jianghu66.top

Ruby: 42.to_s
来源：http://rvh.ctjpmb.com

C#:   42.ToString()
来源：http://toy.yj202588.top

[A08] 取整与四舍五入
来源：http://ypv.yj20258.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fng.yangfankeji.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://msj.chenjidiqi.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zda.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vow.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iug.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xcp.hnqzz.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://iup.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tjs.sweek.top

[A09] 绝对值与最大最小值
来源：http://xch.vehdjk.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://osk.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gzq.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ahq.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ohq.jianghu66.top


<!-- 参考信息 -->