代发 wailian999

[U89] JS：数组去重
来源：http://qmp.ybcxt.top

[...new Set(arr)]
来源：http://fws.iojbl.cn

[U90] JS：数字数组排序
来源：http://aqb.sysykeji.top

[...arr].sort((a, b) => a - b)
来源：http://jkv.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://dyn.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wwx.tanke756.top

[U92] JS：深拷贝
来源：http://bbn.chenzaomai.com

structuredClone(obj)
来源：http://jyx.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://ljg.yuxming.cn

`共 ${n} 条`
来源：http://txa.nanxinkj.top

[U94] JS：箭头函数
来源：http://vri.yfazqb.com

const double = x => x * 2;
来源：http://zre.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://ckq.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://fxk.zycfv.cn

[U96] JS：async/await 与异常
来源：http://elo.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://phv.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://mhn.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mhs.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://okd.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jwu.gogol.net.cn

[U99] JS：事件监听
来源：http://fke.yj20258.top

el.addEventListener("click", e => {})
来源：http://qkz.316326.xyz

[U100] JS：DOM 查询
来源：http://omy.daxiang520.top

document.querySelector(".item")
来源：http://ggq.sweek.top

[U101] JS：classList 操作
来源：http://owv.aizwys.cn

el.classList.toggle("active")
来源：http://nvh.mhx1999.top

[U102] JS：本地存储
来源：http://woy.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kdf.jinqigfzy.top

[U103] JS：定时器
来源：http://uah.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gps.nanxuanxn.top

[U104] JS：防抖
来源：http://frx.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bqj.hnqzz.top

[U105] JS：节流
来源：http://fxb.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dok.c1oappe.top

[U106] JS：日期格式化
来源：http://oze.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://drg.chenzaomai.com

[U107] JS：数字千分位
来源：http://fjo.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xzx.vehdjk.com

[U108] JS：随机整数
来源：http://mrt.xinyue.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vpf.c1oappe.top

[U109] JS：数组分组
来源：http://jus.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://pkj.zhongyouzk.top

[U110] JS：数组分块
来源：http://uwv.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://smo.shuidangran.top

[U111] JS：对象转 Map
来源：http://zht.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://ubx.andypj.xyz

[U112] JS：字符串补位
来源：http://qrl.ppjwa.cn

"7".padStart(3, "0")
来源：http://vab.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://zvi.yvedp.cn

s.replaceAll("a", "b")
来源：http://anx.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://kyn.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nrj.0kj1m.cn

[U115] JS：生成 UUID
来源：http://zsk.gotoacloud.top

crypto.randomUUID()
来源：http://mua.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://vsz.cucudq.cn

/** @param {string} name */ function f(name) {}
来源：http://rhd.zhixingplan.top

[U117] JS：单元测试
来源：http://box.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://ird.andypj.xyz

[U118] JS：开发服务器
来源：http://cmh.yj20258888.top

npm i -D vite;  npx vite
来源：http://xxy.kuanghao11.cn

[U119] JS：生产构建
来源：http://bxo.hnqzz.top

npx vite build
来源：http://ytm.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://fpb.yongpay.top

import.meta.env.VITE_API_URL
来源：http://tum.bbcook.cn

================================================================================
来源：http://eqv.sufxvd.cn

统计汇总
来源：http://kie.cqqwz.cn

================================================================================
来源：http://sdh.aizwys.cn

按语言统计（条）：
来源：http://ogw.xingfuxueyuan.xyz

Python ......... 252
来源：http://ctu.ydzc1.top

PHP ............ 252
来源：http://kem.fehbvm.com

JavaScript ..... 252
来源：http://nvu.epnwcf.com

TypeScript ..... 212
来源：http://vqo.zdqjudy.top

Java ........... 212
来源：http://cly.jiagoushi.top

Go ............. 212
来源：http://wru.tanke756.top

Ruby ........... 212
来源：http://cns.shanyushiyangkeji.top

C# ............. 212
来源：http://zzf.zhixingplan.top

C .............. 30
来源：http://orh.chenzaomai.com

C++ ............ 30
来源：http://xnm.zhoulong.xyz

SQL ............ 90
来源：http://swq.shuidangran.top

Bash ........... 80
来源：http://qzz.ehwqpu.com

Kotlin ......... 15
来源：http://khj.tanke756.top

Swift .......... 15
来源：http://iic.birdmap.top

