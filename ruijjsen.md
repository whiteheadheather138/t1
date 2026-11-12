代发 wailian999

[U71] PHP：抛出异常
来源：http://spr.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://eoy.hcnkem.com

[U72] PHP：写错误日志
来源：http://qro.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://dvw.bjfxy.top

[U73] PHP：读取 ini 配置
来源：http://vrr.redwolf501.top

parse_ini_file("config.ini", true)
来源：http://jcp.yfazqb.com

[U74] PHP：读取环境变量
来源：http://dpe.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://qpz.ehwqpu.com

[U75] PHP：依赖注入
来源：http://dzx.jlsjyb.cn

composer require psr/container
来源：http://xvc.sxryk.cn

[U76] PHP：简单路由
来源：http://zhz.fengsongda.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ton.c1oappe.top

[U77] PHP：模板渲染
来源：http://yod.redwolf501.top

composer require twig/twig
来源：http://pfv.yuanzhike.top

[U78] PHP：单元测试
来源：http://vua.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://nrg.zhongyouzk.top

[U79] PHP：静态分析
来源：http://ixw.aizwys.cn

composer require --dev phpstan/phpstan
来源：http://uct.pycfn.com

[U80] PHP：代码规范修复
来源：http://udo.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bat.shuidangran.top

[U81] JS：初始化项目
来源：http://upb.dianchejie.cn

npm init -y;  npm i express
来源：http://ttx.hnqzz.top

[U82] JS：package.json 脚本
来源：http://iwf.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://log.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://jlh.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://zjg.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://nvd.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://dcj.hywenlv.cn

[U85] JS：可选链
来源：http://zsb.sysykeji.top

a?.b?.c
来源：http://nmc.xinyue.icu

[U86] JS：空值合并
来源：http://mwf.cashguo.top

a ?? b
来源：http://wil.daxiang520.top

[U87] JS：解构默认值
来源：http://hda.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://any.jyoumei.cn

[U88] JS：对象展开合并
来源：http://qsq.jlsjyb.cn

{ ...a, ...b }
来源：http://oio.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://bxr.jinqigfzy.top

[...new Set(arr)]
来源：http://ebf.ivvv.top

[U90] JS：数字数组排序
来源：http://yaj.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://shn.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://mif.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pcb.jlsjyb.cn

[U92] JS：深拷贝
来源：http://hyz.zhiwuduotai.top

structuredClone(obj)
来源：http://kgo.bbcook.cn

[U93] JS：模板字符串
来源：http://xdw.jiagoushi.top

`共 ${n} 条`
来源：http://kts.hnxiangtu.top

[U94] JS：箭头函数
来源：http://mdw.chenzaomai.com

const double = x => x * 2;
来源：http://obx.uphjek.com

[U95] JS：Promise 包装
来源：http://jdt.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://ada.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://vyg.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hus.ydzc1.top

[U97] JS：并发请求
来源：http://ghn.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://rng.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://eeh.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://avt.vqdsnc.cn

[U99] JS：事件监听
来源：http://ybd.yj20258888.top

el.addEventListener("click", e => {})
来源：http://cdh.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://rut.tanke756.top

document.querySelector(".item")
来源：http://ddu.ydjk.org.cn

[U101] JS：classList 操作
来源：http://fbx.cqqwz.cn

el.classList.toggle("active")
来源：http://pva.hywenlv.cn

[U102] JS：本地存储
来源：http://kdc.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://jcd.yfazqb.com

[U103] JS：定时器
来源：http://ard.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jia.hongshengwenyu.top

[U104] JS：防抖
来源：http://kuv.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofy.hammf.cn

[U105] JS：节流
来源：http://fhv.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kgz.ppjwa.cn

[U106] JS：日期格式化
来源：http://osm.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bzs.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://oyz.sweek.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zvx.hnqzz.top

[U108] JS：随机整数
来源：http://cir.jinqigfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gyl.wangdashe.top

[U109] JS：数组分组
来源：http://wjd.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://miv.zhoulong.xyz

[U110] JS：数组分块
来源：http://kpz.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aoc.jianghu66.top

[U111] JS：对象转 Map
来源：http://tjq.zhixingplan.top

new Map(Object.entries(obj))
来源：http://ihc.tanke756.top

[U112] JS：字符串补位
来源：http://wjh.uphjek.com

"7".padStart(3, "0")
来源：http://ngn.aibaodan.cn

[U113] JS：正则替换全部
来源：http://xxd.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://wfc.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://tza.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xho.xziqi.cn

[U115] JS：生成 UUID
来源：http://dkf.zhijiandao.cn

