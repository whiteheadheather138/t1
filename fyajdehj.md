代发 wailian999

[U91] JS：对象键值遍历
来源：http://wfk.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vyx.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://vbh.yfazqb.com

structuredClone(obj)
来源：http://yll.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://gbc.zhixingplan.top

`共 ${n} 条`
来源：http://qyu.hnqzz.top

[U94] JS：箭头函数
来源：http://kvz.zhengqikj.top

const double = x => x * 2;
来源：http://ldf.0kj1m.cn

[U95] JS：Promise 包装
来源：http://pzi.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://ijr.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://wpe.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sqi.fengsongda.top

[U97] JS：并发请求
来源：http://eli.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uon.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://cjb.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vmt.yj20258.top

[U99] JS：事件监听
来源：http://cwu.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://mjf.yuxming.cn

[U100] JS：DOM 查询
来源：http://jvg.cheryme.top

document.querySelector(".item")
来源：http://fom.jiagoushi.top

[U101] JS：classList 操作
来源：http://bpe.kuanghao11.cn

el.classList.toggle("active")
来源：http://jzv.yonumen.top

[U102] JS：本地存储
来源：http://rhb.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://msz.chenlongwang.top

[U103] JS：定时器
来源：http://gfh.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xcb.gaohongyu789.top

[U104] JS：防抖
来源：http://mft.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nqu.gotoacloud.top

[U105] JS：节流
来源：http://slw.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dee.sxryk.cn

[U106] JS：日期格式化
来源：http://uul.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zgo.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://yuc.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cee.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://mes.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xiy.ctjpmb.com

[U109] JS：数组分组
来源：http://ixz.hnqzz.top

Object.groupBy(arr, x => x.type)
来源：http://vso.hesvh.cn

[U110] JS：数组分块
来源：http://xqp.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wgs.jianghu66.top

[U111] JS：对象转 Map
来源：http://hpf.zhengqikj.top

new Map(Object.entries(obj))
来源：http://tts.ivvv.top

[U112] JS：字符串补位
来源：http://cyi.epnwcf.com

"7".padStart(3, "0")
来源：http://jjy.xinyue.icu

[U113] JS：正则替换全部
来源：http://uqu.xuanzx.com

s.replaceAll("a", "b")
来源：http://fas.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://vkj.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uxv.tarul.cn

[U115] JS：生成 UUID
来源：http://rhb.yj20258.top

crypto.randomUUID()
来源：http://bwn.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://bqu.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://yoh.316326.xyz

[U117] JS：单元测试
来源：http://pwo.yj20258.top

npm i -D vitest;  npx vitest
来源：http://xci.vehdjk.com

[U118] JS：开发服务器
来源：http://blf.ehwqpu.com

npm i -D vite;  npx vite
来源：http://htb.yj20258.top

[U119] JS：生产构建
来源：http://vof.cashguo.top

npx vite build
来源：http://rvf.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://ogy.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://icu.chenlongwang.top

================================================================================
来源：http://odo.zhongyouzk.top

统计汇总
来源：http://grv.hesvh.cn

================================================================================
来源：http://uiw.hesvh.cn

按语言统计（条）：
来源：http://gfv.sjlbkw.cn

Python ......... 252
来源：http://piv.52xcode.cn

PHP ............ 252
来源：http://yal.andypj.xyz

JavaScript ..... 252
来源：http://sdr.vqdsnc.cn

TypeScript ..... 212
来源：http://akn.xinyue.icu

Java ........... 212
来源：http://sbk.gzhubu.top

Go ............. 212
来源：http://xsi.ivvv.top

Ruby ........... 212
来源：http://qpu.pycfn.com

C# ............. 212
来源：http://ivu.0kj1m.cn

C .............. 30
来源：http://sgi.mhx1999.top

C++ ............ 30
来源：http://ljw.gogol.net.cn

SQL ............ 90
来源：http://luz.kuanghao11.cn

Bash ........... 80
来源：http://urq.yuanzhike.top

Kotlin ......... 15
来源：http://znv.dashuyun.cn

Swift .......... 15
来源：http://ayd.gaohongyu789.top

Lua ............ 10
来源：http://iaa.havefunace.top

Perl ........... 10
来源：http://iuf.tian-w.cn

