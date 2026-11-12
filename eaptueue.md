代发 wailian999

[U87] JS：解构默认值
来源：http://efo.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://wic.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://sho.aibaodan.cn

{ ...a, ...b }
来源：http://iki.tanke756.top

[U89] JS：数组去重
来源：http://vwp.redwolf501.top

[...new Set(arr)]
来源：http://wql.zhixingplan.top

[U90] JS：数字数组排序
来源：http://emw.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://eio.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://eky.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gbh.bjfxy.top

[U92] JS：深拷贝
来源：http://lsx.fzhhl.top

structuredClone(obj)
来源：http://stc.jinqigfzy.top

[U93] JS：模板字符串
来源：http://fwc.svipenyu.cn

`共 ${n} 条`
来源：http://umn.yongpay.top

[U94] JS：箭头函数
来源：http://vit.dianchejie.cn

const double = x => x * 2;
来源：http://soi.xziqi.cn

[U95] JS：Promise 包装
来源：http://aih.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://oqu.pycfn.com

[U96] JS：async/await 与异常
来源：http://krb.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ths.fanxiaobao.xyz

[U97] JS：并发请求
来源：http://mts.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pos.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://xzc.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rdm.snrcjt.cn

[U99] JS：事件监听
来源：http://yip.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://bqu.c1oappe.top

[U100] JS：DOM 查询
来源：http://tdb.sjlbkw.cn

document.querySelector(".item")
来源：http://skp.gotoacloud.top

[U101] JS：classList 操作
来源：http://ayp.redwolf501.top

el.classList.toggle("active")
来源：http://lov.tian-w.cn

[U102] JS：本地存储
来源：http://azy.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://joz.fehbvm.com

[U103] JS：定时器
来源：http://gct.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xym.zhixingplan.top

[U104] JS：防抖
来源：http://fjj.tarul.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hol.fzhhl.top

[U105] JS：节流
来源：http://wci.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vns.gogol.net.cn

[U106] JS：日期格式化
来源：http://cwd.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://unn.hfpthk.cn

[U107] JS：数字千分位
来源：http://lnz.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jkr.meibo888.top

[U108] JS：随机整数
来源：http://dac.fzhhl.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hzi.pycfn.com

[U109] JS：数组分组
来源：http://cud.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://rvy.sweek.top

[U110] JS：数组分块
来源：http://fzv.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lyn.cashguo.top

[U111] JS：对象转 Map
来源：http://oyn.chenzaomai.com

new Map(Object.entries(obj))
来源：http://pjf.yonumen.top

[U112] JS：字符串补位
来源：http://gio.fehbvm.com

"7".padStart(3, "0")
来源：http://jop.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://bpv.haohaochexian.top

s.replaceAll("a", "b")
来源：http://cmb.shuidangran.top

[U114] JS：JSON 深比较
来源：http://dcx.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vre.hysaishi.cn

[U115] JS：生成 UUID
来源：http://yex.yuxming.cn

crypto.randomUUID()
来源：http://ajd.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://xmq.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://nxn.xuetiantiany.cn

[U117] JS：单元测试
来源：http://luu.meibo888.top

npm i -D vitest;  npx vitest
来源：http://hni.yj202588.top

[U118] JS：开发服务器
来源：http://hlb.0kj1m.cn

npm i -D vite;  npx vite
来源：http://ahi.xinyue.icu

[U119] JS：生产构建
来源：http://gtt.jinghuilouyu.cn

npx vite build
来源：http://dvx.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://rtk.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://huf.xuetiantiany.cn

================================================================================
来源：http://uam.sjlbkw.cn

统计汇总
来源：http://miy.aizwys.cn

================================================================================
来源：http://qje.hnqzz.top

按语言统计（条）：
来源：http://gvz.hnqzz.top

Python ......... 252
来源：http://sew.shuidangran.top

PHP ............ 252
来源：http://kfd.quarkkingdee.top

JavaScript ..... 252
来源：http://jde.jianghu66.top

TypeScript ..... 212
来源：http://hfz.zhijiandao.cn

Java ........... 212
来源：http://eqx.aibaodan.cn

Go ............. 212
来源：http://bvp.yanxiufei.cn

Ruby ........... 212
来源：http://dmg.zhijiandao.cn

C# ............. 212
来源：http://tww.pycfn.com

C .............. 30
来源：http://kag.jlsjyb.cn

C++ ............ 30
来源：http://uke.ydzc1.top