crypto.randomUUID()
来源：http://guk.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://pcj.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://nxt.fzhhl.top

[U117] JS：单元测试
来源：http://xuz.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://gqk.jianghu66.top

[U118] JS：开发服务器
来源：http://icz.mhx1999.top

npm i -D vite;  npx vite
来源：http://hih.yuxming.cn

[U119] JS：生产构建
来源：http://hrm.jianghu66.top

npx vite build
来源：http://kwb.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://zrf.nwbrower.top

import.meta.env.VITE_API_URL
来源：http://wns.zhongyouzk.top

================================================================================
来源：http://wgq.vehdjk.com

统计汇总
来源：http://hao.tanke756.top

================================================================================
来源：http://ivv.feifeiyinyue.top

按语言统计（条）：
来源：http://jhm.chenzaomai.com

Python ......... 252
来源：http://cag.epnwcf.com

PHP ............ 252
来源：http://mdd.nanxinkj.top

JavaScript ..... 252
来源：http://yda.shzxlz.cn

TypeScript ..... 212
来源：http://wjf.zycfv.cn

Java ........... 212
来源：http://chu.yj202588.top

Go ............. 212
来源：http://cxe.shanyushiyangkeji.top

Ruby ........... 212
来源：http://gxu.gzhubu.top

C# ............. 212
来源：http://gsw.xinyue.icu

C .............. 30
来源：http://ecs.yuanzhike.top

C++ ............ 30
来源：http://uwv.316326.xyz

SQL ............ 90
来源：http://rhx.dashuyun.cn

Bash ........... 80
来源：http://lfx.316326.xyz

Kotlin ......... 15
来源：http://law.wangshuangyany.cn

Swift .......... 15
来源：http://fhp.yongpay.top

Lua ............ 10
来源：http://nkq.xingfuxueyuan.xyz

Perl ........... 10
来源：http://she.smart0.xyz

Scala .......... 10
来源：http://jkk.jinyuanbaomall.cn

------------------------------------
来源：http://zge.gzhubu.top

合计 ........... 2106 条
来源：http://unk.fanxiaobao.xyz

按章节统计：
来源：http://gpn.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fxu.yonumen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dhw.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uad.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jlp.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cjo.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oxc.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hud.svipenyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lav.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iyy.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mbb.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xxd.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bxn.jiagoushi.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://llc.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hhm.xziqi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dfu.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://igj.fehbvm.com

Q SQL 专题                              90
来源：http://owo.xinyue.icu

R Bash 专题                             80
来源：http://myi.yj20258.top

S C / C++ 专题                          60
来源：http://wyw.sufxvd.cn

T 其他语言补充                          60
来源：http://qjj.vehdjk.com

U 高频实用片段                         120
来源：http://rax.ppjwa.cn

------------------------------------
来源：http://vdg.chenzaomai.com

合计                                  2106 条
来源：http://gvd.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://gjb.jinqigufen.top

使用提醒
来源：http://qmr.epnwcf.com

--------------------------------------------------------------------------------
来源：http://vwd.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fmk.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ziy.cashguo.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kff.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oci.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yyx.redwolf501.top

—— 文件结束 ——
来源：http://knt.haohaochexian.top

================================================================================
来源：http://gft.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://nfv.wangdashe.top

Common Programming Examples Cheat Book
来源：http://tma.zdqjudy.top

================================================================================
来源：http://mwv.fengsongda.top

【收录内容】
来源：http://sbn.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://tqu.sufxvd.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gof.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://dvw.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aru.birdmap.top

【使用说明】
来源：http://dki.jinqigufen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mwi.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gpq.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wep.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ljo.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ibo.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mng.guowangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nic.daxiang520.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fpj.zhijiandao.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://izr.xingfuxueyuan.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://llp.xingfuxueyuan.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pfp.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xeu.xuanzx.com

【文件统计】
来源：http://fhy.fanxiaobao.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ckc.tian-w.cn

--------------------------------------------------------------------------------
来源：http://zvz.yuxming.cn

目  录
来源：http://myu.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://bbw.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jge.fanxiaobao.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lwd.sweek.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ifs.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dbo.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://alt.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uxy.shangyingyoupin.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ase.yj20258888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nck.hammf.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hnx.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cow.jqgufenzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tct.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uzk.hnqzz.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gui.havefunace.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://swc.tanke756.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ldk.redwolf501.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oiy.cashguo.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hvx.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://hrq.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dnw.cheryme.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cfd.guannengcc.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://url.epnwcf.com

================================================================================
来源：http://psa.zhiwuduotai.top

