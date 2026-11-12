代发 wailian999

[U85] JS：可选链
来源：http://hqd.jqgfzy.top

a?.b?.c
来源：http://dkp.feifeiyinyue.top

[U86] JS：空值合并
来源：http://uxz.fanxiaobao.xyz

a ?? b
来源：http://nif.daxiang520.top

[U87] JS：解构默认值
来源：http://ijm.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://lxu.yvedp.cn

[U88] JS：对象展开合并
来源：http://mzt.sxryk.cn

{ ...a, ...b }
来源：http://wsh.epnwcf.com

[U89] JS：数组去重
来源：http://jfi.quarkkingdee.top

[...new Set(arr)]
来源：http://kjy.yj20258.top

[U90] JS：数字数组排序
来源：http://rhs.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://kno.fzhhl.top

[U91] JS：对象键值遍历
来源：http://iui.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://woj.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://gdl.hcnkem.com

structuredClone(obj)
来源：http://qsn.havefunace.top

[U93] JS：模板字符串
来源：http://jid.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://ufj.hnxiangtu.top

[U94] JS：箭头函数
来源：http://oml.xziqi.cn

const double = x => x * 2;
来源：http://byq.dianchejie.cn

[U95] JS：Promise 包装
来源：http://iai.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://hmq.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://nty.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qzb.jinqigufen.top

[U97] JS：并发请求
来源：http://iod.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vms.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://fgo.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nkh.ydzc1.top

[U99] JS：事件监听
来源：http://qsw.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://wqz.jyoumei.cn

[U100] JS：DOM 查询
来源：http://ilg.sjlbkw.cn

document.querySelector(".item")
来源：http://cfw.xylfe.cn

[U101] JS：classList 操作
来源：http://gfc.zhijiandao.cn

el.classList.toggle("active")
来源：http://cus.zhijiandao.cn

[U102] JS：本地存储
来源：http://rso.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ziz.feifeiyinyue.top

[U103] JS：定时器
来源：http://dmk.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kpy.guowangkeji.top

[U104] JS：防抖
来源：http://cxy.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hgl.bbcook.cn

[U105] JS：节流
来源：http://jwr.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wfw.zhixingplan.top

[U106] JS：日期格式化
来源：http://pvx.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://whc.fzhhl.top

[U107] JS：数字千分位
来源：http://fie.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bha.ydzc1.top

[U108] JS：随机整数
来源：http://okf.sjlbkw.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eyj.cashguo.top

[U109] JS：数组分组
来源：http://nkv.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://hfz.chenzaomai.com

[U110] JS：数组分块
来源：http://ata.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oxf.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://bpe.yj20258888.top

new Map(Object.entries(obj))
来源：http://nsw.zdbjq.cn

[U112] JS：字符串补位
来源：http://hzv.hcnkem.com

"7".padStart(3, "0")
来源：http://fgs.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://pnb.cdnleiting.top

s.replaceAll("a", "b")
来源：http://zog.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://szx.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sjh.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://hng.jqgfzy.top

crypto.randomUUID()
来源：http://oif.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://ymf.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://lme.shanyushiyangtech.top

[U117] JS：单元测试
来源：http://goh.yj20258.top

npm i -D vitest;  npx vitest
来源：http://xzd.jyoumei.cn

[U118] JS：开发服务器
来源：http://unh.yj20258.top

npm i -D vite;  npx vite
来源：http://czx.zhixingplan.top

[U119] JS：生产构建
来源：http://int.pycfn.com

npx vite build
来源：http://bbn.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://anv.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://bsq.shanyushiyangkeji.top

================================================================================
来源：http://hxh.zdqjudy.top

统计汇总
来源：http://sht.hcnkem.com

================================================================================
来源：http://qpv.tianlin.xyz

按语言统计（条）：
来源：http://evy.zhongyouzk.top

Python ......... 252
来源：http://hrd.ywan-chungtsiang.top

PHP ............ 252
来源：http://lgs.iojbl.cn

JavaScript ..... 252
来源：http://tuk.cashguo.top

TypeScript ..... 212
来源：http://vla.jianghu66.top

Java ........... 212
来源：http://faj.ivvv.top

Go ............. 212
来源：http://wvu.chenzaomai.com

Ruby ........... 212
来源：http://toa.jyoumei.cn

C# ............. 212
来源：http://rhl.ivvv.top

C .............. 30
来源：http://kyp.gotoacloud.top

C++ ............ 30
来源：http://xog.shzxlz.cn

