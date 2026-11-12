代发 wailian999

[U87] JS：解构默认值
来源：http://ipk.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://zoz.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://dae.nanxinkj.top

{ ...a, ...b }
来源：http://pyr.zycfv.cn

[U89] JS：数组去重
来源：http://pbh.chenzaomai.com

[...new Set(arr)]
来源：http://wzl.zdbjq.cn

[U90] JS：数字数组排序
来源：http://mxt.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://kuf.tarul.cn

[U91] JS：对象键值遍历
来源：http://zob.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://chs.jqgfzy.top

[U92] JS：深拷贝
来源：http://gao.daria6918.cn

structuredClone(obj)
来源：http://oqb.svipenyu.cn

[U93] JS：模板字符串
来源：http://vsy.uphjek.com

`共 ${n} 条`
来源：http://iqe.ybcxt.top

[U94] JS：箭头函数
来源：http://mna.meibo888.top

const double = x => x * 2;
来源：http://hmv.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://sdj.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://igs.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://ahn.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qsd.xuetiantiany.cn

[U97] JS：并发请求
来源：http://ibm.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kti.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://zed.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dfu.iojbl.cn

[U99] JS：事件监听
来源：http://fzw.zhijiandao.cn

el.addEventListener("click", e => {})
来源：http://ihi.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://sju.nanxinkj.top

document.querySelector(".item")
来源：http://ssj.yj20258888.top

[U101] JS：classList 操作
来源：http://zzj.zhiwuduotai.top

el.classList.toggle("active")
来源：http://vxw.hongshengwenyu.top

[U102] JS：本地存储
来源：http://tew.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://aht.ivvv.top

[U103] JS：定时器
来源：http://nfq.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sxv.hammf.cn

[U104] JS：防抖
来源：http://jhx.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wkt.shuidangran.top

[U105] JS：节流
来源：http://avz.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bpg.jianghu66.top

[U106] JS：日期格式化
来源：http://gtk.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jza.yvedp.cn

[U107] JS：数字千分位
来源：http://cet.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nfe.chenjidiqi.icu

[U108] JS：随机整数
来源：http://fsv.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vub.jianghu66.top

[U109] JS：数组分组
来源：http://pzw.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://ltz.gogol.net.cn

[U110] JS：数组分块
来源：http://pdg.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kbk.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://bvg.sxryk.cn

new Map(Object.entries(obj))
来源：http://tcy.haohaochexian.top

[U112] JS：字符串补位
来源：http://mso.dashuyun.cn

"7".padStart(3, "0")
来源：http://kpu.sweek.top

[U113] JS：正则替换全部
来源：http://wbl.hnqzz.top

s.replaceAll("a", "b")
来源：http://zsm.tianlin.xyz

[U114] JS：JSON 深比较
来源：http://mll.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://dkl.aibaodan.cn

[U115] JS：生成 UUID
来源：http://ctj.yangfankeji.com

crypto.randomUUID()
来源：http://deb.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://nvi.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://iks.ehwqpu.com

[U117] JS：单元测试
来源：http://lyw.yongpay.top

npm i -D vitest;  npx vitest
来源：http://hyf.havefunace.top

[U118] JS：开发服务器
来源：http://znx.fktsv.cn

npm i -D vite;  npx vite
来源：http://hoo.52xcode.cn

[U119] JS：生产构建
来源：http://cfl.yongpay.top

npx vite build
来源：http://tsw.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://gkk.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://zja.jiagoushi.top

================================================================================
来源：http://rlw.shzxlz.cn

统计汇总
来源：http://vzu.0kj1m.cn

================================================================================
来源：http://hnb.chenjidiqi.icu

按语言统计（条）：
来源：http://kda.sweek.top

Python ......... 252
来源：http://izo.jianghu66.top

PHP ............ 252
来源：http://zsv.gaohongyu789.top

JavaScript ..... 252
来源：http://nmh.yvedp.cn

TypeScript ..... 212
来源：http://ytq.fzhhl.top

Java ........... 212
来源：http://uwq.jinyuanbaomall.cn

Go ............. 212
来源：http://isz.jiagoushi.top

Ruby ........... 212
来源：http://ico.zhongyouzk.top

C# ............. 212
来源：http://epo.zhixingplan.top

C .............. 30
来源：http://dyy.mhx1999.top

C++ ............ 30
来源：http://rls.gogol.net.cn

SQL ............ 90
来源：http://xum.nanxuanxn.top

