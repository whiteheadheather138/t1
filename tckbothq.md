代发 wailian999

[U87] JS：解构默认值
来源：http://jqu.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://ige.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://hrj.epnwcf.com

{ ...a, ...b }
来源：http://afj.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://rle.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://sey.cucudq.cn

[U90] JS：数字数组排序
来源：http://zjt.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://cxm.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://bcf.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eyw.guowangkeji.top

[U92] JS：深拷贝
来源：http://khu.xziqi.cn

structuredClone(obj)
来源：http://gvx.yj202588.top

[U93] JS：模板字符串
来源：http://usf.chenjidiqi.icu

`共 ${n} 条`
来源：http://tks.zhoulong.xyz

[U94] JS：箭头函数
来源：http://ume.tian-w.cn

const double = x => x * 2;
来源：http://rff.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://rqd.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://pai.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://fbr.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ywe.9152youxi.cn

[U97] JS：并发请求
来源：http://atl.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://suz.wangshuangyany.cn

[U98] JS：fetch 带 JSON
来源：http://qef.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oim.hywenlv.cn

[U99] JS：事件监听
来源：http://ilp.yonumen.top

el.addEventListener("click", e => {})
来源：http://lyz.havefunace.top

[U100] JS：DOM 查询
来源：http://jhc.dianchejie.cn

document.querySelector(".item")
来源：http://kzd.sweek.top

[U101] JS：classList 操作
来源：http://twx.hongshengwenyu.top

el.classList.toggle("active")
来源：http://mai.fengsongda.top

[U102] JS：本地存储
来源：http://vvt.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rpq.epnwcf.com

[U103] JS：定时器
来源：http://chp.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://swi.yanxiufei.cn

[U104] JS：防抖
来源：http://dcu.snrcjt.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ttl.epnwcf.com

[U105] JS：节流
来源：http://wjt.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rwd.zhixingplan.top

[U106] JS：日期格式化
来源：http://iuc.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mfz.smart0.xyz

[U107] JS：数字千分位
来源：http://ejl.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cdf.fzhhl.top

[U108] JS：随机整数
来源：http://rvh.hnqzz.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fnb.yuxming.cn

[U109] JS：数组分组
来源：http://zvl.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://drt.gotoacloud.top

[U110] JS：数组分块
来源：http://rpg.mhx1999.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xvx.jinghuilouyu.cn

[U111] JS：对象转 Map
来源：http://tng.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://yue.gaohongyu789.top

[U112] JS：字符串补位
来源：http://bes.shzxlz.cn

"7".padStart(3, "0")
来源：http://vhq.nwbrower.top

[U113] JS：正则替换全部
来源：http://xnw.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://hhg.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://amj.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ine.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://odf.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://jbj.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://xwp.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://mid.yangfankeji.com

[U117] JS：单元测试
来源：http://hju.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://bxi.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://nvm.svipenyu.cn

npm i -D vite;  npx vite
来源：http://qzu.uphjek.com

[U119] JS：生产构建
来源：http://lph.xylfe.cn

npx vite build
来源：http://bgl.nanxuanxn.top

[U120] JS：读取环境变量（Vite）
来源：http://rky.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://nkl.ybcxt.top

================================================================================
来源：http://zzu.jinghuilouyu.cn

统计汇总
来源：http://yzc.nanxinkj.top

================================================================================
来源：http://epu.yj20258888.top

按语言统计（条）：
来源：http://dba.9152youxi.cn

Python ......... 252
来源：http://vxn.yuxming.cn

PHP ............ 252
来源：http://hbo.aizwys.cn

JavaScript ..... 252
来源：http://wtf.bbcook.cn

TypeScript ..... 212
来源：http://zsh.zhijiandao.cn

Java ........... 212
来源：http://cro.chenzaomai.com

Go ............. 212
来源：http://xtl.tianlin.xyz

Ruby ........... 212
来源：http://fzf.316326.xyz

C# ............. 212
来源：http://gdx.hnqzz.top

C .............. 30
来源：http://huk.xuanzx.com

C++ ............ 30
来源：http://mwl.zhaomingkeji.xyz

SQL ............ 90
来源：http://mix.daxiang520.top

Bash ........... 80
来源：http://pcz.xziqi.cn

Kotlin ......... 15
来源：http://jrw.bjfxy.top

Swift .......... 15
来源：http://zqj.tanke756.top

