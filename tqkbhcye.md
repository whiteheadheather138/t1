代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://ann.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ghh.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://lpf.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://owh.quarkkingdee.top

[U85] JS：可选链
来源：http://uxk.yj20258.top

a?.b?.c
来源：http://nek.zhixingplan.top

[U86] JS：空值合并
来源：http://rgb.ybcxt.top

a ?? b
来源：http://ibq.yanxiufei.cn

[U87] JS：解构默认值
来源：http://cbj.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://zwy.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://vza.ydjk.org.cn

{ ...a, ...b }
来源：http://pxz.vqdsnc.cn

[U89] JS：数组去重
来源：http://lfe.jyoumei.cn

[...new Set(arr)]
来源：http://iky.sxryk.cn

[U90] JS：数字数组排序
来源：http://nqn.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://hxk.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://amz.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qxi.zhongyouzk.top

[U92] JS：深拷贝
来源：http://nge.jinyuanbaomall.cn

structuredClone(obj)
来源：http://vcx.meibo888.top

[U93] JS：模板字符串
来源：http://ozf.jqgufenzy.top

`共 ${n} 条`
来源：http://epy.nanxinkj.top

[U94] JS：箭头函数
来源：http://gpd.guannengcc.top

const double = x => x * 2;
来源：http://tjr.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://yme.uphjek.com

new Promise((resolve, reject) => {})
来源：http://xat.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://hll.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ycf.nanxuanxn.top

[U97] JS：并发请求
来源：http://gtv.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ivc.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://vka.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kmz.yueranfly.top

[U99] JS：事件监听
来源：http://wcp.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://pwy.cqqwz.cn

[U100] JS：DOM 查询
来源：http://uje.52xcode.cn

document.querySelector(".item")
来源：http://ohr.hysaishi.cn

[U101] JS：classList 操作
来源：http://rkc.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://eje.52xcode.cn

[U102] JS：本地存储
来源：http://ela.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fxa.cashguo.top

[U103] JS：定时器
来源：http://wfu.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qot.mhx1999.top

[U104] JS：防抖
来源：http://aro.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jrr.xinyue.icu

[U105] JS：节流
来源：http://zxw.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ghs.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://hjw.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://znu.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://xkl.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pfq.fktsv.cn

[U108] JS：随机整数
来源：http://alh.dianchejie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jyk.shzxlz.cn

[U109] JS：数组分组
来源：http://aax.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://myt.tianlin.xyz

[U110] JS：数组分块
来源：http://gjv.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rsz.vehdjk.com

[U111] JS：对象转 Map
来源：http://rtd.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://xrx.zdqjudy.top

[U112] JS：字符串补位
来源：http://snw.daxiang520.top

"7".padStart(3, "0")
来源：http://suj.aibaodan.cn

[U113] JS：正则替换全部
来源：http://rch.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://xjg.epnwcf.com

[U114] JS：JSON 深比较
来源：http://pfm.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dai.hesvh.cn

[U115] JS：生成 UUID
来源：http://yst.yj202588.top

crypto.randomUUID()
来源：http://thd.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://nhr.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://wsn.yueranfly.top

[U117] JS：单元测试
来源：http://owl.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://vjh.yvedp.cn

[U118] JS：开发服务器
来源：http://zxq.xziqi.cn

npm i -D vite;  npx vite
来源：http://ngk.yvedp.cn

[U119] JS：生产构建
来源：http://rzc.tanke756.top

npx vite build
来源：http://nsm.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://fhf.sweek.top

import.meta.env.VITE_API_URL
来源：http://nyz.nwbrower.top

================================================================================
来源：http://vih.yueranfly.top

统计汇总
来源：http://fby.cashguo.top

================================================================================
来源：http://zje.52xcode.cn

按语言统计（条）：
来源：http://kjh.daxiang520.top

Python ......... 252
来源：http://drh.sjlbkw.cn

PHP ............ 252
来源：http://lfp.iojbl.cn

JavaScript ..... 252
来源：http://ovl.guannengcc.top

TypeScript ..... 212
来源：http://jix.shanyushiyangkeji.top

Java ........... 212
来源：http://laj.hesvh.cn

Go ............. 212
来源：http://yan.nanxuanxn.top

Ruby ........... 212
来源：http://cqk.316326.xyz

