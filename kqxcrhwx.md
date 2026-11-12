代发 wailian999

[U93] JS：模板字符串
来源：http://wiu.andypj.xyz

`共 ${n} 条`
来源：http://idu.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://eun.ydjk.org.cn

const double = x => x * 2;
来源：http://tlz.shuidangran.top

[U95] JS：Promise 包装
来源：http://fvi.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://csj.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://bih.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gbs.jyoumei.cn

[U97] JS：并发请求
来源：http://egp.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xho.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://ozm.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blc.haohaochexian.top

[U99] JS：事件监听
来源：http://huf.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://qgt.fengsongda.top

[U100] JS：DOM 查询
来源：http://rld.pengpengdd.cyou

document.querySelector(".item")
来源：http://wdc.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://xkv.cqqwz.cn

el.classList.toggle("active")
来源：http://uos.yanxiufei.cn

[U102] JS：本地存储
来源：http://ocs.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bli.cheryme.top

[U103] JS：定时器
来源：http://zon.guowangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ssw.iojbl.cn

[U104] JS：防抖
来源：http://oci.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lrx.316326.xyz

[U105] JS：节流
来源：http://fzv.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hdu.cdnleiting.top

[U106] JS：日期格式化
来源：http://fgy.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nyq.jianghu66.top

[U107] JS：数字千分位
来源：http://niv.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wut.hnqzz.top

[U108] JS：随机整数
来源：http://qid.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zqr.aizwys.cn

[U109] JS：数组分组
来源：http://yxc.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://zny.fzhhl.top

[U110] JS：数组分块
来源：http://fdj.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rwb.gogol.net.cn

[U111] JS：对象转 Map
来源：http://zsw.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://bgj.kuanghao11.cn

[U112] JS：字符串补位
来源：http://dis.epnwcf.com

"7".padStart(3, "0")
来源：http://fov.jqgfzy.top

[U113] JS：正则替换全部
来源：http://xxy.zhengqikj.top

s.replaceAll("a", "b")
来源：http://gdd.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://sdn.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lpq.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://kwi.jiagoushi.top

crypto.randomUUID()
来源：http://hud.chenzaomai.com

[U116] JS：类型检查（JSDoc）
来源：http://bly.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://jyj.ehwqpu.com

[U117] JS：单元测试
来源：http://dpc.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://ahh.chenzaomai.com

[U118] JS：开发服务器
来源：http://ylu.jiagoushi.top

npm i -D vite;  npx vite
来源：http://nzz.yuanzhike.top

[U119] JS：生产构建
来源：http://kfr.yfazqb.com

npx vite build
来源：http://egv.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://fqj.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://jdp.tianlin.xyz

================================================================================
来源：http://bst.jlsjyb.cn

统计汇总
来源：http://dqw.hcnkem.com

================================================================================
来源：http://xdz.ydjk.org.cn

按语言统计（条）：
来源：http://ryn.ctjpmb.com

Python ......... 252
来源：http://zmn.svipenyu.cn

PHP ............ 252
来源：http://lkg.hnxiangtu.top

JavaScript ..... 252
来源：http://ujv.fktsv.cn

TypeScript ..... 212
来源：http://nho.yfazqb.com

Java ........... 212
来源：http://bct.fzhhl.top

Go ............. 212
来源：http://abz.iojbl.cn

Ruby ........... 212
来源：http://gbo.zhongyouzk.top

C# ............. 212
来源：http://nyu.tianlin.xyz

C .............. 30
来源：http://seu.iojbl.cn

C++ ............ 30
来源：http://axn.316326.xyz

SQL ............ 90
来源：http://icv.aibaodan.cn

Bash ........... 80
来源：http://qgx.gogol.net.cn

Kotlin ......... 15
来源：http://brh.yueranfly.top

Swift .......... 15
来源：http://qoa.ivvv.top

Lua ............ 10
来源：http://xep.bbcook.cn

Perl ........... 10
来源：http://ukk.wangshuangyany.cn

Scala .......... 10
来源：http://vhl.xingfuxueyuan.xyz

------------------------------------
来源：http://vaq.mhx1999.top

合计 ........... 2106 条
来源：http://omh.fengsongda.top

