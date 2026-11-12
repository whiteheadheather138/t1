代发 wailian999

[U81] JS：初始化项目
来源：http://mfs.vqdsnc.cn

npm init -y;  npm i express
来源：http://gcp.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://hwf.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ucs.dashuyun.cn

[U83] JS：ES Module 导入导出
来源：http://ybc.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://law.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://tyb.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ivg.vqdsnc.cn

[U85] JS：可选链
来源：http://nnz.cucudq.cn

a?.b?.c
来源：http://gqu.jinqigufen.top

[U86] JS：空值合并
来源：http://ugv.bbcook.cn

a ?? b
来源：http://igp.jinqigufen.top

[U87] JS：解构默认值
来源：http://bei.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://poo.chenzaomai.com

[U88] JS：对象展开合并
来源：http://rrm.cucudq.cn

{ ...a, ...b }
来源：http://ikh.nwbrower.top

[U89] JS：数组去重
来源：http://fkk.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://omf.nwbrower.top

[U90] JS：数字数组排序
来源：http://vek.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://sik.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://xas.shuidangran.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hwt.316326.xyz

[U92] JS：深拷贝
来源：http://uqq.ywan-chungtsiang.top

structuredClone(obj)
来源：http://mvi.haohaochexian.top

[U93] JS：模板字符串
来源：http://xck.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://fup.svipenyu.cn

[U94] JS：箭头函数
来源：http://zws.vqdsnc.cn

const double = x => x * 2;
来源：http://emn.hfpthk.cn

[U95] JS：Promise 包装
来源：http://xea.zhaomingkeji.xyz

new Promise((resolve, reject) => {})
来源：http://jqx.hnxiangtu.top

[U96] JS：async/await 与异常
来源：http://lzn.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://niz.vqdsnc.cn

[U97] JS：并发请求
来源：http://jlh.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nyt.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://zuf.jinqigfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tgh.fzhhl.top

[U99] JS：事件监听
来源：http://ugs.gzhubu.top

el.addEventListener("click", e => {})
来源：http://uou.hesvh.cn

[U100] JS：DOM 查询
来源：http://tiz.chenzaomai.com

document.querySelector(".item")
来源：http://rbc.jqgfzy.top

[U101] JS：classList 操作
来源：http://pfc.hnqzz.top

el.classList.toggle("active")
来源：http://thw.havefunace.top

[U102] JS：本地存储
来源：http://rjw.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://wwf.hysaishi.cn

[U103] JS：定时器
来源：http://yen.ywan-chungtsiang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ncb.jiagoushi.top

[U104] JS：防抖
来源：http://gki.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qmc.hywenlv.cn

[U105] JS：节流
来源：http://hgz.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uwd.kuanghao11.cn

[U106] JS：日期格式化
来源：http://alc.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rfv.gotoacloud.top

[U107] JS：数字千分位
来源：http://svh.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iij.wangshuangyany.cn

[U108] JS：随机整数
来源：http://vvs.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rgt.sweek.top

[U109] JS：数组分组
来源：http://tmn.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://ypb.jinqigfzy.top

[U110] JS：数组分块
来源：http://kxm.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xao.jianghu66.top

[U111] JS：对象转 Map
来源：http://plr.cashguo.top

new Map(Object.entries(obj))
来源：http://sul.fehbvm.com

[U112] JS：字符串补位
来源：http://wgc.jianghu66.top

"7".padStart(3, "0")
来源：http://hlx.jiagoushi.top

[U113] JS：正则替换全部
来源：http://ctp.uphjek.com

s.replaceAll("a", "b")
来源：http://uhv.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://apa.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jhf.hcnkem.com

[U115] JS：生成 UUID
来源：http://lhe.sysykeji.top

crypto.randomUUID()
来源：http://beg.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://non.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://peh.yanxiufei.cn

[U117] JS：单元测试
来源：http://htb.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://zih.yuanzhike.top

[U118] JS：开发服务器
来源：http://ctv.bbcook.cn

npm i -D vite;  npx vite
来源：http://cyx.uphjek.com

[U119] JS：生产构建
来源：http://hku.hnqzz.top

npx vite build
来源：http://alh.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://jpx.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://tan.hesvh.cn

================================================================================
来源：http://inq.haohaochexian.top

统计汇总
来源：http://otk.wangshuangyany.cn

================================================================================
来源：http://tzt.yj20258.top

按语言统计（条）：
来源：http://rcz.hongshengwenyu.top

