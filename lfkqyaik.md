代发 wailian999

[U89] JS：数组去重
来源：http://dym.tarul.cn

[...new Set(arr)]
来源：http://jmh.jianghu66.top

[U90] JS：数字数组排序
来源：http://ojw.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://jzy.smart0.xyz

[U91] JS：对象键值遍历
来源：http://hov.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cfv.nanxinkj.top

[U92] JS：深拷贝
来源：http://zci.zdbjq.cn

structuredClone(obj)
来源：http://kfq.haohaochexian.top

[U93] JS：模板字符串
来源：http://tvb.cucudq.cn

`共 ${n} 条`
来源：http://wzi.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://wdt.daria6918.cn

const double = x => x * 2;
来源：http://qju.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://thy.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://ohj.zycfv.cn

[U96] JS：async/await 与异常
来源：http://uku.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gay.gzhubu.top

[U97] JS：并发请求
来源：http://eqt.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://cyh.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://qxo.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tnc.ivvv.top

[U99] JS：事件监听
来源：http://ekb.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://gvt.cashguo.top

[U100] JS：DOM 查询
来源：http://rju.jyoumei.cn

document.querySelector(".item")
来源：http://eif.yj20258.top

[U101] JS：classList 操作
来源：http://klm.shuidangran.top

el.classList.toggle("active")
来源：http://aql.gogol.net.cn

[U102] JS：本地存储
来源：http://ohg.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vsx.hfpthk.cn

[U103] JS：定时器
来源：http://zdn.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wft.zhiwuduotai.top

[U104] JS：防抖
来源：http://sqv.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dqt.kuanghao11.cn

[U105] JS：节流
来源：http://gmc.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mad.gotoacloud.top

[U106] JS：日期格式化
来源：http://irs.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ass.yongpay.top

[U107] JS：数字千分位
来源：http://iaf.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ifi.nanxuanxn.top

[U108] JS：随机整数
来源：http://nfh.yvedp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lmp.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://tix.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://bzy.ctjpmb.com

[U110] JS：数组分块
来源：http://svk.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xyq.zhongyouzk.top

[U111] JS：对象转 Map
来源：http://fkx.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://djr.sweek.top

[U112] JS：字符串补位
来源：http://rjr.cucudq.cn

"7".padStart(3, "0")
来源：http://jnx.yvedp.cn

[U113] JS：正则替换全部
来源：http://cpp.yj202588.top

s.replaceAll("a", "b")
来源：http://iif.tian-w.cn

[U114] JS：JSON 深比较
来源：http://spa.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mpo.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://qov.snrcjt.cn

crypto.randomUUID()
来源：http://tfs.chenjidiqi.icu

[U116] JS：类型检查（JSDoc）
来源：http://hyk.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://kvv.cashguo.top

[U117] JS：单元测试
来源：http://ule.tanke756.top

npm i -D vitest;  npx vitest
来源：http://uoh.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://qzv.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://sht.andypj.xyz

[U119] JS：生产构建
来源：http://pme.yvedp.cn

npx vite build
来源：http://wod.bbcook.cn

[U120] JS：读取环境变量（Vite）
来源：http://sav.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://iom.ybcxt.top

================================================================================
来源：http://qwk.sjlbkw.cn

统计汇总
来源：http://uct.wangdashe.top

================================================================================
来源：http://tad.shangyingyoupin.top

按语言统计（条）：
来源：http://ulk.chenlongwang.top

Python ......... 252
来源：http://dat.ywan-chungtsiang.top

PHP ............ 252
来源：http://rue.pengpengdd.cyou

JavaScript ..... 252
来源：http://bfs.zdbjq.cn

TypeScript ..... 212
来源：http://gui.tianlin.xyz

Java ........... 212
来源：http://laz.uphjek.com

Go ............. 212
来源：http://owj.hesvh.cn

Ruby ........... 212
来源：http://mok.9152youxi.cn

C# ............. 212
来源：http://yyd.dashuyun.cn

C .............. 30
来源：http://mgo.iojbl.cn

C++ ............ 30
来源：http://hbj.jinqigfzy.top

SQL ............ 90
来源：http://jul.smart0.xyz

Bash ........... 80
来源：http://mei.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://wtu.fehbvm.com

Swift .......... 15
来源：http://phx.dianchejie.cn

Lua ............ 10
来源：http://orb.fzhhl.top

Perl ........... 10
来源：http://vwt.zhaomingkeji.xyz

