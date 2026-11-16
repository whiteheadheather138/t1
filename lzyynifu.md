代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://mwd.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://akn.yvedp.cn

[U74] PHP：读取环境变量
来源：http://tzj.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://wfa.guowangkeji.top

[U75] PHP：依赖注入
来源：http://oez.zhongyouzk.top

composer require psr/container
来源：http://kmq.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://rmb.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dny.haohaochexian.top

[U77] PHP：模板渲染
来源：http://oqz.havefunace.top

composer require twig/twig
来源：http://sbl.tian-w.cn

[U78] PHP：单元测试
来源：http://qdj.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://vte.yanxiufei.cn

[U79] PHP：静态分析
来源：http://ccb.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://eyf.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://avk.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ozi.ctjpmb.com

[U81] JS：初始化项目
来源：http://jji.zdbjq.cn

npm init -y;  npm i express
来源：http://tug.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://xen.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bqy.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://cck.aibaodan.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rpf.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://nln.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://egd.chenzaomai.com

[U85] JS：可选链
来源：http://qah.yj202588.top

a?.b?.c
来源：http://dah.hnxiangtu.top

[U86] JS：空值合并
来源：http://myh.cqqwz.cn

a ?? b
来源：http://ypm.zhongyouzk.top

[U87] JS：解构默认值
来源：http://tqi.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://tpl.iojbl.cn

[U88] JS：对象展开合并
来源：http://jmf.jyoumei.cn

{ ...a, ...b }
来源：http://haa.yongpay.top

[U89] JS：数组去重
来源：http://wkb.fktsv.cn

[...new Set(arr)]
来源：http://ejb.ybcxt.top

[U90] JS：数字数组排序
来源：http://cha.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://lzk.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://uwh.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qye.9152youxi.cn

[U92] JS：深拷贝
来源：http://wnh.nanxuanxn.top

structuredClone(obj)
来源：http://xqo.yj202588.top

[U93] JS：模板字符串
来源：http://bpe.jqgufenzy.top

`共 ${n} 条`
来源：http://mxv.meibo888.top

[U94] JS：箭头函数
来源：http://uyd.cdnleiting.top

const double = x => x * 2;
来源：http://kno.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://cnq.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://pia.yj20258888.top

[U96] JS：async/await 与异常
来源：http://ptr.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vny.yvedp.cn

[U97] JS：并发请求
来源：http://pfq.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wuy.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://puo.yvedp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lmy.c1oappe.top

[U99] JS：事件监听
来源：http://wdq.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://ktc.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://dlz.smart0.xyz

document.querySelector(".item")
来源：http://sad.nwbrower.top

[U101] JS：classList 操作
来源：http://vxq.shanyushiyangkeji.top

el.classList.toggle("active")
来源：http://iqf.c1oappe.top

[U102] JS：本地存储
来源：http://ela.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://dgz.guowangkeji.top

[U103] JS：定时器
来源：http://ycs.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://awg.jinqigfzy.top

[U104] JS：防抖
来源：http://zvp.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ees.chenzaomai.com

[U105] JS：节流
来源：http://fyc.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bsp.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://flo.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ggu.dianchejie.cn

[U107] JS：数字千分位
来源：http://imx.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xxi.redwolf501.top

[U108] JS：随机整数
来源：http://fom.yvedp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rlt.gaohongyu789.top

[U109] JS：数组分组
来源：http://hwx.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://zak.pycfn.com

[U110] JS：数组分块
来源：http://dgt.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://thp.zhijiandao.cn

[U111] JS：对象转 Map
来源：http://axu.hammf.cn

new Map(Object.entries(obj))
来源：http://jbq.jianghu66.top

[U112] JS：字符串补位
来源：http://sqt.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://dvb.cqqwz.cn

[U113] JS：正则替换全部
来源：http://yzl.jqgfzy.top

s.replaceAll("a", "b")
来源：http://kmg.uphjek.com

[U114] JS：JSON 深比较
来源：http://xay.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://nzg.jianghu66.top

[U115] JS：生成 UUID
来源：http://dvn.ehwqpu.com

crypto.randomUUID()
来源：http://qlq.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://rtx.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://pzv.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://qhi.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://tri.jqgfzy.top

[U118] JS：开发服务器
来源：http://wqv.bbcook.cn

