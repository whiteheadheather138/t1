代发 wailian999

[U91] JS：对象键值遍历
来源：http://hvy.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mpn.jinqigufen.top

[U92] JS：深拷贝
来源：http://qqh.jinghuilouyu.cn

structuredClone(obj)
来源：http://cif.nanxuanxn.top

[U93] JS：模板字符串
来源：http://www.fanxiaobao.xyz

`共 ${n} 条`
来源：http://sff.yongpay.top

[U94] JS：箭头函数
来源：http://vda.xylfe.cn

const double = x => x * 2;
来源：http://fad.xinyue.icu

[U95] JS：Promise 包装
来源：http://dpo.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://wwa.jiagoushi.top

[U96] JS：async/await 与异常
来源：http://cal.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ldm.tian-w.cn

[U97] JS：并发请求
来源：http://cbo.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dug.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://gjm.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cna.jqgufenzy.top

[U99] JS：事件监听
来源：http://kxq.vehdjk.com

el.addEventListener("click", e => {})
来源：http://swx.hcnkem.com

[U100] JS：DOM 查询
来源：http://pwk.fanxiaobao.xyz

document.querySelector(".item")
来源：http://wxy.xuanzx.com

[U101] JS：classList 操作
来源：http://rsy.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://wwc.yj20258.top

[U102] JS：本地存储
来源：http://sxd.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://prs.hnxiangtu.top

[U103] JS：定时器
来源：http://rwv.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uzx.fktsv.cn

[U104] JS：防抖
来源：http://vzk.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpx.daxiang520.top

[U105] JS：节流
来源：http://mlc.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jzu.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://aye.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wht.zdbjq.cn

[U107] JS：数字千分位
来源：http://vnh.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dlb.gogol.net.cn

[U108] JS：随机整数
来源：http://jre.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kyo.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://day.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://auy.fzhhl.top

[U110] JS：数组分块
来源：http://lec.tian-w.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zvc.meibo888.top

[U111] JS：对象转 Map
来源：http://tjd.ydjk.org.cn

new Map(Object.entries(obj))
来源：http://smp.xziqi.cn

[U112] JS：字符串补位
来源：http://uvo.yanxiufei.cn

"7".padStart(3, "0")
来源：http://bgp.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://xhf.wangdashe.top

s.replaceAll("a", "b")
来源：http://ajh.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://bew.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pcc.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://zwr.jianghu66.top

crypto.randomUUID()
来源：http://lwd.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://xhn.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://kth.pycfn.com

[U117] JS：单元测试
来源：http://xsl.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://mwx.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://ezg.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://hfp.gotoacloud.top

[U119] JS：生产构建
来源：http://ayl.hysaishi.cn

npx vite build
来源：http://yev.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://gtb.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://yeq.nanxinkj.top

================================================================================
来源：http://alv.gzhubu.top

统计汇总
来源：http://crp.cheryme.top

================================================================================
来源：http://olp.sufxvd.cn

按语言统计（条）：
来源：http://oyh.fzhhl.top

Python ......... 252
来源：http://luh.uphjek.com

PHP ............ 252
来源：http://jkj.vqdsnc.cn

JavaScript ..... 252
来源：http://oss.feifeiyinyue.top

TypeScript ..... 212
来源：http://imz.316326.xyz

Java ........... 212
来源：http://gig.hammf.cn

Go ............. 212
来源：http://rqg.xuetiantiany.cn

Ruby ........... 212
来源：http://ppm.daxiang520.top

C# ............. 212
来源：http://jfo.tianlin.xyz

C .............. 30
来源：http://ecm.jinqigfzy.top

C++ ............ 30
来源：http://ziv.fehbvm.com

SQL ............ 90
来源：http://hrd.c1oappe.top

Bash ........... 80
来源：http://xyq.birdmap.top

Kotlin ......... 15
来源：http://jbk.nanxinkj.top

Swift .......... 15
来源：http://kgo.shangyingyoupin.top

Lua ............ 10
来源：http://hsa.fehbvm.com

Perl ........... 10
来源：http://ikx.cqqwz.cn

Scala .......... 10
来源：http://wan.dianchejie.cn

------------------------------------
来源：http://yuq.shzxlz.cn

合计 ........... 2106 条
来源：http://fzc.316326.xyz

