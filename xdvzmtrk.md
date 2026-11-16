代发 wailian999

[U69] PHP：PDO 预处理
来源：http://szq.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jkj.bjfxy.top

[U70] PHP：PDO 事务
来源：http://xpy.chenjidiqi.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ect.hfpthk.cn

[U71] PHP：抛出异常
来源：http://rqp.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://jiz.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://yyu.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://jwp.yj202588.top

[U73] PHP：读取 ini 配置
来源：http://oem.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://iix.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://iin.gaohongyu789.top

getenv("APP_ENV") ?: "production"
来源：http://sgi.yj20258888.top

[U75] PHP：依赖注入
来源：http://pht.ctjpmb.com

composer require psr/container
来源：http://noh.xuanzx.com

[U76] PHP：简单路由
来源：http://fcy.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ncm.xinyue.icu

[U77] PHP：模板渲染
来源：http://vhd.vqdsnc.cn

composer require twig/twig
来源：http://tpi.epnwcf.com

[U78] PHP：单元测试
来源：http://cma.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://gyo.aizwys.cn

[U79] PHP：静态分析
来源：http://bod.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://zky.jqgufenzy.top

[U80] PHP：代码规范修复
来源：http://vdb.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://anc.gotoacloud.top

[U81] JS：初始化项目
来源：http://cah.pycfn.com

npm init -y;  npm i express
来源：http://ipy.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://ymf.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://avp.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://dta.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uev.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://jjz.ydzc1.top

module.exports = { a };  const { a } = require("./m");
来源：http://mjd.nanxinkj.top

[U85] JS：可选链
来源：http://jfv.cheryme.top

a?.b?.c
来源：http://riu.yanxiufei.cn

[U86] JS：空值合并
来源：http://rrh.jyoumei.cn

a ?? b
来源：http://iru.xuanzx.com

[U87] JS：解构默认值
来源：http://yfh.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://mqc.dashuyun.cn

[U88] JS：对象展开合并
来源：http://ret.daria6918.cn

{ ...a, ...b }
来源：http://ivl.fehbvm.com

[U89] JS：数组去重
来源：http://bru.cdnleiting.top

[...new Set(arr)]
来源：http://iep.sufxvd.cn

[U90] JS：数字数组排序
来源：http://ols.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://bly.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://dca.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxq.hfpthk.cn

[U92] JS：深拷贝
来源：http://nef.mhx1999.top

structuredClone(obj)
来源：http://uid.snrcjt.cn

[U93] JS：模板字符串
来源：http://skr.fzhhl.top

`共 ${n} 条`
来源：http://egu.bbcook.cn

[U94] JS：箭头函数
来源：http://vcb.tianlin.xyz

const double = x => x * 2;
来源：http://crd.smart0.xyz

[U95] JS：Promise 包装
来源：http://whq.smart0.xyz

new Promise((resolve, reject) => {})
来源：http://rvn.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://nmf.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://umy.hnxiangtu.top

[U97] JS：并发请求
来源：http://wfw.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xhu.hnxiangtu.top

[U98] JS：fetch 带 JSON
来源：http://por.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ajo.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://nlq.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://yqq.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://yrp.fzhhl.top

document.querySelector(".item")
来源：http://nga.jyoumei.cn

[U101] JS：classList 操作
来源：http://kqt.cdnleiting.top

el.classList.toggle("active")
来源：http://woi.jinyuanbaomall.cn

[U102] JS：本地存储
来源：http://fvc.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fcu.shanyushiyangtech.top

[U103] JS：定时器
来源：http://nga.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://awc.snrcjt.cn

[U104] JS：防抖
来源：http://bkh.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kje.zhaomingkeji.xyz

[U105] JS：节流
来源：http://vdm.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dka.gogol.net.cn

[U106] JS：日期格式化
来源：http://tcx.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://apq.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://miu.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lju.gzhubu.top

[U108] JS：随机整数
来源：http://lro.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vwf.yj202588.top

[U109] JS：数组分组
来源：http://ioq.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://elg.xinyue.icu

[U110] JS：数组分块
来源：http://vtl.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jin.fehbvm.com

[U111] JS：对象转 Map
来源：http://wie.hfpthk.cn

new Map(Object.entries(obj))
来源：http://fnw.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://rka.zdbjq.cn

"7".padStart(3, "0")
来源：http://kjd.aibaodan.cn