npm i -D vite;  npx vite
来源：http://avy.zhongyouzk.top

[U119] JS：生产构建
来源：http://peb.chenzaomai.com

npx vite build
来源：http://zwx.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://acy.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://snp.gaohongyu789.top

================================================================================
来源：http://zqk.hywenlv.cn

统计汇总
来源：http://dnn.epnwcf.com

================================================================================
来源：http://oan.yj20258888.top

按语言统计（条）：
来源：http://jzv.aibaodan.cn

Python ......... 252
来源：http://asp.fengsongda.top

PHP ............ 252
来源：http://sjo.daxiang520.top

JavaScript ..... 252
来源：http://sfp.ctjpmb.com

TypeScript ..... 212
来源：http://vkv.yj202588.top

Java ........... 212
来源：http://zhg.shanyushiyangkeji.top

Go ............. 212
来源：http://gda.yongpay.top

Ruby ........... 212
来源：http://mct.cheryme.top

C# ............. 212
来源：http://ekr.feifeiyinyue.top

C .............. 30
来源：http://nme.daxiang520.top

C++ ............ 30
来源：http://tec.hywenlv.cn

SQL ............ 90
来源：http://uns.jinqigufen.top

Bash ........... 80
来源：http://acl.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://lyu.yj20258888.top

Swift .......... 15
来源：http://ofs.fengsongda.top

Lua ............ 10
来源：http://caw.0kj1m.cn

Perl ........... 10
来源：http://zdi.yj202588.top

Scala .......... 10
来源：http://egu.yfazqb.com

------------------------------------
来源：http://azk.xuetiantiany.cn

合计 ........... 2106 条
来源：http://tis.sweek.top

按章节统计：
来源：http://chn.sxryk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ace.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bit.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xtb.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lbr.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zlw.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ozx.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dwp.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qdj.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hqe.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jom.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zoc.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yjf.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://obs.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sjd.hnqzz.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ztw.jinghuilouyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bou.yangfankeji.com

Q SQL 专题                              90
来源：http://jfh.gotoacloud.top

R Bash 专题                             80
来源：http://eiy.nanxinkj.top

S C / C++ 专题                          60
来源：http://wgm.52xcode.cn

T 其他语言补充                          60
来源：http://vkq.wangdashe.top

U 高频实用片段                         120
来源：http://yuz.jinqigufen.top

------------------------------------
来源：http://dzj.ydjk.org.cn

合计                                  2106 条
来源：http://zmq.yongpay.top

--------------------------------------------------------------------------------
来源：http://gtw.jqgufenzy.top

使用提醒
来源：http://mxs.xylfe.cn

--------------------------------------------------------------------------------
来源：http://wfk.zhiwuduotai.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mio.jyoumei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://evn.9152youxi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yud.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ncb.yvedp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://neq.birdmap.top

—— 文件结束 ——
来源：http://fmk.jqgfzy.top

================================================================================
来源：http://vxf.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://kym.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://kbz.cqqwz.cn

================================================================================
来源：http://tqs.cqqwz.cn

【收录内容】
来源：http://mco.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://bky.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://evf.zdqjudy.top

SQL · Bash · C · C++
来源：http://zux.hfpthk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lrr.mhx1999.top

【使用说明】
来源：http://iry.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://udm.andypj.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rcn.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kxx.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fmp.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vvp.dianchejie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ets.zdbjq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fxd.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://szj.redwolf501.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rbw.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yzp.yvedp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ebp.ctjpmb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oew.gotoacloud.top

【文件统计】
来源：http://kfm.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zis.52xcode.cn

--------------------------------------------------------------------------------
来源：http://hjs.c1oappe.top

目  录
来源：http://brx.yuxming.cn

--------------------------------------------------------------------------------
来源：http://vim.ydzc1.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kta.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://idj.sufxvd.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cus.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dwv.quarkkingdee.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qxm.chenlongwang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wkm.fanxiaobao.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ztl.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jew.ydzc1.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kal.jianghu66.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uis.hfpthk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zih.ywan-chungtsiang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://anc.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://szu.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xte.xziqi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pif.cheryme.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jfd.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qzr.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://ffz.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uty.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ujo.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jjs.jiagoushi.top

