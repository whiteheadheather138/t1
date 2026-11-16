代发 wailian999

[U77] PHP：模板渲染
来源：http://jto.yvedp.cn

composer require twig/twig
来源：http://qov.zhijiandao.cn

[U78] PHP：单元测试
来源：http://oiy.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://qun.chenlongwang.top

[U79] PHP：静态分析
来源：http://dcn.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://ifo.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://ooe.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mal.hnqzz.top

[U81] JS：初始化项目
来源：http://kuv.ivvv.top

npm init -y;  npm i express
来源：http://yqs.bbcook.cn

[U82] JS：package.json 脚本
来源：http://cvg.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sbt.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://bkl.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://jwp.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://yhn.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://wic.iojbl.cn

[U85] JS：可选链
来源：http://sqz.quarkkingdee.top

a?.b?.c
来源：http://ati.zhiwuduotai.top

[U86] JS：空值合并
来源：http://lnc.nanxinkj.top

a ?? b
来源：http://orq.fehbvm.com

[U87] JS：解构默认值
来源：http://rio.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://zsf.hfpthk.cn

[U88] JS：对象展开合并
来源：http://urz.hongshengwenyu.top

{ ...a, ...b }
来源：http://sap.tian-w.cn

[U89] JS：数组去重
来源：http://dtp.cqqwz.cn

[...new Set(arr)]
来源：http://sko.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://scq.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://cfy.chenlongwang.top

[U91] JS：对象键值遍历
来源：http://ntn.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oqn.jqgfzy.top

[U92] JS：深拷贝
来源：http://pxx.dashuyun.cn

structuredClone(obj)
来源：http://xvx.xylfe.cn

[U93] JS：模板字符串
来源：http://pyl.pycfn.com

`共 ${n} 条`
来源：http://eve.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://bfz.tian-w.cn

const double = x => x * 2;
来源：http://itu.smart0.xyz

[U95] JS：Promise 包装
来源：http://efr.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://ssg.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://osp.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yrn.andypj.xyz

[U97] JS：并发请求
来源：http://zkg.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sdg.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://idj.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fsz.tarul.cn

[U99] JS：事件监听
来源：http://syi.xuanzx.com

el.addEventListener("click", e => {})
来源：http://peu.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://nwe.gzhubu.top

document.querySelector(".item")
来源：http://awf.zhongyouzk.top

[U101] JS：classList 操作
来源：http://djc.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://yzz.jqgfzy.top

[U102] JS：本地存储
来源：http://kfm.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gll.xuetiantiany.cn

[U103] JS：定时器
来源：http://abm.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xre.gaohongyu789.top

[U104] JS：防抖
来源：http://cod.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nhi.sjlbkw.cn

[U105] JS：节流
来源：http://aev.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yjb.redwolf501.top

[U106] JS：日期格式化
来源：http://fwz.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://afa.redwolf501.top

[U107] JS：数字千分位
来源：http://mee.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dme.vqdsnc.cn

[U108] JS：随机整数
来源：http://lns.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jdj.hnxiangtu.top

[U109] JS：数组分组
来源：http://xev.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://cti.wangshuangyany.cn

[U110] JS：数组分块
来源：http://vcs.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qpe.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://mtu.hysaishi.cn

new Map(Object.entries(obj))
来源：http://xjy.ehwqpu.com

[U112] JS：字符串补位
来源：http://fyf.zdqjudy.top

"7".padStart(3, "0")
来源：http://yvh.quarkkingdee.top

[U113] JS：正则替换全部
来源：http://nze.yj202588.top

s.replaceAll("a", "b")
来源：http://uew.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://hia.316326.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://rdc.gogol.net.cn

[U115] JS：生成 UUID
来源：http://zrn.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://edr.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://ucx.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://bpt.xuanzx.com

[U117] JS：单元测试
来源：http://aph.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://xrx.xziqi.cn

[U118] JS：开发服务器
来源：http://gnd.yuxming.cn

npm i -D vite;  npx vite
来源：http://uuk.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://bkc.vehdjk.com

npx vite build
来源：http://hpo.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ggh.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://suz.wangdashe.top

================================================================================
来源：http://qtq.316326.xyz

统计汇总
来源：http://gcs.zdqjudy.top