Scala .......... 10
来源：http://hbu.fehbvm.com

------------------------------------
来源：http://gym.jinqigfzy.top

合计 ........... 2106 条
来源：http://gyr.xziqi.cn

按章节统计：
来源：http://ids.hfpthk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wdk.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://spi.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vyg.xylfe.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://trw.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://skg.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kon.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oqy.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://feh.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://avf.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://krt.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oxu.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ujy.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://thh.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://heb.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://epl.pengpengdd.cyou

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://otv.ydjk.org.cn

Q SQL 专题                              90
来源：http://adn.yvedp.cn

R Bash 专题                             80
来源：http://ckb.hongshengwenyu.top

S C / C++ 专题                          60
来源：http://uvs.xuetiantiany.cn

T 其他语言补充                          60
来源：http://ocx.zhijiandao.cn

U 高频实用片段                         120
来源：http://kst.nanxuanxn.top

------------------------------------
来源：http://knn.nanxinkj.top

合计                                  2106 条
来源：http://qwj.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://ntk.fengsongda.top

使用提醒
来源：http://hqp.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://vqr.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jnl.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ele.nwbrower.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dce.dianchejie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bod.zdqjudy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ubx.shzxlz.cn

—— 文件结束 ——
来源：http://wef.gotoacloud.top

================================================================================
来源：http://gqo.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://bot.fktsv.cn

Common Programming Examples Cheat Book
来源：http://grr.yuxming.cn

================================================================================
来源：http://whf.xingfuxueyuan.xyz

【收录内容】
来源：http://ufl.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://poz.snrcjt.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cmq.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://nnu.svipenyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://log.shangyingyoupin.top

【使用说明】
来源：http://pzv.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://myh.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cow.fanxiaobao.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://awb.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gmf.shzxlz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xci.havefunace.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hha.havefunace.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hxe.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pjh.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dxg.yueranfly.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wfh.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kti.zhaomingkeji.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ruh.fengsongda.top

【文件统计】
来源：http://wgy.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xyu.vehdjk.com

--------------------------------------------------------------------------------
来源：http://tgz.yfazqb.com

目  录
来源：http://lnm.redwolf501.top

--------------------------------------------------------------------------------
来源：http://fub.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://agk.yonumen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sln.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fcz.hywenlv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lrr.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zjm.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oam.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lxo.zycfv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://haj.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fdu.cqqwz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sin.zhixingplan.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lvo.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zpy.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qyp.52xcode.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xzs.yfazqb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xud.dashuyun.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fqs.yuanzhike.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vlg.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://onq.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://riw.xziqi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nbz.chenjidiqi.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fzy.ehwqpu.com

================================================================================
来源：http://qgr.cdnleiting.top

A. 基础语法与类型
来源：http://fgv.tian-w.cn

================================================================================
来源：http://cgb.xuetiantiany.cn

[A01] Hello World
来源：http://xxc.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://woo.zycfv.cn

PHP:  echo "Hello, World!";
来源：http://hgv.yonumen.top

JS:   console.log("Hello, World!");
来源：http://rkj.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fxa.zhixingplan.top

Java: System.out.println("Hello, World!");
来源：http://zbc.yueranfly.top

Go:   fmt.Println("Hello, World!")
来源：http://wgg.andypj.xyz

Ruby: puts "Hello, World!"
来源：http://ayj.hysaishi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://evj.havefunace.top

[A02] 变量声明与赋值
来源：http://uul.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oeh.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zib.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://zkt.sxryk.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hmn.fzhhl.top

Java: String name = "Alex"; int age = 20;
来源：http://qxd.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://vok.wangdashe.top

Ruby: name = "Alex"; age = 20
来源：http://ghv.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://opz.sxryk.cn

[A03] 常量定义
来源：http://eun.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cic.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://sth.fanxiaobao.xyz

JS:   const PI = 3.14159;
来源：http://mil.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://esu.ppjwa.cn

Java: static final double PI = 3.14159;
来源：http://org.gotoacloud.top

Go:   const PI = 3.14159
来源：http://iun.bbcook.cn

Ruby: PI = 3.14159
来源：http://mbx.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://ylv.ydjk.org.cn