C# ............. 212
来源：http://rdk.cheryme.top

C .............. 30
来源：http://ndw.redwolf501.top

C++ ............ 30
来源：http://vlx.uphjek.com

SQL ............ 90
来源：http://oip.shangyingyoupin.top

Bash ........... 80
来源：http://uti.yj20258888.top

Kotlin ......... 15
来源：http://xfs.jyoumei.cn

Swift .......... 15
来源：http://pec.fktsv.cn

Lua ............ 10
来源：http://coz.jlsjyb.cn

Perl ........... 10
来源：http://sac.fanxiaobao.xyz

Scala .......... 10
来源：http://oiy.haohaochexian.top

------------------------------------
来源：http://azn.hywenlv.cn

合计 ........... 2106 条
来源：http://bee.9152youxi.cn

按章节统计：
来源：http://etm.mhx1999.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bnx.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ref.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jjs.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nyd.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iju.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fri.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fbw.yj20258888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wpo.chenjidiqi.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oqu.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tjg.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://coc.bbcook.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kpd.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hkg.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lwe.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lkp.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://swg.quarkkingdee.top

Q SQL 专题                              90
来源：http://ytq.gzhubu.top

R Bash 专题                             80
来源：http://fse.hywenlv.cn

S C / C++ 专题                          60
来源：http://tdy.hywenlv.cn

T 其他语言补充                          60
来源：http://kbq.zhiwuduotai.top

U 高频实用片段                         120
来源：http://zei.ctjpmb.com

------------------------------------
来源：http://xwv.cheryme.top

合计                                  2106 条
来源：http://iau.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://dta.ybcxt.top

使用提醒
来源：http://bsi.yonumen.top

--------------------------------------------------------------------------------
来源：http://lyk.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uow.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rio.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://utd.fzhhl.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vgf.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://olv.yuxming.cn

—— 文件结束 ——
来源：http://wsf.cdnleiting.top

================================================================================
来源：http://lan.chenjidiqi.icu

程序语言常见例子速查手册（2024 版）
来源：http://mjc.havefunace.top

Common Programming Examples Cheat Book
来源：http://eja.bbcook.cn

================================================================================
来源：http://klm.316326.xyz

【收录内容】
来源：http://wuq.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ryw.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://orx.zhongyouzk.top

SQL · Bash · C · C++
来源：http://nmq.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://luu.aizwys.cn

【使用说明】
来源：http://ztr.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hvh.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hlk.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ltj.316326.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://daj.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://aoj.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lhk.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oap.vehdjk.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uzz.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nac.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vfb.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mrq.shanyushiyangtech.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://why.sjlbkw.cn

【文件统计】
来源：http://tvn.jinyuanbaomall.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eul.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://trs.mhx1999.top

目  录
来源：http://kgn.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://ysf.xuetiantiany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yfo.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mkf.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vdy.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yta.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vpu.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tjx.yuxming.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://igc.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jtp.xingfuxueyuan.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hst.hongshengwenyu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qcq.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rer.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://npp.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lhp.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jar.ydjk.org.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lnp.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xhf.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rwz.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ncu.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vrl.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bvk.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kcy.feifeiyinyue.top

================================================================================
来源：http://jwz.jiagoushi.top

A. 基础语法与类型
来源：http://lxz.xuetiantiany.cn

================================================================================
来源：http://mxv.yonumen.top

[A01] Hello World
来源：http://obj.ybcxt.top

Py:   print("Hello, World!")
来源：http://hgh.yanxiufei.cn

PHP:  echo "Hello, World!";
来源：http://nps.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://uax.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vbp.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://tmi.haohaochexian.top

Go:   fmt.Println("Hello, World!")
来源：http://wms.havefunace.top

Ruby: puts "Hello, World!"
来源：http://uqk.quarkkingdee.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gub.cucudq.cn

[A02] 变量声明与赋值
来源：http://xuc.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oor.fehbvm.com

PHP:  $name = "Alex"; $age = 20;
来源：http://btf.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rzz.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://feh.jianghu66.top

Java: String name = "Alex"; int age = 20;
来源：http://kwx.mhx1999.top

Go:   name := "Alex"; age := 20
来源：http://xue.ppjwa.cn