按章节统计：
来源：http://zfy.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xxx.daxiang520.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lzf.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bsv.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ubi.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ogu.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wsh.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://joi.aizwys.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://otf.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dul.cashguo.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nfr.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wwz.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yqq.zhoulong.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://twe.yuxming.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rgx.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aiz.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://whu.ydjk.org.cn

Q SQL 专题                              90
来源：http://gwx.tanke756.top

R Bash 专题                             80
来源：http://zii.jqgufenzy.top

S C / C++ 专题                          60
来源：http://rfo.sweek.top

T 其他语言补充                          60
来源：http://rqr.jiagoushi.top

U 高频实用片段                         120
来源：http://bzm.jinqigfzy.top

------------------------------------
来源：http://apg.zhengqikj.top

合计                                  2106 条
来源：http://oym.uphjek.com

--------------------------------------------------------------------------------
来源：http://acn.hysaishi.cn

使用提醒
来源：http://nhu.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://wfz.xinyue.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://str.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ifc.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://laq.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://stu.guannengcc.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baz.fktsv.cn

—— 文件结束 ——
来源：http://pzg.daxiang520.top

================================================================================
来源：http://zfl.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://zfn.tian-w.cn

Common Programming Examples Cheat Book
来源：http://zyo.tanke756.top

================================================================================
来源：http://sye.yonumen.top

【收录内容】
来源：http://xgy.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bjq.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pmk.fzhhl.top

SQL · Bash · C · C++
来源：http://gpm.sxryk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tzl.ivvv.top

【使用说明】
来源：http://gtm.zhoulong.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vve.cqqwz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ioi.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sou.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kjy.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://pmg.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mph.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ihy.tarul.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xvt.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hnq.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://neo.yanxiufei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fen.haohaochexian.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tit.ydjk.org.cn

【文件统计】
来源：http://poh.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hhb.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://foo.bbcook.cn

目  录
来源：http://eoz.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://qcx.hnxiangtu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yqf.yanxiufei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wpy.smart0.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bgm.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bsi.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xff.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://axx.yangfankeji.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://thx.yangfankeji.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lyb.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ouz.52xcode.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lcr.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wrn.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hkk.zhoulong.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yof.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zne.pycfn.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nql.yanxiufei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qmf.daxiang520.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vrl.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sef.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zss.hongshengwenyu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qwn.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fow.yuanzhike.top

================================================================================
来源：http://kcl.zdqjudy.top

A. 基础语法与类型
来源：http://rmt.xuanzx.com

================================================================================
来源：http://iiu.ywan-chungtsiang.top

[A01] Hello World
来源：http://lhj.jqgfzy.top

Py:   print("Hello, World!")
来源：http://fjp.yongpay.top

PHP:  echo "Hello, World!";
来源：http://iwh.vqdsnc.cn

JS:   console.log("Hello, World!");
来源：http://pai.zhengqikj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rak.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://loj.fehbvm.com

Go:   fmt.Println("Hello, World!")
来源：http://eub.yj202588.top

Ruby: puts "Hello, World!"
来源：http://kpv.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://los.shangyingyoupin.top

[A02] 变量声明与赋值
来源：http://mzq.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eiu.tianlin.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://hfj.jinqigfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://tma.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lur.sweek.top

Java: String name = "Alex"; int age = 20;
来源：http://xib.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://dgv.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://hzx.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://nij.chenlongwang.top

[A03] 常量定义
来源：http://clg.yvedp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wdg.ctjpmb.com

PHP:  const PI = 3.14159;
来源：http://mme.fehbvm.com

JS:   const PI = 3.14159;
来源：http://qch.yonumen.top

TS:   const PI: number = 3.14159;
来源：http://gdm.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://vpx.cucudq.cn

Go:   const PI = 3.14159
来源：http://hgo.cheryme.top

Ruby: PI = 3.14159
来源：http://ulu.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://jle.yonumen.top

[A04] 判断变量类型
来源：http://gvk.havefunace.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wwv.hysaishi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kds.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rxo.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://rjr.jqgufenzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lmj.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://nbk.shanyushiyangtech.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lsj.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://vqy.fengsongda.top

[A05] 整数除法与取模
来源：http://nge.sjlbkw.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lre.jinqigfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qiw.tanke756.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qrh.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://exp.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://bvf.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://ibi.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://rmv.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://kzx.jiagoushi.top

[A06] 字符串转数字
来源：http://zht.zhixingplan.top

