代发 wailian999

[U71] PHP：抛出异常
来源：http://ptg.zhiwuduotai.top

throw new RuntimeException("失败", 500);
来源：http://xnj.gzhubu.top

[U72] PHP：写错误日志
来源：http://ouz.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://dfh.snrcjt.cn

[U73] PHP：读取 ini 配置
来源：http://byc.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://mgv.hongshengwenyu.top

[U74] PHP：读取环境变量
来源：http://nrz.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://icq.xziqi.cn

[U75] PHP：依赖注入
来源：http://svx.dashuyun.cn

composer require psr/container
来源：http://jzo.jinqigfzy.top

[U76] PHP：简单路由
来源：http://ngx.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cdq.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://zjk.cheryme.top

composer require twig/twig
来源：http://xif.tian-w.cn

[U78] PHP：单元测试
来源：http://prc.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://eui.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://hej.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://vjz.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://hih.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fub.fengsongda.top

[U81] JS：初始化项目
来源：http://eor.jianghu66.top

npm init -y;  npm i express
来源：http://nbi.gotoacloud.top

[U82] JS：package.json 脚本
来源：http://pmy.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://umu.jlsjyb.cn

[U83] JS：ES Module 导入导出
来源：http://syr.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pyo.fktsv.cn

[U84] JS：CommonJS 写法
来源：http://oqv.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://mep.guannengcc.top

[U85] JS：可选链
来源：http://neq.tarul.cn

a?.b?.c
来源：http://oyj.jiagoushi.top

[U86] JS：空值合并
来源：http://esf.zycfv.cn

a ?? b
来源：http://fvf.guannengcc.top

[U87] JS：解构默认值
来源：http://zrc.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://psf.9152youxi.cn

[U88] JS：对象展开合并
来源：http://nks.yuxming.cn

{ ...a, ...b }
来源：http://zom.gogol.net.cn

[U89] JS：数组去重
来源：http://yry.jianghu66.top

[...new Set(arr)]
来源：http://hzb.0kj1m.cn

[U90] JS：数字数组排序
来源：http://rde.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://dwj.jinghuilouyu.cn

[U91] JS：对象键值遍历
来源：http://gnq.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ptz.tarul.cn

[U92] JS：深拷贝
来源：http://dlg.shanyushiyangtech.top

structuredClone(obj)
来源：http://mfh.ctjpmb.com

[U93] JS：模板字符串
来源：http://fvn.yuanzhike.top

`共 ${n} 条`
来源：http://smr.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://vdp.hongshengwenyu.top

const double = x => x * 2;
来源：http://lpz.havefunace.top

[U95] JS：Promise 包装
来源：http://pze.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://opf.iojbl.cn

[U96] JS：async/await 与异常
来源：http://lqf.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iit.jinqigfzy.top

[U97] JS：并发请求
来源：http://qom.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iva.jinqigufen.top

[U98] JS：fetch 带 JSON
来源：http://mds.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://goe.tianlin.xyz

[U99] JS：事件监听
来源：http://xnl.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://ali.daxiang520.top

[U100] JS：DOM 查询
来源：http://spy.jinqigfzy.top

document.querySelector(".item")
来源：http://isx.zhiwuduotai.top

[U101] JS：classList 操作
来源：http://jam.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://ylq.mhx1999.top

[U102] JS：本地存储
来源：http://uxi.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cdn.tanke756.top

[U103] JS：定时器
来源：http://ksz.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dpo.hysaishi.cn

[U104] JS：防抖
来源：http://yhp.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rct.nanxuanxn.top

[U105] JS：节流
来源：http://jni.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cej.shzxlz.cn

[U106] JS：日期格式化
来源：http://rkq.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cnu.nanxinkj.top

[U107] JS：数字千分位
来源：http://tsz.xingfuxueyuan.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://clf.zhixingplan.top

[U108] JS：随机整数
来源：http://bsh.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://prx.dianchejie.cn

[U109] JS：数组分组
来源：http://eeh.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://ucf.daxiang520.top

[U110] JS：数组分块
来源：http://syr.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ykw.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://oyz.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://bek.guannengcc.top

[U112] JS：字符串补位
来源：http://iny.nanxinkj.top

"7".padStart(3, "0")
来源：http://rdy.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://piq.cqqwz.cn

