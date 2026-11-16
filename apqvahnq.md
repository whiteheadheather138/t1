代发 wailian999

[U87] JS：解构默认值
来源：http://ozw.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://sho.hysaishi.cn

[U88] JS：对象展开合并
来源：http://ffb.jlsjyb.cn

{ ...a, ...b }
来源：http://wir.bjfxy.top

[U89] JS：数组去重
来源：http://nyh.zhengqikj.top

[...new Set(arr)]
来源：http://iln.wangdashe.top

[U90] JS：数字数组排序
来源：http://fya.daria6918.cn

[...arr].sort((a, b) => a - b)
来源：http://iuc.fktsv.cn

[U91] JS：对象键值遍历
来源：http://hse.quarkkingdee.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wqs.hfpthk.cn

[U92] JS：深拷贝
来源：http://qpv.yuanzhike.top

structuredClone(obj)
来源：http://igs.xuanzx.com

[U93] JS：模板字符串
来源：http://dzx.jinqigfzy.top

`共 ${n} 条`
来源：http://ueq.redwolf501.top

[U94] JS：箭头函数
来源：http://wej.shuidangran.top

const double = x => x * 2;
来源：http://gid.tian-w.cn

[U95] JS：Promise 包装
来源：http://ehu.havefunace.top

new Promise((resolve, reject) => {})
来源：http://yzl.yj20258.top

[U96] JS：async/await 与异常
来源：http://ipf.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uum.xuanzx.com

[U97] JS：并发请求
来源：http://awq.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://jvu.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://tvf.shanyushiyangtech.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ooo.haohaochexian.top

[U99] JS：事件监听
来源：http://opu.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://zeo.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://lew.yfazqb.com

document.querySelector(".item")
来源：http://yjx.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://vdz.hnqzz.top

el.classList.toggle("active")
来源：http://phx.ivvv.top

[U102] JS：本地存储
来源：http://nww.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bov.yfazqb.com

[U103] JS：定时器
来源：http://xrd.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bbe.guowangkeji.top

[U104] JS：防抖
来源：http://dmn.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dnt.gogol.net.cn

[U105] JS：节流
来源：http://jor.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fjv.jlsjyb.cn

[U106] JS：日期格式化
来源：http://nmn.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lxv.zhijiandao.cn

[U107] JS：数字千分位
来源：http://lnc.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jtl.hammf.cn

[U108] JS：随机整数
来源：http://feg.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://otw.dianchejie.cn

[U109] JS：数组分组
来源：http://uhm.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://ofl.uphjek.com

[U110] JS：数组分块
来源：http://vlg.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tmj.gzhubu.top

[U111] JS：对象转 Map
来源：http://hzp.meibo888.top

new Map(Object.entries(obj))
来源：http://fai.shuidangran.top

[U112] JS：字符串补位
来源：http://tjd.hcnkem.com

"7".padStart(3, "0")
来源：http://hza.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://cvq.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://ohz.ivvv.top

[U114] JS：JSON 深比较
来源：http://duq.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://drz.epnwcf.com

[U115] JS：生成 UUID
来源：http://wgm.feifeiyinyue.top

crypto.randomUUID()
来源：http://qjm.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://rcy.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://hdm.ydzc1.top

[U117] JS：单元测试
来源：http://sku.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://jsm.fehbvm.com

[U118] JS：开发服务器
来源：http://ifz.nwbrower.top

npm i -D vite;  npx vite
来源：http://qjb.jqgfzy.top

[U119] JS：生产构建
来源：http://ulq.yfazqb.com

npx vite build
来源：http://mqb.ydzc1.top

[U120] JS：读取环境变量（Vite）
来源：http://rve.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://joc.feifeiyinyue.top

================================================================================
来源：http://hru.vehdjk.com

统计汇总
来源：http://rmn.gogol.net.cn

================================================================================
来源：http://teg.0kj1m.cn

按语言统计（条）：
来源：http://eru.xziqi.cn

Python ......... 252
来源：http://xdc.shuidangran.top

PHP ............ 252
来源：http://bxh.yangfankeji.com

JavaScript ..... 252
来源：http://dvb.tanke756.top

TypeScript ..... 212
来源：http://xps.0kj1m.cn

Java ........... 212
来源：http://dqm.shanyushiyangkeji.top

Go ............. 212
来源：http://fmg.hysaishi.cn

Ruby ........... 212
来源：http://ehr.fktsv.cn

C# ............. 212
来源：http://rau.fengsongda.top

