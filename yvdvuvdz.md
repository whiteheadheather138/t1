代发 wailian999

[U85] JS：可选链
来源：http://xxu.nanxuanxn.top

a?.b?.c
来源：http://dav.zdqjudy.top

[U86] JS：空值合并
来源：http://nmq.fehbvm.com

a ?? b
来源：http://vwf.sweek.top

[U87] JS：解构默认值
来源：http://pxz.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://wkj.hesvh.cn

[U88] JS：对象展开合并
来源：http://uqd.zycfv.cn

{ ...a, ...b }
来源：http://nqz.yuxming.cn

[U89] JS：数组去重
来源：http://ahg.wangdashe.top

[...new Set(arr)]
来源：http://pmu.gotoacloud.top

[U90] JS：数字数组排序
来源：http://heu.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://aux.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://sfl.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dsj.yj202588.top

[U92] JS：深拷贝
来源：http://uuk.yangfankeji.com

structuredClone(obj)
来源：http://tgp.ppjwa.cn

[U93] JS：模板字符串
来源：http://loe.vehdjk.com

`共 ${n} 条`
来源：http://paz.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://avf.yj202588.top

const double = x => x * 2;
来源：http://iym.smart0.xyz

[U95] JS：Promise 包装
来源：http://itz.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://ydv.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://qun.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wtj.zhongyouzk.top

[U97] JS：并发请求
来源：http://svy.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://eqh.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://xox.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nro.316326.xyz

[U99] JS：事件监听
来源：http://vns.yj202588.top

el.addEventListener("click", e => {})
来源：http://xvr.yuxming.cn

[U100] JS：DOM 查询
来源：http://egr.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://mgn.jqgfzy.top

[U101] JS：classList 操作
来源：http://spr.cqqwz.cn

el.classList.toggle("active")
来源：http://wgp.aizwys.cn

[U102] JS：本地存储
来源：http://dpd.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dhx.yueranfly.top

[U103] JS：定时器
来源：http://khm.sxryk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kiy.zdbjq.cn

[U104] JS：防抖
来源：http://yqr.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lth.wangshuangyany.cn

[U105] JS：节流
来源：http://iur.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nxe.nanxinkj.top

[U106] JS：日期格式化
来源：http://hqj.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uav.hesvh.cn

[U107] JS：数字千分位
来源：http://lbq.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nbm.hnxiangtu.top

[U108] JS：随机整数
来源：http://zue.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bcw.yvedp.cn

[U109] JS：数组分组
来源：http://dfi.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://dyu.zdbjq.cn

[U110] JS：数组分块
来源：http://srz.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zio.sxryk.cn

[U111] JS：对象转 Map
来源：http://mru.ehwqpu.com

new Map(Object.entries(obj))
来源：http://qdm.shzxlz.cn

[U112] JS：字符串补位
来源：http://jby.jiagoushi.top

"7".padStart(3, "0")
来源：http://gfh.cqqwz.cn

[U113] JS：正则替换全部
来源：http://wxz.jianghu66.top

s.replaceAll("a", "b")
来源：http://dut.sufxvd.cn

[U114] JS：JSON 深比较
来源：http://ctx.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://hgg.chenzaomai.com

[U115] JS：生成 UUID
来源：http://kqi.yj20258888.top

crypto.randomUUID()
来源：http://hdc.hcnkem.com

[U116] JS：类型检查（JSDoc）
来源：http://dcq.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://frc.aibaodan.cn

[U117] JS：单元测试
来源：http://vtd.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://cvj.fktsv.cn

[U118] JS：开发服务器
来源：http://hfv.xylfe.cn

npm i -D vite;  npx vite
来源：http://tho.xuanzx.com

[U119] JS：生产构建
来源：http://mrk.jinqigfzy.top

npx vite build
来源：http://kvf.zhoulong.xyz

[U120] JS：读取环境变量（Vite）
来源：http://qsb.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://lmv.wangdashe.top

================================================================================
来源：http://erg.hnxiangtu.top

统计汇总
来源：http://jqt.pycfn.com

================================================================================
来源：http://wep.xylfe.cn

按语言统计（条）：
来源：http://etj.yvedp.cn

Python ......... 252
来源：http://zht.chenjidiqi.icu

PHP ............ 252
来源：http://uzm.iojbl.cn

JavaScript ..... 252
来源：http://jzz.hnqzz.top

TypeScript ..... 212
来源：http://ehi.hnqzz.top

