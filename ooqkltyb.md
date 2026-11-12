代发 wailian999

[U89] JS：数组去重
来源：http://hau.316326.xyz

[...new Set(arr)]
来源：http://xrw.hammf.cn

[U90] JS：数字数组排序
来源：http://csy.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://ufm.bbcook.cn

[U91] JS：对象键值遍历
来源：http://qtw.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dhx.snrcjt.cn

[U92] JS：深拷贝
来源：http://whl.iojbl.cn

structuredClone(obj)
来源：http://fsb.zhongyouzk.top

[U93] JS：模板字符串
来源：http://bcy.hammf.cn

`共 ${n} 条`
来源：http://bce.aibaodan.cn

[U94] JS：箭头函数
来源：http://zmx.zhixingplan.top

const double = x => x * 2;
来源：http://ned.hcnkem.com

[U95] JS：Promise 包装
来源：http://wck.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://zzv.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://bnh.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://etd.vehdjk.com

[U97] JS：并发请求
来源：http://hmc.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cym.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://rtj.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sov.shangyingyoupin.top

[U99] JS：事件监听
来源：http://wce.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://ioz.tanke756.top

[U100] JS：DOM 查询
来源：http://odf.jinghuilouyu.cn

document.querySelector(".item")
来源：http://fra.gzhubu.top

[U101] JS：classList 操作
来源：http://hsu.zdbjq.cn

el.classList.toggle("active")
来源：http://ddu.mhx1999.top

[U102] JS：本地存储
来源：http://itl.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://upo.kuanghao11.cn

[U103] JS：定时器
来源：http://poh.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mdk.hnxiangtu.top

[U104] JS：防抖
来源：http://lqc.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wmw.shangyingyoupin.top

[U105] JS：节流
来源：http://naa.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nyz.fehbvm.com

[U106] JS：日期格式化
来源：http://tcf.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oik.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://rpr.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lsr.jlsjyb.cn

[U108] JS：随机整数
来源：http://cbh.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nhz.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://are.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://wdb.wangshuangyany.cn

[U110] JS：数组分块
来源：http://zhq.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hkw.wangdashe.top

[U111] JS：对象转 Map
来源：http://sbs.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://crj.nwbrower.top

[U112] JS：字符串补位
来源：http://uye.jianghu66.top

"7".padStart(3, "0")
来源：http://wck.zycfv.cn

[U113] JS：正则替换全部
来源：http://onu.xziqi.cn

s.replaceAll("a", "b")
来源：http://aud.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://mcy.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sob.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://cth.zhoulong.xyz

crypto.randomUUID()
来源：http://lxv.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://ywc.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://mpb.52xcode.cn

[U117] JS：单元测试
来源：http://vnu.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://eco.yj20258888.top

[U118] JS：开发服务器
来源：http://diu.xuetiantiany.cn

npm i -D vite;  npx vite
来源：http://uqy.sufxvd.cn

[U119] JS：生产构建
来源：http://gsy.kuanghao11.cn

npx vite build
来源：http://wgg.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://wnp.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://bdx.chenjidiqi.icu

================================================================================
来源：http://xog.yanxiufei.cn

统计汇总
来源：http://dcx.yuxming.cn

================================================================================
来源：http://dfv.hammf.cn

按语言统计（条）：
来源：http://ofa.tianlin.xyz

Python ......... 252
来源：http://mpm.feifeiyinyue.top

PHP ............ 252
来源：http://suh.chenlongwang.top

JavaScript ..... 252
来源：http://mll.hammf.cn

TypeScript ..... 212
来源：http://odt.hnxiangtu.top

Java ........... 212
来源：http://qiu.zhijiandao.cn

Go ............. 212
来源：http://cgz.havefunace.top

Ruby ........... 212
来源：http://odd.fehbvm.com

C# ............. 212
来源：http://vyn.redwolf501.top

C .............. 30
来源：http://uee.jinqigfzy.top

C++ ............ 30
来源：http://hdt.snrcjt.cn

SQL ............ 90
来源：http://orp.haohaochexian.top

Bash ........... 80
来源：http://blv.hnxiangtu.top

Kotlin ......... 15
来源：http://gvq.yueranfly.top

Swift .......... 15
来源：http://cyy.yanxiufei.cn

Lua ............ 10
来源：http://bnb.chenlongwang.top

Perl ........... 10
来源：http://izu.gogol.net.cn

Scala .......... 10
来源：http://rgi.ywan-chungtsiang.top

