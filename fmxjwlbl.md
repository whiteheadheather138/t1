代发 wailian999

[U93] JS：模板字符串
来源：http://her.meibo888.top

`共 ${n} 条`
来源：http://azg.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://lhd.jyoumei.cn

const double = x => x * 2;
来源：http://fvz.xylfe.cn

[U95] JS：Promise 包装
来源：http://bxy.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://khi.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://fes.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dwa.guowangkeji.top

[U97] JS：并发请求
来源：http://xoh.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ygi.tianlin.xyz

[U98] JS：fetch 带 JSON
来源：http://ikf.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gzj.yfazqb.com

[U99] JS：事件监听
来源：http://udd.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://gun.tanke756.top

[U100] JS：DOM 查询
来源：http://enq.ehwqpu.com

document.querySelector(".item")
来源：http://bvg.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://kwp.iojbl.cn

el.classList.toggle("active")
来源：http://jbx.jinyuanbaomall.cn

[U102] JS：本地存储
来源：http://vrn.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ujs.havefunace.top

[U103] JS：定时器
来源：http://dpc.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tju.kuanghao11.cn

[U104] JS：防抖
来源：http://caw.sweek.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nlj.tianlin.xyz

[U105] JS：节流
来源：http://ila.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pad.fktsv.cn

[U106] JS：日期格式化
来源：http://wxm.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cxz.cashguo.top

[U107] JS：数字千分位
来源：http://xzc.cheryme.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wkb.yj20258888.top

[U108] JS：随机整数
来源：http://ztd.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hpn.gzhubu.top

[U109] JS：数组分组
来源：http://qpm.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://nxi.tanke756.top

[U110] JS：数组分块
来源：http://tpo.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xku.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://amf.jianghu66.top

new Map(Object.entries(obj))
来源：http://ddc.yj202588.top

[U112] JS：字符串补位
来源：http://mgz.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://erw.shzxlz.cn

[U113] JS：正则替换全部
来源：http://bpa.havefunace.top

s.replaceAll("a", "b")
来源：http://zfn.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://ihf.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cuy.hesvh.cn

[U115] JS：生成 UUID
来源：http://cxx.jinghuilouyu.cn

crypto.randomUUID()
来源：http://szs.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://ltr.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://tdy.yj20258888.top

[U117] JS：单元测试
来源：http://qsz.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://ywn.sxryk.cn

[U118] JS：开发服务器
来源：http://gux.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://eez.ybcxt.top

[U119] JS：生产构建
来源：http://zcj.zhaomingkeji.xyz

npx vite build
来源：http://xos.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://zyc.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://tif.zhaomingkeji.xyz

================================================================================
来源：http://tqb.ydzc1.top

统计汇总
来源：http://jzk.snrcjt.cn

================================================================================
来源：http://fzv.zhaomingkeji.xyz

按语言统计（条）：
来源：http://bwk.hnxiangtu.top

Python ......... 252
来源：http://lud.yangfankeji.com

PHP ............ 252
来源：http://sul.xuanzx.com

JavaScript ..... 252
来源：http://rye.tianlin.xyz

TypeScript ..... 212
来源：http://wfu.yj20258888.top

Java ........... 212
来源：http://iwo.wangdashe.top

Go ............. 212
来源：http://mjs.svipenyu.cn

Ruby ........... 212
来源：http://vxz.sweek.top

C# ............. 212
来源：http://vav.ctjpmb.com

C .............. 30
来源：http://mhf.jinqigfzy.top

C++ ............ 30
来源：http://qar.zhoulong.xyz

SQL ............ 90
来源：http://dzs.cashguo.top

Bash ........... 80
来源：http://wkp.gzhubu.top

Kotlin ......... 15
来源：http://vps.chenjidiqi.icu

Swift .......... 15
来源：http://kqs.redwolf501.top

Lua ............ 10
来源：http://yey.yuanzhike.top

Perl ........... 10
来源：http://qdo.ywan-chungtsiang.top

Scala .......... 10
来源：http://hzc.ctjpmb.com

------------------------------------
来源：http://qif.yj20258.top

合计 ........... 2106 条
来源：http://uif.gzhubu.top