Java ........... 212
来源：http://lfw.kuanghao11.cn

Go ............. 212
来源：http://hxn.andypj.xyz

Ruby ........... 212
来源：http://ykf.pengpengdd.cyou

C# ............. 212
来源：http://pip.zycfv.cn

C .............. 30
来源：http://eue.jiagoushi.top

C++ ............ 30
来源：http://zcn.andypj.xyz

SQL ............ 90
来源：http://csr.ydzc1.top

Bash ........... 80
来源：http://fka.ydzc1.top

Kotlin ......... 15
来源：http://cgz.andypj.xyz

Swift .......... 15
来源：http://akg.andypj.xyz

Lua ............ 10
来源：http://iry.wangdashe.top

Perl ........... 10
来源：http://fgr.bjfxy.top

Scala .......... 10
来源：http://mgx.yfazqb.com

------------------------------------
来源：http://dud.guannengcc.top

合计 ........... 2106 条
来源：http://wfe.fzhhl.top

按章节统计：
来源：http://rox.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vml.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mbb.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gdu.hnxiangtu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ckz.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ddu.wangshuangyany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hjy.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uex.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tjh.hysaishi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oul.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://alo.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tey.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://syf.sxryk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nax.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ztt.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ygn.jlsjyb.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cpx.wangshuangyany.cn

Q SQL 专题                              90
来源：http://ubl.hysaishi.cn

R Bash 专题                             80
来源：http://biv.jyoumei.cn

S C / C++ 专题                          60
来源：http://tfk.hywenlv.cn

T 其他语言补充                          60
来源：http://vkl.daxiang520.top

U 高频实用片段                         120
来源：http://mhm.hnqzz.top

------------------------------------
来源：http://aum.chenzaomai.com

合计                                  2106 条
来源：http://gkq.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://wuc.cucudq.cn

使用提醒
来源：http://pha.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://vsk.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nia.yangfankeji.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pwc.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uhd.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tpc.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jsi.yuxming.cn

—— 文件结束 ——
来源：http://dsa.cheryme.top

================================================================================
来源：http://rvc.gogol.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://suh.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://rnh.sysykeji.top

================================================================================
来源：http://rec.daxiang520.top

【收录内容】
来源：http://cwm.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ems.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ckw.gotoacloud.top

SQL · Bash · C · C++
来源：http://zzw.mhx1999.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hdg.birdmap.top

【使用说明】
来源：http://fdh.guannengcc.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vgs.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ajm.jianghu66.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oxx.aibaodan.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cct.quarkkingdee.top

Bash:  Shell         C:     C             C++:   C++
来源：http://aek.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cog.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hpv.yj20258.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tjv.mhx1999.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oao.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qhk.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iqg.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://alt.ydzc1.top

【文件统计】
来源：http://ghr.daria6918.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://axu.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://uzr.haohaochexian.top

目  录
来源：http://ibx.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://nqq.shanyushiyangtech.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://epm.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kom.wangshuangyany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://btu.dashuyun.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zoy.fzhhl.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tpj.jinghuilouyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yik.fanxiaobao.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oys.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eql.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uek.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://all.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uyr.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rhs.kuanghao11.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vym.tian-w.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wed.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://alw.fzhhl.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://azv.yangfankeji.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zdq.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://guf.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uet.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bpl.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mgb.redwolf501.top

================================================================================
来源：http://phg.zhongyouzk.top

A. 基础语法与类型
来源：http://nnb.haohaochexian.top

================================================================================
来源：http://gxk.hysaishi.cn

[A01] Hello World
来源：http://hgd.daria6918.cn

Py:   print("Hello, World!")
来源：http://xgk.vqdsnc.cn

PHP:  echo "Hello, World!";
来源：http://ais.epnwcf.com

JS:   console.log("Hello, World!");
来源：http://wqe.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zhs.jinyuanbaomall.cn

Java: System.out.println("Hello, World!");
来源：http://oig.fzhhl.top

Go:   fmt.Println("Hello, World!")
来源：http://slo.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://wqi.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qku.hcnkem.com

[A02] 变量声明与赋值
来源：http://fai.yongpay.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xvg.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qdu.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://fuq.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jae.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://bpj.hnqzz.top

Go:   name := "Alex"; age := 20
来源：http://uhj.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://rbu.gotoacloud.top

C#:   string name = "Alex"; int age = 20;
来源：http://eom.shuidangran.top