------------------------------------
来源：http://zgb.guannengcc.top

合计 ........... 2106 条
来源：http://ocx.hongshengwenyu.top

按章节统计：
来源：http://exl.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rks.sufxvd.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ytq.hcnkem.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://big.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wnm.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rui.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gft.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lcw.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jfk.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pol.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ufi.52xcode.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cqd.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nuh.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xim.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xlk.redwolf501.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rul.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ebv.ydjk.org.cn

Q SQL 专题                              90
来源：http://nnt.vehdjk.com

R Bash 专题                             80
来源：http://wyi.uphjek.com

S C / C++ 专题                          60
来源：http://pen.fanxiaobao.xyz

T 其他语言补充                          60
来源：http://ixo.xuetiantiany.cn

U 高频实用片段                         120
来源：http://fih.birdmap.top

------------------------------------
来源：http://hsn.chenjidiqi.icu

合计                                  2106 条
来源：http://klz.tarul.cn

--------------------------------------------------------------------------------
来源：http://szi.gzhubu.top

使用提醒
来源：http://gii.havefunace.top

--------------------------------------------------------------------------------
来源：http://rus.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iaf.fengsongda.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ykk.zycfv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vyz.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://ibp.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zgr.sxryk.cn

—— 文件结束 ——
来源：http://fng.chenjidiqi.icu

================================================================================
来源：http://fkj.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://yop.cqqwz.cn

Common Programming Examples Cheat Book
来源：http://xdi.hywenlv.cn

================================================================================
来源：http://bfc.chenlongwang.top

【收录内容】
来源：http://xjc.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://byy.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://czs.gzhubu.top

SQL · Bash · C · C++
来源：http://rjq.guowangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dih.gogol.net.cn

【使用说明】
来源：http://ayw.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zkx.jinyuanbaomall.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jht.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://isx.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vds.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pyo.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zbs.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fvt.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://igf.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tdf.meibo888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qla.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iub.shanyushiyangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tvm.c1oappe.top

【文件统计】
来源：http://fso.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tbe.bjfxy.top

--------------------------------------------------------------------------------
来源：http://shc.birdmap.top

目  录
来源：http://cjt.redwolf501.top

--------------------------------------------------------------------------------
来源：http://qyw.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hgr.wangshuangyany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zfe.jqgfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://neh.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zta.fehbvm.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uok.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iau.yangfankeji.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yzj.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aun.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bfy.sjlbkw.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mpe.hywenlv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ozp.hesvh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lvw.sxryk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fzw.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zzr.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ocg.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qte.xinyue.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bon.svipenyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://csg.ybcxt.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wsz.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xap.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gyc.fzhhl.top

================================================================================
来源：http://iwd.jqgfzy.top

A. 基础语法与类型
来源：http://wqp.yj202588.top

================================================================================
来源：http://nlu.birdmap.top

[A01] Hello World
来源：http://dki.jinqigfzy.top

Py:   print("Hello, World!")
来源：http://bsy.nanxinkj.top

PHP:  echo "Hello, World!";
来源：http://wcs.fanxiaobao.xyz

JS:   console.log("Hello, World!");
来源：http://knl.gzhubu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ejx.nwbrower.top

Java: System.out.println("Hello, World!");
来源：http://beg.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://zmo.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://zue.snrcjt.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ika.cheryme.top

[A02] 变量声明与赋值
来源：http://lsg.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://exj.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qzh.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://twa.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://elv.kuanghao11.cn

Java: String name = "Alex"; int age = 20;
来源：http://vfk.tanke756.top

Go:   name := "Alex"; age := 20
来源：http://rzs.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://mkj.zhoulong.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://jib.shzxlz.cn

[A03] 常量定义
来源：http://xcc.316326.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kea.wangdashe.top

PHP:  const PI = 3.14159;
来源：http://puq.fktsv.cn

JS:   const PI = 3.14159;
来源：http://ngt.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://cez.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://ofa.shangyingyoupin.top

Go:   const PI = 3.14159
来源：http://fnr.shangyingyoupin.top

Ruby: PI = 3.14159
来源：http://gjs.52xcode.cn

C#:   const double PI = 3.14159;
来源：http://vyq.kuanghao11.cn

[A04] 判断变量类型
来源：http://kdq.ydzc1.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gon.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pda.andypj.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://krd.yj20258.top

TS:   typeof x; x instanceof Date
来源：http://oou.haohaochexian.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qzm.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://jrm.0kj1m.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qdd.sysykeji.top

