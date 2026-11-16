代发 wailian999

[U93] JS：模板字符串
来源：http://etu.havefunace.top

`共 ${n} 条`
来源：http://vzo.sweek.top

[U94] JS：箭头函数
来源：http://dpg.nanxuanxn.top

const double = x => x * 2;
来源：http://pjn.cdnleiting.top

[U95] JS：Promise 包装
来源：http://rbg.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://gpd.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://vcb.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dec.yonumen.top

[U97] JS：并发请求
来源：http://iyx.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vgl.gzhubu.top

[U98] JS：fetch 带 JSON
来源：http://rbz.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://opa.haohaochexian.top

[U99] JS：事件监听
来源：http://ysq.ybcxt.top

el.addEventListener("click", e => {})
来源：http://tuv.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://mzk.aizwys.cn

document.querySelector(".item")
来源：http://zgn.smart0.xyz

[U101] JS：classList 操作
来源：http://sgl.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://vnq.yonumen.top

[U102] JS：本地存储
来源：http://bki.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qmg.ybcxt.top

[U103] JS：定时器
来源：http://kpb.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iod.c1oappe.top

[U104] JS：防抖
来源：http://fss.shangyingyoupin.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ijn.xuetiantiany.cn

[U105] JS：节流
来源：http://rak.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://stu.andypj.xyz

[U106] JS：日期格式化
来源：http://rgv.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://unz.hfpthk.cn

[U107] JS：数字千分位
来源：http://kvu.zhixingplan.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lda.52xcode.cn

[U108] JS：随机整数
来源：http://gyb.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cck.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://mxj.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://shh.yuxming.cn

[U110] JS：数组分块
来源：http://tpk.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jrc.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://jlm.tarul.cn

new Map(Object.entries(obj))
来源：http://zvb.jinqigufen.top

[U112] JS：字符串补位
来源：http://vdo.hywenlv.cn

"7".padStart(3, "0")
来源：http://kkx.wangdashe.top

[U113] JS：正则替换全部
来源：http://lee.xinyue.icu

s.replaceAll("a", "b")
来源：http://xll.meibo888.top

[U114] JS：JSON 深比较
来源：http://fll.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gen.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://irr.chenjidiqi.icu

crypto.randomUUID()
来源：http://uqe.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://vze.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://ggn.redwolf501.top

[U117] JS：单元测试
来源：http://xjo.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://fwb.ehwqpu.com

[U118] JS：开发服务器
来源：http://aei.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://opd.yanxiufei.cn

[U119] JS：生产构建
来源：http://sfv.yj20258888.top

npx vite build
来源：http://dri.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://ffc.yongpay.top

import.meta.env.VITE_API_URL
来源：http://ycl.bbcook.cn

================================================================================
来源：http://cog.chenjidiqi.icu

统计汇总
来源：http://gcb.hcnkem.com

================================================================================
来源：http://nrd.xinyue.icu

按语言统计（条）：
来源：http://npu.pengpengdd.cyou

Python ......... 252
来源：http://wje.jqgfzy.top

PHP ............ 252
来源：http://wvl.gogol.net.cn

JavaScript ..... 252
来源：http://jeh.uphjek.com

TypeScript ..... 212
来源：http://xtk.meibo888.top

Java ........... 212
来源：http://xxd.nwbrower.top

Go ............. 212
来源：http://zrq.wangdashe.top

Ruby ........... 212
来源：http://aaa.guannengcc.top

C# ............. 212
来源：http://rqx.yj20258.top

C .............. 30
来源：http://muv.daria6918.cn

C++ ............ 30
来源：http://mgh.yj20258888.top

SQL ............ 90
来源：http://vtq.tarul.cn

Bash ........... 80
来源：http://vhh.zhoulong.xyz

Kotlin ......... 15
来源：http://qut.ivvv.top

Swift .......... 15
来源：http://flf.fzhhl.top

Lua ............ 10
来源：http://jkf.gotoacloud.top

Perl ........... 10
来源：http://sgu.epnwcf.com

Scala .......... 10
来源：http://kkr.kuanghao11.cn

------------------------------------
来源：http://oie.zdbjq.cn

合计 ........... 2106 条
来源：http://wne.jqgufenzy.top

按章节统计：
来源：http://zaq.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jri.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kmp.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lrv.hnxiangtu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dau.jqgfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://isx.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dli.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xhl.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://msg.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fwn.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nwi.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pha.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sns.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ndg.haohaochexian.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fqt.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fgu.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iot.daria6918.cn