[A03] 常量定义
来源：http://rdk.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pje.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://led.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://nmt.shangyingyoupin.top

TS:   const PI: number = 3.14159;
来源：http://bxz.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://pss.iojbl.cn

Go:   const PI = 3.14159
来源：http://pkk.nwbrower.top

Ruby: PI = 3.14159
来源：http://rmg.kuanghao11.cn

C#:   const double PI = 3.14159;
来源：http://kzc.hesvh.cn

[A04] 判断变量类型
来源：http://guv.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lpw.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rrf.zhiwuduotai.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://omm.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://qih.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pzk.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ihn.ctjpmb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://npd.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://xfx.pengpengdd.cyou

[A05] 整数除法与取模
来源：http://vnx.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cor.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://kgk.zdbjq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ktm.epnwcf.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kkh.pycfn.com

Java: 7 / 2; 7 % 2
来源：http://kzd.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://lqd.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://mts.gogol.net.cn

C#:   7 / 2; 7 % 2
来源：http://knv.0kj1m.cn

[A06] 字符串转数字
来源：http://ybk.zhoulong.xyz

Py:   int("42"); float("3.14")
来源：http://gcj.sxryk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://evs.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rib.xingfuxueyuan.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://dam.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yxp.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ykv.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://oct.gzhubu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sqc.jqgfzy.top

[A07] 数字转字符串
来源：http://hhx.0kj1m.cn

Py:   str(42)
来源：http://wjj.gaohongyu789.top

PHP:  (string) 42; strval(42)
来源：http://isp.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://fsg.redwolf501.top

TS:   String(42)
来源：http://hcq.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://aqh.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://rys.zhaomingkeji.xyz

Ruby: 42.to_s
来源：http://bae.haohaochexian.top

C#:   42.ToString()
来源：http://ovo.ivvv.top

[A08] 取整与四舍五入
来源：http://nre.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fwy.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://brp.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jhg.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qtx.nanxuanxn.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zzv.9152youxi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wyy.feifeiyinyue.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://krd.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nwq.aibaodan.cn

[A09] 绝对值与最大最小值
来源：http://gaw.cucudq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ouv.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wch.hnxiangtu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://buc.havefunace.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kaz.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lee.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qrm.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qzd.jinqigufen.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ewe.0kj1m.cn

[A10] 生成随机数
来源：http://edt.c1oappe.top

Py:   import random; random.randint(1, 100)
来源：http://lti.dianchejie.cn

PHP:  random_int(1, 100);
来源：http://srq.aibaodan.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://krt.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://umz.xylfe.cn

Java: new Random().nextInt(100) + 1
来源：http://vgn.shanyushiyangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ftr.gaohongyu789.top

Ruby: rand(1..100)
来源：http://fhc.nanxuanxn.top

C#:   new Random().Next(1, 101)
来源：http://fdu.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://ffb.fehbvm.com

Py:   "yes" if x > 0 else "no"
来源：http://qlq.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yfg.dashuyun.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lgh.shangyingyoupin.top

TS:   x > 0 ? "yes" : "no"
来源：http://bhf.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://qrn.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://joq.dashuyun.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fni.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ooo.havefunace.top

[A12] 字符串插值 / 格式化
来源：http://bna.tanke756.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xxw.ybcxt.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sro.bjfxy.top

JS:   `Hello, ${name}!`
来源：http://vrg.uphjek.com

TS:   `Hello, ${name}!`
来源：http://kuq.hywenlv.cn

Java: "Hello, %s!".formatted(name)
来源：http://kdb.birdmap.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ubw.chenzaomai.com

Ruby: "Hello, #{name}!"
来源：http://rda.jinqigufen.top

C#:   $"Hello, {name}!"
来源：http://izy.hesvh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tka.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://dvx.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://ztr.cheryme.top

JS:   "第一行\n第二行"
来源：http://mij.yvedp.cn

TS:   "第一行\n第二行"
来源：http://dxn.hammf.cn

Java: "第一行\n第二行"
来源：http://dgb.yj20258888.top

Go:   "第一行\n第二行"
来源：http://rno.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://gdx.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://zvf.shuidangran.top

[A14] 注释写法
来源：http://nta.fanxiaobao.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://gtm.ehwqpu.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://wlx.chenjidiqi.icu

JS:   // 单行；/* 多行 */
来源：http://eyt.redwolf501.top


<!-- 参考信息 -->