[U113] JS：正则替换全部
来源：http://fjy.bjfxy.top

s.replaceAll("a", "b")
来源：http://pzu.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://txg.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nja.redwolf501.top

[U115] JS：生成 UUID
来源：http://rzy.jyoumei.cn

crypto.randomUUID()
来源：http://dus.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://qgp.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://tdc.haohaochexian.top

[U117] JS：单元测试
来源：http://lyq.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://osq.pycfn.com

[U118] JS：开发服务器
来源：http://hyx.zhengqikj.top

npm i -D vite;  npx vite
来源：http://ybq.yj202588.top

[U119] JS：生产构建
来源：http://fpe.chenzaomai.com

npx vite build
来源：http://alx.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://emo.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://ybl.wangdashe.top

================================================================================
来源：http://sml.ydjk.org.cn

统计汇总
来源：http://odp.shuidangran.top

================================================================================
来源：http://xvu.jinghuilouyu.cn

按语言统计（条）：
来源：http://wei.zhengqikj.top

Python ......... 252
来源：http://hol.vehdjk.com

PHP ............ 252
来源：http://tvb.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://vkp.guowangkeji.top

TypeScript ..... 212
来源：http://fce.zhoulong.xyz

Java ........... 212
来源：http://ktq.cashguo.top

Go ............. 212
来源：http://coq.epnwcf.com

Ruby ........... 212
来源：http://bex.tian-w.cn

C# ............. 212
来源：http://qlz.gotoacloud.top

C .............. 30
来源：http://lyk.jqgufenzy.top

C++ ............ 30
来源：http://gsh.xuanzx.com

SQL ............ 90
来源：http://tpe.yuxming.cn

Bash ........... 80
来源：http://xnb.xylfe.cn

Kotlin ......... 15
来源：http://frp.jinyuanbaomall.cn

Swift .......... 15
来源：http://xjp.ybcxt.top

Lua ............ 10
来源：http://xpt.hcnkem.com

Perl ........... 10
来源：http://ojh.ywan-chungtsiang.top

Scala .......... 10
来源：http://nta.xingfuxueyuan.xyz

------------------------------------
来源：http://rsc.haohaochexian.top

合计 ........... 2106 条
来源：http://wut.0kj1m.cn

按章节统计：
来源：http://rjz.xuanzx.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pqf.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://axv.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fag.chenlongwang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bff.daxiang520.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lmg.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dmz.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bvj.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iwq.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lmq.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jou.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bpp.jqgufenzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ifk.ybcxt.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tgq.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://clb.svipenyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rnw.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ahr.hongshengwenyu.top

Q SQL 专题                              90
来源：http://btq.cucudq.cn

R Bash 专题                             80
来源：http://okj.zhixingplan.top

S C / C++ 专题                          60
来源：http://kyl.fanxiaobao.xyz

T 其他语言补充                          60
来源：http://ynz.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://zwp.xuetiantiany.cn

------------------------------------
来源：http://cdm.sweek.top

合计                                  2106 条
来源：http://otp.ydzc1.top

--------------------------------------------------------------------------------
来源：http://gjg.iojbl.cn

使用提醒
来源：http://mls.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://dpz.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yny.zhiwuduotai.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qlt.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://skm.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bkt.birdmap.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sip.yj202588.top

—— 文件结束 ——
来源：http://ndg.jiagoushi.top

================================================================================
来源：http://dau.zhengqikj.top

程序语言常见例子速查手册（2024 版）
来源：http://znj.svipenyu.cn

Common Programming Examples Cheat Book
来源：http://qmj.birdmap.top

================================================================================
来源：http://doj.yfazqb.com

【收录内容】
来源：http://djz.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ojy.yj20258.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eic.tian-w.cn

SQL · Bash · C · C++
来源：http://epn.epnwcf.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gjo.ctjpmb.com

【使用说明】
来源：http://eld.daria6918.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://odu.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://igd.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rnz.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kqw.yonumen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ixe.cdnleiting.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wuj.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ier.yangfankeji.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ayq.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qhc.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://boj.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gav.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hop.dianchejie.cn

【文件统计】
来源：http://pto.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wzb.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://mbx.uphjek.com

目  录
来源：http://gin.bbcook.cn