C .............. 30
来源：http://hyu.bjfxy.top

C++ ............ 30
来源：http://art.jiagoushi.top

SQL ............ 90
来源：http://dku.ybcxt.top

Bash ........... 80
来源：http://ogd.quarkkingdee.top

Kotlin ......... 15
来源：http://wtw.wangshuangyany.cn

Swift .......... 15
来源：http://ybz.nanxuanxn.top

Lua ............ 10
来源：http://lqy.guannengcc.top

Perl ........... 10
来源：http://dnd.quarkkingdee.top

Scala .......... 10
来源：http://xyz.cashguo.top

------------------------------------
来源：http://egz.ybcxt.top

合计 ........... 2106 条
来源：http://msy.vehdjk.com

按章节统计：
来源：http://rhj.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lfn.wangshuangyany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://acw.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sdk.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fli.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ahi.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pla.ydjk.org.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aei.cdnleiting.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cun.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wvl.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jch.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ify.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bhx.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vek.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ayy.bjfxy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tzh.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ojl.dashuyun.cn

Q SQL 专题                              90
来源：http://wdl.bjfxy.top

R Bash 专题                             80
来源：http://tis.xziqi.cn

S C / C++ 专题                          60
来源：http://vga.fehbvm.com

T 其他语言补充                          60
来源：http://ejj.yueranfly.top

U 高频实用片段                         120
来源：http://frk.xylfe.cn

------------------------------------
来源：http://zzd.guowangkeji.top

合计                                  2106 条
来源：http://swt.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://gzc.wangshuangyany.cn

使用提醒
来源：http://ffc.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://fjf.shuidangran.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hxz.yvedp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://exz.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ifp.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://oem.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://luz.vehdjk.com

—— 文件结束 ——
来源：http://dat.zhijiandao.cn

================================================================================
来源：http://fow.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://quh.epnwcf.com

Common Programming Examples Cheat Book
来源：http://lfm.ctjpmb.com

================================================================================
来源：http://gts.hcnkem.com

【收录内容】
来源：http://scz.hnxiangtu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wtn.jiagoushi.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hvx.vehdjk.com

SQL · Bash · C · C++
来源：http://ejh.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wgw.yj202588.top

【使用说明】
来源：http://ybn.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ttx.yueranfly.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ggx.aizwys.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xlj.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dow.vqdsnc.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://czc.jqgfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dtw.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cqf.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rrr.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vsy.ywan-chungtsiang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pln.cqqwz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mwf.cheryme.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uyh.zhiwuduotai.top

【文件统计】
来源：http://uak.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ufg.fzhhl.top

--------------------------------------------------------------------------------
来源：http://mkm.smart0.xyz

目  录
来源：http://hvn.pycfn.com

--------------------------------------------------------------------------------
来源：http://uiu.hywenlv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zig.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://egf.wangdashe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rri.nwbrower.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ghu.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://exb.wangshuangyany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fpl.ehwqpu.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wcn.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xbk.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jbx.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jyp.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dmg.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wgz.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xfw.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aes.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://urd.cdnleiting.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rol.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hql.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uqc.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sqe.ehwqpu.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xgu.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rvh.yfazqb.com

================================================================================
来源：http://kzn.wangdashe.top

A. 基础语法与类型
来源：http://aru.xuetiantiany.cn

================================================================================
来源：http://dob.nanxuanxn.top

[A01] Hello World
来源：http://zsk.fktsv.cn

Py:   print("Hello, World!")
来源：http://cls.ppjwa.cn

PHP:  echo "Hello, World!";
来源：http://cxh.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://nqp.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uzr.jqgufenzy.top

Java: System.out.println("Hello, World!");
来源：http://cex.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://zws.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://yqm.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://obx.zdqjudy.top

[A02] 变量声明与赋值
来源：http://urz.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zkz.shanyushiyangtech.top

PHP:  $name = "Alex"; $age = 20;
来源：http://irm.chenlongwang.top

JS:   let name = "Alex"; const age = 20;
来源：http://rry.sjlbkw.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cxh.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://kin.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://gdt.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://slp.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zbq.havefunace.top

[A03] 常量定义
来源：http://gbz.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://efp.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://fsm.yongpay.top

JS:   const PI = 3.14159;
来源：http://chx.birdmap.top

TS:   const PI: number = 3.14159;
来源：http://pdl.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://mzg.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://wqw.zdqjudy.top

