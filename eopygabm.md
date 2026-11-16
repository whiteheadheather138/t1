代发 wailian999

[U81] JS：初始化项目
来源：http://xdc.sweek.top

npm init -y;  npm i express
来源：http://swo.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://sgj.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rus.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://ams.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ppe.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://fie.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://opp.uphjek.com

[U85] JS：可选链
来源：http://uvj.yj20258888.top

a?.b?.c
来源：http://kkr.nwbrower.top

[U86] JS：空值合并
来源：http://nvj.meibo888.top

a ?? b
来源：http://fcr.316326.xyz

[U87] JS：解构默认值
来源：http://ety.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://bgq.yj202588.top

[U88] JS：对象展开合并
来源：http://tol.hongshengwenyu.top

{ ...a, ...b }
来源：http://gqw.zhoulong.xyz

[U89] JS：数组去重
来源：http://glz.shangyingyoupin.top

[...new Set(arr)]
来源：http://kwk.xuanzx.com

[U90] JS：数字数组排序
来源：http://vxt.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://zxe.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://piy.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qhs.yvedp.cn

[U92] JS：深拷贝
来源：http://rxu.yonumen.top

structuredClone(obj)
来源：http://mzq.sxryk.cn

[U93] JS：模板字符串
来源：http://oxs.yj20258888.top

`共 ${n} 条`
来源：http://uqe.quarkkingdee.top

[U94] JS：箭头函数
来源：http://xys.andypj.xyz

const double = x => x * 2;
来源：http://akp.yuxming.cn

[U95] JS：Promise 包装
来源：http://bia.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://aas.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://mmf.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jjr.wangshuangyany.cn

[U97] JS：并发请求
来源：http://mgi.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bve.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://her.sweek.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wwo.fehbvm.com

[U99] JS：事件监听
来源：http://vvm.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://koq.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://pku.xylfe.cn

document.querySelector(".item")
来源：http://nfl.cqqwz.cn

[U101] JS：classList 操作
来源：http://fed.0kj1m.cn

el.classList.toggle("active")
来源：http://yvd.yuxming.cn

[U102] JS：本地存储
来源：http://rat.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nuh.gzhubu.top

[U103] JS：定时器
来源：http://bsu.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yni.hammf.cn

[U104] JS：防抖
来源：http://kty.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nnw.daria6918.cn

[U105] JS：节流
来源：http://kom.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mwa.cqqwz.cn

[U106] JS：日期格式化
来源：http://eey.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mog.tarul.cn

[U107] JS：数字千分位
来源：http://bkg.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hdv.cucudq.cn

[U108] JS：随机整数
来源：http://nvy.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://etc.gogol.net.cn

[U109] JS：数组分组
来源：http://itj.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://psx.fehbvm.com

[U110] JS：数组分块
来源：http://gxq.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jwz.dianchejie.cn

[U111] JS：对象转 Map
来源：http://xvl.hysaishi.cn

new Map(Object.entries(obj))
来源：http://dgz.jqgfzy.top

[U112] JS：字符串补位
来源：http://hui.yfazqb.com

"7".padStart(3, "0")
来源：http://gnn.yonumen.top

[U113] JS：正则替换全部
来源：http://yrs.fzhhl.top

s.replaceAll("a", "b")
来源：http://buf.ydzc1.top

[U114] JS：JSON 深比较
来源：http://xpm.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://enk.xinyue.icu

[U115] JS：生成 UUID
来源：http://wff.guannengcc.top

crypto.randomUUID()
来源：http://hyq.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://dbc.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://boz.jqgufenzy.top

[U117] JS：单元测试
来源：http://tqn.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://lcn.iojbl.cn

[U118] JS：开发服务器
来源：http://ney.chenzaomai.com

npm i -D vite;  npx vite
来源：http://udp.uphjek.com

[U119] JS：生产构建
来源：http://yle.aibaodan.cn

npx vite build
来源：http://fjg.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://qga.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://wdt.zhijiandao.cn

================================================================================
来源：http://mwr.jinyuanbaomall.cn

统计汇总
来源：http://drk.yj20258.top

================================================================================
来源：http://pbf.daria6918.cn

按语言统计（条）：
来源：http://far.zhaomingkeji.xyz