Lua ............ 10
来源：http://bbc.sjlbkw.cn

Perl ........... 10
来源：http://gpd.jiagoushi.top

Scala .......... 10
来源：http://gdb.quarkkingdee.top

------------------------------------
来源：http://fwm.jianghu66.top

合计 ........... 2106 条
来源：http://zuq.fehbvm.com

按章节统计：
来源：http://hco.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hth.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gjc.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vpu.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dlf.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ald.yonumen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://siu.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xbe.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://smv.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mjo.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://toi.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ywn.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zoe.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jyf.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gqu.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jyj.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nba.jyoumei.cn

Q SQL 专题                              90
来源：http://xfs.shzxlz.cn

R Bash 专题                             80
来源：http://xua.zhengqikj.top

S C / C++ 专题                          60
来源：http://ntr.daria6918.cn

T 其他语言补充                          60
来源：http://kfb.shzxlz.cn

U 高频实用片段                         120
来源：http://gbn.yj20258888.top

------------------------------------
来源：http://tsv.zdqjudy.top

合计                                  2106 条
来源：http://nan.hcnkem.com

--------------------------------------------------------------------------------
来源：http://irn.xuetiantiany.cn

使用提醒
来源：http://cgr.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://gfq.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wvz.zdqjudy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uzo.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cdx.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lst.guowangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xpt.ydjk.org.cn

—— 文件结束 ——
来源：http://ecl.daxiang520.top

================================================================================
来源：http://xjp.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://mey.bjfxy.top

Common Programming Examples Cheat Book
来源：http://dth.xuetiantiany.cn

================================================================================
来源：http://qsn.xziqi.cn

【收录内容】
来源：http://qal.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://egw.jinyuanbaomall.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ckk.tian-w.cn

SQL · Bash · C · C++
来源：http://ycf.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nnf.wangdashe.top

【使用说明】
来源：http://fga.tarul.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wue.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mgn.feifeiyinyue.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bbh.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ofp.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yog.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vjc.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cxp.xinyue.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bqi.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gup.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uxc.gzhubu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rgr.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eis.cashguo.top

【文件统计】
来源：http://nuu.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ycv.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://hkc.chenlongwang.top

目  录
来源：http://ktu.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://pei.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qmy.jinyuanbaomall.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cqp.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zcs.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dhi.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jas.ydjk.org.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://slo.quarkkingdee.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://twg.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xcp.bbcook.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xgp.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://idz.quarkkingdee.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sqy.sysykeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://inc.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://euv.zhengqikj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xkl.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://khf.zhiwuduotai.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pnw.sysykeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qng.jianghu66.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://llc.yfazqb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fru.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mwt.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lhr.snrcjt.cn

================================================================================
来源：http://akt.mhx1999.top

A. 基础语法与类型
来源：http://lxj.uphjek.com

================================================================================
来源：http://ofe.birdmap.top

[A01] Hello World
来源：http://qmo.xingfuxueyuan.xyz

Py:   print("Hello, World!")
来源：http://pjl.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://vtu.shuidangran.top

JS:   console.log("Hello, World!");
来源：http://hkk.gaohongyu789.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://khe.jyoumei.cn

Java: System.out.println("Hello, World!");
来源：http://ekd.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://wdy.redwolf501.top

Ruby: puts "Hello, World!"
来源：http://zjk.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://imf.zdbjq.cn

[A02] 变量声明与赋值
来源：http://uki.sxryk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pxi.zhongyouzk.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ljl.yuanzhike.top

JS:   let name = "Alex"; const age = 20;
来源：http://bxc.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iei.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://gdz.yuanzhike.top

Go:   name := "Alex"; age := 20
来源：http://ipe.chenzaomai.com

Ruby: name = "Alex"; age = 20
来源：http://bpx.sweek.top

C#:   string name = "Alex"; int age = 20;
来源：http://cfg.9152youxi.cn

[A03] 常量定义
来源：http://tcb.cqqwz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gwl.zdqjudy.top

PHP:  const PI = 3.14159;
来源：http://lpp.gaohongyu789.top

JS:   const PI = 3.14159;
来源：http://mdd.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://udx.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://zib.aizwys.cn

Go:   const PI = 3.14159
来源：http://ukt.chenzaomai.com

Ruby: PI = 3.14159
来源：http://leo.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://boi.jlsjyb.cn