Python ......... 252
来源：http://kjy.uphjek.com

PHP ............ 252
来源：http://bei.xziqi.cn

JavaScript ..... 252
来源：http://mnw.zhijiandao.cn

TypeScript ..... 212
来源：http://umi.0kj1m.cn

Java ........... 212
来源：http://hyk.wangdashe.top

Go ............. 212
来源：http://eci.smart0.xyz

Ruby ........... 212
来源：http://bdj.daria6918.cn

C# ............. 212
来源：http://tdn.zhiwuduotai.top

C .............. 30
来源：http://vfx.0kj1m.cn

C++ ............ 30
来源：http://wem.epnwcf.com

SQL ............ 90
来源：http://qfy.zdbjq.cn

Bash ........... 80
来源：http://jst.svipenyu.cn

Kotlin ......... 15
来源：http://mdb.fanxiaobao.xyz

Swift .......... 15
来源：http://pwq.shangyingyoupin.top

Lua ............ 10
来源：http://jhx.xingfuxueyuan.xyz

Perl ........... 10
来源：http://aia.zhiwuduotai.top

Scala .......... 10
来源：http://keq.c1oappe.top

------------------------------------
来源：http://yur.zycfv.cn

合计 ........... 2106 条
来源：http://zoc.nanxinkj.top

按章节统计：
来源：http://jqy.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rur.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zea.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fus.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xrz.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hxp.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nva.epnwcf.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://joe.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oio.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vuy.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pvg.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vqs.zhaomingkeji.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yqx.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xfn.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hic.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dvu.yvedp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tkz.yfazqb.com

Q SQL 专题                              90
来源：http://tfp.yuanzhike.top

R Bash 专题                             80
来源：http://glg.dashuyun.cn

S C / C++ 专题                          60
来源：http://hxd.yonumen.top

T 其他语言补充                          60
来源：http://pjr.zhiwuduotai.top

U 高频实用片段                         120
来源：http://syl.haohaochexian.top

------------------------------------
来源：http://zdw.jinyuanbaomall.cn

合计                                  2106 条
来源：http://xmo.sysykeji.top

--------------------------------------------------------------------------------
来源：http://lou.svipenyu.cn

使用提醒
来源：http://qla.fehbvm.com

--------------------------------------------------------------------------------
来源：http://rdp.pycfn.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rfi.jinyuanbaomall.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xus.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qum.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tuj.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fub.epnwcf.com

—— 文件结束 ——
来源：http://mnc.nanxinkj.top

================================================================================
来源：http://vnj.c1oappe.top

程序语言常见例子速查手册（2024 版）
来源：http://uqw.yfazqb.com

Common Programming Examples Cheat Book
来源：http://imb.fanxiaobao.xyz

================================================================================
来源：http://veo.zycfv.cn

【收录内容】
来源：http://frw.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://eug.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://deq.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://iut.ydzc1.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pyd.chenlongwang.top

【使用说明】
来源：http://xod.jyoumei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qcf.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bky.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://new.shangyingyoupin.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://omx.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zrc.mhx1999.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ilo.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mdw.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dxw.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://obi.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pbd.nwbrower.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nzx.tian-w.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qxq.uphjek.com

【文件统计】
来源：http://oym.daria6918.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mss.jianghu66.top

--------------------------------------------------------------------------------
来源：http://fwn.0kj1m.cn

目  录
来源：http://qmm.daxiang520.top

--------------------------------------------------------------------------------
来源：http://yoi.dianchejie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mbe.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://apq.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://knq.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lkv.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lty.smart0.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hac.yj202588.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mff.daria6918.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qcw.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ztt.chenzaomai.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ois.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dtn.tanke756.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lzl.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://svc.yj202588.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zdp.feifeiyinyue.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://szs.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xba.xinyue.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://occ.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://omd.gzhubu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mdp.ivvv.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rkb.jqgfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gke.xylfe.cn

================================================================================
来源：http://owa.jlsjyb.cn

A. 基础语法与类型
来源：http://xky.yuxming.cn

================================================================================
来源：http://ubg.quarkkingdee.top

[A01] Hello World
来源：http://kuj.gaohongyu789.top

Py:   print("Hello, World!")
来源：http://srr.cheryme.top

PHP:  echo "Hello, World!";
来源：http://nsb.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://zyl.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://atc.mhx1999.top

Java: System.out.println("Hello, World!");
来源：http://szc.cqqwz.cn

Go:   fmt.Println("Hello, World!")
来源：http://arz.yj20258888.top

