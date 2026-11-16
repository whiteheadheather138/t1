代发 wailian999

[U91] JS：对象键值遍历
来源：http://xld.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vjf.gzhubu.top

[U92] JS：深拷贝
来源：http://mco.fzhhl.top

structuredClone(obj)
来源：http://pfe.tanke756.top

[U93] JS：模板字符串
来源：http://hdt.chenlongwang.top

`共 ${n} 条`
来源：http://mux.zdqjudy.top

[U94] JS：箭头函数
来源：http://nts.cdnleiting.top

const double = x => x * 2;
来源：http://ipk.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://xfm.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://hwh.tanke756.top

[U96] JS：async/await 与异常
来源：http://ysz.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fnt.daxiang520.top

[U97] JS：并发请求
来源：http://jeq.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kuu.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://osg.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tya.jqgufenzy.top

[U99] JS：事件监听
来源：http://ybb.yfazqb.com

el.addEventListener("click", e => {})
来源：http://rev.hnqzz.top

[U100] JS：DOM 查询
来源：http://idw.yongpay.top

document.querySelector(".item")
来源：http://rtp.nanxuanxn.top

[U101] JS：classList 操作
来源：http://des.dianchejie.cn

el.classList.toggle("active")
来源：http://bno.yanxiufei.cn

[U102] JS：本地存储
来源：http://jru.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wpf.yueranfly.top

[U103] JS：定时器
来源：http://mox.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hsi.zhijiandao.cn

[U104] JS：防抖
来源：http://ems.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://asm.zhengqikj.top

[U105] JS：节流
来源：http://wri.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qlo.yvedp.cn

[U106] JS：日期格式化
来源：http://slh.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kot.yangfankeji.com

[U107] JS：数字千分位
来源：http://qal.zhixingplan.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fju.shzxlz.cn

[U108] JS：随机整数
来源：http://hsd.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kay.pengpengdd.cyou

[U109] JS：数组分组
来源：http://czw.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://aeo.snrcjt.cn

[U110] JS：数组分块
来源：http://ynl.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://khr.zycfv.cn

[U111] JS：对象转 Map
来源：http://xkd.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://ywv.yj20258.top

[U112] JS：字符串补位
来源：http://ygj.jyoumei.cn

"7".padStart(3, "0")
来源：http://bpo.zhengqikj.top

[U113] JS：正则替换全部
来源：http://fiy.zhengqikj.top

s.replaceAll("a", "b")
来源：http://hjv.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://hfc.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://klb.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://cpy.aibaodan.cn

crypto.randomUUID()
来源：http://xki.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://lsk.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://fcq.yj20258.top

[U117] JS：单元测试
来源：http://umk.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://uay.sxryk.cn

[U118] JS：开发服务器
来源：http://ugp.svipenyu.cn

npm i -D vite;  npx vite
来源：http://cfx.cashguo.top

[U119] JS：生产构建
来源：http://swv.pengpengdd.cyou

npx vite build
来源：http://bxo.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://srm.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://edh.chenjidiqi.icu

================================================================================
来源：http://ikt.shuidangran.top

统计汇总
来源：http://rvw.cucudq.cn

================================================================================
来源：http://bry.ybcxt.top

按语言统计（条）：
来源：http://vzu.hfpthk.cn

Python ......... 252
来源：http://hjv.zdbjq.cn

PHP ............ 252
来源：http://yuy.mhx1999.top

JavaScript ..... 252
来源：http://lxr.0kj1m.cn

TypeScript ..... 212
来源：http://zjs.jqgfzy.top

Java ........... 212
来源：http://fmf.yanxiufei.cn

Go ............. 212
来源：http://ueg.hammf.cn

Ruby ........... 212
来源：http://zzw.shangyingyoupin.top

C# ............. 212
来源：http://iuu.sweek.top

C .............. 30
来源：http://ykd.gogol.net.cn

C++ ............ 30
来源：http://zpi.xziqi.cn

SQL ............ 90
来源：http://yil.dashuyun.cn

Bash ........... 80
来源：http://hta.yj20258.top

Kotlin ......... 15
来源：http://vvo.yj202588.top

Swift .......... 15
来源：http://ibm.redwolf501.top

Lua ............ 10
来源：http://whh.guowangkeji.top

Perl ........... 10
来源：http://pii.sxryk.cn

Scala .......... 10
来源：http://vtx.hongshengwenyu.top

------------------------------------
来源：http://ahy.chenzaomai.com

合计 ........... 2106 条
来源：http://xqp.cdnleiting.top

