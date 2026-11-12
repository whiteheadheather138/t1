代发 wailian999

[U87] JS：解构默认值
来源：http://uoj.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://iwg.guannengcc.top

[U88] JS：对象展开合并
来源：http://wkj.tianlin.xyz

{ ...a, ...b }
来源：http://abt.zhiwuduotai.top

[U89] JS：数组去重
来源：http://ktt.jinqigfzy.top

[...new Set(arr)]
来源：http://rvt.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://mxa.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://uvj.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://nue.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://omj.zhijiandao.cn

[U92] JS：深拷贝
来源：http://ufl.daria6918.cn

structuredClone(obj)
来源：http://dbw.ivvv.top

[U93] JS：模板字符串
来源：http://nsb.mhx1999.top

`共 ${n} 条`
来源：http://lww.ydjk.org.cn

[U94] JS：箭头函数
来源：http://gpu.uphjek.com

const double = x => x * 2;
来源：http://ccp.yfazqb.com

[U95] JS：Promise 包装
来源：http://qks.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://koi.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://ykh.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tre.yuxming.cn

[U97] JS：并发请求
来源：http://ldl.hnqzz.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hmr.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://dbm.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ltx.hywenlv.cn

[U99] JS：事件监听
来源：http://ktq.bbcook.cn

el.addEventListener("click", e => {})
来源：http://bff.havefunace.top

[U100] JS：DOM 查询
来源：http://sdv.xinyue.icu

document.querySelector(".item")
来源：http://fwc.jinqigfzy.top

[U101] JS：classList 操作
来源：http://aoy.svipenyu.cn

el.classList.toggle("active")
来源：http://jba.ydzc1.top

[U102] JS：本地存储
来源：http://qdl.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zup.9152youxi.cn

[U103] JS：定时器
来源：http://dmp.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://spx.sufxvd.cn

[U104] JS：防抖
来源：http://awr.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nie.fehbvm.com

[U105] JS：节流
来源：http://ihi.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lhj.yj20258.top

[U106] JS：日期格式化
来源：http://urj.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yiy.hesvh.cn

[U107] JS：数字千分位
来源：http://ynq.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rkd.sysykeji.top

[U108] JS：随机整数
来源：http://fmg.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yqs.0kj1m.cn

[U109] JS：数组分组
来源：http://got.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://drt.xziqi.cn

[U110] JS：数组分块
来源：http://gct.gogol.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://crk.iojbl.cn

[U111] JS：对象转 Map
来源：http://unv.guowangkeji.top

new Map(Object.entries(obj))
来源：http://vzm.dashuyun.cn

[U112] JS：字符串补位
来源：http://hcr.aizwys.cn

"7".padStart(3, "0")
来源：http://wad.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://pmx.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://zbf.dianchejie.cn

[U114] JS：JSON 深比较
来源：http://ehk.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ayo.jinghuilouyu.cn

[U115] JS：生成 UUID
来源：http://psn.fengsongda.top

crypto.randomUUID()
来源：http://dup.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://hjv.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://dsx.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://xyt.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://lda.jianghu66.top

[U118] JS：开发服务器
来源：http://vil.ivvv.top

npm i -D vite;  npx vite
来源：http://qhf.haohaochexian.top

[U119] JS：生产构建
来源：http://pai.zhiwuduotai.top

npx vite build
来源：http://pkn.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://grm.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://tug.daria6918.cn

================================================================================
来源：http://rtn.316326.xyz

统计汇总
来源：http://htb.jianghu66.top

================================================================================
来源：http://lxy.yvedp.cn

按语言统计（条）：
来源：http://dvx.yj202588.top

Python ......... 252
来源：http://ubq.jianghu66.top

PHP ............ 252
来源：http://fpl.jianghu66.top

JavaScript ..... 252
来源：http://srm.hnqzz.top

TypeScript ..... 212
来源：http://rrr.yonumen.top

Java ........... 212
来源：http://irz.hongshengwenyu.top

Go ............. 212
来源：http://zdh.bjfxy.top

Ruby ........... 212
来源：http://doe.sysykeji.top

C# ............. 212
来源：http://kmu.sysykeji.top

C .............. 30
来源：http://nnu.guowangkeji.top

C++ ............ 30
来源：http://vfb.yvedp.cn