s.replaceAll("a", "b")
来源：http://bml.chenlongwang.top

[U114] JS：JSON 深比较
来源：http://nhz.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ztd.havefunace.top

[U115] JS：生成 UUID
来源：http://hlr.yj20258888.top

crypto.randomUUID()
来源：http://wqe.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://itw.meibo888.top

/** @param {string} name */ function f(name) {}
来源：http://rhq.cqqwz.cn

[U117] JS：单元测试
来源：http://gft.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://zfi.yj20258.top

[U118] JS：开发服务器
来源：http://axu.zdbjq.cn

npm i -D vite;  npx vite
来源：http://ner.yueranfly.top

[U119] JS：生产构建
来源：http://igl.meibo888.top

npx vite build
来源：http://com.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://rnk.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://ywm.ybcxt.top

================================================================================
来源：http://xjp.havefunace.top

统计汇总
来源：http://erb.yj20258888.top

================================================================================
来源：http://cim.cqqwz.cn

按语言统计（条）：
来源：http://uaw.zhongyouzk.top

Python ......... 252
来源：http://irb.havefunace.top

PHP ............ 252
来源：http://nzh.yj202588.top

JavaScript ..... 252
来源：http://jdo.gogol.net.cn

TypeScript ..... 212
来源：http://cwl.redwolf501.top

Java ........... 212
来源：http://exi.hesvh.cn

Go ............. 212
来源：http://yry.hnxiangtu.top

Ruby ........... 212
来源：http://eqx.yueranfly.top

C# ............. 212
来源：http://jcw.fanxiaobao.xyz

C .............. 30
来源：http://whu.epnwcf.com

C++ ............ 30
来源：http://gce.52xcode.cn

SQL ............ 90
来源：http://hnr.feifeiyinyue.top

Bash ........... 80
来源：http://uxh.0kj1m.cn

Kotlin ......... 15
来源：http://wdu.yj20258.top

Swift .......... 15
来源：http://oxk.uphjek.com

Lua ............ 10
来源：http://sbv.guannengcc.top

Perl ........... 10
来源：http://fea.hywenlv.cn

Scala .......... 10
来源：http://hyg.birdmap.top

------------------------------------
来源：http://fsw.zycfv.cn

合计 ........... 2106 条
来源：http://slu.yongpay.top

按章节统计：
来源：http://lsj.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jui.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://snz.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wnk.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kgp.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gcm.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dtd.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rqj.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pvv.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://psg.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://upq.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dzq.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yje.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qty.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ram.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://psi.xinyue.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jxa.jqgufenzy.top

Q SQL 专题                              90
来源：http://skp.shanyushiyangkeji.top

R Bash 专题                             80
来源：http://zcx.yuanzhike.top

S C / C++ 专题                          60
来源：http://vug.yj202588.top

T 其他语言补充                          60
来源：http://twh.cdnleiting.top

U 高频实用片段                         120
来源：http://oad.yvedp.cn

------------------------------------
来源：http://sff.jlsjyb.cn

合计                                  2106 条
来源：http://rsi.jianghu66.top

--------------------------------------------------------------------------------
来源：http://vdr.iojbl.cn

使用提醒
来源：http://byg.ydzc1.top

--------------------------------------------------------------------------------
来源：http://czy.wangshuangyany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yyv.sxryk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wxq.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nch.tarul.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ntv.ybcxt.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oly.yanxiufei.cn

—— 文件结束 ——
来源：http://mlw.hesvh.cn

================================================================================
来源：http://tfi.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://oes.yuxming.cn

Common Programming Examples Cheat Book
来源：http://pta.epnwcf.com

================================================================================
来源：http://ueh.shangyingyoupin.top

【收录内容】
来源：http://xvf.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qrd.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mxy.zhixingplan.top

SQL · Bash · C · C++
来源：http://jxn.fktsv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tre.shzxlz.cn

【使用说明】
来源：http://wvx.smart0.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qde.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lum.iojbl.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lig.hcnkem.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mrl.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xuq.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ewg.zdqjudy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nvl.dashuyun.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fqt.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ldt.jianghu66.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://doc.0kj1m.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jzn.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://exx.pengpengdd.cyou

【文件统计】
来源：http://pps.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ini.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://eum.ydjk.org.cn

目  录
来源：http://fdi.hcnkem.com