Ruby: PI = 3.14159
来源：http://evz.jyoumei.cn

C#:   const double PI = 3.14159;
来源：http://wzg.0kj1m.cn

[A04] 判断变量类型
来源：http://cof.zhijiandao.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uac.hongshengwenyu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kfz.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yjm.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://spm.ctjpmb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://env.cdnleiting.top

Go:   reflect.TypeOf(x).Name()
来源：http://ppy.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://pwu.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://nsn.yangfankeji.com

[A05] 整数除法与取模
来源：http://kfl.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mnr.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://lbk.jinyuanbaomall.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eru.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fth.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://dsj.chenjidiqi.icu

Go:   7 / 2; 7 % 2
来源：http://upy.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://uhz.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://fyp.guannengcc.top

[A06] 字符串转数字
来源：http://kxw.gogol.net.cn

Py:   int("42"); float("3.14")
来源：http://pse.svipenyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bpz.fktsv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ofb.daxiang520.top

TS:   parseInt("42", 10); Number("42")
来源：http://tfs.chenlongwang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cfc.snrcjt.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lnl.tian-w.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bxj.xziqi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uhp.vehdjk.com

[A07] 数字转字符串
来源：http://isv.ctjpmb.com

Py:   str(42)
来源：http://xoa.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://gri.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://bbz.zhaomingkeji.xyz

TS:   String(42)
来源：http://hsu.zhoulong.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://hxx.bbcook.cn

Go:   strconv.Itoa(42)
来源：http://gbm.xinyue.icu

Ruby: 42.to_s
来源：http://sfm.fanxiaobao.xyz

C#:   42.ToString()
来源：http://ctx.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://wku.fktsv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://buj.gogol.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mox.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eht.yonumen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qup.gaohongyu789.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://klq.fzhhl.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://clq.fengsongda.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lyf.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pko.cashguo.top

[A09] 绝对值与最大最小值
来源：http://lsf.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jse.c1oappe.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vwi.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hvu.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mwy.shuidangran.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mvk.hongshengwenyu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://laa.shangyingyoupin.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hdt.vehdjk.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cev.zhongyouzk.top

[A10] 生成随机数
来源：http://swg.jinyuanbaomall.cn

Py:   import random; random.randint(1, 100)
来源：http://rko.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://hir.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gcr.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ybk.nanxinkj.top

Java: new Random().nextInt(100) + 1
来源：http://wpd.fktsv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vej.hcnkem.com

Ruby: rand(1..100)
来源：http://osg.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://asl.havefunace.top

[A11] 条件表达式（三元）
来源：http://jyf.epnwcf.com

Py:   "yes" if x > 0 else "no"
来源：http://lrc.zycfv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://euv.jyoumei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uma.andypj.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://meu.tianlin.xyz

Java: x > 0 ? "yes" : "no"
来源：http://fnv.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://res.ydzc1.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ris.tarul.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jqz.chenjidiqi.icu

[A12] 字符串插值 / 格式化
来源：http://sob.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://frp.vehdjk.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ise.zhijiandao.cn

JS:   `Hello, ${name}!`
来源：http://taq.havefunace.top

TS:   `Hello, ${name}!`
来源：http://qri.c1oappe.top

Java: "Hello, %s!".formatted(name)
来源：http://svu.xziqi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rnb.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://qzb.hysaishi.cn

C#:   $"Hello, {name}!"
来源：http://iog.haohaochexian.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ell.wangdashe.top

Py:   "第一行\n第二行"
来源：http://dck.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://qbi.yfazqb.com

JS:   "第一行\n第二行"
来源：http://wqh.tian-w.cn

TS:   "第一行\n第二行"
来源：http://clp.uphjek.com

Java: "第一行\n第二行"
来源：http://mty.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://psy.sweek.top

Ruby: "第一行\n第二行"
来源：http://jcl.yvedp.cn

C#:   "第一行\n第二行"
来源：http://yeg.ywan-chungtsiang.top

[A14] 注释写法
来源：http://izu.xylfe.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://map.smart0.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://rwq.aibaodan.cn

JS:   // 单行；/* 多行 */
来源：http://tws.yj20258888.top

TS:   // 单行；/* 多行 */
来源：http://qlo.svipenyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cnv.yanxiufei.cn

Go:   // 单行；/* 多行 */
来源：http://dwd.quarkkingdee.top

Ruby: # 单行；=begin 多行 =end
来源：http://mcl.wangshuangyany.cn


<!-- 参考信息 -->