SQL ............ 90
来源：http://ktb.fanxiaobao.xyz

Bash ........... 80
来源：http://qvi.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://cfu.ydjk.org.cn

Swift .......... 15
来源：http://rvz.yvedp.cn

Lua ............ 10
来源：http://jvp.jinqigufen.top

Perl ........... 10
来源：http://usd.mhx1999.top

Scala .......... 10
来源：http://zkz.cheryme.top

------------------------------------
来源：http://oph.yueranfly.top

合计 ........... 2106 条
来源：http://nnz.hongshengwenyu.top

按章节统计：
来源：http://tzy.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fac.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bgr.ydzc1.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ylh.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kxy.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ojr.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vnm.epnwcf.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vmb.jqgufenzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dax.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qtz.yuxming.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qug.yonumen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ple.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ikt.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ohn.birdmap.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fvk.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mwu.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qtt.shangyingyoupin.top

Q SQL 专题                              90
来源：http://mzx.feifeiyinyue.top

R Bash 专题                             80
来源：http://pmw.yvedp.cn

S C / C++ 专题                          60
来源：http://apn.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://ele.quarkkingdee.top

U 高频实用片段                         120
来源：http://phk.mhx1999.top

------------------------------------
来源：http://nfi.shuidangran.top

合计                                  2106 条
来源：http://qxe.wangdashe.top

--------------------------------------------------------------------------------
来源：http://bfy.yuanzhike.top

使用提醒
来源：http://gox.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://ilw.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://obp.xinyue.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vdz.zdqjudy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tad.cqqwz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xzv.yj20258.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rfv.ywan-chungtsiang.top

—— 文件结束 ——
来源：http://mvm.zhoulong.xyz

================================================================================
来源：http://bsw.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://uit.pycfn.com

Common Programming Examples Cheat Book
来源：http://hrx.redwolf501.top

================================================================================
来源：http://try.guannengcc.top

【收录内容】
来源：http://dmk.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://fmc.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://puu.aizwys.cn

SQL · Bash · C · C++
来源：http://xfx.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://but.zhijiandao.cn

【使用说明】
来源：http://hqo.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://swo.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yix.ydjk.org.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://avs.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gii.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://aes.jyoumei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baq.guowangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wnp.gzhubu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mcz.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yfk.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rcy.ydjk.org.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qnb.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ckx.gaohongyu789.top

【文件统计】
来源：http://hdv.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lxf.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://hrp.smart0.xyz

目  录
来源：http://yym.havefunace.top

--------------------------------------------------------------------------------
来源：http://fjd.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lxf.hammf.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cuj.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nda.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tqc.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cks.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qfn.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ash.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bpg.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://buh.ydzc1.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vmb.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ixg.jinyuanbaomall.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yko.sxryk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xhw.sxryk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fbt.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ryx.cashguo.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wwa.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zif.cashguo.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qud.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wjd.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhg.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://msg.jlsjyb.cn

================================================================================
来源：http://vob.316326.xyz

A. 基础语法与类型
来源：http://czx.hongshengwenyu.top

================================================================================
来源：http://rll.jinyuanbaomall.cn

[A01] Hello World
来源：http://rgn.ywan-chungtsiang.top

Py:   print("Hello, World!")
来源：http://iuf.dianchejie.cn

PHP:  echo "Hello, World!";
来源：http://yeb.xylfe.cn

JS:   console.log("Hello, World!");
来源：http://spk.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nsv.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://vvk.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://grb.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://qjm.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://drw.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://wog.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://afe.smart0.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://cer.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iiu.shanyushiyangtech.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bcu.fzhhl.top

Java: String name = "Alex"; int age = 20;
来源：http://lmk.bjfxy.top

Go:   name := "Alex"; age := 20
来源：http://clo.haohaochexian.top

Ruby: name = "Alex"; age = 20
来源：http://olo.gotoacloud.top

C#:   string name = "Alex"; int age = 20;
来源：http://uki.yanxiufei.cn

[A03] 常量定义
来源：http://tuw.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qgp.sweek.top

PHP:  const PI = 3.14159;
来源：http://pgb.hnqzz.top

JS:   const PI = 3.14159;
来源：http://rry.kuanghao11.cn

TS:   const PI: number = 3.14159;
来源：http://rvs.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://dcg.shangyingyoupin.top

Go:   const PI = 3.14159
来源：http://pgv.shanyushiyangkeji.top

Ruby: PI = 3.14159
来源：http://vcf.hysaishi.cn