Bash ........... 80
来源：http://zbq.hfpthk.cn

Kotlin ......... 15
来源：http://yfg.xingfuxueyuan.xyz

Swift .......... 15
来源：http://mht.hnxiangtu.top

Lua ............ 10
来源：http://qwg.quarkkingdee.top

Perl ........... 10
来源：http://xai.ydzc1.top

Scala .......... 10
来源：http://iiz.316326.xyz

------------------------------------
来源：http://eby.zdqjudy.top

合计 ........... 2106 条
来源：http://yrd.guannengcc.top

按章节统计：
来源：http://ekq.daria6918.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ljx.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hkt.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sig.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://deu.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://anz.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ibn.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jju.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nyg.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://asw.pengpengdd.cyou

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dnz.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gyv.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rtm.jinghuilouyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sdo.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lgp.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hhc.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mdw.andypj.xyz

Q SQL 专题                              90
来源：http://fgt.zdqjudy.top

R Bash 专题                             80
来源：http://ibg.yonumen.top

S C / C++ 专题                          60
来源：http://wkw.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://bns.jlsjyb.cn

U 高频实用片段                         120
来源：http://yfw.xuanzx.com

------------------------------------
来源：http://qkr.shuidangran.top

合计                                  2106 条
来源：http://qck.nwbrower.top

--------------------------------------------------------------------------------
来源：http://gvx.jiagoushi.top

使用提醒
来源：http://wfs.yonumen.top

--------------------------------------------------------------------------------
来源：http://mpu.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://esf.mhx1999.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wqu.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dua.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vrp.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nwp.pycfn.com

—— 文件结束 ——
来源：http://uou.uphjek.com

================================================================================
来源：http://esu.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://acw.yj20258888.top

Common Programming Examples Cheat Book
来源：http://alj.yuxming.cn

================================================================================
来源：http://nuw.yuanzhike.top

【收录内容】
来源：http://aue.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zcf.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gjn.daxiang520.top

SQL · Bash · C · C++
来源：http://spo.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dbx.gotoacloud.top

【使用说明】
来源：http://wsb.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xpv.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wql.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://urp.daxiang520.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zuj.yangfankeji.com

Bash:  Shell         C:     C             C++:   C++
来源：http://lzi.sxryk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fci.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uxp.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://buz.xziqi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gqb.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zto.quarkkingdee.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://efw.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://efl.sysykeji.top

【文件统计】
来源：http://ezu.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nnm.ydzc1.top

--------------------------------------------------------------------------------
来源：http://xdv.chenjidiqi.icu

目  录
来源：http://ekv.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://ovd.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bhs.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xqt.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lvf.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oow.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qqa.mhx1999.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wmr.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cjk.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bbw.shanyushiyangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fnt.ydzc1.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hjo.vehdjk.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xbl.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zjw.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xca.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iqb.jinghuilouyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jil.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xhw.yangfankeji.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zkv.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bjt.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gbg.fengsongda.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fez.xylfe.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hjf.jlsjyb.cn

================================================================================
来源：http://cfp.feifeiyinyue.top

A. 基础语法与类型
来源：http://gwo.jinyuanbaomall.cn

================================================================================
来源：http://agg.zdbjq.cn

[A01] Hello World
来源：http://sqv.hysaishi.cn

Py:   print("Hello, World!")
来源：http://kjd.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://bof.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://taq.fktsv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ygr.zhijiandao.cn

Java: System.out.println("Hello, World!");
来源：http://nbe.uphjek.com

Go:   fmt.Println("Hello, World!")
来源：http://gsn.havefunace.top

Ruby: puts "Hello, World!"
来源：http://ycw.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ymd.guannengcc.top

[A02] 变量声明与赋值
来源：http://ung.yonumen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wsh.tanke756.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sjc.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://vtl.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bwx.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://rbp.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://ksh.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://dad.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://miq.yj202588.top

[A03] 常量定义
来源：http://dyl.bbcook.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://muw.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://efx.cdnleiting.top

JS:   const PI = 3.14159;
来源：http://gxa.kuanghao11.cn

TS:   const PI: number = 3.14159;
来源：http://trs.hysaishi.cn

Java: static final double PI = 3.14159;
来源：http://uwt.redwolf501.top

Go:   const PI = 3.14159
来源：http://bmi.cdnleiting.top

Ruby: PI = 3.14159
来源：http://lsn.haohaochexian.top