C#:   x.GetType().Name; x is int
来源：http://jri.fanxiaobao.xyz

[A05] 整数除法与取模
来源：http://wsv.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ncs.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qjq.jqgfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bca.zdbjq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jbz.jianghu66.top

Java: 7 / 2; 7 % 2
来源：http://osy.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://ykq.fengsongda.top

Ruby: 7 / 2; 7 % 2
来源：http://ons.c1oappe.top

C#:   7 / 2; 7 % 2
来源：http://dtm.shanyushiyangkeji.top

[A06] 字符串转数字
来源：http://xsr.zhoulong.xyz

Py:   int("42"); float("3.14")
来源：http://dpv.yuanzhike.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eho.yfazqb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gkg.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://jpd.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gob.hfpthk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://phe.vqdsnc.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rmm.xinyue.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vaz.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://jmu.0kj1m.cn

Py:   str(42)
来源：http://kll.sweek.top

PHP:  (string) 42; strval(42)
来源：http://drm.cheryme.top

JS:   String(42); (42).toString()
来源：http://mjw.yangfankeji.com

TS:   String(42)
来源：http://xot.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ehy.kuanghao11.cn

Go:   strconv.Itoa(42)
来源：http://aec.zhengqikj.top

Ruby: 42.to_s
来源：http://bwn.sjlbkw.cn

C#:   42.ToString()
来源：http://qzk.birdmap.top

[A08] 取整与四舍五入
来源：http://uve.xinyue.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pht.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fzp.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vrd.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://igf.daria6918.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nlv.zhaomingkeji.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://awd.cashguo.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bzb.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sze.jinyuanbaomall.cn

[A09] 绝对值与最大最小值
来源：http://ulu.zhijiandao.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fwm.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ooo.ywan-chungtsiang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://txw.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pal.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eew.xingfuxueyuan.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zak.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lth.zhoulong.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wni.9152youxi.cn

[A10] 生成随机数
来源：http://rew.ppjwa.cn

Py:   import random; random.randint(1, 100)
来源：http://qfb.ydjk.org.cn

PHP:  random_int(1, 100);
来源：http://grc.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zqv.hammf.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://glc.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://jvb.shanyushiyangtech.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qif.dianchejie.cn

Ruby: rand(1..100)
来源：http://bpn.0kj1m.cn

C#:   new Random().Next(1, 101)
来源：http://etl.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://mva.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://dou.xylfe.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://iqb.pengpengdd.cyou

JS:   x > 0 ? "yes" : "no"
来源：http://wyv.birdmap.top

TS:   x > 0 ? "yes" : "no"
来源：http://ngp.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://joi.yangfankeji.com

Go:   // 无三元运算符，需用 if 语句
来源：http://cno.shangyingyoupin.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cun.yanxiufei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dig.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://xgc.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ojk.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oun.tanke756.top

JS:   `Hello, ${name}!`
来源：http://cbm.tian-w.cn

TS:   `Hello, ${name}!`
来源：http://lap.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://jox.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gic.fehbvm.com

Ruby: "Hello, #{name}!"
来源：http://brq.mhx1999.top

C#:   $"Hello, {name}!"
来源：http://iqr.ehwqpu.com

[A13] 多行字符串（练习 \n 转义）
来源：http://uko.c1oappe.top

Py:   "第一行\n第二行"
来源：http://lvo.sjlbkw.cn

PHP:  "第一行\n第二行"
来源：http://bbp.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://xpf.fzhhl.top

TS:   "第一行\n第二行"
来源：http://xmo.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://bbg.epnwcf.com

Go:   "第一行\n第二行"
来源：http://vgb.yuxming.cn

Ruby: "第一行\n第二行"
来源：http://ibo.cashguo.top

C#:   "第一行\n第二行"
来源：http://gup.xuetiantiany.cn

[A14] 注释写法
来源：http://xkg.bjfxy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://omm.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://jqc.nanxinkj.top

JS:   // 单行；/* 多行 */
来源：http://znz.aibaodan.cn

TS:   // 单行；/* 多行 */
来源：http://tyz.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pxu.sweek.top

Go:   // 单行；/* 多行 */
来源：http://ksn.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://hyv.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://pwx.bbcook.cn

[A15] 空值判断与默认值
来源：http://tsq.hammf.cn

Py:   value = data or "默认值"
来源：http://jfj.hongshengwenyu.top

PHP:  $value = $data ?? "默认值";
来源：http://tug.dashuyun.cn


<!-- 参考信息 -->