按章节统计：
来源：http://uiu.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xml.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lvn.fengsongda.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pxo.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://spi.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uof.wangshuangyany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fmp.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jlh.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wex.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://idk.cheryme.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://chx.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vkn.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rqk.52xcode.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yfs.sysykeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gqu.zdbjq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ukq.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ort.gzhubu.top

Q SQL 专题                              90
来源：http://lyc.ehwqpu.com

R Bash 专题                             80
来源：http://ivm.yj20258.top

S C / C++ 专题                          60
来源：http://teg.yj20258888.top

T 其他语言补充                          60
来源：http://osg.dashuyun.cn

U 高频实用片段                         120
来源：http://hhx.yanxiufei.cn

------------------------------------
来源：http://bbl.cdnleiting.top

合计                                  2106 条
来源：http://etr.smart0.xyz

--------------------------------------------------------------------------------
来源：http://jry.xingfuxueyuan.xyz

使用提醒
来源：http://zwe.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://kzl.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xix.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vtn.xuanzx.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fwb.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gvk.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jxp.shangyingyoupin.top

—— 文件结束 ——
来源：http://jjy.aibaodan.cn

================================================================================
来源：http://tgi.tianlin.xyz

程序语言常见例子速查手册（2024 版）
来源：http://vra.aizwys.cn

Common Programming Examples Cheat Book
来源：http://uqm.xylfe.cn

================================================================================
来源：http://ehs.gotoacloud.top

【收录内容】
来源：http://zdp.yanxiufei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lhu.yongpay.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://buo.fktsv.cn

SQL · Bash · C · C++
来源：http://ryt.ywan-chungtsiang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dmv.yongpay.top

【使用说明】
来源：http://yzm.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tnd.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://grk.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oka.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rxr.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://jpa.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tjo.svipenyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uia.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dlw.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://atx.havefunace.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jdh.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xtv.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uqj.vehdjk.com

【文件统计】
来源：http://wmu.jlsjyb.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oao.yj202588.top

--------------------------------------------------------------------------------
来源：http://zpf.yj202588.top

目  录
来源：http://sea.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://mpz.aibaodan.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wzj.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bqd.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tok.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://brg.jiagoushi.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bhx.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ygg.bbcook.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://afq.quarkkingdee.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nzd.xingfuxueyuan.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qwt.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yql.shanyushiyangtech.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://max.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yvh.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cst.vehdjk.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fpq.xingfuxueyuan.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jdj.yangfankeji.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jex.mhx1999.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dbz.shuidangran.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rgq.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wek.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lrc.cucudq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dqg.gotoacloud.top

================================================================================
来源：http://pof.shuidangran.top

A. 基础语法与类型
来源：http://aeh.zhongyouzk.top

================================================================================
来源：http://vme.316326.xyz

[A01] Hello World
来源：http://smq.nanxuanxn.top

Py:   print("Hello, World!")
来源：http://nbf.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://zvl.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://jmr.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sbp.jlsjyb.cn

Java: System.out.println("Hello, World!");
来源：http://vwb.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://bjp.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://add.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://brt.uphjek.com

[A02] 变量声明与赋值
来源：http://wdq.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lwk.hnxiangtu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fya.jinqigfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://piq.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lgf.xylfe.cn

Java: String name = "Alex"; int age = 20;
来源：http://hzr.pengpengdd.cyou

Go:   name := "Alex"; age := 20
来源：http://wxl.jqgfzy.top

Ruby: name = "Alex"; age = 20
来源：http://irb.gzhubu.top

C#:   string name = "Alex"; int age = 20;
来源：http://nhp.snrcjt.cn

[A03] 常量定义
来源：http://tjw.jinqigufen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sxi.sxryk.cn

PHP:  const PI = 3.14159;
来源：http://kqm.smart0.xyz

JS:   const PI = 3.14159;
来源：http://jfz.aibaodan.cn

TS:   const PI: number = 3.14159;
来源：http://ike.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://tkq.epnwcf.com

Go:   const PI = 3.14159
来源：http://gbr.yj202588.top

Ruby: PI = 3.14159
来源：http://dmo.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://xhu.dashuyun.cn

[A04] 判断变量类型
来源：http://ank.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://fkb.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://clq.xingfuxueyuan.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tma.dianchejie.cn

TS:   typeof x; x instanceof Date
来源：http://jny.cdnleiting.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gck.daria6918.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sqa.chenlongwang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tee.daria6918.cn

C#:   x.GetType().Name; x is int
来源：http://hap.fzhhl.top

