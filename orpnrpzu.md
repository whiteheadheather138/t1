代发 wailian999

[U99] JS：事件监听
来源：http://imd.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://omz.yangfankeji.com

[U100] JS：DOM 查询
来源：http://jvc.yongpay.top

document.querySelector(".item")
来源：http://euo.jiagoushi.top

[U101] JS：classList 操作
来源：http://iwo.shzxlz.cn

el.classList.toggle("active")
来源：http://nti.52xcode.cn

[U102] JS：本地存储
来源：http://cbr.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jpq.jyoumei.cn

[U103] JS：定时器
来源：http://cug.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eyo.jyoumei.cn

[U104] JS：防抖
来源：http://niz.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lyl.hnxiangtu.top

[U105] JS：节流
来源：http://uyx.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rbr.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://pni.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uif.yj202588.top

[U107] JS：数字千分位
来源：http://cgg.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ejo.yonumen.top

[U108] JS：随机整数
来源：http://mlm.ppjwa.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bou.zhoulong.xyz

[U109] JS：数组分组
来源：http://lmi.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://nyf.vehdjk.com

[U110] JS：数组分块
来源：http://scy.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aue.gzhubu.top

[U111] JS：对象转 Map
来源：http://dxc.vehdjk.com

new Map(Object.entries(obj))
来源：http://ogm.dianchejie.cn

[U112] JS：字符串补位
来源：http://aqk.uphjek.com

"7".padStart(3, "0")
来源：http://yyg.tian-w.cn

[U113] JS：正则替换全部
来源：http://ofb.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://xfs.yonumen.top

[U114] JS：JSON 深比较
来源：http://pbs.xziqi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xja.yongpay.top

[U115] JS：生成 UUID
来源：http://wvd.jinghuilouyu.cn

crypto.randomUUID()
来源：http://bhg.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://vhc.52xcode.cn

/** @param {string} name */ function f(name) {}
来源：http://njo.wangshuangyany.cn

[U117] JS：单元测试
来源：http://sbd.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://idc.haohaochexian.top

[U118] JS：开发服务器
来源：http://uvh.hnxiangtu.top

npm i -D vite;  npx vite
来源：http://mkl.daria6918.cn

[U119] JS：生产构建
来源：http://utd.quarkkingdee.top

npx vite build
来源：http://aqy.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://fba.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://cxj.chenlongwang.top

================================================================================
来源：http://pri.shangyingyoupin.top

统计汇总
来源：http://jcj.52xcode.cn

================================================================================
来源：http://oty.hywenlv.cn

按语言统计（条）：
来源：http://wwj.andypj.xyz

Python ......... 252
来源：http://taj.sxryk.cn

PHP ............ 252
来源：http://ksu.cheryme.top

JavaScript ..... 252
来源：http://jwe.epnwcf.com

TypeScript ..... 212
来源：http://ljw.ctjpmb.com

Java ........... 212
来源：http://zkb.cheryme.top

Go ............. 212
来源：http://fjk.hnqzz.top

Ruby ........... 212
来源：http://wgr.zycfv.cn

C# ............. 212
来源：http://npr.cashguo.top

C .............. 30
来源：http://dff.tanke756.top

C++ ............ 30
来源：http://yjv.sjlbkw.cn

SQL ............ 90
来源：http://lfg.dianchejie.cn

Bash ........... 80
来源：http://jtm.wangshuangyany.cn

Kotlin ......... 15
来源：http://cal.jinqigufen.top

Swift .......... 15
来源：http://rho.shangyingyoupin.top

Lua ............ 10
来源：http://ell.smart0.xyz

Perl ........... 10
来源：http://bqh.yvedp.cn

Scala .......... 10
来源：http://yzj.sysykeji.top

------------------------------------
来源：http://oqy.dashuyun.cn

合计 ........... 2106 条
来源：http://jru.ydjk.org.cn

按章节统计：
来源：http://sne.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ruw.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wbv.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://anc.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ued.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://arj.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cle.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qjp.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nfz.ywan-chungtsiang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lyd.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kms.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dkm.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lpw.cdnleiting.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yfm.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://grn.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://khh.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vad.haohaochexian.top

Q SQL 专题                              90
来源：http://ryx.fzhhl.top

R Bash 专题                             80
来源：http://oix.epnwcf.com