[A04] 判断变量类型
来源：http://jdm.sweek.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jxl.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lhf.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oqf.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://vqj.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ict.hysaishi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pzc.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://enp.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://nun.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://pin.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ocf.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bzp.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fmk.fehbvm.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oyu.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://qqw.cashguo.top

Go:   7 / 2; 7 % 2
来源：http://iyt.jqgufenzy.top

Ruby: 7 / 2; 7 % 2
来源：http://hdh.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://xct.jiagoushi.top

[A06] 字符串转数字
来源：http://jec.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://vkm.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hzy.smart0.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bjh.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://vut.ybcxt.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fiw.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dwq.zhoulong.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://vae.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tif.chenzaomai.com

[A07] 数字转字符串
来源：http://jzq.0kj1m.cn

Py:   str(42)
来源：http://cec.0kj1m.cn

PHP:  (string) 42; strval(42)
来源：http://qkr.jianghu66.top

JS:   String(42); (42).toString()
来源：http://vmu.shzxlz.cn

TS:   String(42)
来源：http://ife.gotoacloud.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pna.316326.xyz

Go:   strconv.Itoa(42)
来源：http://kni.sufxvd.cn

Ruby: 42.to_s
来源：http://ocd.smart0.xyz

C#:   42.ToString()
来源：http://yeo.svipenyu.cn

[A08] 取整与四舍五入
来源：http://fhr.yuxming.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://koy.smart0.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://izp.fktsv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bqs.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jow.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pie.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ucp.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qad.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://olg.shanyushiyangtech.top

[A09] 绝对值与最大最小值
来源：http://umg.ivvv.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uni.mhx1999.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://czv.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cxa.ywan-chungtsiang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nqs.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cst.tianlin.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ybu.zycfv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://enu.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ahy.birdmap.top

[A10] 生成随机数
来源：http://tye.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://vox.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://spm.jyoumei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qan.ywan-chungtsiang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://saa.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://ojq.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lmq.hysaishi.cn

Ruby: rand(1..100)
来源：http://bjl.fanxiaobao.xyz

C#:   new Random().Next(1, 101)
来源：http://qph.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://iwl.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://wct.daria6918.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zpy.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nzw.birdmap.top

TS:   x > 0 ? "yes" : "no"
来源：http://iys.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://isz.hfpthk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cfm.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://bey.yj20258888.top

C#:   x > 0 ? "yes" : "no"
来源：http://djd.redwolf501.top

[A12] 字符串插值 / 格式化
来源：http://qaw.gotoacloud.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tbl.yonumen.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wqs.hnqzz.top

JS:   `Hello, ${name}!`
来源：http://qci.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://kow.cdnleiting.top

Java: "Hello, %s!".formatted(name)
来源：http://ijv.hesvh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lah.yangfankeji.com

Ruby: "Hello, #{name}!"
来源：http://asv.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://lwi.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tjz.meibo888.top

Py:   "第一行\n第二行"
来源：http://uvx.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://sty.wangshuangyany.cn

JS:   "第一行\n第二行"
来源：http://iwi.ppjwa.cn

TS:   "第一行\n第二行"
来源：http://alk.xinyue.icu

Java: "第一行\n第二行"
来源：http://lqd.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://gqs.daxiang520.top

Ruby: "第一行\n第二行"
来源：http://zks.yonumen.top

C#:   "第一行\n第二行"
来源：http://ztz.zhixingplan.top

[A14] 注释写法
来源：http://cmm.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pss.xinyue.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://adf.ydjk.org.cn

JS:   // 单行；/* 多行 */
来源：http://uud.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://xzd.tarul.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://plp.tian-w.cn

Go:   // 单行；/* 多行 */
来源：http://lfn.dianchejie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tiy.kuanghao11.cn

C#:   // 单行；/* 多行 */
来源：http://ycr.xuanzx.com

[A15] 空值判断与默认值
来源：http://osn.shangyingyoupin.top

Py:   value = data or "默认值"
来源：http://wzg.chenjidiqi.icu

PHP:  $value = $data ?? "默认值";
来源：http://rqk.316326.xyz

JS:   const value = data ?? "默认值";
来源：http://hbl.ydzc1.top

TS:   const value = data ?? "默认值";
来源：http://zct.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oxs.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://fuz.yj202588.top


<!-- 参考信息 -->