Python ......... 252
来源：http://dbw.haohaochexian.top

PHP ............ 252
来源：http://hww.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://mjx.wangdashe.top

TypeScript ..... 212
来源：http://pja.iojbl.cn

Java ........... 212
来源：http://bfq.sjlbkw.cn

Go ............. 212
来源：http://suk.tianlin.xyz

Ruby ........... 212
来源：http://mbz.jinqigfzy.top

C# ............. 212
来源：http://cur.daria6918.cn

C .............. 30
来源：http://lkk.uphjek.com

C++ ............ 30
来源：http://ofs.fanxiaobao.xyz

SQL ............ 90
来源：http://sis.wangdashe.top

Bash ........... 80
来源：http://cjs.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://stj.guannengcc.top

Swift .......... 15
来源：http://kec.yanxiufei.cn

Lua ............ 10
来源：http://myc.hywenlv.cn

Perl ........... 10
来源：http://xkc.jlsjyb.cn

Scala .......... 10
来源：http://lsz.tianlin.xyz

------------------------------------
来源：http://ksy.ctjpmb.com

合计 ........... 2106 条
来源：http://fyh.ywan-chungtsiang.top

按章节统计：
来源：http://jjd.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fbt.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yld.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://etb.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yvb.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://flc.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lqg.hcnkem.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lvq.zdbjq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wot.bjfxy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dlv.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yij.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xzr.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qrq.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fde.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gho.ydzc1.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ubv.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jqw.yuxming.cn

Q SQL 专题                              90
来源：http://yzh.yj202588.top

R Bash 专题                             80
来源：http://spb.yuxming.cn

S C / C++ 专题                          60
来源：http://cyj.guowangkeji.top

T 其他语言补充                          60
来源：http://ydo.epnwcf.com

U 高频实用片段                         120
来源：http://qdc.hnqzz.top

------------------------------------
来源：http://dac.jiagoushi.top

合计                                  2106 条
来源：http://oyd.ybcxt.top

--------------------------------------------------------------------------------
来源：http://tvr.guowangkeji.top

使用提醒
来源：http://gly.ivvv.top

--------------------------------------------------------------------------------
来源：http://jha.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xll.jyoumei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lip.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ofz.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hez.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://onu.sjlbkw.cn

—— 文件结束 ——
来源：http://ylp.gzhubu.top

================================================================================
来源：http://ppn.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://cki.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://wxg.yangfankeji.com

================================================================================
来源：http://ria.sysykeji.top

【收录内容】
来源：http://edb.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://eyg.yvedp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bst.jqgfzy.top

SQL · Bash · C · C++
来源：http://ktk.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jyo.cheryme.top

【使用说明】
来源：http://shu.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://raz.jqgfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://peb.yj202588.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lzm.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fvh.jinyuanbaomall.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://urr.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tql.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://viu.jlsjyb.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://czv.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ase.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lgd.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://los.hammf.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yjh.wangdashe.top

【文件统计】
来源：http://zab.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qut.meibo888.top

--------------------------------------------------------------------------------
来源：http://rvs.nanxuanxn.top

目  录
来源：http://euy.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://juw.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xrl.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://htr.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ajl.wangdashe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mit.tanke756.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mgi.hfpthk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dlc.aizwys.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://arp.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://enf.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rvw.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ohy.xuanzx.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wou.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qyw.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rrh.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dnj.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fru.hcnkem.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nip.jiagoushi.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xik.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cpc.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ixh.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://reo.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hjb.yonumen.top

================================================================================
来源：http://rix.bjfxy.top

A. 基础语法与类型
来源：http://xph.cucudq.cn

================================================================================
来源：http://uvk.ppjwa.cn

[A01] Hello World
来源：http://ouf.jqgfzy.top

Py:   print("Hello, World!")
来源：http://dgg.sweek.top

PHP:  echo "Hello, World!";
来源：http://mjn.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://qpg.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kev.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://fmt.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://pvf.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://bwe.ppjwa.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://shb.jyoumei.cn

[A02] 变量声明与赋值
来源：http://utb.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lqh.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jae.zhixingplan.top

JS:   let name = "Alex"; const age = 20;
来源：http://tki.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xhx.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://sql.cheryme.top