--------------------------------------------------------------------------------
来源：http://xap.jinghuilouyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kcx.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tjq.fanxiaobao.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kuu.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://axj.zycfv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iub.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ltm.snrcjt.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jzg.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uzo.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tmx.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yap.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qlc.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vuu.yuanzhike.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sok.daxiang520.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://scp.zhiwuduotai.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gqw.yanxiufei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wql.yj20258888.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://isk.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zzh.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vve.zdbjq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://skx.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kcr.bjfxy.top

================================================================================
来源：http://kvu.52xcode.cn

A. 基础语法与类型
来源：http://ahv.9152youxi.cn

================================================================================
来源：http://ngl.jinyuanbaomall.cn

[A01] Hello World
来源：http://qdn.hfpthk.cn

Py:   print("Hello, World!")
来源：http://vkr.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://rpd.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://twy.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jww.yj202588.top

Java: System.out.println("Hello, World!");
来源：http://ady.feifeiyinyue.top

Go:   fmt.Println("Hello, World!")
来源：http://kkm.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://tjr.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://zhx.sysykeji.top

[A02] 变量声明与赋值
来源：http://uua.jianghu66.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xrt.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nmo.aizwys.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qav.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lsf.gzhubu.top

Java: String name = "Alex"; int age = 20;
来源：http://rpr.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://xdc.tarul.cn

Ruby: name = "Alex"; age = 20
来源：http://jfw.daria6918.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dub.jinqigfzy.top

[A03] 常量定义
来源：http://jjv.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tdp.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://msa.sjlbkw.cn

JS:   const PI = 3.14159;
来源：http://cjk.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://kup.uphjek.com

Java: static final double PI = 3.14159;
来源：http://yfq.wangshuangyany.cn

Go:   const PI = 3.14159
来源：http://hsb.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://urm.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://kyy.yanxiufei.cn

[A04] 判断变量类型
来源：http://zdq.fzhhl.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://khy.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://znm.smart0.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xye.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://bch.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ikr.nwbrower.top

Go:   reflect.TypeOf(x).Name()
来源：http://whf.andypj.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://ash.shangyingyoupin.top

C#:   x.GetType().Name; x is int
来源：http://yni.gotoacloud.top

[A05] 整数除法与取模
来源：http://hyj.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cfl.9152youxi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kjm.tanke756.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aim.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gze.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://yov.yongpay.top

Go:   7 / 2; 7 % 2
来源：http://tyb.cucudq.cn

Ruby: 7 / 2; 7 % 2
来源：http://tnh.fanxiaobao.xyz

C#:   7 / 2; 7 % 2
来源：http://noa.cashguo.top

[A06] 字符串转数字
来源：http://jil.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://nce.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xbt.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dgl.ybcxt.top

TS:   parseInt("42", 10); Number("42")
来源：http://kpq.uphjek.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zww.yj20258.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cot.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yeg.guannengcc.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dvp.ivvv.top

[A07] 数字转字符串
来源：http://jda.vehdjk.com

Py:   str(42)
来源：http://ihr.gaohongyu789.top

PHP:  (string) 42; strval(42)
来源：http://lwc.zycfv.cn

JS:   String(42); (42).toString()
来源：http://ecl.tian-w.cn

TS:   String(42)
来源：http://wdj.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pnp.jianghu66.top

Go:   strconv.Itoa(42)
来源：http://tgq.hongshengwenyu.top

Ruby: 42.to_s
来源：http://dbg.quarkkingdee.top

C#:   42.ToString()
来源：http://chv.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://llp.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bkv.sxryk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ube.yueranfly.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oso.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rok.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://awy.yj20258.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://esf.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://yaw.dashuyun.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oip.zhixingplan.top

[A09] 绝对值与最大最小值
来源：http://hat.quarkkingdee.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pgm.daria6918.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zsv.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nbp.yangfankeji.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://enk.hnqzz.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dig.c1oappe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://taf.zhoulong.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://koz.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ohp.ehwqpu.com

[A10] 生成随机数
来源：http://vui.havefunace.top

Py:   import random; random.randint(1, 100)
来源：http://ttx.zdbjq.cn

PHP:  random_int(1, 100);
来源：http://fky.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bgd.snrcjt.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mkx.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://fjz.yuanzhike.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lmq.jqgufenzy.top

Ruby: rand(1..100)
来源：http://obv.tarul.cn


<!-- 参考信息 -->