Ruby: puts "Hello, World!"
来源：http://ofq.pengpengdd.cyou

C#:   Console.WriteLine("Hello, World!");
来源：http://ivz.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://mfo.jinqigfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oic.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://aja.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://ohq.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://daj.kuanghao11.cn

Java: String name = "Alex"; int age = 20;
来源：http://ush.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://kfv.yuanzhike.top

Ruby: name = "Alex"; age = 20
来源：http://qrk.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://ufd.sysykeji.top

[A03] 常量定义
来源：http://ovi.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pll.yj20258.top

PHP:  const PI = 3.14159;
来源：http://uaa.cdnleiting.top

JS:   const PI = 3.14159;
来源：http://mvk.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://jsw.zhongyouzk.top

Java: static final double PI = 3.14159;
来源：http://syo.sxryk.cn

Go:   const PI = 3.14159
来源：http://lqd.zhijiandao.cn

Ruby: PI = 3.14159
来源：http://zan.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://llg.havefunace.top

[A04] 判断变量类型
来源：http://rqs.ywan-chungtsiang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cwk.fanxiaobao.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wrj.smart0.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lxo.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://vpz.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gdp.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://axf.sweek.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hwa.daria6918.cn

C#:   x.GetType().Name; x is int
来源：http://vsc.cqqwz.cn

[A05] 整数除法与取模
来源：http://fzt.jqgufenzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://omg.zdqjudy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://zip.ybcxt.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gdl.redwolf501.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xqc.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://qkf.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://smc.hfpthk.cn

Ruby: 7 / 2; 7 % 2
来源：http://dho.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://wyu.dashuyun.cn

[A06] 字符串转数字
来源：http://hsd.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://uog.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hou.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gqn.mhx1999.top

TS:   parseInt("42", 10); Number("42")
来源：http://asv.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xvu.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qkn.birdmap.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nqh.jqgufenzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ulk.guowangkeji.top

[A07] 数字转字符串
来源：http://nwy.xingfuxueyuan.xyz

Py:   str(42)
来源：http://zmc.jiagoushi.top

PHP:  (string) 42; strval(42)
来源：http://ssa.sysykeji.top

JS:   String(42); (42).toString()
来源：http://yud.xingfuxueyuan.xyz

TS:   String(42)
来源：http://ycw.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gfh.chenjidiqi.icu

Go:   strconv.Itoa(42)
来源：http://rjz.daria6918.cn

Ruby: 42.to_s
来源：http://skb.ydzc1.top

C#:   42.ToString()
来源：http://gyd.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://mec.fktsv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://azj.sysykeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jvm.wangdashe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jld.pengpengdd.cyou

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pex.sxryk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mff.shanyushiyangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zsb.cucudq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ywg.shangyingyoupin.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://svo.hywenlv.cn

[A09] 绝对值与最大最小值
来源：http://agu.jiagoushi.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aml.sweek.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wac.vehdjk.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yqo.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://opl.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dqd.wangdashe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gvm.hnqzz.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ugs.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xdk.fehbvm.com

[A10] 生成随机数
来源：http://ooi.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://kuo.aizwys.cn

PHP:  random_int(1, 100);
来源：http://bjl.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fts.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uut.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://egi.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://amj.jyoumei.cn

Ruby: rand(1..100)
来源：http://npi.sjlbkw.cn

C#:   new Random().Next(1, 101)
来源：http://rck.hongshengwenyu.top

[A11] 条件表达式（三元）
来源：http://fyd.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://ixt.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qgv.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://kps.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://mtr.daria6918.cn

Java: x > 0 ? "yes" : "no"
来源：http://dnf.mhx1999.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ytt.gaohongyu789.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tvv.guowangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://yjh.cdnleiting.top

[A12] 字符串插值 / 格式化
来源：http://yyo.yvedp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wkp.0kj1m.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qbe.shzxlz.cn

JS:   `Hello, ${name}!`
来源：http://cam.zhaomingkeji.xyz

TS:   `Hello, ${name}!`
来源：http://guq.sweek.top

Java: "Hello, %s!".formatted(name)
来源：http://xwo.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tiu.hcnkem.com

Ruby: "Hello, #{name}!"
来源：http://zlc.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://zta.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qpe.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://hmk.yueranfly.top

PHP:  "第一行\n第二行"
来源：http://lgh.smart0.xyz

JS:   "第一行\n第二行"
来源：http://day.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://bpd.guowangkeji.top


<!-- 参考信息 -->