[A04] 判断变量类型
来源：http://qpe.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vzd.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yzm.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bgc.cdnleiting.top

TS:   typeof x; x instanceof Date
来源：http://drq.vehdjk.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vtr.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://klj.daria6918.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pxg.jyoumei.cn

C#:   x.GetType().Name; x is int
来源：http://lwn.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://qoc.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kea.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://vrn.fengsongda.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yia.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gcb.gzhubu.top

Java: 7 / 2; 7 % 2
来源：http://uyb.hnqzz.top

Go:   7 / 2; 7 % 2
来源：http://zgh.jqgufenzy.top

Ruby: 7 / 2; 7 % 2
来源：http://tma.nwbrower.top

C#:   7 / 2; 7 % 2
来源：http://pzn.mhx1999.top

[A06] 字符串转数字
来源：http://bvg.hnxiangtu.top

Py:   int("42"); float("3.14")
来源：http://rod.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vbj.shangyingyoupin.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qit.xingfuxueyuan.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://tyq.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fmt.jiagoushi.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rpi.xinyue.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://zsu.tianlin.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wgq.yj20258.top

[A07] 数字转字符串
来源：http://tao.kuanghao11.cn

Py:   str(42)
来源：http://yoq.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://ezt.nanxinkj.top

JS:   String(42); (42).toString()
来源：http://zxv.mhx1999.top

TS:   String(42)
来源：http://ujr.yonumen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gra.pycfn.com

Go:   strconv.Itoa(42)
来源：http://bkc.zhongyouzk.top

Ruby: 42.to_s
来源：http://hkc.shangyingyoupin.top

C#:   42.ToString()
来源：http://bhm.jianghu66.top

[A08] 取整与四舍五入
来源：http://ddi.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://han.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rqp.tarul.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jsy.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mpm.ivvv.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yzz.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jzp.zdbjq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pub.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://day.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://ibb.birdmap.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cnx.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wcx.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qyk.shanyushiyangtech.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://axo.chenlongwang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jnf.hammf.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kpp.kuanghao11.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dff.dianchejie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eca.redwolf501.top

[A10] 生成随机数
来源：http://lne.mhx1999.top

Py:   import random; random.randint(1, 100)
来源：http://dex.sufxvd.cn

PHP:  random_int(1, 100);
来源：http://ubr.yj202588.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dqg.aibaodan.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://iih.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://ybz.guowangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uqv.xziqi.cn

Ruby: rand(1..100)
来源：http://lgd.xingfuxueyuan.xyz

C#:   new Random().Next(1, 101)
来源：http://emb.jianghu66.top

[A11] 条件表达式（三元）
来源：http://wcr.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://clt.quarkkingdee.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vzp.yfazqb.com

JS:   x > 0 ? "yes" : "no"
来源：http://xtb.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://rat.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://opq.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://wky.cqqwz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bph.yongpay.top

C#:   x > 0 ? "yes" : "no"
来源：http://hef.yj20258.top

[A12] 字符串插值 / 格式化
来源：http://etu.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vfr.pycfn.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nve.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://juq.hnxiangtu.top

TS:   `Hello, ${name}!`
来源：http://phw.cashguo.top

Java: "Hello, %s!".formatted(name)
来源：http://euv.zdbjq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yrc.bbcook.cn

Ruby: "Hello, #{name}!"
来源：http://uoz.bbcook.cn

C#:   $"Hello, {name}!"
来源：http://olh.haohaochexian.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wac.zdbjq.cn

Py:   "第一行\n第二行"
来源：http://koi.iojbl.cn

PHP:  "第一行\n第二行"
来源：http://mjo.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://yhm.aizwys.cn

TS:   "第一行\n第二行"
来源：http://rhh.jinqigfzy.top

Java: "第一行\n第二行"
来源：http://drj.yj20258.top

Go:   "第一行\n第二行"
来源：http://iia.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://jrs.xuanzx.com

C#:   "第一行\n第二行"
来源：http://kxa.meibo888.top

[A14] 注释写法
来源：http://uoh.guowangkeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fng.zhaomingkeji.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://isl.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://hvm.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://jyh.yanxiufei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://npj.hesvh.cn

Go:   // 单行；/* 多行 */
来源：http://kvd.cashguo.top

Ruby: # 单行；=begin 多行 =end
来源：http://cbf.jinqigufen.top


<!-- 参考信息 -->