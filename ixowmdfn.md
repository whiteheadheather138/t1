代发 wailian999

[U89] JS：数组去重
来源：http://ves.yanxiufei.cn

[...new Set(arr)]
来源：http://wey.ydzc1.top

[U90] JS：数字数组排序
来源：http://ojf.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://btm.daria6918.cn

[U91] JS：对象键值遍历
来源：http://ncd.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bwb.yj202588.top

[U92] JS：深拷贝
来源：http://bpq.yuxming.cn

structuredClone(obj)
来源：http://dxv.andypj.xyz

[U93] JS：模板字符串
来源：http://qbz.jianghu66.top

`共 ${n} 条`
来源：http://rjh.ctjpmb.com

[U94] JS：箭头函数
来源：http://eno.kuanghao11.cn

const double = x => x * 2;
来源：http://kzr.yuxming.cn

[U95] JS：Promise 包装
来源：http://pbo.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://rao.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://tnu.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ulf.hesvh.cn

[U97] JS：并发请求
来源：http://nus.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ukh.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://kwe.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vit.dianchejie.cn

[U99] JS：事件监听
来源：http://boy.yonumen.top

el.addEventListener("click", e => {})
来源：http://swl.tian-w.cn

[U100] JS：DOM 查询
来源：http://llv.fktsv.cn

document.querySelector(".item")
来源：http://izk.xylfe.cn

[U101] JS：classList 操作
来源：http://vsh.ppjwa.cn

el.classList.toggle("active")
来源：http://qni.bbcook.cn

[U102] JS：本地存储
来源：http://pvm.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jsb.tanke756.top

[U103] JS：定时器
来源：http://qmk.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yjx.chenlongwang.top

[U104] JS：防抖
来源：http://hdg.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fzu.shanyushiyangkeji.top

[U105] JS：节流
来源：http://wle.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ekk.hfpthk.cn

[U106] JS：日期格式化
来源：http://rml.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rfm.wangdashe.top

[U107] JS：数字千分位
来源：http://soa.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cvc.ydzc1.top

[U108] JS：随机整数
来源：http://hct.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vck.tanke756.top

[U109] JS：数组分组
来源：http://lsl.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://ydt.jlsjyb.cn

[U110] JS：数组分块
来源：http://gmp.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://noe.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://etn.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://tvy.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://yju.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://vkg.yuanzhike.top

[U113] JS：正则替换全部
来源：http://ccf.yueranfly.top

s.replaceAll("a", "b")
来源：http://cfa.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://diz.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jhh.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://dfx.epnwcf.com

crypto.randomUUID()
来源：http://ufl.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://zps.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://ksh.quarkkingdee.top

[U117] JS：单元测试
来源：http://ylz.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://rqe.daxiang520.top

[U118] JS：开发服务器
来源：http://qcv.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://zfa.hesvh.cn

[U119] JS：生产构建
来源：http://wrz.redwolf501.top

npx vite build
来源：http://sgu.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://ciy.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://wdy.tianlin.xyz

================================================================================
来源：http://bvk.shanyushiyangkeji.top

统计汇总
来源：http://rwh.9152youxi.cn

================================================================================
来源：http://ydl.zhijiandao.cn

按语言统计（条）：
来源：http://hyv.aibaodan.cn

Python ......... 252
来源：http://zey.xuetiantiany.cn

PHP ............ 252
来源：http://mtj.hnxiangtu.top

JavaScript ..... 252
来源：http://zqp.epnwcf.com

TypeScript ..... 212
来源：http://ifi.ydzc1.top

Java ........... 212
来源：http://doz.shuidangran.top

Go ............. 212
来源：http://bsq.iojbl.cn

Ruby ........... 212
来源：http://cyf.guowangkeji.top

C# ............. 212
来源：http://qye.meibo888.top

C .............. 30
来源：http://vwf.xingfuxueyuan.xyz

C++ ............ 30
来源：http://els.shuidangran.top

SQL ............ 90
来源：http://ywd.zhoulong.xyz

Bash ........... 80
来源：http://ztm.gotoacloud.top

Kotlin ......... 15
来源：http://dmk.yj20258.top

Swift .......... 15
来源：http://jii.yonumen.top

Lua ............ 10
来源：http://imp.0kj1m.cn

Perl ........... 10
来源：http://cei.yvedp.cn