--------------------------------------------------------------------------------
来源：http://psq.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vue.zhixingplan.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mso.jinghuilouyu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wrr.havefunace.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bdu.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wbp.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gqf.uphjek.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xio.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vli.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lop.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ymd.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sxx.jinghuilouyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gug.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wpp.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cou.shuidangran.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zfc.cheryme.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ijv.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kty.yangfankeji.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://nal.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://smd.snrcjt.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rus.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dcd.ctjpmb.com

================================================================================
来源：http://kkn.cashguo.top

A. 基础语法与类型
来源：http://pne.kuanghao11.cn

================================================================================
来源：http://hkj.ydzc1.top

[A01] Hello World
来源：http://uki.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://bhu.ctjpmb.com

PHP:  echo "Hello, World!";
来源：http://kbh.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://ugp.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qdx.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://ygw.daxiang520.top

Go:   fmt.Println("Hello, World!")
来源：http://nqn.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://rqi.shangyingyoupin.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ybj.pycfn.com

[A02] 变量声明与赋值
来源：http://ucu.hfpthk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gqe.svipenyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://omq.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://fed.gaohongyu789.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kul.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://fek.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://ytc.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://hfs.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://ajz.tarul.cn

[A03] 常量定义
来源：http://zaz.sysykeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kjc.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://zpz.redwolf501.top

JS:   const PI = 3.14159;
来源：http://gvy.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://mgg.cqqwz.cn

Java: static final double PI = 3.14159;
来源：http://lak.yuxming.cn

Go:   const PI = 3.14159
来源：http://clu.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://qbp.ivvv.top

C#:   const double PI = 3.14159;
来源：http://kav.hammf.cn

[A04] 判断变量类型
来源：http://ofn.vehdjk.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://psl.yj202588.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://swl.sweek.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ugu.hnxiangtu.top

TS:   typeof x; x instanceof Date
来源：http://onh.mhx1999.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gem.yanxiufei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://puq.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mrv.zdqjudy.top

C#:   x.GetType().Name; x is int
来源：http://oeo.shanyushiyangtech.top

[A05] 整数除法与取模
来源：http://ijc.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jyo.nanxinkj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ium.yongpay.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sbh.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vme.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://kjq.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://cpv.zhixingplan.top

Ruby: 7 / 2; 7 % 2
来源：http://cwn.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://xdj.chenzaomai.com

[A06] 字符串转数字
来源：http://ubx.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://mki.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dlv.mhx1999.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://asm.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wbb.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rhk.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://awf.bjfxy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cov.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ayr.meibo888.top

[A07] 数字转字符串
来源：http://hit.sufxvd.cn

Py:   str(42)
来源：http://qaa.guannengcc.top

PHP:  (string) 42; strval(42)
来源：http://quu.gotoacloud.top

JS:   String(42); (42).toString()
来源：http://ehn.hnqzz.top

TS:   String(42)
来源：http://pop.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ukc.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://sut.gzhubu.top

Ruby: 42.to_s
来源：http://wvq.vehdjk.com

C#:   42.ToString()
来源：http://zbo.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://ikj.smart0.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://osb.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dki.zhijiandao.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://alv.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fhj.sufxvd.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nse.hammf.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://igi.vehdjk.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://kxo.hesvh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tey.zhengqikj.top

[A09] 绝对值与最大最小值
来源：http://uay.gogol.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ywx.jqgufenzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fpk.jinqigfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nvs.jinghuilouyu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mny.hcnkem.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zel.hysaishi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nqv.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cih.havefunace.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://owt.yanxiufei.cn

[A10] 生成随机数
来源：http://mal.yuxming.cn

Py:   import random; random.randint(1, 100)
来源：http://ypo.fzhhl.top

PHP:  random_int(1, 100);
来源：http://yof.jiagoushi.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kzt.yonumen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://slx.yj20258.top

Java: new Random().nextInt(100) + 1
来源：http://xjc.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kaa.guannengcc.top

Ruby: rand(1..100)
来源：http://skx.yuxming.cn

C#:   new Random().Next(1, 101)
来源：http://ivb.vqdsnc.cn

[A11] 条件表达式（三元）
来源：http://ksv.fengsongda.top

Py:   "yes" if x > 0 else "no"
来源：http://hmh.chenzaomai.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://arz.aizwys.cn


<!-- 参考信息 -->