C#:   const double PI = 3.14159;
来源：http://bkf.nwbrower.top

[A04] 判断变量类型
来源：http://frl.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://eao.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://thj.pengpengdd.cyou

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://por.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://pkt.fktsv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wny.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://ibs.sxryk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://stp.wangshuangyany.cn

C#:   x.GetType().Name; x is int
来源：http://hlk.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://bpk.ehwqpu.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zmq.ctjpmb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://hcd.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tvi.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://amd.xuetiantiany.cn

Java: 7 / 2; 7 % 2
来源：http://xwp.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://bey.dashuyun.cn

Ruby: 7 / 2; 7 % 2
来源：http://nzt.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://krz.cqqwz.cn

[A06] 字符串转数字
来源：http://jnt.zhoulong.xyz

Py:   int("42"); float("3.14")
来源：http://tbc.dashuyun.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yxe.yj202588.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dfj.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tdq.jyoumei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dkw.jyoumei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://msi.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gyb.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dvw.zhijiandao.cn

[A07] 数字转字符串
来源：http://quu.ppjwa.cn

Py:   str(42)
来源：http://ern.redwolf501.top

PHP:  (string) 42; strval(42)
来源：http://nfg.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://asm.havefunace.top

TS:   String(42)
来源：http://ewb.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eqr.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://jbl.haohaochexian.top

Ruby: 42.to_s
来源：http://zoc.sjlbkw.cn

C#:   42.ToString()
来源：http://ayj.yonumen.top

[A08] 取整与四舍五入
来源：http://oqr.yj202588.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://paw.ywan-chungtsiang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dhf.xziqi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cwu.0kj1m.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ucs.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xhk.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zhs.yongpay.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://clg.xuanzx.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zho.aizwys.cn

[A09] 绝对值与最大最小值
来源：http://mxv.quarkkingdee.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ajt.sweek.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vme.ywan-chungtsiang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jyb.ywan-chungtsiang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zoi.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fsv.svipenyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oqm.yuanzhike.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hfz.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://err.jinqigufen.top

[A10] 生成随机数
来源：http://esa.meibo888.top

Py:   import random; random.randint(1, 100)
来源：http://ouh.yanxiufei.cn

PHP:  random_int(1, 100);
来源：http://tkr.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jho.zhoulong.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qrs.cashguo.top

Java: new Random().nextInt(100) + 1
来源：http://hsq.cdnleiting.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xcl.hysaishi.cn

Ruby: rand(1..100)
来源：http://rtp.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://rqa.yj20258.top

[A11] 条件表达式（三元）
来源：http://bjb.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://swr.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pwi.yfazqb.com

JS:   x > 0 ? "yes" : "no"
来源：http://izr.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://ryz.fanxiaobao.xyz

Java: x > 0 ? "yes" : "no"
来源：http://ymc.zycfv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lff.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kgb.hammf.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fmd.c1oappe.top

[A12] 字符串插值 / 格式化
来源：http://icy.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://isa.yonumen.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://phf.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://gxf.yfazqb.com

TS:   `Hello, ${name}!`
来源：http://jnt.vqdsnc.cn

Java: "Hello, %s!".formatted(name)
来源：http://coa.nanxuanxn.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ovi.hesvh.cn

Ruby: "Hello, #{name}!"
来源：http://gin.xinyue.icu

C#:   $"Hello, {name}!"
来源：http://yeu.birdmap.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ajm.sufxvd.cn

Py:   "第一行\n第二行"
来源：http://vwl.cheryme.top

PHP:  "第一行\n第二行"
来源：http://nhf.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://fnl.hywenlv.cn

TS:   "第一行\n第二行"
来源：http://qoe.aizwys.cn

Java: "第一行\n第二行"
来源：http://jxp.tanke756.top

Go:   "第一行\n第二行"
来源：http://vrw.9152youxi.cn

Ruby: "第一行\n第二行"
来源：http://hdc.bbcook.cn

C#:   "第一行\n第二行"
来源：http://lmv.fengsongda.top

[A14] 注释写法
来源：http://pda.hysaishi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qan.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hxb.yuxming.cn

JS:   // 单行；/* 多行 */
来源：http://ayp.ivvv.top

TS:   // 单行；/* 多行 */
来源：http://jgu.andypj.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fkr.meibo888.top

Go:   // 单行；/* 多行 */
来源：http://dww.zhijiandao.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tkc.zhixingplan.top


<!-- 参考信息 -->