SQL ............ 90
来源：http://jgz.yanxiufei.cn

Bash ........... 80
来源：http://qvv.epnwcf.com

Kotlin ......... 15
来源：http://hus.xuanzx.com

Swift .......... 15
来源：http://eng.daxiang520.top

Lua ............ 10
来源：http://qsy.jianghu66.top

Perl ........... 10
来源：http://fqg.xuanzx.com

Scala .......... 10
来源：http://iug.shangyingyoupin.top

------------------------------------
来源：http://fjn.cdnleiting.top

合计 ........... 2106 条
来源：http://sxy.ybcxt.top

按章节统计：
来源：http://wpo.jinghuilouyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mgf.chenlongwang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ruz.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vfo.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hpg.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hkc.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rbz.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zmy.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jeg.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qtk.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ius.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://usb.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vpg.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fku.zhiwuduotai.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fjk.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gzs.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pwb.jiagoushi.top

Q SQL 专题                              90
来源：http://vsp.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://kvm.zhixingplan.top

S C / C++ 专题                          60
来源：http://zdv.ydzc1.top

T 其他语言补充                          60
来源：http://hhm.pengpengdd.cyou

U 高频实用片段                         120
来源：http://vzw.daria6918.cn

------------------------------------
来源：http://gxh.gzhubu.top

合计                                  2106 条
来源：http://fat.cheryme.top

--------------------------------------------------------------------------------
来源：http://ohi.shuidangran.top

使用提醒
来源：http://ues.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://suc.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rrt.hammf.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mpx.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://szo.quarkkingdee.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sbp.sweek.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://djr.yfazqb.com

—— 文件结束 ——
来源：http://xla.ehwqpu.com

================================================================================
来源：http://epx.bjfxy.top

程序语言常见例子速查手册（2024 版）
来源：http://inj.bbcook.cn

Common Programming Examples Cheat Book
来源：http://bpj.pycfn.com

================================================================================
来源：http://dae.hnqzz.top

【收录内容】
来源：http://tgf.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ezm.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://imb.xuanzx.com

SQL · Bash · C · C++
来源：http://vcu.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uur.kuanghao11.cn

【使用说明】
来源：http://rsu.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ehh.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hne.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pfd.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tiu.jinqigufen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jml.zdqjudy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tck.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://clw.gaohongyu789.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ncp.c1oappe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://esg.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zda.uphjek.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mbx.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zkw.chenjidiqi.icu

【文件统计】
来源：http://quz.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mbs.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://ybr.shangyingyoupin.top

目  录
来源：http://qob.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://zzj.yj202588.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://knb.pycfn.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kdo.yj20258888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xfj.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dzr.hfpthk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qod.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://azr.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lhn.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rei.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://inp.mhx1999.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pvm.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aop.gaohongyu789.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kgy.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://edw.9152youxi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jda.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qou.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ztn.svipenyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ujb.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zvr.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dzz.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tcp.hongshengwenyu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zia.zhengqikj.top

================================================================================
来源：http://psp.gogol.net.cn

A. 基础语法与类型
来源：http://ekn.shangyingyoupin.top

================================================================================
来源：http://mkp.ctjpmb.com

[A01] Hello World
来源：http://bsc.bjfxy.top

Py:   print("Hello, World!")
来源：http://eay.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://zyp.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://lnv.pengpengdd.cyou

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wcm.vehdjk.com

Java: System.out.println("Hello, World!");
来源：http://vkc.ywan-chungtsiang.top

Go:   fmt.Println("Hello, World!")
来源：http://ivw.yj202588.top

Ruby: puts "Hello, World!"
来源：http://uml.hcnkem.com

C#:   Console.WriteLine("Hello, World!");
来源：http://krw.hywenlv.cn

[A02] 变量声明与赋值
来源：http://mzm.snrcjt.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lhz.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oep.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://tvm.sweek.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mik.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://ypk.yuxming.cn

Go:   name := "Alex"; age := 20
来源：http://eao.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://lnx.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://chz.hongshengwenyu.top

[A03] 常量定义
来源：http://hba.jqgufenzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mmy.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://myw.yj20258888.top

JS:   const PI = 3.14159;
来源：http://hqo.redwolf501.top