Ruby: name = "Alex"; age = 20
来源：http://ojw.hfpthk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mbq.yfazqb.com

[A03] 常量定义
来源：http://oej.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qmv.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://kpn.xinyue.icu

JS:   const PI = 3.14159;
来源：http://ygr.chenzaomai.com

TS:   const PI: number = 3.14159;
来源：http://mni.jinghuilouyu.cn

Java: static final double PI = 3.14159;
来源：http://jcg.hysaishi.cn

Go:   const PI = 3.14159
来源：http://ttg.hcnkem.com

Ruby: PI = 3.14159
来源：http://bbf.guowangkeji.top

C#:   const double PI = 3.14159;
来源：http://mlm.hammf.cn

[A04] 判断变量类型
来源：http://kwd.fzhhl.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://aal.yj20258.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mge.bbcook.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ppf.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://efz.feifeiyinyue.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rqi.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://nms.hammf.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vur.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://eze.gzhubu.top

[A05] 整数除法与取模
来源：http://pyw.jinghuilouyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hfv.yonumen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kmy.fehbvm.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qki.yuanzhike.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bih.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://zmk.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://hop.hcnkem.com

Ruby: 7 / 2; 7 % 2
来源：http://dpo.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://apj.ydjk.org.cn

[A06] 字符串转数字
来源：http://zjz.nanxinkj.top

Py:   int("42"); float("3.14")
来源：http://szk.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yxd.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pia.mhx1999.top

TS:   parseInt("42", 10); Number("42")
来源：http://xla.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mri.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rqw.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xrd.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rre.52xcode.cn

[A07] 数字转字符串
来源：http://aim.xuetiantiany.cn

Py:   str(42)
来源：http://xqu.xingfuxueyuan.xyz

PHP:  (string) 42; strval(42)
来源：http://fqr.jiagoushi.top

JS:   String(42); (42).toString()
来源：http://ypq.pycfn.com

TS:   String(42)
来源：http://pgh.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zmu.ctjpmb.com

Go:   strconv.Itoa(42)
来源：http://umk.jyoumei.cn

Ruby: 42.to_s
来源：http://zcy.zdqjudy.top

C#:   42.ToString()
来源：http://ino.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://hfy.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://crh.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://was.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oms.nanxinkj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://znk.yj20258.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://spd.zhaomingkeji.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tow.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://otw.zhoulong.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jsg.zhengqikj.top

[A09] 绝对值与最大最小值
来源：http://smg.jinyuanbaomall.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://okz.haohaochexian.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xul.hnxiangtu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fop.gaohongyu789.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uix.ivvv.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fzw.cdnleiting.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qcu.daria6918.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lhx.hywenlv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gpp.sufxvd.cn

[A10] 生成随机数
来源：http://cnh.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://yjq.ydjk.org.cn

PHP:  random_int(1, 100);
来源：http://ktj.fanxiaobao.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vec.yonumen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zck.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://eem.hesvh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bkl.pycfn.com

Ruby: rand(1..100)
来源：http://kuc.ywan-chungtsiang.top

C#:   new Random().Next(1, 101)
来源：http://feg.316326.xyz

[A11] 条件表达式（三元）
来源：http://oon.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://coc.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ntn.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gnx.jianghu66.top

TS:   x > 0 ? "yes" : "no"
来源：http://xxg.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://yhs.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sov.zdbjq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dzg.xingfuxueyuan.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://hfh.cucudq.cn

[A12] 字符串插值 / 格式化
来源：http://wwz.zdqjudy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sbr.ybcxt.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gcx.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://vap.xuetiantiany.cn

TS:   `Hello, ${name}!`
来源：http://yxe.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://qtl.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yah.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://kee.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://otb.hesvh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dda.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://tuh.yj20258888.top

PHP:  "第一行\n第二行"
来源：http://huj.cucudq.cn

JS:   "第一行\n第二行"
来源：http://ahc.iojbl.cn

TS:   "第一行\n第二行"
来源：http://ynw.guowangkeji.top

Java: "第一行\n第二行"
来源：http://rjt.zdbjq.cn

Go:   "第一行\n第二行"
来源：http://sau.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://fbj.shzxlz.cn

C#:   "第一行\n第二行"
来源：http://nhu.jlsjyb.cn


<!-- 参考信息 -->