按章节统计：
来源：http://yar.sxryk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mui.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ozs.cdnleiting.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vji.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rno.fanxiaobao.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://poy.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://exo.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jpa.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://brf.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rbl.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tjt.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hye.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ytz.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qqi.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vmv.ywan-chungtsiang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://his.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jll.zhengqikj.top

Q SQL 专题                              90
来源：http://rte.zdbjq.cn

R Bash 专题                             80
来源：http://enm.yuanzhike.top

S C / C++ 专题                          60
来源：http://kvc.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://wjp.jianghu66.top

U 高频实用片段                         120
来源：http://qee.hongshengwenyu.top

------------------------------------
来源：http://ewz.fanxiaobao.xyz

合计                                  2106 条
来源：http://xgp.xuanzx.com

--------------------------------------------------------------------------------
来源：http://oip.gotoacloud.top

使用提醒
来源：http://hjd.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://qcu.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xud.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wib.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wem.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dxt.gzhubu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zdr.yfazqb.com

—— 文件结束 ——
来源：http://goj.vqdsnc.cn

================================================================================
来源：http://twy.gotoacloud.top

程序语言常见例子速查手册（2024 版）
来源：http://vyj.ehwqpu.com

Common Programming Examples Cheat Book
来源：http://snx.cucudq.cn

================================================================================
来源：http://wfk.yj20258888.top

【收录内容】
来源：http://iil.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rdd.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ncv.yanxiufei.cn

SQL · Bash · C · C++
来源：http://ntq.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sfk.gogol.net.cn

【使用说明】
来源：http://tzo.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dkr.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cfm.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://akr.ydjk.org.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kec.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cca.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://abf.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rik.vehdjk.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jfn.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qyx.zhixingplan.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zze.tian-w.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rwf.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uzp.gaohongyu789.top

【文件统计】
来源：http://irl.jlsjyb.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hqy.gzhubu.top

--------------------------------------------------------------------------------
来源：http://sns.yvedp.cn

目  录
来源：http://xss.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://axf.nanxuanxn.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uwy.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uff.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gta.fengsongda.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lbx.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ovm.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://scm.jyoumei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://byg.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zyj.cdnleiting.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vla.fengsongda.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oer.zdqjudy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zfd.pengpengdd.cyou

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fzc.ppjwa.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fqx.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mfe.gogol.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pum.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yye.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bsm.ydjk.org.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nnp.jianghu66.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fnj.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oxt.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mcr.shuidangran.top

================================================================================
来源：http://dcr.sjlbkw.cn

A. 基础语法与类型
来源：http://dle.vqdsnc.cn

================================================================================
来源：http://jpk.redwolf501.top

[A01] Hello World
来源：http://ldf.yangfankeji.com

Py:   print("Hello, World!")
来源：http://wqy.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://qsj.bbcook.cn

JS:   console.log("Hello, World!");
来源：http://ixq.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://swt.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://bqr.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://heg.cheryme.top

Ruby: puts "Hello, World!"
来源：http://rvs.snrcjt.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uge.bjfxy.top

[A02] 变量声明与赋值
来源：http://lzi.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ikx.zhongyouzk.top

PHP:  $name = "Alex"; $age = 20;
来源：http://opd.quarkkingdee.top

JS:   let name = "Alex"; const age = 20;
来源：http://tsu.guannengcc.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://quq.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://kjf.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://eyt.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://soa.sxryk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pjq.shuidangran.top

[A03] 常量定义
来源：http://qhj.yongpay.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uqg.hongshengwenyu.top

PHP:  const PI = 3.14159;
来源：http://mwg.yj202588.top

JS:   const PI = 3.14159;
来源：http://sht.ywan-chungtsiang.top

TS:   const PI: number = 3.14159;
来源：http://pdj.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://vjg.yj202588.top

Go:   const PI = 3.14159
来源：http://ecp.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://trd.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://jgh.hammf.cn

[A04] 判断变量类型
来源：http://lvz.jinghuilouyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://omu.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kzi.yfazqb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dnz.yonumen.top

TS:   typeof x; x instanceof Date
来源：http://yvy.hnxiangtu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://spl.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://nvu.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ksv.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://wqe.gotoacloud.top

[A05] 整数除法与取模
来源：http://cgt.jinqigufen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gtf.shanyushiyangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://trg.jqgfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mwk.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yyo.gogol.net.cn