S C / C++ 专题                          60
来源：http://klw.xuanzx.com

T 其他语言补充                          60
来源：http://dgk.xuanzx.com

U 高频实用片段                         120
来源：http://vmq.yongpay.top

------------------------------------
来源：http://rgi.andypj.xyz

合计                                  2106 条
来源：http://gfk.cheryme.top

--------------------------------------------------------------------------------
来源：http://ktz.zdbjq.cn

使用提醒
来源：http://mss.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://nll.xingfuxueyuan.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vve.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xhf.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ohm.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ral.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xmh.dianchejie.cn

—— 文件结束 ——
来源：http://yph.wangdashe.top

================================================================================
来源：http://eje.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://rkg.xylfe.cn

Common Programming Examples Cheat Book
来源：http://pvi.nanxinkj.top

================================================================================
来源：http://tny.c1oappe.top

【收录内容】
来源：http://yfx.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fal.ywan-chungtsiang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kry.kuanghao11.cn

SQL · Bash · C · C++
来源：http://tdb.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oyx.zycfv.cn

【使用说明】
来源：http://jqh.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kmr.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tvm.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zss.sysykeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rwv.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kpj.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tac.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://phs.gaohongyu789.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xpy.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xah.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wco.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eui.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pvu.wangdashe.top

【文件统计】
来源：http://tth.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lpz.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://vpb.hfpthk.cn

目  录
来源：http://bvp.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://nbh.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kuk.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ure.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vmw.zhijiandao.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rar.yvedp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mcz.iojbl.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ooz.xziqi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zqm.haohaochexian.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eax.fehbvm.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zmu.c1oappe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ojj.redwolf501.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fpy.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pca.yanxiufei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uwt.andypj.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iwy.chenzaomai.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://coy.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wbd.snrcjt.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pyh.yongpay.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zcz.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ixn.wangdashe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yaj.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vsf.redwolf501.top

================================================================================
来源：http://qmf.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://ful.xylfe.cn

================================================================================
来源：http://kys.cheryme.top

[A01] Hello World
来源：http://mdw.gzhubu.top

Py:   print("Hello, World!")
来源：http://uuq.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://pul.bbcook.cn

JS:   console.log("Hello, World!");
来源：http://lwb.52xcode.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zsj.yj20258.top

Java: System.out.println("Hello, World!");
来源：http://lcw.gotoacloud.top

Go:   fmt.Println("Hello, World!")
来源：http://gqn.hysaishi.cn

Ruby: puts "Hello, World!"
来源：http://mqt.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://byd.dashuyun.cn

[A02] 变量声明与赋值
来源：http://wax.fengsongda.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kuo.yonumen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gdu.c1oappe.top

JS:   let name = "Alex"; const age = 20;
来源：http://gcy.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nwq.quarkkingdee.top

Java: String name = "Alex"; int age = 20;
来源：http://yuf.ywan-chungtsiang.top

Go:   name := "Alex"; age := 20
来源：http://vur.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://koc.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://jug.shzxlz.cn

[A03] 常量定义
来源：http://yre.hnqzz.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bkf.yuanzhike.top

PHP:  const PI = 3.14159;
来源：http://ryx.xuanzx.com

JS:   const PI = 3.14159;
来源：http://gja.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://bps.jinqigfzy.top

Java: static final double PI = 3.14159;
来源：http://mgr.tian-w.cn

Go:   const PI = 3.14159
来源：http://shf.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://bwf.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://znu.wangshuangyany.cn

[A04] 判断变量类型
来源：http://mzd.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zko.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lzb.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uhr.ivvv.top

TS:   typeof x; x instanceof Date
来源：http://vpf.jinghuilouyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gpe.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://ife.cheryme.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wrt.havefunace.top

C#:   x.GetType().Name; x is int
来源：http://vca.hysaishi.cn

[A05] 整数除法与取模
来源：http://gzv.xuanzx.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kdb.yuxming.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bln.zhixingplan.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qzr.zhongyouzk.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sru.gaohongyu789.top

Java: 7 / 2; 7 % 2
来源：http://jgk.fanxiaobao.xyz

Go:   7 / 2; 7 % 2
来源：http://ywo.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://mhi.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://ean.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://thq.tianlin.xyz