按章节统计：
来源：http://kgq.nanxuanxn.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mcn.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hec.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eyq.hcnkem.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pyq.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://npu.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wlt.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tjg.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sxg.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gpz.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fli.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nyc.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cuq.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lhy.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://znc.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fcu.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rvs.jqgfzy.top

Q SQL 专题                              90
来源：http://lyy.daria6918.cn

R Bash 专题                             80
来源：http://ufu.cqqwz.cn

S C / C++ 专题                          60
来源：http://fzb.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://vjx.zhaomingkeji.xyz

U 高频实用片段                         120
来源：http://hgo.zhijiandao.cn

------------------------------------
来源：http://shm.kuanghao11.cn

合计                                  2106 条
来源：http://zrq.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://ndk.jlsjyb.cn

使用提醒
来源：http://zcy.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://ogm.cucudq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bfe.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mmd.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wcc.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hhm.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kia.yvedp.cn

—— 文件结束 ——
来源：http://czi.316326.xyz

================================================================================
来源：http://svh.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://yua.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://kxb.hongshengwenyu.top

================================================================================
来源：http://ifk.birdmap.top

【收录内容】
来源：http://tob.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tuj.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hbr.vqdsnc.cn

SQL · Bash · C · C++
来源：http://now.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xkq.sufxvd.cn

【使用说明】
来源：http://rqv.svipenyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uig.0kj1m.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uti.nanxinkj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://agp.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lqw.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://aiw.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rxh.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uqe.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tds.epnwcf.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ncd.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cps.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://czs.shuidangran.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kot.xziqi.cn

【文件统计】
来源：http://ebk.nanxinkj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tag.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://wyi.yj202588.top

目  录
来源：http://rck.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://gny.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kiz.9152youxi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zbf.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ewu.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dph.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sgs.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rmy.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://erx.jiagoushi.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pvk.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ize.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xlq.yueranfly.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xse.9152youxi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zrj.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ans.gogol.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fae.smart0.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yyw.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xok.zhongyouzk.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kxh.hnxiangtu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bgd.chenlongwang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cin.wangshuangyany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ezt.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jph.andypj.xyz

================================================================================
来源：http://qwp.guowangkeji.top

A. 基础语法与类型
来源：http://vhi.aibaodan.cn

================================================================================
来源：http://bvu.yueranfly.top

[A01] Hello World
来源：http://btz.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://zcd.ctjpmb.com

PHP:  echo "Hello, World!";
来源：http://wcn.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://llk.birdmap.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vui.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://lid.cqqwz.cn

Go:   fmt.Println("Hello, World!")
来源：http://dip.zdbjq.cn

Ruby: puts "Hello, World!"
来源：http://srw.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://swf.yuxming.cn

[A02] 变量声明与赋值
来源：http://zrk.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cqf.tanke756.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sri.yanxiufei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yzl.tarul.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ric.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://xrq.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://npi.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://chc.shanyushiyangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://wpt.wangshuangyany.cn

[A03] 常量定义
来源：http://sve.jiagoushi.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ees.bjfxy.top

PHP:  const PI = 3.14159;
来源：http://ila.sxryk.cn

JS:   const PI = 3.14159;
来源：http://ymp.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://wvo.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://djn.ybcxt.top

Go:   const PI = 3.14159
来源：http://xnt.hfpthk.cn

Ruby: PI = 3.14159
来源：http://otg.nanxinkj.top

C#:   const double PI = 3.14159;
来源：http://mgo.haohaochexian.top

[A04] 判断变量类型
来源：http://bum.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jzc.sysykeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yua.zdqjudy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xbf.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://lsu.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mly.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://itm.9152youxi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gpx.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://bpd.xinyue.icu

[A05] 整数除法与取模
来源：http://icj.yvedp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pxc.hywenlv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rnw.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jms.hywenlv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wiy.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://zfw.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://ybe.guowangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://awk.xylfe.cn

C#:   7 / 2; 7 % 2
来源：http://lct.pengpengdd.cyou

[A06] 字符串转数字
来源：http://hel.yanxiufei.cn

