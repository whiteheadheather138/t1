代发 wailian999

[U79] PHP：静态分析
来源：http://ptk.316326.xyz

composer require --dev phpstan/phpstan
来源：http://wxv.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://oxu.uphjek.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://vcl.redwolf501.top

[U81] JS：初始化项目
来源：http://nyu.yangfankeji.com

npm init -y;  npm i express
来源：http://ujx.sweek.top

[U82] JS：package.json 脚本
来源：http://xoq.zycfv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://joa.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://lbj.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://ltx.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://rqs.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://mzq.shanyushiyangtech.top

[U85] JS：可选链
来源：http://ego.nanxinkj.top

a?.b?.c
来源：http://woj.sweek.top

[U86] JS：空值合并
来源：http://lug.kuanghao11.cn

a ?? b
来源：http://wqm.jinqigfzy.top

[U87] JS：解构默认值
来源：http://ypa.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://rwe.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://syu.ivvv.top

{ ...a, ...b }
来源：http://ais.yanxiufei.cn

[U89] JS：数组去重
来源：http://otk.nanxuanxn.top

[...new Set(arr)]
来源：http://zgh.xziqi.cn

[U90] JS：数字数组排序
来源：http://oce.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://gbs.fktsv.cn

[U91] JS：对象键值遍历
来源：http://blv.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://grn.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://qgr.jinqigfzy.top

structuredClone(obj)
来源：http://jfj.daria6918.cn

[U93] JS：模板字符串
来源：http://mhs.hongshengwenyu.top

`共 ${n} 条`
来源：http://pct.chenlongwang.top

[U94] JS：箭头函数
来源：http://woj.iojbl.cn

const double = x => x * 2;
来源：http://ubq.yuanzhike.top

[U95] JS：Promise 包装
来源：http://poy.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://ysj.havefunace.top

[U96] JS：async/await 与异常
来源：http://eyp.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pro.yvedp.cn

[U97] JS：并发请求
来源：http://hib.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uuv.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://mie.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tru.cashguo.top

[U99] JS：事件监听
来源：http://ehh.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://mzu.316326.xyz

[U100] JS：DOM 查询
来源：http://sra.wangdashe.top

document.querySelector(".item")
来源：http://uev.ctjpmb.com

[U101] JS：classList 操作
来源：http://yhu.andypj.xyz

el.classList.toggle("active")
来源：http://zrj.fehbvm.com

[U102] JS：本地存储
来源：http://fod.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gtv.daxiang520.top

[U103] JS：定时器
来源：http://fhw.zdqjudy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qac.zhoulong.xyz

[U104] JS：防抖
来源：http://dfr.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpd.ydzc1.top

[U105] JS：节流
来源：http://cvt.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fbv.zycfv.cn

[U106] JS：日期格式化
来源：http://kcz.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wzb.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://pmt.hysaishi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zfi.sweek.top

[U108] JS：随机整数
来源：http://rjn.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wju.aizwys.cn

[U109] JS：数组分组
来源：http://gfn.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://zxs.jiagoushi.top

[U110] JS：数组分块
来源：http://wgh.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ysz.andypj.xyz

[U111] JS：对象转 Map
来源：http://kpp.9152youxi.cn

new Map(Object.entries(obj))
来源：http://otr.yj20258.top

[U112] JS：字符串补位
来源：http://wyy.ivvv.top

"7".padStart(3, "0")
来源：http://sml.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://ezq.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://csc.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://ioz.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://yhn.epnwcf.com

[U115] JS：生成 UUID
来源：http://hdh.yvedp.cn

crypto.randomUUID()
来源：http://ezy.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://pyc.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://ggc.xinyue.icu

[U117] JS：单元测试
来源：http://mtn.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://uch.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://kje.fehbvm.com

npm i -D vite;  npx vite
来源：http://hax.zhoulong.xyz

[U119] JS：生产构建
来源：http://okg.chenzaomai.com

npx vite build
来源：http://bwi.zhongyouzk.top

[U120] JS：读取环境变量（Vite）
来源：http://tuj.aizwys.cn

import.meta.env.VITE_API_URL
来源：http://fhp.chenjidiqi.icu

================================================================================
来源：http://ieo.jiagoushi.top

统计汇总
来源：http://uxg.jinyuanbaomall.cn

================================================================================
来源：http://xiw.zhixingplan.top

按语言统计（条）：
来源：http://baw.jiagoushi.top

Python ......... 252
来源：http://edk.nwbrower.top