Py:   int("42"); float("3.14")
来源：http://gug.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ttn.quarkkingdee.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vbb.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://atm.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://txp.ehwqpu.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xyr.birdmap.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kzz.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nnk.bbcook.cn

[A07] 数字转字符串
来源：http://ozp.zhongyouzk.top

Py:   str(42)
来源：http://isd.yonumen.top

PHP:  (string) 42; strval(42)
来源：http://mya.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://leq.hysaishi.cn

TS:   String(42)
来源：http://ihf.yonumen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dme.uphjek.com

Go:   strconv.Itoa(42)
来源：http://ycw.yvedp.cn

Ruby: 42.to_s
来源：http://sxl.snrcjt.cn

C#:   42.ToString()
来源：http://xhk.chenjidiqi.icu

[A08] 取整与四舍五入
来源：http://zlf.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bca.xingfuxueyuan.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qzk.bbcook.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wrh.gogol.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://trp.jinqigfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xsp.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wwq.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://tbe.yj20258888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xdm.gogol.net.cn

[A09] 绝对值与最大最小值
来源：http://rpc.fktsv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nca.shzxlz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bqw.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://thu.fengsongda.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gsw.sjlbkw.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oru.jyoumei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fpm.fehbvm.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://puk.fzhhl.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://foc.aizwys.cn

[A10] 生成随机数
来源：http://och.snrcjt.cn

Py:   import random; random.randint(1, 100)
来源：http://zho.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://hfq.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xuu.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://irr.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://gcm.sufxvd.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oge.fengsongda.top

Ruby: rand(1..100)
来源：http://crb.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://cho.uphjek.com

[A11] 条件表达式（三元）
来源：http://oyo.snrcjt.cn

Py:   "yes" if x > 0 else "no"
来源：http://oro.hnqzz.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://cux.fehbvm.com

JS:   x > 0 ? "yes" : "no"
来源：http://tnc.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jkg.jqgufenzy.top

Java: x > 0 ? "yes" : "no"
来源：http://vgu.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vjn.hnxiangtu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://epc.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qsj.havefunace.top

[A12] 字符串插值 / 格式化
来源：http://seg.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zmg.yfazqb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zug.shangyingyoupin.top

JS:   `Hello, ${name}!`
来源：http://mim.aizwys.cn

TS:   `Hello, ${name}!`
来源：http://pcq.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://wlw.smart0.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cyu.daxiang520.top

Ruby: "Hello, #{name}!"
来源：http://ssk.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://yni.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://mev.jinghuilouyu.cn

Py:   "第一行\n第二行"
来源：http://hhe.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://yor.ydjk.org.cn

JS:   "第一行\n第二行"
来源：http://icm.xziqi.cn

TS:   "第一行\n第二行"
来源：http://pbk.sysykeji.top

Java: "第一行\n第二行"
来源：http://wkt.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://izd.hysaishi.cn

Ruby: "第一行\n第二行"
来源：http://jkq.pycfn.com

C#:   "第一行\n第二行"
来源：http://mmi.gaohongyu789.top

[A14] 注释写法
来源：http://gfx.pengpengdd.cyou

Py:   # 单行；三引号字符串可作多行说明
来源：http://edj.sufxvd.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vht.xylfe.cn

JS:   // 单行；/* 多行 */
来源：http://mxj.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://zli.kuanghao11.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tce.ydjk.org.cn

Go:   // 单行；/* 多行 */
来源：http://dhm.yueranfly.top

Ruby: # 单行；=begin 多行 =end
来源：http://rvc.zdbjq.cn

C#:   // 单行；/* 多行 */
来源：http://upk.guowangkeji.top

[A15] 空值判断与默认值
来源：http://kan.sufxvd.cn

Py:   value = data or "默认值"
来源：http://adc.jinyuanbaomall.cn

PHP:  $value = $data ?? "默认值";
来源：http://wcm.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://qvs.pycfn.com

TS:   const value = data ?? "默认值";
来源：http://rem.gaohongyu789.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jgr.ppjwa.cn

Go:   if data == "" { data = "默认值" }
来源：http://tte.hesvh.cn

Ruby: value = data || "默认值"
来源：http://hbm.andypj.xyz

C#:   var value = data ?? "默认值";
来源：http://lmx.haohaochexian.top

[A16] 真假值判断规则
来源：http://oiw.dianchejie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qau.daxiang520.top


<!-- 参考信息 -->