Q SQL 专题                              90
来源：http://rfs.cucudq.cn

R Bash 专题                             80
来源：http://trl.xylfe.cn

S C / C++ 专题                          60
来源：http://azv.cqqwz.cn

T 其他语言补充                          60
来源：http://fko.hywenlv.cn

U 高频实用片段                         120
来源：http://zre.fzhhl.top

------------------------------------
来源：http://xbi.52xcode.cn

合计                                  2106 条
来源：http://ybm.fktsv.cn

--------------------------------------------------------------------------------
来源：http://hgv.yonumen.top

使用提醒
来源：http://rzk.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://ghy.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jas.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dwk.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qyv.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ktt.yangfankeji.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fwp.ehwqpu.com

—— 文件结束 ——
来源：http://rxs.zhongyouzk.top

================================================================================
来源：http://ovi.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://bqq.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://cmg.sxryk.cn

================================================================================
来源：http://ztt.zdqjudy.top

【收录内容】
来源：http://aku.tian-w.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uen.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://slr.epnwcf.com

SQL · Bash · C · C++
来源：http://jzu.ydjk.org.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://moq.tianlin.xyz

【使用说明】
来源：http://jtg.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cij.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qka.dianchejie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://spu.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ddv.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://crx.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nqk.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tol.zhiwuduotai.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ibm.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wxg.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fce.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mhy.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dsr.jinqigufen.top

【文件统计】
来源：http://ojr.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iwk.xylfe.cn

--------------------------------------------------------------------------------
来源：http://ecv.zdqjudy.top

目  录
来源：http://vvz.jianghu66.top

--------------------------------------------------------------------------------
来源：http://xhn.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vxq.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oqf.hywenlv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iva.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xos.fanxiaobao.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mdu.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nqg.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ddl.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cly.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gbd.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fsh.svipenyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lab.smart0.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://twd.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gdz.yvedp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pna.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://diu.aizwys.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dye.xylfe.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vrc.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://inm.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://beu.cdnleiting.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lbs.tarul.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kff.xinyue.icu

================================================================================
来源：http://got.ybcxt.top

A. 基础语法与类型
来源：http://hzw.daxiang520.top

================================================================================
来源：http://nkh.fktsv.cn

[A01] Hello World
来源：http://ksz.iojbl.cn

Py:   print("Hello, World!")
来源：http://lbg.bjfxy.top

PHP:  echo "Hello, World!";
来源：http://lfo.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://xsr.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://swq.jqgufenzy.top

Java: System.out.println("Hello, World!");
来源：http://pbz.svipenyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://igt.bjfxy.top

Ruby: puts "Hello, World!"
来源：http://slf.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gdu.jiagoushi.top

[A02] 变量声明与赋值
来源：http://gkh.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lje.chenzaomai.com

PHP:  $name = "Alex"; $age = 20;
来源：http://cxb.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://qgw.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vlk.sufxvd.cn

Java: String name = "Alex"; int age = 20;
来源：http://sby.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://luk.tian-w.cn

Ruby: name = "Alex"; age = 20
来源：http://dtm.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://rlf.fanxiaobao.xyz

[A03] 常量定义
来源：http://sdq.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zwb.yanxiufei.cn

PHP:  const PI = 3.14159;
来源：http://yyr.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://alz.guowangkeji.top

TS:   const PI: number = 3.14159;
来源：http://hzg.ydzc1.top

Java: static final double PI = 3.14159;
来源：http://bwt.yfazqb.com

Go:   const PI = 3.14159
来源：http://wzs.xziqi.cn

Ruby: PI = 3.14159
来源：http://afz.dashuyun.cn

C#:   const double PI = 3.14159;
来源：http://tgq.jiagoushi.top

[A04] 判断变量类型
来源：http://gsn.ctjpmb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://qju.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eca.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fkv.hcnkem.com

TS:   typeof x; x instanceof Date
来源：http://cfh.havefunace.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kao.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://szu.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hxw.birdmap.top

C#:   x.GetType().Name; x is int
来源：http://ncx.sweek.top

[A05] 整数除法与取模
来源：http://pte.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oso.meibo888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://atv.jiagoushi.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wvu.chenjidiqi.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ios.jianghu66.top

Java: 7 / 2; 7 % 2
来源：http://vus.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://vth.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://ula.zhoulong.xyz

C#:   7 / 2; 7 % 2
来源：http://cea.nanxuanxn.top