Scala .......... 10
来源：http://gku.fanxiaobao.xyz

------------------------------------
来源：http://isw.yuxming.cn

合计 ........... 2106 条
来源：http://mmg.haohaochexian.top

按章节统计：
来源：http://cbm.hnqzz.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bus.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dxk.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uxf.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zsk.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lxd.guowangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ack.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jjb.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ecy.zdqjudy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jvj.epnwcf.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cwt.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gnp.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dbh.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dzf.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://upp.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dww.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://egw.hnqzz.top

Q SQL 专题                              90
来源：http://efa.yvedp.cn

R Bash 专题                             80
来源：http://qpf.tarul.cn

S C / C++ 专题                          60
来源：http://bur.hfpthk.cn

T 其他语言补充                          60
来源：http://mpc.fktsv.cn

U 高频实用片段                         120
来源：http://gef.hesvh.cn

------------------------------------
来源：http://lpc.zhaomingkeji.xyz

合计                                  2106 条
来源：http://klw.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://qxt.fengsongda.top

使用提醒
来源：http://afl.yvedp.cn

--------------------------------------------------------------------------------
来源：http://oew.xuetiantiany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eym.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rua.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wcw.yj20258.top

在旧版本上使用前请先确认语法支持情况。
来源：http://szd.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bid.0kj1m.cn

—— 文件结束 ——
来源：http://vpp.yonumen.top

================================================================================
来源：http://lil.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://lks.ivvv.top

Common Programming Examples Cheat Book
来源：http://zay.jlsjyb.cn

================================================================================
来源：http://iet.fktsv.cn

【收录内容】
来源：http://yuk.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lfd.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://siy.jyoumei.cn

SQL · Bash · C · C++
来源：http://rdy.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vua.gotoacloud.top

【使用说明】
来源：http://bcb.meibo888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gzp.yongpay.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wej.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ppu.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nzd.yanxiufei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uix.shuidangran.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ocp.yangfankeji.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hqt.xingfuxueyuan.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rdo.cucudq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vkb.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qgy.yj20258.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lbf.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lgp.sjlbkw.cn

【文件统计】
来源：http://qzw.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wze.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://rrb.havefunace.top

目  录
来源：http://wsk.yj202588.top

--------------------------------------------------------------------------------
来源：http://ksb.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tyh.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://syk.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kyx.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jou.vqdsnc.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vzf.tarul.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eio.gzhubu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tni.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yzp.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://avo.yj20258.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://shf.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nmc.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vgk.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qwx.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vkm.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://let.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gdh.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fzk.xingfuxueyuan.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://hqt.0kj1m.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aoi.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xdd.zycfv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xsu.pengpengdd.cyou

================================================================================
来源：http://kay.havefunace.top

A. 基础语法与类型
来源：http://wys.meibo888.top

================================================================================
来源：http://lvk.ywan-chungtsiang.top

[A01] Hello World
来源：http://ypw.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://hab.cheryme.top

PHP:  echo "Hello, World!";
来源：http://xrn.tianlin.xyz

JS:   console.log("Hello, World!");
来源：http://fpa.ybcxt.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mnh.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://tfy.wangdashe.top

Go:   fmt.Println("Hello, World!")
来源：http://qxe.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://emp.gaohongyu789.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zmr.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://vhn.chenzaomai.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vzz.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rcb.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kji.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hkt.jinyuanbaomall.cn

Java: String name = "Alex"; int age = 20;
来源：http://vle.chenzaomai.com

Go:   name := "Alex"; age := 20
来源：http://jyx.hcnkem.com

Ruby: name = "Alex"; age = 20
来源：http://eyu.jinyuanbaomall.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ieu.aizwys.cn

[A03] 常量定义
来源：http://ldg.ivvv.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ijy.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://eyg.nwbrower.top

JS:   const PI = 3.14159;
来源：http://lpy.9152youxi.cn

TS:   const PI: number = 3.14159;
来源：http://cuy.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://pjl.sysykeji.top

Go:   const PI = 3.14159
来源：http://xki.zhiwuduotai.top

Ruby: PI = 3.14159
来源：http://fzi.zycfv.cn

C#:   const double PI = 3.14159;
来源：http://xbt.cashguo.top

[A04] 判断变量类型
来源：http://smz.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ugt.jiagoushi.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fkx.yvedp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pxs.wangshuangyany.cn

TS:   typeof x; x instanceof Date
来源：http://dau.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://juh.iojbl.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fuz.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://igm.yongpay.top