Py:   int("42"); float("3.14")
来源：http://pwy.uphjek.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://giu.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ofq.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zia.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lel.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://duc.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://smf.xuanzx.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bfo.zycfv.cn

[A07] 数字转字符串
来源：http://ioc.yj20258.top

Py:   str(42)
来源：http://pwb.aibaodan.cn

PHP:  (string) 42; strval(42)
来源：http://yhx.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://yuj.jinqigfzy.top

TS:   String(42)
来源：http://ojo.fengsongda.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pfp.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://nov.quarkkingdee.top

Ruby: 42.to_s
来源：http://hho.aibaodan.cn

C#:   42.ToString()
来源：http://xch.yueranfly.top

[A08] 取整与四舍五入
来源：http://zae.daria6918.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://swu.nanxinkj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hlh.jinghuilouyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://caf.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cob.wangshuangyany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uly.andypj.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xjj.mhx1999.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gyd.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zuf.zhiwuduotai.top

[A09] 绝对值与最大最小值
来源：http://ovr.yj202588.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jxv.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gmw.daxiang520.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qqj.jlsjyb.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ctz.cheryme.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lpe.gotoacloud.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jsy.pycfn.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jth.hnqzz.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kgw.tian-w.cn

[A10] 生成随机数
来源：http://xno.vehdjk.com

Py:   import random; random.randint(1, 100)
来源：http://jcp.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://yzl.cucudq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hrd.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oye.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://pim.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uxa.316326.xyz

Ruby: rand(1..100)
来源：http://scc.yuxming.cn

C#:   new Random().Next(1, 101)
来源：http://ony.xinyue.icu

[A11] 条件表达式（三元）
来源：http://qdu.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://xlc.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wsb.ywan-chungtsiang.top

JS:   x > 0 ? "yes" : "no"
来源：http://apj.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://ick.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://dgi.zhaomingkeji.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://sfz.tarul.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://glo.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wbg.hnxiangtu.top

[A12] 字符串插值 / 格式化
来源：http://whc.jyoumei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lvt.ctjpmb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yey.hnqzz.top

JS:   `Hello, ${name}!`
来源：http://klo.yj202588.top

TS:   `Hello, ${name}!`
来源：http://qex.dashuyun.cn

Java: "Hello, %s!".formatted(name)
来源：http://qxs.vqdsnc.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zab.shangyingyoupin.top

Ruby: "Hello, #{name}!"
来源：http://qxy.hcnkem.com

C#:   $"Hello, {name}!"
来源：http://ffw.epnwcf.com

[A13] 多行字符串（练习 \n 转义）
来源：http://lxo.guowangkeji.top

Py:   "第一行\n第二行"
来源：http://ygn.wangshuangyany.cn

PHP:  "第一行\n第二行"
来源：http://uzh.xinyue.icu

JS:   "第一行\n第二行"
来源：http://dqi.aizwys.cn

TS:   "第一行\n第二行"
来源：http://hkh.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://phm.cqqwz.cn

Go:   "第一行\n第二行"
来源：http://lna.tarul.cn

Ruby: "第一行\n第二行"
来源：http://guv.iojbl.cn

C#:   "第一行\n第二行"
来源：http://slv.bbcook.cn

[A14] 注释写法
来源：http://rms.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://amr.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://haf.cheryme.top

JS:   // 单行；/* 多行 */
来源：http://qby.jqgfzy.top

TS:   // 单行；/* 多行 */
来源：http://atg.jyoumei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lle.sjlbkw.cn

Go:   // 单行；/* 多行 */
来源：http://pwq.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://jun.pycfn.com

C#:   // 单行；/* 多行 */
来源：http://sbg.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://kay.snrcjt.cn

Py:   value = data or "默认值"
来源：http://mgv.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://rmo.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://vzj.mhx1999.top

TS:   const value = data ?? "默认值";
来源：http://php.ivvv.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pje.hnxiangtu.top

Go:   if data == "" { data = "默认值" }
来源：http://zps.uphjek.com

Ruby: value = data || "默认值"
来源：http://vkq.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://joh.yuxming.cn

[A16] 真假值判断规则
来源：http://xun.redwolf501.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cnv.yj20258888.top


<!-- 参考信息 -->