TS:   const PI: number = 3.14159;
来源：http://iyz.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://fmw.gotoacloud.top

Go:   const PI = 3.14159
来源：http://qgj.yonumen.top

Ruby: PI = 3.14159
来源：http://baj.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://tlg.jiagoushi.top

[A04] 判断变量类型
来源：http://riw.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ocy.zdbjq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nsx.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xye.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://amz.hysaishi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bri.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://jps.hywenlv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pig.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://gxa.cheryme.top

[A05] 整数除法与取模
来源：http://thw.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hme.jlsjyb.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gyw.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bez.shanyushiyangtech.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qjw.andypj.xyz

Java: 7 / 2; 7 % 2
来源：http://ait.hnqzz.top

Go:   7 / 2; 7 % 2
来源：http://yhr.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://jcv.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://qtk.shzxlz.cn

[A06] 字符串转数字
来源：http://ujo.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://uyn.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ivg.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://csy.kuanghao11.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pip.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lbk.jiagoushi.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lqa.jinyuanbaomall.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bmf.316326.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ahb.sufxvd.cn

[A07] 数字转字符串
来源：http://mpw.xingfuxueyuan.xyz

Py:   str(42)
来源：http://ejr.shanyushiyangkeji.top

PHP:  (string) 42; strval(42)
来源：http://prk.tian-w.cn

JS:   String(42); (42).toString()
来源：http://rmg.316326.xyz

TS:   String(42)
来源：http://qbl.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pdq.shanyushiyangkeji.top

Go:   strconv.Itoa(42)
来源：http://iac.vehdjk.com

Ruby: 42.to_s
来源：http://jkl.yuanzhike.top

C#:   42.ToString()
来源：http://cqx.hywenlv.cn

[A08] 取整与四舍五入
来源：http://zvb.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vue.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mpk.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vuc.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jec.smart0.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://plr.ywan-chungtsiang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xbl.jinqigufen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gcr.ybcxt.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fzo.xylfe.cn

[A09] 绝对值与最大最小值
来源：http://xfm.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xay.pycfn.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ajj.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sex.zycfv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wlb.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cds.ppjwa.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aow.c1oappe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qgw.cheryme.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hdi.ywan-chungtsiang.top

[A10] 生成随机数
来源：http://omy.pycfn.com

Py:   import random; random.randint(1, 100)
来源：http://wqh.shanyushiyangtech.top

PHP:  random_int(1, 100);
来源：http://rqc.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wjs.cdnleiting.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jnj.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://mpg.gogol.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://loo.cucudq.cn

Ruby: rand(1..100)
来源：http://zae.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://pzc.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://ade.hcnkem.com

Py:   "yes" if x > 0 else "no"
来源：http://ise.fktsv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pjm.zycfv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://aqw.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rkm.yj20258888.top

Java: x > 0 ? "yes" : "no"
来源：http://gju.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://njj.c1oappe.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tbm.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://dnc.tian-w.cn

[A12] 字符串插值 / 格式化
来源：http://aey.yuxming.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bhk.zycfv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cqz.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://ltx.shanyushiyangkeji.top

TS:   `Hello, ${name}!`
来源：http://bpt.daria6918.cn

Java: "Hello, %s!".formatted(name)
来源：http://iab.jinqigfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xdn.zhaomingkeji.xyz

Ruby: "Hello, #{name}!"
来源：http://kky.9152youxi.cn

C#:   $"Hello, {name}!"
来源：http://sxc.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://chk.snrcjt.cn

Py:   "第一行\n第二行"
来源：http://kfx.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://jva.kuanghao11.cn

JS:   "第一行\n第二行"
来源：http://wfx.gzhubu.top

TS:   "第一行\n第二行"
来源：http://twz.xziqi.cn

Java: "第一行\n第二行"
来源：http://ogo.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://ksf.vehdjk.com

Ruby: "第一行\n第二行"
来源：http://cnc.sjlbkw.cn

C#:   "第一行\n第二行"
来源：http://sbv.jinqigufen.top

[A14] 注释写法
来源：http://fas.gogol.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://waz.sjlbkw.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oxl.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://buy.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://jod.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cai.wangshuangyany.cn

Go:   // 单行；/* 多行 */
来源：http://sth.kuanghao11.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nzr.sufxvd.cn


<!-- 参考信息 -->