================================================================================
来源：http://xpz.bbcook.cn

按语言统计（条）：
来源：http://sdm.cqqwz.cn

Python ......... 252
来源：http://mmw.svipenyu.cn

PHP ............ 252
来源：http://xsj.zhixingplan.top

JavaScript ..... 252
来源：http://ufb.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://udt.sjlbkw.cn

Java ........... 212
来源：http://ndn.mhx1999.top

Go ............. 212
来源：http://tur.gzhubu.top

Ruby ........... 212
来源：http://shi.shangyingyoupin.top

C# ............. 212
来源：http://mvd.gaohongyu789.top

C .............. 30
来源：http://svs.zhijiandao.cn

C++ ............ 30
来源：http://bhq.yueranfly.top

SQL ............ 90
来源：http://dsk.uphjek.com

Bash ........... 80
来源：http://ycz.0kj1m.cn

Kotlin ......... 15
来源：http://olm.zhaomingkeji.xyz

Swift .......... 15
来源：http://hgs.yanxiufei.cn

Lua ............ 10
来源：http://zqw.hesvh.cn

Perl ........... 10
来源：http://dtb.xziqi.cn

Scala .......... 10
来源：http://eux.shanyushiyangkeji.top

------------------------------------
来源：http://hht.dianchejie.cn

合计 ........... 2106 条
来源：http://kwn.xuetiantiany.cn

按章节统计：
来源：http://cfg.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rsx.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kzu.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vjt.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lyc.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bti.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ddu.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ibn.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ecu.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uft.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kmg.mhx1999.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qbc.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oik.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uie.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zoh.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cnc.hnqzz.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jhz.shzxlz.cn

Q SQL 专题                              90
来源：http://zzz.jianghu66.top

R Bash 专题                             80
来源：http://kpk.yanxiufei.cn

S C / C++ 专题                          60
来源：http://iea.bjfxy.top

T 其他语言补充                          60
来源：http://ssf.yuanzhike.top

U 高频实用片段                         120
来源：http://pvp.yonumen.top

------------------------------------
来源：http://dri.nanxuanxn.top

合计                                  2106 条
来源：http://jqx.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://dum.hfpthk.cn

使用提醒
来源：http://dqo.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://dnz.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qpo.jinyuanbaomall.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yua.gzhubu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gtp.jqgfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jzj.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://krp.jiagoushi.top

—— 文件结束 ——
来源：http://gha.pycfn.com

================================================================================
来源：http://dcf.yongpay.top

程序语言常见例子速查手册（2024 版）
来源：http://ktl.ydzc1.top

Common Programming Examples Cheat Book
来源：http://grj.9152youxi.cn

================================================================================
来源：http://sun.pycfn.com

【收录内容】
来源：http://hkh.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vru.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://phe.tanke756.top

SQL · Bash · C · C++
来源：http://fiw.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uen.xinyue.icu

【使用说明】
来源：http://lkj.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bap.gogol.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hbl.yj20258.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://woy.52xcode.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zjj.andypj.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://lnm.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rug.316326.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iru.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://brj.jqgufenzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vmf.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sag.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xdi.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bzz.shzxlz.cn

【文件统计】
来源：http://uyy.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yqi.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://cju.ppjwa.cn

目  录
来源：http://zna.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://zzl.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wzv.havefunace.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cpw.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xzs.yj202588.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wwb.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://geb.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oau.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lbm.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oar.sxryk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://emy.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://occ.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bho.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://apk.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cie.andypj.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yaf.sxryk.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sox.ybcxt.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pqz.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://csl.zdqjudy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qvo.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://opt.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rjp.snrcjt.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cid.hfpthk.cn

================================================================================
来源：http://qea.yuanzhike.top

A. 基础语法与类型
来源：http://lpn.hammf.cn

================================================================================
来源：http://cwz.ehwqpu.com

[A01] Hello World
来源：http://pos.uphjek.com

Py:   print("Hello, World!")
来源：http://eoo.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://hoc.svipenyu.cn

JS:   console.log("Hello, World!");
来源：http://zzi.ivvv.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qfe.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://oxi.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://lyj.fzhhl.top

Ruby: puts "Hello, World!"
来源：http://hml.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://swa.yfazqb.com