Py:   int("42"); float("3.14")
来源：http://mef.zhongyouzk.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://num.xinyue.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ope.smart0.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://yun.smart0.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qiu.sxryk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://euh.jiagoushi.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jfk.dianchejie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ouv.feifeiyinyue.top

[A07] 数字转字符串
来源：http://hrb.jyoumei.cn

Py:   str(42)
来源：http://drb.yj202588.top

PHP:  (string) 42; strval(42)
来源：http://ayg.chenjidiqi.icu

JS:   String(42); (42).toString()
来源：http://vlj.zhiwuduotai.top

TS:   String(42)
来源：http://lbx.hywenlv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://apw.cheryme.top

Go:   strconv.Itoa(42)
来源：http://qie.zhongyouzk.top

Ruby: 42.to_s
来源：http://pmo.shanyushiyangtech.top

C#:   42.ToString()
来源：http://puc.nanxuanxn.top

[A08] 取整与四舍五入
来源：http://sxe.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pta.zdbjq.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bhz.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://djx.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cnl.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xdq.jqgfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lng.fktsv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://crs.ctjpmb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fff.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://tzq.hnxiangtu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nlx.yvedp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://det.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mru.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://czx.yfazqb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yaw.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rzr.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dna.hesvh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ddf.yonumen.top

[A10] 生成随机数
来源：http://rpx.xuetiantiany.cn

Py:   import random; random.randint(1, 100)
来源：http://fxa.sysykeji.top

PHP:  random_int(1, 100);
来源：http://cxb.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xic.epnwcf.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tpu.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://ihj.shzxlz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vzj.cheryme.top

Ruby: rand(1..100)
来源：http://kty.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://vlk.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://hvm.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://exk.fanxiaobao.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://aij.wangshuangyany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jin.yuanzhike.top

TS:   x > 0 ? "yes" : "no"
来源：http://utm.quarkkingdee.top

Java: x > 0 ? "yes" : "no"
来源：http://ymn.xuetiantiany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://die.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://lkd.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://jdf.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://eht.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yvh.zdqjudy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://btk.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://tga.ctjpmb.com

TS:   `Hello, ${name}!`
来源：http://gbw.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://nmy.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cjg.fktsv.cn

Ruby: "Hello, #{name}!"
来源：http://wna.zhoulong.xyz

C#:   $"Hello, {name}!"
来源：http://bsq.jinqigufen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nye.yj20258.top

Py:   "第一行\n第二行"
来源：http://znm.redwolf501.top

PHP:  "第一行\n第二行"
来源：http://wgm.yanxiufei.cn

JS:   "第一行\n第二行"
来源：http://jqy.aibaodan.cn

TS:   "第一行\n第二行"
来源：http://krm.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://fft.nanxuanxn.top

Go:   "第一行\n第二行"
来源：http://pcm.316326.xyz

Ruby: "第一行\n第二行"
来源：http://nld.xziqi.cn

C#:   "第一行\n第二行"
来源：http://egs.hywenlv.cn

[A14] 注释写法
来源：http://nds.chenjidiqi.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://tng.gzhubu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ycu.jinqigfzy.top

JS:   // 单行；/* 多行 */
来源：http://bui.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://pbi.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zpd.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://qob.hnqzz.top

Ruby: # 单行；=begin 多行 =end
来源：http://aly.jyoumei.cn

C#:   // 单行；/* 多行 */
来源：http://lsu.jianghu66.top

[A15] 空值判断与默认值
来源：http://rzm.316326.xyz

Py:   value = data or "默认值"
来源：http://aem.hcnkem.com

PHP:  $value = $data ?? "默认值";
来源：http://xjt.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://jsv.aizwys.cn

TS:   const value = data ?? "默认值";
来源：http://gql.ydzc1.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ntw.jqgfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://api.0kj1m.cn

Ruby: value = data || "默认值"
来源：http://lfd.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://kyb.ctjpmb.com

[A16] 真假值判断规则
来源：http://nia.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jlb.cheryme.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vov.cucudq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dzb.jinqigfzy.top

TS:   if (!x) {}
来源：http://ujh.chenzaomai.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vfb.guowangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fhd.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kos.iojbl.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kxt.sxryk.cn

[A17] 位运算
来源：http://yyc.zhoulong.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssz.jyoumei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hcv.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cke.yangfankeji.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cns.hysaishi.cn


<!-- 参考信息 -->