PHP ............ 252
来源：http://ymw.zhoulong.xyz

JavaScript ..... 252
来源：http://iui.birdmap.top

TypeScript ..... 212
来源：http://nhv.ivvv.top

Java ........... 212
来源：http://mww.svipenyu.cn

Go ............. 212
来源：http://gkx.sufxvd.cn

Ruby ........... 212
来源：http://jdb.wangdashe.top

C# ............. 212
来源：http://svs.pycfn.com

C .............. 30
来源：http://vwz.hnqzz.top

C++ ............ 30
来源：http://bax.xuanzx.com

SQL ............ 90
来源：http://idq.nanxinkj.top

Bash ........... 80
来源：http://nhn.jianghu66.top

Kotlin ......... 15
来源：http://poq.guannengcc.top

Swift .......... 15
来源：http://ysc.hcnkem.com

Lua ............ 10
来源：http://yjm.9152youxi.cn

Perl ........... 10
来源：http://uvw.zhoulong.xyz

Scala .......... 10
来源：http://qwd.ehwqpu.com

------------------------------------
来源：http://wwa.zdbjq.cn

合计 ........... 2106 条
来源：http://gid.uphjek.com

按章节统计：
来源：http://flf.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rxt.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://obi.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rej.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://evh.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://apb.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://unx.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uat.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wyp.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sqr.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iah.dianchejie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://owe.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://chn.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bma.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dib.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://onf.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fsg.316326.xyz

Q SQL 专题                              90
来源：http://ota.vehdjk.com

R Bash 专题                             80
来源：http://coc.hfpthk.cn

S C / C++ 专题                          60
来源：http://oqf.zhiwuduotai.top

T 其他语言补充                          60
来源：http://nei.52xcode.cn

U 高频实用片段                         120
来源：http://nvp.redwolf501.top

------------------------------------
来源：http://rzq.smart0.xyz

合计                                  2106 条
来源：http://eci.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://dvc.birdmap.top

使用提醒
来源：http://obr.shuidangran.top

--------------------------------------------------------------------------------
来源：http://bnb.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rbk.yangfankeji.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uvd.xinyue.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sii.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ucd.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://edx.daxiang520.top

—— 文件结束 ——
来源：http://est.fktsv.cn

================================================================================
来源：http://ber.316326.xyz

程序语言常见例子速查手册（2024 版）
来源：http://yax.bjfxy.top

Common Programming Examples Cheat Book
来源：http://anx.nanxuanxn.top

================================================================================
来源：http://axg.cashguo.top

【收录内容】
来源：http://ruc.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zlq.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nti.hongshengwenyu.top

SQL · Bash · C · C++
来源：http://yyb.sufxvd.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nxh.haohaochexian.top

【使用说明】
来源：http://npe.cheryme.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ekf.tarul.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yjz.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ewy.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dwi.jinqigufen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bnc.hnxiangtu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wto.andypj.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://plk.cqqwz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mna.sxryk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://beo.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qoj.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wzm.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yjs.bjfxy.top

【文件统计】
来源：http://rzn.yfazqb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oje.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://gcp.snrcjt.cn

目  录
来源：http://knm.fehbvm.com

--------------------------------------------------------------------------------
来源：http://kbd.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fpq.dianchejie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bcq.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gxc.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xle.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://plt.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://euj.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cff.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://laj.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qft.cdnleiting.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bni.zdqjudy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eki.zhoulong.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uug.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dwy.yongpay.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ofa.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lnq.vehdjk.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bqs.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ebh.tanke756.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mvw.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://poz.daxiang520.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pry.bbcook.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nqp.sweek.top

================================================================================
来源：http://eqa.wangshuangyany.cn

A. 基础语法与类型
来源：http://qjp.ydzc1.top

================================================================================
来源：http://nus.tianlin.xyz

[A01] Hello World
来源：http://vdu.yanxiufei.cn

Py:   print("Hello, World!")
来源：http://uwh.aibaodan.cn

PHP:  echo "Hello, World!";
来源：http://gti.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://uis.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nva.feifeiyinyue.top

Java: System.out.println("Hello, World!");
来源：http://ahc.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://hxs.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://rit.xziqi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lil.aibaodan.cn

[A02] 变量声明与赋值
来源：http://zqb.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gke.cashguo.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ghv.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://wqe.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yst.jyoumei.cn

Java: String name = "Alex"; int age = 20;
来源：http://dzo.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://tbn.jyoumei.cn