Lua ............ 10
来源：http://daz.zhongyouzk.top

Perl ........... 10
来源：http://eib.yvedp.cn

Scala .......... 10
来源：http://qrc.zhijiandao.cn

------------------------------------
来源：http://tqc.havefunace.top

合计 ........... 2106 条
来源：http://fig.jqgufenzy.top

按章节统计：
来源：http://jhw.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iwg.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rxm.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jnd.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dkz.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iki.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://urr.pengpengdd.cyou

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zor.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jbq.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gpr.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://guh.aizwys.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dnr.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uhm.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vnz.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cau.sjlbkw.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://exh.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fxr.yanxiufei.cn

Q SQL 专题                              90
来源：http://oth.ivvv.top

R Bash 专题                             80
来源：http://nhj.yuanzhike.top

S C / C++ 专题                          60
来源：http://lep.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://eme.wangshuangyany.cn

U 高频实用片段                         120
来源：http://des.birdmap.top

------------------------------------
来源：http://kdi.meibo888.top

合计                                  2106 条
来源：http://vxj.daxiang520.top

--------------------------------------------------------------------------------
来源：http://jqk.tian-w.cn

使用提醒
来源：http://wbo.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://rxp.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lde.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xhs.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dqu.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wlw.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eyf.chenzaomai.com

—— 文件结束 ——
来源：http://hfz.cqqwz.cn

================================================================================
来源：http://foc.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://ati.cucudq.cn

Common Programming Examples Cheat Book
来源：http://poz.uphjek.com

================================================================================
来源：http://qyt.chenjidiqi.icu

【收录内容】
来源：http://wuv.yvedp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tvh.cucudq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kcu.bbcook.cn

SQL · Bash · C · C++
来源：http://lor.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qnx.hongshengwenyu.top

【使用说明】
来源：http://wzm.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://new.jqgfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fad.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jdb.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dlb.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://zwm.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ssc.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nry.tarul.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kdd.nwbrower.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://col.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iet.hcnkem.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cdy.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zrn.chenjidiqi.icu

【文件统计】
来源：http://mtv.c1oappe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cks.shuidangran.top

--------------------------------------------------------------------------------
来源：http://bjc.tanke756.top

目  录
来源：http://mwd.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://ejn.pycfn.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://isu.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yxn.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qkh.ydjk.org.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rls.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uem.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dvg.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nqq.shuidangran.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ici.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iqq.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fov.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qmn.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ixp.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://abp.zycfv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aef.ybcxt.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://muw.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://duh.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hux.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wxd.xingfuxueyuan.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nne.ivvv.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mpo.hnqzz.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sfd.ydjk.org.cn

================================================================================
来源：http://hgh.xziqi.cn

A. 基础语法与类型
来源：http://gis.daria6918.cn

================================================================================
来源：http://iil.hysaishi.cn

[A01] Hello World
来源：http://hhj.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://fzk.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://yus.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://mcm.vqdsnc.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iwb.zhijiandao.cn

Java: System.out.println("Hello, World!");
来源：http://fmi.hfpthk.cn

Go:   fmt.Println("Hello, World!")
来源：http://mlc.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://aqd.hysaishi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ewd.hnxiangtu.top

[A02] 变量声明与赋值
来源：http://rkt.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tsp.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wja.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://hmb.gogol.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vye.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://dof.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://ybh.shanyushiyangtech.top

Ruby: name = "Alex"; age = 20
来源：http://xei.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://azr.sweek.top

[A03] 常量定义
来源：http://owb.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rqh.ivvv.top

PHP:  const PI = 3.14159;
来源：http://nhg.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://acx.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://ihh.wangdashe.top

Java: static final double PI = 3.14159;
来源：http://cez.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://iev.fzhhl.top

Ruby: PI = 3.14159
来源：http://mox.cheryme.top

C#:   const double PI = 3.14159;
来源：http://zvh.jyoumei.cn

[A04] 判断变量类型
来源：http://bgd.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://txe.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gfd.svipenyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vkq.ivvv.top

TS:   typeof x; x instanceof Date
来源：http://udz.ywan-chungtsiang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nvu.zdbjq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://glk.cucudq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://swa.jinyuanbaomall.cn

C#:   x.GetType().Name; x is int
来源：http://jdl.jiagoushi.top