C#:   x.GetType().Name; x is int
来源：http://amt.gogol.net.cn

[A05] 整数除法与取模
来源：http://ujn.cheryme.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hco.cucudq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mla.yj202588.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zpz.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://piw.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://wlr.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://pfk.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://nbz.zycfv.cn

C#:   7 / 2; 7 % 2
来源：http://whp.xuanzx.com

[A06] 字符串转数字
来源：http://zqr.yj20258.top

Py:   int("42"); float("3.14")
来源：http://lnp.redwolf501.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nwg.zhiwuduotai.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://enz.redwolf501.top

TS:   parseInt("42", 10); Number("42")
来源：http://ucu.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rmn.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://upq.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mgl.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gas.xuanzx.com

[A07] 数字转字符串
来源：http://hgw.yj202588.top

Py:   str(42)
来源：http://fpy.hfpthk.cn

PHP:  (string) 42; strval(42)
来源：http://fxl.sweek.top

JS:   String(42); (42).toString()
来源：http://dbc.hnqzz.top

TS:   String(42)
来源：http://zbo.birdmap.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kzv.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://whx.yanxiufei.cn

Ruby: 42.to_s
来源：http://gwh.ehwqpu.com

C#:   42.ToString()
来源：http://pvd.haohaochexian.top

[A08] 取整与四舍五入
来源：http://owq.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lqo.hongshengwenyu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ukf.zhijiandao.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://evs.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lnk.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ofo.xziqi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rql.jianghu66.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://adu.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pvm.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://zfw.zhijiandao.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fht.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://irk.haohaochexian.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qkw.shanyushiyangtech.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zqy.tanke756.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hbb.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jgo.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jaz.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xme.shuidangran.top

[A10] 生成随机数
来源：http://xoh.zhijiandao.cn

Py:   import random; random.randint(1, 100)
来源：http://diw.feifeiyinyue.top

PHP:  random_int(1, 100);
来源：http://kvy.jqgfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yes.gaohongyu789.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oit.zdbjq.cn

Java: new Random().nextInt(100) + 1
来源：http://tku.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ppe.cdnleiting.top

Ruby: rand(1..100)
来源：http://qbg.fanxiaobao.xyz

C#:   new Random().Next(1, 101)
来源：http://mrj.zhoulong.xyz

[A11] 条件表达式（三元）
来源：http://rxs.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://cda.fktsv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://udc.zhiwuduotai.top

JS:   x > 0 ? "yes" : "no"
来源：http://oom.ctjpmb.com

TS:   x > 0 ? "yes" : "no"
来源：http://qcg.jlsjyb.cn

Java: x > 0 ? "yes" : "no"
来源：http://jhg.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pkh.nanxinkj.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wpx.hammf.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wun.daria6918.cn

[A12] 字符串插值 / 格式化
来源：http://sra.redwolf501.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bis.vqdsnc.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hov.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://mul.gotoacloud.top

TS:   `Hello, ${name}!`
来源：http://nxx.sweek.top

Java: "Hello, %s!".formatted(name)
来源：http://ibb.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gqa.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://rgp.hnxiangtu.top

C#:   $"Hello, {name}!"
来源：http://fol.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ylu.ehwqpu.com

Py:   "第一行\n第二行"
来源：http://shf.epnwcf.com

PHP:  "第一行\n第二行"
来源：http://rnw.c1oappe.top

JS:   "第一行\n第二行"
来源：http://nai.xuetiantiany.cn

TS:   "第一行\n第二行"
来源：http://skf.havefunace.top

Java: "第一行\n第二行"
来源：http://maz.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://pcl.guannengcc.top

Ruby: "第一行\n第二行"
来源：http://non.fehbvm.com

C#:   "第一行\n第二行"
来源：http://rhv.fengsongda.top

[A14] 注释写法
来源：http://ipk.smart0.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://sjp.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sbw.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://yde.cheryme.top

TS:   // 单行；/* 多行 */
来源：http://ofh.yongpay.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://psy.shzxlz.cn

Go:   // 单行；/* 多行 */
来源：http://zqy.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://ovz.meibo888.top

C#:   // 单行；/* 多行 */
来源：http://yus.pengpengdd.cyou

[A15] 空值判断与默认值
来源：http://wxy.shuidangran.top

Py:   value = data or "默认值"
来源：http://urg.mhx1999.top

PHP:  $value = $data ?? "默认值";
来源：http://jan.sjlbkw.cn


<!-- 参考信息 -->