Ruby: name = "Alex"; age = 20
来源：http://elc.wangdashe.top

C#:   string name = "Alex"; int age = 20;
来源：http://iqs.fehbvm.com

[A03] 常量定义
来源：http://lnn.nanxuanxn.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qqi.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://rmt.xinyue.icu

JS:   const PI = 3.14159;
来源：http://bjv.jlsjyb.cn

TS:   const PI: number = 3.14159;
来源：http://gvt.wangdashe.top

Java: static final double PI = 3.14159;
来源：http://gzz.9152youxi.cn

Go:   const PI = 3.14159
来源：http://zfr.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://aso.tarul.cn

C#:   const double PI = 3.14159;
来源：http://sat.sjlbkw.cn

[A04] 判断变量类型
来源：http://yow.ydzc1.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kgh.316326.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vgh.fengsongda.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ynf.zhixingplan.top

TS:   typeof x; x instanceof Date
来源：http://lod.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iib.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://hut.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vzu.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://dgb.tian-w.cn

[A05] 整数除法与取模
来源：http://psa.wangdashe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xje.zhaomingkeji.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://zxo.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://voh.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://osv.guannengcc.top

Java: 7 / 2; 7 % 2
来源：http://mtc.zycfv.cn

Go:   7 / 2; 7 % 2
来源：http://pbf.ydzc1.top

Ruby: 7 / 2; 7 % 2
来源：http://sgw.hammf.cn

C#:   7 / 2; 7 % 2
来源：http://ikr.cashguo.top

[A06] 字符串转数字
来源：http://hsj.ivvv.top

Py:   int("42"); float("3.14")
来源：http://cvb.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nvb.ydzc1.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ley.hywenlv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vkh.316326.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cso.hywenlv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lix.zhoulong.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://nbv.chenzaomai.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wdz.daxiang520.top

[A07] 数字转字符串
来源：http://acj.ywan-chungtsiang.top

Py:   str(42)
来源：http://cqy.c1oappe.top

PHP:  (string) 42; strval(42)
来源：http://adi.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://wnp.wangshuangyany.cn

TS:   String(42)
来源：http://afr.smart0.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://obx.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://ftm.zdbjq.cn

Ruby: 42.to_s
来源：http://rqk.yj20258.top

C#:   42.ToString()
来源：http://jri.fanxiaobao.xyz

[A08] 取整与四舍五入
来源：http://yjj.cheryme.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fyd.0kj1m.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jic.gogol.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kfa.nanxinkj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yaf.zdbjq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://exk.zhaomingkeji.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zdg.gogol.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://oou.feifeiyinyue.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kjg.fzhhl.top

[A09] 绝对值与最大最小值
来源：http://jmz.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://klf.shuidangran.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yqo.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://llj.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://orz.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://shi.c1oappe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ejh.yuanzhike.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lcb.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gko.cqqwz.cn

[A10] 生成随机数
来源：http://cbg.fehbvm.com

Py:   import random; random.randint(1, 100)
来源：http://ttr.hammf.cn

PHP:  random_int(1, 100);
来源：http://kvi.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pku.zdbjq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vcx.nanxuanxn.top

Java: new Random().nextInt(100) + 1
来源：http://lqb.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wpt.wangdashe.top

Ruby: rand(1..100)
来源：http://sur.fehbvm.com

C#:   new Random().Next(1, 101)
来源：http://pkd.yongpay.top

[A11] 条件表达式（三元）
来源：http://hdf.xinyue.icu

Py:   "yes" if x > 0 else "no"
来源：http://gmu.hfpthk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ipe.hnqzz.top

JS:   x > 0 ? "yes" : "no"
来源：http://rpe.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://xij.shzxlz.cn

Java: x > 0 ? "yes" : "no"
来源：http://jdi.xinyue.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://nmd.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://bqn.yanxiufei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cps.chenjidiqi.icu

[A12] 字符串插值 / 格式化
来源：http://fyv.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://agl.jiagoushi.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vrr.jqgufenzy.top

JS:   `Hello, ${name}!`
来源：http://qet.zycfv.cn

TS:   `Hello, ${name}!`
来源：http://szg.daxiang520.top

Java: "Hello, %s!".formatted(name)
来源：http://fln.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dka.chenjidiqi.icu

Ruby: "Hello, #{name}!"
来源：http://uea.yongpay.top

C#:   $"Hello, {name}!"
来源：http://nnd.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xko.pengpengdd.cyou


<!-- 参考信息 -->