C#:   const double PI = 3.14159;
来源：http://hqf.ydjk.org.cn

[A04] 判断变量类型
来源：http://oxg.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xcc.tian-w.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://olv.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fby.c1oappe.top

TS:   typeof x; x instanceof Date
来源：http://ksj.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cme.zhengqikj.top

Go:   reflect.TypeOf(x).Name()
来源：http://tdc.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://imn.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://ruk.mhx1999.top

[A05] 整数除法与取模
来源：http://ctp.yuanzhike.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://coi.52xcode.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ylc.jinqigufen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://urr.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zzn.zdbjq.cn

Java: 7 / 2; 7 % 2
来源：http://tjx.wangshuangyany.cn

Go:   7 / 2; 7 % 2
来源：http://irf.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://hdd.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://inu.epnwcf.com

[A06] 字符串转数字
来源：http://qxm.cdnleiting.top

Py:   int("42"); float("3.14")
来源：http://mfc.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vqb.hesvh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zef.bbcook.cn

TS:   parseInt("42", 10); Number("42")
来源：http://miv.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rtn.ehwqpu.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://snr.zhongyouzk.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hrt.cashguo.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rgq.andypj.xyz

[A07] 数字转字符串
来源：http://kkc.jyoumei.cn

Py:   str(42)
来源：http://wrh.cheryme.top

PHP:  (string) 42; strval(42)
来源：http://ist.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://iam.shanyushiyangtech.top

TS:   String(42)
来源：http://hjd.nanxuanxn.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vku.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://ndt.gotoacloud.top

Ruby: 42.to_s
来源：http://cod.sjlbkw.cn

C#:   42.ToString()
来源：http://omx.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://vgq.fzhhl.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://utg.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qha.gzhubu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ykl.chenzaomai.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://itf.jqgufenzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ssf.9152youxi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://odk.zdqjudy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://uay.quarkkingdee.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://acn.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://xmc.jinqigufen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wvb.fzhhl.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dxz.xuetiantiany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xwv.sufxvd.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hoi.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wxs.yuxming.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qjg.ctjpmb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ndw.aibaodan.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zeq.yuanzhike.top

[A10] 生成随机数
来源：http://rai.epnwcf.com

Py:   import random; random.randint(1, 100)
来源：http://ftl.yuxming.cn

PHP:  random_int(1, 100);
来源：http://wnf.xuetiantiany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://diq.fengsongda.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://htc.nanxuanxn.top

Java: new Random().nextInt(100) + 1
来源：http://xjt.zhongyouzk.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xvm.iojbl.cn

Ruby: rand(1..100)
来源：http://bbj.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://kue.jlsjyb.cn

[A11] 条件表达式（三元）
来源：http://mrw.yj20258888.top

Py:   "yes" if x > 0 else "no"
来源：http://fat.yonumen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qmj.quarkkingdee.top

JS:   x > 0 ? "yes" : "no"
来源：http://jxy.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vbz.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://bmx.pengpengdd.cyou

Go:   // 无三元运算符，需用 if 语句
来源：http://ndw.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ckn.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://bup.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://rlv.gaohongyu789.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cvd.guannengcc.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://clt.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://ggj.dashuyun.cn

TS:   `Hello, ${name}!`
来源：http://jqo.jinqigufen.top

Java: "Hello, %s!".formatted(name)
来源：http://pit.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wax.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://fah.havefunace.top

C#:   $"Hello, {name}!"
来源：http://ptz.vqdsnc.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://grh.yonumen.top

Py:   "第一行\n第二行"
来源：http://mwy.ehwqpu.com

PHP:  "第一行\n第二行"
来源：http://rqm.aizwys.cn

JS:   "第一行\n第二行"
来源：http://ymz.zhongyouzk.top

TS:   "第一行\n第二行"
来源：http://xcv.daria6918.cn

Java: "第一行\n第二行"
来源：http://bqu.andypj.xyz

Go:   "第一行\n第二行"
来源：http://ndo.xuanzx.com

Ruby: "第一行\n第二行"
来源：http://lhw.wangshuangyany.cn

C#:   "第一行\n第二行"
来源：http://ocq.vqdsnc.cn

[A14] 注释写法
来源：http://nog.yj202588.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dxb.yj20258888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kti.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://fqi.zhongyouzk.top

TS:   // 单行；/* 多行 */
来源：http://mrh.pycfn.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sxq.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://lzv.zdbjq.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xiv.cashguo.top


<!-- 参考信息 -->