[A05] 整数除法与取模
来源：http://eny.chenjidiqi.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uqi.meibo888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://yus.fzhhl.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pon.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ppn.zhaomingkeji.xyz

Java: 7 / 2; 7 % 2
来源：http://ufu.sweek.top

Go:   7 / 2; 7 % 2
来源：http://rqo.cqqwz.cn

Ruby: 7 / 2; 7 % 2
来源：http://sjf.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://sgs.sxryk.cn

[A06] 字符串转数字
来源：http://xad.cashguo.top

Py:   int("42"); float("3.14")
来源：http://ltu.jlsjyb.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lvs.yj202588.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ybx.hongshengwenyu.top

TS:   parseInt("42", 10); Number("42")
来源：http://nba.xinyue.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aky.xinyue.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gns.52xcode.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://klg.sxryk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://maa.chenlongwang.top

[A07] 数字转字符串
来源：http://vnf.sufxvd.cn

Py:   str(42)
来源：http://xcu.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://uyh.gogol.net.cn

JS:   String(42); (42).toString()
来源：http://tnu.yuanzhike.top

TS:   String(42)
来源：http://rjl.xinyue.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://lcs.52xcode.cn

Go:   strconv.Itoa(42)
来源：http://hkr.uphjek.com

Ruby: 42.to_s
来源：http://wtp.yueranfly.top

C#:   42.ToString()
来源：http://ejn.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://vri.xziqi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mwl.cashguo.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ofj.wangdashe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://igu.xylfe.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mxw.sufxvd.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cxy.mhx1999.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tgw.nanxuanxn.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mtg.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xsl.havefunace.top

[A09] 绝对值与最大最小值
来源：http://dhw.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pzc.gzhubu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wih.pengpengdd.cyou

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rxk.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nrj.cqqwz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dik.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xwd.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://riy.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kfu.pycfn.com

[A10] 生成随机数
来源：http://rzw.hcnkem.com

Py:   import random; random.randint(1, 100)
来源：http://tck.52xcode.cn

PHP:  random_int(1, 100);
来源：http://uho.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ztf.xziqi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://svm.fengsongda.top

Java: new Random().nextInt(100) + 1
来源：http://vmk.epnwcf.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sqd.sufxvd.cn

Ruby: rand(1..100)
来源：http://isd.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://msi.cqqwz.cn

[A11] 条件表达式（三元）
来源：http://cfy.hnxiangtu.top

Py:   "yes" if x > 0 else "no"
来源：http://lck.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nzl.ctjpmb.com

JS:   x > 0 ? "yes" : "no"
来源：http://bhs.wangshuangyany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://inp.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://slq.sjlbkw.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bgt.hywenlv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vro.9152youxi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://axl.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://nzy.yuxming.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jcr.ivvv.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://psv.sxryk.cn

JS:   `Hello, ${name}!`
来源：http://ijz.zhongyouzk.top

TS:   `Hello, ${name}!`
来源：http://jrn.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://uya.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zfc.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://uud.quarkkingdee.top

C#:   $"Hello, {name}!"
来源：http://hyl.uphjek.com

[A13] 多行字符串（练习 \n 转义）
来源：http://fsy.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://kfj.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://gqd.yj20258.top

JS:   "第一行\n第二行"
来源：http://oes.tarul.cn

TS:   "第一行\n第二行"
来源：http://gdw.pycfn.com

Java: "第一行\n第二行"
来源：http://jgh.zdbjq.cn

Go:   "第一行\n第二行"
来源：http://tus.havefunace.top

Ruby: "第一行\n第二行"
来源：http://xji.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://pve.guowangkeji.top

[A14] 注释写法
来源：http://rkj.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sol.uphjek.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://oed.jinqigfzy.top

JS:   // 单行；/* 多行 */
来源：http://jwg.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://ipo.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nfv.guowangkeji.top

Go:   // 单行；/* 多行 */
来源：http://fid.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://sae.dianchejie.cn

C#:   // 单行；/* 多行 */
来源：http://qhu.ybcxt.top

[A15] 空值判断与默认值
来源：http://cfo.aizwys.cn

Py:   value = data or "默认值"
来源：http://mnv.guowangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://gxp.chenjidiqi.icu

JS:   const value = data ?? "默认值";
来源：http://bjq.daxiang520.top

TS:   const value = data ?? "默认值";
来源：http://vsg.shanyushiyangtech.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mnr.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://hrl.ctjpmb.com


<!-- 参考信息 -->