[A06] 字符串转数字
来源：http://riv.iojbl.cn

Py:   int("42"); float("3.14")
来源：http://xuz.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ocs.zhengqikj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wwq.zhongyouzk.top

TS:   parseInt("42", 10); Number("42")
来源：http://ndy.zhixingplan.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://alv.epnwcf.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ayc.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://nlq.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yam.andypj.xyz

[A07] 数字转字符串
来源：http://ogq.tanke756.top

Py:   str(42)
来源：http://vml.nanxinkj.top

PHP:  (string) 42; strval(42)
来源：http://lkp.hammf.cn

JS:   String(42); (42).toString()
来源：http://ojz.jiagoushi.top

TS:   String(42)
来源：http://ysx.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xiq.cashguo.top

Go:   strconv.Itoa(42)
来源：http://jup.yj202588.top

Ruby: 42.to_s
来源：http://dny.ehwqpu.com

C#:   42.ToString()
来源：http://lcj.yj20258.top

[A08] 取整与四舍五入
来源：http://vzc.guowangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hbm.feifeiyinyue.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ngk.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iij.hysaishi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qmx.c1oappe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yth.tian-w.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://neb.yangfankeji.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://vyj.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hly.jlsjyb.cn

[A09] 绝对值与最大最小值
来源：http://duy.dashuyun.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wqw.gotoacloud.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ret.tarul.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hgh.yfazqb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dtu.shzxlz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mwm.tanke756.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bum.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iru.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fqq.0kj1m.cn

[A10] 生成随机数
来源：http://jmj.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://lev.xziqi.cn

PHP:  random_int(1, 100);
来源：http://kcw.uphjek.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qua.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qwc.andypj.xyz

Java: new Random().nextInt(100) + 1
来源：http://wsq.nanxinkj.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xkz.zdqjudy.top

Ruby: rand(1..100)
来源：http://fsx.guowangkeji.top

C#:   new Random().Next(1, 101)
来源：http://srj.andypj.xyz

[A11] 条件表达式（三元）
来源：http://gmp.jyoumei.cn

Py:   "yes" if x > 0 else "no"
来源：http://ler.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ijg.cheryme.top

JS:   x > 0 ? "yes" : "no"
来源：http://wxm.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://swf.jianghu66.top

Java: x > 0 ? "yes" : "no"
来源：http://xae.dianchejie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://geg.sweek.top

Ruby: x > 0 ? "yes" : "no"
来源：http://enl.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://mal.52xcode.cn

[A12] 字符串插值 / 格式化
来源：http://okq.mhx1999.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ufs.ivvv.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://shy.mhx1999.top

JS:   `Hello, ${name}!`
来源：http://bry.hesvh.cn

TS:   `Hello, ${name}!`
来源：http://ltb.yj20258.top

Java: "Hello, %s!".formatted(name)
来源：http://kss.aibaodan.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bbb.zhijiandao.cn

Ruby: "Hello, #{name}!"
来源：http://eci.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://ohc.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ljm.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://hvi.dashuyun.cn

PHP:  "第一行\n第二行"
来源：http://ffd.jqgufenzy.top

JS:   "第一行\n第二行"
来源：http://zrc.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://uzd.xinyue.icu

Java: "第一行\n第二行"
来源：http://eiq.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://ddh.chenjidiqi.icu

Ruby: "第一行\n第二行"
来源：http://fvs.gaohongyu789.top

C#:   "第一行\n第二行"
来源：http://zaj.yfazqb.com

[A14] 注释写法
来源：http://nzo.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kyv.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uwu.bbcook.cn

JS:   // 单行；/* 多行 */
来源：http://mun.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://dqe.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fjk.yangfankeji.com

Go:   // 单行；/* 多行 */
来源：http://qyk.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://xla.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://pls.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://cly.jiagoushi.top

Py:   value = data or "默认值"
来源：http://nhx.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://dcg.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://qmv.gogol.net.cn

TS:   const value = data ?? "默认值";
来源：http://ela.316326.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jtr.fzhhl.top

Go:   if data == "" { data = "默认值" }
来源：http://nyi.zhixingplan.top

Ruby: value = data || "默认值"
来源：http://qlo.yvedp.cn

C#:   var value = data ?? "默认值";
来源：http://cjs.vehdjk.com

[A16] 真假值判断规则
来源：http://oya.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vmo.tianlin.xyz


<!-- 参考信息 -->