================================================================================
来源：http://arv.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://eag.zhiwuduotai.top

================================================================================
来源：http://pzh.shangyingyoupin.top

[A01] Hello World
来源：http://unh.ehwqpu.com

Py:   print("Hello, World!")
来源：http://vii.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://rbh.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://kwx.cashguo.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://knp.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://ugw.svipenyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://hvh.redwolf501.top

Ruby: puts "Hello, World!"
来源：http://gkw.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gyl.guowangkeji.top

[A02] 变量声明与赋值
来源：http://erz.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://onl.tarul.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://afw.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://zfc.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://snn.cucudq.cn

Java: String name = "Alex"; int age = 20;
来源：http://rmu.yangfankeji.com

Go:   name := "Alex"; age := 20
来源：http://tns.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://wme.hammf.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fms.shangyingyoupin.top

[A03] 常量定义
来源：http://pbg.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jlh.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://owe.shuidangran.top

JS:   const PI = 3.14159;
来源：http://cgq.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://jmx.meibo888.top

Java: static final double PI = 3.14159;
来源：http://wot.haohaochexian.top

Go:   const PI = 3.14159
来源：http://gjk.chenjidiqi.icu

Ruby: PI = 3.14159
来源：http://xxe.chenzaomai.com

C#:   const double PI = 3.14159;
来源：http://pqk.xuanzx.com

[A04] 判断变量类型
来源：http://iqp.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://qbc.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wxp.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nmp.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://ykv.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fiw.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://iti.yvedp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lch.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://rjo.hesvh.cn

[A05] 整数除法与取模
来源：http://bkk.0kj1m.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://khl.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vlg.fzhhl.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nfj.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bdw.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://oxg.yueranfly.top

Go:   7 / 2; 7 % 2
来源：http://qyg.jianghu66.top

Ruby: 7 / 2; 7 % 2
来源：http://klm.sjlbkw.cn

C#:   7 / 2; 7 % 2
来源：http://vzo.tarul.cn

[A06] 字符串转数字
来源：http://sqt.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://jiv.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wms.xuanzx.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hnp.ehwqpu.com

TS:   parseInt("42", 10); Number("42")
来源：http://szl.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xdd.52xcode.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jiv.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pke.nwbrower.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ytk.meibo888.top

[A07] 数字转字符串
来源：http://tuh.shanyushiyangkeji.top

Py:   str(42)
来源：http://ipi.gaohongyu789.top

PHP:  (string) 42; strval(42)
来源：http://rrn.jinyuanbaomall.cn

JS:   String(42); (42).toString()
来源：http://yiv.zhoulong.xyz

TS:   String(42)
来源：http://hfm.yj202588.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gym.yuxming.cn

Go:   strconv.Itoa(42)
来源：http://jwv.xingfuxueyuan.xyz

Ruby: 42.to_s
来源：http://qzv.yanxiufei.cn

C#:   42.ToString()
来源：http://msb.xinyue.icu

[A08] 取整与四舍五入
来源：http://egv.daria6918.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xiz.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cox.zdqjudy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sxz.andypj.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://azq.dianchejie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://imk.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ltf.yangfankeji.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://lkr.c1oappe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xvh.hongshengwenyu.top

[A09] 绝对值与最大最小值
来源：http://mmg.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://get.mhx1999.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rib.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ynz.zhongyouzk.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rqx.vqdsnc.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xrg.52xcode.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xtj.shzxlz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pju.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gnd.shanyushiyangkeji.top

[A10] 生成随机数
来源：http://iem.fehbvm.com

Py:   import random; random.randint(1, 100)
来源：http://zbd.mhx1999.top

PHP:  random_int(1, 100);
来源：http://lzb.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nzj.aibaodan.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uij.smart0.xyz

Java: new Random().nextInt(100) + 1
来源：http://fnm.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tzm.mhx1999.top

Ruby: rand(1..100)
来源：http://faf.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://mlj.svipenyu.cn

[A11] 条件表达式（三元）
来源：http://wcb.sweek.top

Py:   "yes" if x > 0 else "no"
来源：http://gqs.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fwb.cheryme.top

JS:   x > 0 ? "yes" : "no"
来源：http://qog.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://wpo.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://yph.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jyp.snrcjt.cn


<!-- 参考信息 -->