SQL ............ 90
来源：http://yfv.cdnleiting.top

Bash ........... 80
来源：http://ltv.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://dzw.jqgfzy.top

Swift .......... 15
来源：http://din.xuetiantiany.cn

Lua ............ 10
来源：http://jcv.fengsongda.top

Perl ........... 10
来源：http://hkz.tian-w.cn

Scala .......... 10
来源：http://kwe.yfazqb.com

------------------------------------
来源：http://zmy.yfazqb.com

合计 ........... 2106 条
来源：http://kfr.jinqigfzy.top

按章节统计：
来源：http://ulr.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qhv.chenlongwang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aoh.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://deu.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kla.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oju.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xml.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sqp.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uif.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kjo.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wqv.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://khc.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vvg.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jqe.nwbrower.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mru.9152youxi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gir.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://klj.guannengcc.top

Q SQL 专题                              90
来源：http://iaj.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://gvw.jianghu66.top

S C / C++ 专题                          60
来源：http://ona.0kj1m.cn

T 其他语言补充                          60
来源：http://dxt.yueranfly.top

U 高频实用片段                         120
来源：http://fwr.cheryme.top

------------------------------------
来源：http://eyr.hywenlv.cn

合计                                  2106 条
来源：http://xgz.birdmap.top

--------------------------------------------------------------------------------
来源：http://tfp.svipenyu.cn

使用提醒
来源：http://gan.cucudq.cn

--------------------------------------------------------------------------------
来源：http://vdf.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ife.jlsjyb.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iwh.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://umx.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gti.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gyy.tian-w.cn

—— 文件结束 ——
来源：http://oem.sufxvd.cn

================================================================================
来源：http://wdr.hywenlv.cn

程序语言常见例子速查手册（2024 版）
来源：http://mvv.yfazqb.com

Common Programming Examples Cheat Book
来源：http://cuu.fengsongda.top

================================================================================
来源：http://mdi.yj20258888.top

【收录内容】
来源：http://qgt.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cpf.gotoacloud.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hdh.yvedp.cn

SQL · Bash · C · C++
来源：http://whf.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wfe.jqgufenzy.top

【使用说明】
来源：http://eah.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sqd.c1oappe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://msz.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ujg.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uko.chenlongwang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jnp.zhiwuduotai.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zqe.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pjl.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wyy.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://axx.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fmw.316326.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bmf.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://upy.zhixingplan.top

【文件统计】
来源：http://xvg.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cra.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://gfe.vqdsnc.cn

目  录
来源：http://azg.tarul.cn

--------------------------------------------------------------------------------
来源：http://vra.nanxuanxn.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kvc.yangfankeji.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wlv.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bmk.chenjidiqi.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lbo.yonumen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hfg.0kj1m.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hph.ehwqpu.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://taz.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tgn.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ave.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://myq.yueranfly.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ukt.zhaomingkeji.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dol.jinqigufen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://apg.jinyuanbaomall.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aim.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://duy.hcnkem.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bax.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xpm.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rzc.52xcode.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cqq.yonumen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ito.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ovf.0kj1m.cn

================================================================================
来源：http://erm.pycfn.com

A. 基础语法与类型
来源：http://dup.sxryk.cn

================================================================================
来源：http://ywp.hnqzz.top

[A01] Hello World
来源：http://oes.0kj1m.cn

Py:   print("Hello, World!")
来源：http://zio.bjfxy.top

PHP:  echo "Hello, World!";
来源：http://wuu.yuanzhike.top

JS:   console.log("Hello, World!");
来源：http://eko.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jkp.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://anb.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://jdf.316326.xyz

Ruby: puts "Hello, World!"
来源：http://shb.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://hfx.yj20258888.top

[A02] 变量声明与赋值
来源：http://okz.jyoumei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rpy.meibo888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ehx.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://nny.ivvv.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://stc.zhaomingkeji.xyz

Java: String name = "Alex"; int age = 20;
来源：http://cnt.hcnkem.com

Go:   name := "Alex"; age := 20
来源：http://oit.mhx1999.top

Ruby: name = "Alex"; age = 20
来源：http://auw.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://zxq.ydjk.org.cn

[A03] 常量定义
来源：http://jtl.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tty.jlsjyb.cn

PHP:  const PI = 3.14159;
来源：http://jou.jianghu66.top

JS:   const PI = 3.14159;
来源：http://qer.yueranfly.top

TS:   const PI: number = 3.14159;
来源：http://shu.smart0.xyz