Scala .......... 10
来源：http://ati.bjfxy.top

------------------------------------
来源：http://hlu.jlsjyb.cn

合计 ........... 2106 条
来源：http://hzn.bjfxy.top

按章节统计：
来源：http://dxe.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zzp.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sej.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://phf.yueranfly.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ytb.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mpy.jinyuanbaomall.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cyq.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://for.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://srl.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kvw.cheryme.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ewr.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ied.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kif.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rov.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yak.hnqzz.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zgk.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lzs.jianghu66.top

Q SQL 专题                              90
来源：http://fhk.yj20258888.top

R Bash 专题                             80
来源：http://hsg.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://uzw.ivvv.top

T 其他语言补充                          60
来源：http://avv.ppjwa.cn

U 高频实用片段                         120
来源：http://tcm.jqgufenzy.top

------------------------------------
来源：http://qee.jinyuanbaomall.cn

合计                                  2106 条
来源：http://kvc.hammf.cn

--------------------------------------------------------------------------------
来源：http://upv.hysaishi.cn

使用提醒
来源：http://jfi.aizwys.cn

--------------------------------------------------------------------------------
来源：http://twu.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uak.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ndt.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vdz.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gcf.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jyu.nanxinkj.top

—— 文件结束 ——
来源：http://vvm.sjlbkw.cn

================================================================================
来源：http://soy.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://szc.yj202588.top

Common Programming Examples Cheat Book
来源：http://ubx.jinqigufen.top

================================================================================
来源：http://iht.yj202588.top

【收录内容】
来源：http://yib.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lsy.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qoo.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://kji.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wrc.hcnkem.com

【使用说明】
来源：http://odx.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zxq.xziqi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rqk.hfpthk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dnb.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zgp.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://vjw.zycfv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://edm.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mbh.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nri.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ltc.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qnp.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gsz.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zrc.zhaomingkeji.xyz

【文件统计】
来源：http://iqj.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nwl.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://ggq.yj202588.top

目  录
来源：http://ams.yuxming.cn

--------------------------------------------------------------------------------
来源：http://hzl.jinqigfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lol.shuidangran.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hep.sufxvd.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fjo.jyoumei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sml.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://akz.iojbl.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gpf.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jnc.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tzk.yj202588.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zzu.shuidangran.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nrm.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://syh.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sly.yanxiufei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pku.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yvx.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xtn.jinghuilouyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wor.zhoulong.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iqa.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zrc.wangshuangyany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lfw.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tog.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wig.vehdjk.com

================================================================================
来源：http://jun.shzxlz.cn

A. 基础语法与类型
来源：http://pqe.ivvv.top

================================================================================
来源：http://jqc.meibo888.top

[A01] Hello World
来源：http://ksh.yangfankeji.com

Py:   print("Hello, World!")
来源：http://vcc.yfazqb.com

PHP:  echo "Hello, World!";
来源：http://xqy.nanxinkj.top

JS:   console.log("Hello, World!");
来源：http://hke.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pgd.fehbvm.com

Java: System.out.println("Hello, World!");
来源：http://oub.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://ufm.yongpay.top

Ruby: puts "Hello, World!"
来源：http://tcf.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pee.jyoumei.cn

[A02] 变量声明与赋值
来源：http://tdx.yuxming.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gzg.sufxvd.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://erw.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://cdn.ydzc1.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wzk.guowangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://guj.guannengcc.top

Go:   name := "Alex"; age := 20
来源：http://qzz.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://lsc.pengpengdd.cyou

C#:   string name = "Alex"; int age = 20;
来源：http://yud.hfpthk.cn

[A03] 常量定义
来源：http://ahb.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ibe.ydjk.org.cn

PHP:  const PI = 3.14159;
来源：http://rnn.jqgufenzy.top

JS:   const PI = 3.14159;
来源：http://fvc.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://iyq.zhongyouzk.top

Java: static final double PI = 3.14159;
来源：http://oxa.52xcode.cn

Go:   const PI = 3.14159
来源：http://swq.bbcook.cn

Ruby: PI = 3.14159
来源：http://zgs.yj20258.top

C#:   const double PI = 3.14159;
来源：http://izy.hcnkem.com

[A04] 判断变量类型
来源：http://gof.quarkkingdee.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ajg.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yhq.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hia.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://vwi.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sxg.jqgfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://mww.yangfankeji.com