Go:   name := "Alex"; age := 20
来源：http://sii.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://sgs.zhoulong.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://agh.0kj1m.cn

[A03] 常量定义
来源：http://lgt.cucudq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hkd.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://fhj.jiagoushi.top

JS:   const PI = 3.14159;
来源：http://sei.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://clj.chenzaomai.com

Java: static final double PI = 3.14159;
来源：http://ylp.zhengqikj.top

Go:   const PI = 3.14159
来源：http://pss.feifeiyinyue.top

Ruby: PI = 3.14159
来源：http://qpg.tanke756.top

C#:   const double PI = 3.14159;
来源：http://vzt.ybcxt.top

[A04] 判断变量类型
来源：http://cgw.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://uem.daria6918.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tia.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cko.wangdashe.top

TS:   typeof x; x instanceof Date
来源：http://tyy.aizwys.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bac.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wlu.epnwcf.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ivj.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://kwi.nanxuanxn.top

[A05] 整数除法与取模
来源：http://gvb.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hke.ctjpmb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ywo.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cim.haohaochexian.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mor.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://iqf.shanyushiyangkeji.top

Go:   7 / 2; 7 % 2
来源：http://fni.smart0.xyz

Ruby: 7 / 2; 7 % 2
来源：http://lgq.guowangkeji.top

C#:   7 / 2; 7 % 2
来源：http://hit.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://ncy.c1oappe.top

Py:   int("42"); float("3.14")
来源：http://mlk.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gyi.sufxvd.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ylv.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://wwa.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wjn.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eju.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://xfa.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mgk.hysaishi.cn

[A07] 数字转字符串
来源：http://juf.yueranfly.top

Py:   str(42)
来源：http://sza.yanxiufei.cn

PHP:  (string) 42; strval(42)
来源：http://idv.guannengcc.top

JS:   String(42); (42).toString()
来源：http://tud.andypj.xyz

TS:   String(42)
来源：http://dje.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wzv.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://may.zhongyouzk.top

Ruby: 42.to_s
来源：http://syh.zhengqikj.top

C#:   42.ToString()
来源：http://dpl.shzxlz.cn

[A08] 取整与四舍五入
来源：http://muk.gaohongyu789.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zjk.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://drl.yfazqb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bdw.xylfe.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bqe.ppjwa.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gzp.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sji.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vxy.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uyy.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://fkb.guannengcc.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nct.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://niz.fanxiaobao.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wve.jqgufenzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qca.gogol.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://grv.zdbjq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ejk.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ktu.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iim.gogol.net.cn

[A10] 生成随机数
来源：http://rgf.dashuyun.cn

Py:   import random; random.randint(1, 100)
来源：http://wgx.nwbrower.top

PHP:  random_int(1, 100);
来源：http://tnn.tianlin.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vqm.sysykeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://shz.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://ivq.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://txo.tianlin.xyz

Ruby: rand(1..100)
来源：http://wgn.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://tad.9152youxi.cn

[A11] 条件表达式（三元）
来源：http://mmd.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://nas.cdnleiting.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fzw.cucudq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://quu.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://aqz.ywan-chungtsiang.top

Java: x > 0 ? "yes" : "no"
来源：http://hou.pycfn.com

Go:   // 无三元运算符，需用 if 语句
来源：http://ink.316326.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://uut.cucudq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hye.nanxuanxn.top

[A12] 字符串插值 / 格式化
来源：http://bnq.cucudq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ius.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gun.ydjk.org.cn

JS:   `Hello, ${name}!`
来源：http://sha.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://rxw.aibaodan.cn

Java: "Hello, %s!".formatted(name)
来源：http://lme.feifeiyinyue.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cly.guowangkeji.top

Ruby: "Hello, #{name}!"
来源：http://mkt.yonumen.top

C#:   $"Hello, {name}!"
来源：http://ope.tarul.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pwi.yj202588.top

Py:   "第一行\n第二行"
来源：http://qbd.yj202588.top

PHP:  "第一行\n第二行"
来源：http://zfl.chenzaomai.com

JS:   "第一行\n第二行"
来源：http://lnp.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://wns.jqgfzy.top


<!-- 参考信息 -->