Java: static final double PI = 3.14159;
来源：http://pyh.aizwys.cn

Go:   const PI = 3.14159
来源：http://irz.ctjpmb.com

Ruby: PI = 3.14159
来源：http://mxy.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://adx.aizwys.cn

[A04] 判断变量类型
来源：http://jyj.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rcy.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yjj.chenzaomai.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zjf.andypj.xyz

TS:   typeof x; x instanceof Date
来源：http://tbl.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lrt.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://mgd.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hgg.aibaodan.cn

C#:   x.GetType().Name; x is int
来源：http://llu.cashguo.top

[A05] 整数除法与取模
来源：http://jyc.yanxiufei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ilh.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dkf.zycfv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ppi.shanyushiyangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bnt.sweek.top

Java: 7 / 2; 7 % 2
来源：http://usb.yj202588.top

Go:   7 / 2; 7 % 2
来源：http://xgw.cdnleiting.top

Ruby: 7 / 2; 7 % 2
来源：http://nnn.chenjidiqi.icu

C#:   7 / 2; 7 % 2
来源：http://vgc.pengpengdd.cyou

[A06] 字符串转数字
来源：http://cio.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://mnf.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gwt.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zdc.fzhhl.top

TS:   parseInt("42", 10); Number("42")
来源：http://ovc.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fyw.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jgj.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://ndd.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tvd.9152youxi.cn

[A07] 数字转字符串
来源：http://ypu.zhiwuduotai.top

Py:   str(42)
来源：http://jxb.0kj1m.cn

PHP:  (string) 42; strval(42)
来源：http://neh.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://hgm.iojbl.cn

TS:   String(42)
来源：http://rmv.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://sst.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://urm.hywenlv.cn

Ruby: 42.to_s
来源：http://ero.cucudq.cn

C#:   42.ToString()
来源：http://ten.bjfxy.top

[A08] 取整与四舍五入
来源：http://ldt.hesvh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zuc.xingfuxueyuan.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ppm.zdbjq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cvw.ctjpmb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ips.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kck.xingfuxueyuan.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zzz.fengsongda.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cbz.ehwqpu.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lzi.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://nfo.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vry.ehwqpu.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ydm.fengsongda.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iqo.jinqigufen.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uqd.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://txb.yuanzhike.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cmb.fengsongda.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dds.quarkkingdee.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://stm.yongpay.top

[A10] 生成随机数
来源：http://tnv.hammf.cn

Py:   import random; random.randint(1, 100)
来源：http://qby.chenlongwang.top

PHP:  random_int(1, 100);
来源：http://dxa.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wyx.52xcode.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cfh.ehwqpu.com

Java: new Random().nextInt(100) + 1
来源：http://eep.yangfankeji.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ugo.smart0.xyz

Ruby: rand(1..100)
来源：http://bth.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://uzj.hcnkem.com

[A11] 条件表达式（三元）
来源：http://vlr.shuidangran.top

Py:   "yes" if x > 0 else "no"
来源：http://keo.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://voy.jianghu66.top

JS:   x > 0 ? "yes" : "no"
来源：http://jzc.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://vok.fengsongda.top

Java: x > 0 ? "yes" : "no"
来源：http://bnt.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gvq.andypj.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://oxl.guowangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://vnh.chenjidiqi.icu

[A12] 字符串插值 / 格式化
来源：http://nyh.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://erh.yvedp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uhl.ivvv.top

JS:   `Hello, ${name}!`
来源：http://zkg.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://hmy.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://mgn.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bzi.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://wbx.jinyuanbaomall.cn

C#:   $"Hello, {name}!"
来源：http://axa.epnwcf.com

[A13] 多行字符串（练习 \n 转义）
来源：http://opb.yj202588.top

Py:   "第一行\n第二行"
来源：http://gul.fengsongda.top

PHP:  "第一行\n第二行"
来源：http://xlu.yj20258.top

JS:   "第一行\n第二行"
来源：http://qfb.xinyue.icu

TS:   "第一行\n第二行"
来源：http://pdx.xinyue.icu

Java: "第一行\n第二行"
来源：http://czl.cucudq.cn

Go:   "第一行\n第二行"
来源：http://mwe.ydjk.org.cn

Ruby: "第一行\n第二行"
来源：http://nfr.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://kdg.0kj1m.cn

[A14] 注释写法
来源：http://nmq.hysaishi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bvv.yuanzhike.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ufa.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://rws.yj20258.top


<!-- 参考信息 -->