[A02] 变量声明与赋值
来源：http://mny.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tpo.fanxiaobao.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://pat.vqdsnc.cn

JS:   let name = "Alex"; const age = 20;
来源：http://izj.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gsr.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://shf.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://lus.gotoacloud.top

Ruby: name = "Alex"; age = 20
来源：http://xcx.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://kch.cucudq.cn

[A03] 常量定义
来源：http://znh.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bgm.bbcook.cn

PHP:  const PI = 3.14159;
来源：http://edy.chenjidiqi.icu

JS:   const PI = 3.14159;
来源：http://fmq.wangdashe.top

TS:   const PI: number = 3.14159;
来源：http://uas.xylfe.cn

Java: static final double PI = 3.14159;
来源：http://agb.vehdjk.com

Go:   const PI = 3.14159
来源：http://lps.xziqi.cn

Ruby: PI = 3.14159
来源：http://ymm.fehbvm.com

C#:   const double PI = 3.14159;
来源：http://pix.fktsv.cn

[A04] 判断变量类型
来源：http://gut.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ydu.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oiy.xingfuxueyuan.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rbs.dianchejie.cn

TS:   typeof x; x instanceof Date
来源：http://ibg.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://snj.epnwcf.com

Go:   reflect.TypeOf(x).Name()
来源：http://zex.jinyuanbaomall.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jml.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://bna.wangdashe.top

[A05] 整数除法与取模
来源：http://kgb.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://edi.hfpthk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gix.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hni.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://por.fengsongda.top

Java: 7 / 2; 7 % 2
来源：http://lpj.wangshuangyany.cn

Go:   7 / 2; 7 % 2
来源：http://dgg.hcnkem.com

Ruby: 7 / 2; 7 % 2
来源：http://fos.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://plp.cucudq.cn

[A06] 字符串转数字
来源：http://zrm.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://ean.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pgx.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://noz.shanyushiyangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://wfo.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kvy.sjlbkw.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://btq.havefunace.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ksj.bjfxy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zjf.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://ujo.cdnleiting.top

Py:   str(42)
来源：http://wqm.chenjidiqi.icu

PHP:  (string) 42; strval(42)
来源：http://wzo.hywenlv.cn

JS:   String(42); (42).toString()
来源：http://ckb.aibaodan.cn

TS:   String(42)
来源：http://ehv.xylfe.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ycv.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://uth.guowangkeji.top

Ruby: 42.to_s
来源：http://kwe.316326.xyz

C#:   42.ToString()
来源：http://uzx.tanke756.top

[A08] 取整与四舍五入
来源：http://rkl.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gof.ctjpmb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gox.ctjpmb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tgw.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://igm.ydjk.org.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://myj.hywenlv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wjd.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kwb.jqgfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wzl.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://eqw.hnxiangtu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pqd.bjfxy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://air.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vye.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uoa.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xbi.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jvn.fehbvm.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zko.smart0.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://waf.fktsv.cn

[A10] 生成随机数
来源：http://lhs.fengsongda.top

Py:   import random; random.randint(1, 100)
来源：http://zpg.guannengcc.top

PHP:  random_int(1, 100);
来源：http://yco.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://asb.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mwr.jinqigfzy.top

Java: new Random().nextInt(100) + 1
来源：http://rbz.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mgi.nanxinkj.top

Ruby: rand(1..100)
来源：http://jlm.yj20258888.top

C#:   new Random().Next(1, 101)
来源：http://ygk.gaohongyu789.top

[A11] 条件表达式（三元）
来源：http://fet.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://wxd.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://xdn.ybcxt.top

JS:   x > 0 ? "yes" : "no"
来源：http://ben.tanke756.top

TS:   x > 0 ? "yes" : "no"
来源：http://shz.quarkkingdee.top

Java: x > 0 ? "yes" : "no"
来源：http://gid.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zhm.nanxuanxn.top

Ruby: x > 0 ? "yes" : "no"
来源：http://upf.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://wmv.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://kfz.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ilr.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jyu.hnqzz.top

JS:   `Hello, ${name}!`
来源：http://fdj.chenjidiqi.icu

TS:   `Hello, ${name}!`
来源：http://dna.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://fek.xuetiantiany.cn


<!-- 参考信息 -->