Java: 7 / 2; 7 % 2
来源：http://cne.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://kzb.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://yfm.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://inv.guowangkeji.top

[A06] 字符串转数字
来源：http://uwu.jinyuanbaomall.cn

Py:   int("42"); float("3.14")
来源：http://fro.hesvh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aiz.shanyushiyangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nhr.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cka.snrcjt.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dpj.jiagoushi.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://adz.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://you.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wlv.xingfuxueyuan.xyz

[A07] 数字转字符串
来源：http://qas.hongshengwenyu.top

Py:   str(42)
来源：http://cqn.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://sgq.yueranfly.top

JS:   String(42); (42).toString()
来源：http://qay.zdqjudy.top

TS:   String(42)
来源：http://kuf.cucudq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eos.ppjwa.cn

Go:   strconv.Itoa(42)
来源：http://srb.aizwys.cn

Ruby: 42.to_s
来源：http://tdt.gaohongyu789.top

C#:   42.ToString()
来源：http://mmh.meibo888.top

[A08] 取整与四舍五入
来源：http://vil.tarul.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yfn.iojbl.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ztr.yonumen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wij.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ehu.zdqjudy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://own.aizwys.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rls.9152youxi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wdd.316326.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aqg.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://isy.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wow.fzhhl.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zcj.jinqigufen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zwk.meibo888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://odz.shangyingyoupin.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bhp.uphjek.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ghu.fanxiaobao.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yeg.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jpq.jianghu66.top

[A10] 生成随机数
来源：http://sbc.cdnleiting.top

Py:   import random; random.randint(1, 100)
来源：http://pmj.sjlbkw.cn

PHP:  random_int(1, 100);
来源：http://xij.snrcjt.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rxj.c1oappe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pea.fengsongda.top

Java: new Random().nextInt(100) + 1
来源：http://acc.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ccs.gogol.net.cn

Ruby: rand(1..100)
来源：http://tqe.wangshuangyany.cn

C#:   new Random().Next(1, 101)
来源：http://nme.cashguo.top

[A11] 条件表达式（三元）
来源：http://vgv.ivvv.top

Py:   "yes" if x > 0 else "no"
来源：http://wou.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pbx.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://axx.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jco.zhijiandao.cn

Java: x > 0 ? "yes" : "no"
来源：http://wdt.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://iyg.nanxuanxn.top

Ruby: x > 0 ? "yes" : "no"
来源：http://giw.yuanzhike.top

C#:   x > 0 ? "yes" : "no"
来源：http://hgz.zhoulong.xyz

[A12] 字符串插值 / 格式化
来源：http://kgt.havefunace.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aep.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sla.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://wbo.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://qyw.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://wdl.sweek.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://djk.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://pvk.jqgfzy.top

C#:   $"Hello, {name}!"
来源：http://vwb.52xcode.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wrx.sweek.top

Py:   "第一行\n第二行"
来源：http://vap.dianchejie.cn

PHP:  "第一行\n第二行"
来源：http://fvs.daria6918.cn

JS:   "第一行\n第二行"
来源：http://aqj.zhengqikj.top

TS:   "第一行\n第二行"
来源：http://xmo.jinghuilouyu.cn

Java: "第一行\n第二行"
来源：http://hmb.wangdashe.top

Go:   "第一行\n第二行"
来源：http://dnn.wangshuangyany.cn

Ruby: "第一行\n第二行"
来源：http://dqu.yj20258.top

C#:   "第一行\n第二行"
来源：http://bcl.ehwqpu.com

[A14] 注释写法
来源：http://zsb.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qed.ctjpmb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://umb.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://ndc.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://rdf.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uzr.sjlbkw.cn

Go:   // 单行；/* 多行 */
来源：http://tir.zhoulong.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://rwq.xylfe.cn

C#:   // 单行；/* 多行 */
来源：http://nwv.hfpthk.cn

[A15] 空值判断与默认值
来源：http://rsg.xylfe.cn

Py:   value = data or "默认值"
来源：http://tik.dianchejie.cn

PHP:  $value = $data ?? "默认值";
来源：http://apk.guowangkeji.top

JS:   const value = data ?? "默认值";
来源：http://bwq.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://ysg.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rsr.xziqi.cn

Go:   if data == "" { data = "默认值" }
来源：http://sml.hammf.cn


<!-- 参考信息 -->