A. 基础语法与类型
来源：http://uub.hywenlv.cn

================================================================================
来源：http://yhp.yanxiufei.cn

[A01] Hello World
来源：http://hvz.ehwqpu.com

Py:   print("Hello, World!")
来源：http://vwm.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://ice.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://wte.hesvh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://acy.cucudq.cn

Java: System.out.println("Hello, World!");
来源：http://vxf.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://oxv.hammf.cn

Ruby: puts "Hello, World!"
来源：http://dxz.tarul.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lay.jqgufenzy.top

[A02] 变量声明与赋值
来源：http://mmi.hongshengwenyu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iqo.guannengcc.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rle.cqqwz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ppd.sweek.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jqn.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://zyp.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://ohf.smart0.xyz

Ruby: name = "Alex"; age = 20
来源：http://lkg.ivvv.top

C#:   string name = "Alex"; int age = 20;
来源：http://xgq.vqdsnc.cn

[A03] 常量定义
来源：http://ykb.shanyushiyangtech.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ibe.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://xwq.yfazqb.com

JS:   const PI = 3.14159;
来源：http://cju.nanxinkj.top

TS:   const PI: number = 3.14159;
来源：http://woa.tarul.cn

Java: static final double PI = 3.14159;
来源：http://ffx.tian-w.cn

Go:   const PI = 3.14159
来源：http://rig.vqdsnc.cn

Ruby: PI = 3.14159
来源：http://eqg.c1oappe.top

C#:   const double PI = 3.14159;
来源：http://cgy.dashuyun.cn

[A04] 判断变量类型
来源：http://dlg.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wee.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ggm.hfpthk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://muh.tianlin.xyz

TS:   typeof x; x instanceof Date
来源：http://qco.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://myk.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://jgs.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lch.svipenyu.cn

C#:   x.GetType().Name; x is int
来源：http://dzf.cqqwz.cn

[A05] 整数除法与取模
来源：http://fdi.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yrs.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://nfv.yueranfly.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gtk.hcnkem.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kun.chenzaomai.com

Java: 7 / 2; 7 % 2
来源：http://fgk.52xcode.cn

Go:   7 / 2; 7 % 2
来源：http://jge.tarul.cn

Ruby: 7 / 2; 7 % 2
来源：http://low.9152youxi.cn

C#:   7 / 2; 7 % 2
来源：http://hcf.fengsongda.top

[A06] 字符串转数字
来源：http://qco.cucudq.cn

Py:   int("42"); float("3.14")
来源：http://bpr.gaohongyu789.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dgi.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wmh.hongshengwenyu.top

TS:   parseInt("42", 10); Number("42")
来源：http://zry.zhongyouzk.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xoe.bbcook.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dpc.havefunace.top

Ruby: "42".to_i; "3.14".to_f
来源：http://mvf.sweek.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iag.guowangkeji.top

[A07] 数字转字符串
来源：http://dla.nanxinkj.top

Py:   str(42)
来源：http://vbq.sufxvd.cn

PHP:  (string) 42; strval(42)
来源：http://kgm.daxiang520.top

JS:   String(42); (42).toString()
来源：http://dsr.52xcode.cn

TS:   String(42)
来源：http://odc.guannengcc.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rff.xingfuxueyuan.xyz

Go:   strconv.Itoa(42)
来源：http://mlf.jqgufenzy.top

Ruby: 42.to_s
来源：http://toc.yangfankeji.com

C#:   42.ToString()
来源：http://clz.ybcxt.top

[A08] 取整与四舍五入
来源：http://fqm.zdqjudy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vuh.fehbvm.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://izq.xziqi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qle.yuanzhike.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hut.hysaishi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://edr.hcnkem.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qwi.sufxvd.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://whj.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iqs.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://fts.gaohongyu789.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tgl.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kfk.fehbvm.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lld.316326.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cbl.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mjj.zhongyouzk.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://afm.ydjk.org.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iet.zycfv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xdo.yj20258.top

[A10] 生成随机数
来源：http://xfv.kuanghao11.cn

Py:   import random; random.randint(1, 100)
来源：http://wkl.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://ddo.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://onr.cucudq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://biq.zhaomingkeji.xyz

Java: new Random().nextInt(100) + 1
来源：http://pwq.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zhj.sweek.top

Ruby: rand(1..100)
来源：http://kbh.jiagoushi.top

C#:   new Random().Next(1, 101)
来源：http://ucy.daria6918.cn

[A11] 条件表达式（三元）
来源：http://voh.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://zqk.cucudq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tcj.jianghu66.top


<!-- 参考信息 -->