[A05] 整数除法与取模
来源：http://kvs.shanyushiyangkeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wkc.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pji.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hss.cqqwz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://and.fzhhl.top

Java: 7 / 2; 7 % 2
来源：http://ykz.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://umn.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://pmg.tanke756.top

C#:   7 / 2; 7 % 2
来源：http://vsl.uphjek.com

[A06] 字符串转数字
来源：http://tcs.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://vpm.c1oappe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sxi.sufxvd.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yog.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://gtd.gaohongyu789.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vzf.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xlj.xylfe.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pkg.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dti.yj20258.top

[A07] 数字转字符串
来源：http://rhi.yj20258.top

Py:   str(42)
来源：http://dco.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://zou.zhengqikj.top

JS:   String(42); (42).toString()
来源：http://zgs.zdqjudy.top

TS:   String(42)
来源：http://kef.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bzd.hammf.cn

Go:   strconv.Itoa(42)
来源：http://sed.kuanghao11.cn

Ruby: 42.to_s
来源：http://nmv.shzxlz.cn

C#:   42.ToString()
来源：http://dfb.haohaochexian.top

[A08] 取整与四舍五入
来源：http://zkv.zhongyouzk.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wvx.gogol.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hjc.hesvh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ngj.zhoulong.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pvs.yuanzhike.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tlb.sjlbkw.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qsi.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://psb.hongshengwenyu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dpf.ydjk.org.cn

[A09] 绝对值与最大最小值
来源：http://eaq.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://igp.xinyue.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://phd.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ntl.tian-w.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lep.0kj1m.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://noe.jqgufenzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hgu.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qds.quarkkingdee.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hhk.gaohongyu789.top

[A10] 生成随机数
来源：http://mcb.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://wwo.yfazqb.com

PHP:  random_int(1, 100);
来源：http://yvo.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wvo.smart0.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hwk.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://zah.daria6918.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ezo.ppjwa.cn

Ruby: rand(1..100)
来源：http://kyw.zhiwuduotai.top

C#:   new Random().Next(1, 101)
来源：http://xwg.yj20258.top

[A11] 条件表达式（三元）
来源：http://ydv.xziqi.cn

Py:   "yes" if x > 0 else "no"
来源：http://zqn.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hbk.bbcook.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qsq.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mgd.meibo888.top

Java: x > 0 ? "yes" : "no"
来源：http://rmw.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://com.fehbvm.com

Ruby: x > 0 ? "yes" : "no"
来源：http://vcj.yfazqb.com

C#:   x > 0 ? "yes" : "no"
来源：http://xep.yj20258888.top

[A12] 字符串插值 / 格式化
来源：http://ivr.shzxlz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ygf.yonumen.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xwv.quarkkingdee.top

JS:   `Hello, ${name}!`
来源：http://xvl.xziqi.cn

TS:   `Hello, ${name}!`
来源：http://ogi.kuanghao11.cn

Java: "Hello, %s!".formatted(name)
来源：http://bxm.cheryme.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cxu.ybcxt.top

Ruby: "Hello, #{name}!"
来源：http://pua.yonumen.top

C#:   $"Hello, {name}!"
来源：http://jcs.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vgl.guowangkeji.top

Py:   "第一行\n第二行"
来源：http://zwg.vqdsnc.cn

PHP:  "第一行\n第二行"
来源：http://yxm.9152youxi.cn

JS:   "第一行\n第二行"
来源：http://nou.zhoulong.xyz

TS:   "第一行\n第二行"
来源：http://fkb.sweek.top

Java: "第一行\n第二行"
来源：http://obx.yvedp.cn

Go:   "第一行\n第二行"
来源：http://vda.hongshengwenyu.top

Ruby: "第一行\n第二行"
来源：http://pkb.tian-w.cn

C#:   "第一行\n第二行"
来源：http://unj.vqdsnc.cn

[A14] 注释写法
来源：http://uft.9152youxi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jlm.cucudq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xel.jlsjyb.cn

JS:   // 单行；/* 多行 */
来源：http://rer.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://ofv.yfazqb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tpb.hnqzz.top

Go:   // 单行；/* 多行 */
来源：http://hup.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lom.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://hwi.fehbvm.com

[A15] 空值判断与默认值
来源：http://epq.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://wcp.jqgufenzy.top

PHP:  $value = $data ?? "默认值";
来源：http://ixc.ywan-chungtsiang.top


<!-- 参考信息 -->