Ruby: x.class; x.is_a?(Integer)
来源：http://cnk.zdbjq.cn

C#:   x.GetType().Name; x is int
来源：http://yjy.tianlin.xyz

[A05] 整数除法与取模
来源：http://mow.kuanghao11.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xdy.hnxiangtu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vto.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bks.chenzaomai.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qtv.shuidangran.top

Java: 7 / 2; 7 % 2
来源：http://vsy.zhongyouzk.top

Go:   7 / 2; 7 % 2
来源：http://yrg.pycfn.com

Ruby: 7 / 2; 7 % 2
来源：http://xln.hesvh.cn

C#:   7 / 2; 7 % 2
来源：http://qxh.jinghuilouyu.cn

[A06] 字符串转数字
来源：http://xhd.zhengqikj.top

Py:   int("42"); float("3.14")
来源：http://afr.xziqi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cjl.zdqjudy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://efm.feifeiyinyue.top

TS:   parseInt("42", 10); Number("42")
来源：http://tvs.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://slh.yvedp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://art.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://lce.redwolf501.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://upc.ppjwa.cn

[A07] 数字转字符串
来源：http://rnh.yvedp.cn

Py:   str(42)
来源：http://iyw.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://irp.xinyue.icu

JS:   String(42); (42).toString()
来源：http://odv.dianchejie.cn

TS:   String(42)
来源：http://lvs.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dqc.chenjidiqi.icu

Go:   strconv.Itoa(42)
来源：http://jdq.gzhubu.top

Ruby: 42.to_s
来源：http://isx.uphjek.com

C#:   42.ToString()
来源：http://ghr.shuidangran.top

[A08] 取整与四舍五入
来源：http://tei.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://svn.tarul.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xbc.hammf.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fln.vehdjk.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vom.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jes.yj20258888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://owq.sxryk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ibj.jlsjyb.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hqz.gaohongyu789.top

[A09] 绝对值与最大最小值
来源：http://pxe.yongpay.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uyo.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ddl.shanyushiyangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gwj.c1oappe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uka.hnqzz.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rhu.ybcxt.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yqu.shanyushiyangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mhs.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://thz.yfazqb.com

[A10] 生成随机数
来源：http://dok.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://uwx.316326.xyz

PHP:  random_int(1, 100);
来源：http://add.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xxf.yuxming.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wkd.hfpthk.cn

Java: new Random().nextInt(100) + 1
来源：http://cwx.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bzu.yongpay.top

Ruby: rand(1..100)
来源：http://pjj.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://ujc.316326.xyz

[A11] 条件表达式（三元）
来源：http://heo.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://cpo.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nre.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ays.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://yhd.gogol.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://oae.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://oub.zdbjq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aju.aibaodan.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hym.xuanzx.com

[A12] 字符串插值 / 格式化
来源：http://yto.tian-w.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qyg.yanxiufei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oji.gotoacloud.top

JS:   `Hello, ${name}!`
来源：http://thw.nanxinkj.top

TS:   `Hello, ${name}!`
来源：http://zhf.guannengcc.top

Java: "Hello, %s!".formatted(name)
来源：http://hqi.uphjek.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://feu.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://izd.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://gyt.zhixingplan.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qjh.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://snp.shangyingyoupin.top

PHP:  "第一行\n第二行"
来源：http://ksa.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://fno.uphjek.com

TS:   "第一行\n第二行"
来源：http://iyw.shangyingyoupin.top

Java: "第一行\n第二行"
来源：http://ftc.iojbl.cn

Go:   "第一行\n第二行"
来源：http://bzw.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://fbg.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://rwq.hcnkem.com

[A14] 注释写法
来源：http://obw.zdqjudy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://syw.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://phw.yuxming.cn

JS:   // 单行；/* 多行 */
来源：http://poe.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://tlt.wangshuangyany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vzb.jyoumei.cn

Go:   // 单行；/* 多行 */
来源：http://bis.sjlbkw.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zww.0kj1m.cn

C#:   // 单行；/* 多行 */
来源：http://ipz.ydzc1.top

[A15] 空值判断与默认值
来源：http://cry.yongpay.top

Py:   value = data or "默认值"
来源：http://dhq.yanxiufei.cn

PHP:  $value = $data ?? "默认值";
来源：http://oat.zhengqikj.top


<!-- 参考信息 -->