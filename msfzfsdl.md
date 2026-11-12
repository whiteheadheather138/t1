代发 wailian999

[U67] PHP：处理文件上传
来源：http://vsn.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iyk.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://mzi.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://inr.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://ksb.bjfxy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://upl.nwbrower.top

[U70] PHP：PDO 事务
来源：http://moa.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ccb.wangdashe.top

[U71] PHP：抛出异常
来源：http://dkb.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://iph.dashuyun.cn

[U72] PHP：写错误日志
来源：http://cem.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://pjz.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://jep.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://ukr.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://mfi.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://lxg.zdqjudy.top

[U75] PHP：依赖注入
来源：http://grs.xziqi.cn

composer require psr/container
来源：http://nfu.jqgufenzy.top

[U76] PHP：简单路由
来源：http://yzx.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ecl.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://dsb.aibaodan.cn

composer require twig/twig
来源：http://csi.hfpthk.cn

[U78] PHP：单元测试
来源：http://vwa.pycfn.com

composer require --dev phpunit/phpunit
来源：http://jvh.ehwqpu.com

[U79] PHP：静态分析
来源：http://ijh.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://caj.pycfn.com

[U80] PHP：代码规范修复
来源：http://vej.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uyc.xinyue.icu

[U81] JS：初始化项目
来源：http://uxg.fktsv.cn

npm init -y;  npm i express
来源：http://pjt.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://bgb.zdbjq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vdc.xingfuxueyuan.xyz

[U83] JS：ES Module 导入导出
来源：http://got.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://qwm.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://ayh.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://fda.yfazqb.com

[U85] JS：可选链
来源：http://gcr.wangshuangyany.cn

a?.b?.c
来源：http://kqe.cucudq.cn

[U86] JS：空值合并
来源：http://zba.zhiwuduotai.top

a ?? b
来源：http://bbk.andypj.xyz

[U87] JS：解构默认值
来源：http://big.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://mzo.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://wrd.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://qfg.ydjk.org.cn

[U89] JS：数组去重
来源：http://qwy.dashuyun.cn

[...new Set(arr)]
来源：http://xxh.sufxvd.cn

[U90] JS：数字数组排序
来源：http://eqj.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://cll.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://dvk.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ovc.9152youxi.cn

[U92] JS：深拷贝
来源：http://ypa.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://mcm.zdbjq.cn

[U93] JS：模板字符串
来源：http://uuz.9152youxi.cn

`共 ${n} 条`
来源：http://aul.ybcxt.top

[U94] JS：箭头函数
来源：http://xym.jinghuilouyu.cn

const double = x => x * 2;
来源：http://kyg.vehdjk.com

[U95] JS：Promise 包装
来源：http://oja.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://vis.yj202588.top

[U96] JS：async/await 与异常
来源：http://her.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cxa.shuidangran.top

[U97] JS：并发请求
来源：http://nwa.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pwt.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://wll.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zzg.xylfe.cn

[U99] JS：事件监听
来源：http://yww.cdnleiting.top

el.addEventListener("click", e => {})
来源：http://xro.shzxlz.cn

[U100] JS：DOM 查询
来源：http://end.guowangkeji.top

document.querySelector(".item")
来源：http://abb.hnqzz.top

[U101] JS：classList 操作
来源：http://vhy.sweek.top

el.classList.toggle("active")
来源：http://knb.ehwqpu.com

[U102] JS：本地存储
来源：http://fco.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ntp.feifeiyinyue.top

[U103] JS：定时器
来源：http://nqq.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://miv.hywenlv.cn

[U104] JS：防抖
来源：http://vbm.cucudq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vcq.yueranfly.top

[U105] JS：节流
来源：http://qvk.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mqh.cdnleiting.top

[U106] JS：日期格式化
来源：http://zhl.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xum.jlsjyb.cn

[U107] JS：数字千分位
来源：http://jpx.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cvf.svipenyu.cn

[U108] JS：随机整数
来源：http://tig.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qbg.hesvh.cn

[U109] JS：数组分组
来源：http://msy.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://ryi.shuidangran.top

[U110] JS：数组分块
来源：http://eqe.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rzt.sufxvd.cn

[U111] JS：对象转 Map
来源：http://gax.9152youxi.cn

new Map(Object.entries(obj))
来源：http://ynv.chenzaomai.com

[U112] JS：字符串补位
来源：http://frn.vehdjk.com

"7".padStart(3, "0")
来源：http://oll.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://psm.nanxinkj.top

s.replaceAll("a", "b")
来源：http://fiw.yonumen.top

[U114] JS：JSON 深比较
来源：http://lgf.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sdb.gzhubu.top

[U115] JS：生成 UUID
来源：http://wby.uphjek.com

crypto.randomUUID()
来源：http://jyx.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://brq.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://veq.snrcjt.cn

[U117] JS：单元测试
来源：http://beg.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://hxo.xinyue.icu

[U118] JS：开发服务器
来源：http://mon.cucudq.cn

npm i -D vite;  npx vite
来源：http://jgp.yuxming.cn

[U119] JS：生产构建
来源：http://zbi.tanke756.top

npx vite build
来源：http://xiz.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://imq.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://epf.hcnkem.com

================================================================================
来源：http://zbw.ybcxt.top

统计汇总
来源：http://tdq.ydzc1.top

================================================================================
来源：http://mdf.zhiwuduotai.top

按语言统计（条）：
来源：http://pzj.tanke756.top

Python ......... 252
来源：http://oue.gaohongyu789.top

PHP ............ 252
来源：http://ccs.gzhubu.top

JavaScript ..... 252
来源：http://aic.chenlongwang.top

TypeScript ..... 212
来源：http://vif.vqdsnc.cn

Java ........... 212
来源：http://zch.zhongyouzk.top

Go ............. 212
来源：http://lax.xuetiantiany.cn

Ruby ........... 212
来源：http://shu.gogol.net.cn

C# ............. 212
来源：http://qvd.hnqzz.top

C .............. 30
来源：http://hod.epnwcf.com

C++ ............ 30
来源：http://ihs.birdmap.top

SQL ............ 90
来源：http://ova.sysykeji.top

Bash ........... 80
来源：http://jiq.xuanzx.com

Kotlin ......... 15
来源：http://vlb.ppjwa.cn

Swift .......... 15
来源：http://oak.vqdsnc.cn

Lua ............ 10
来源：http://nin.fanxiaobao.xyz

Perl ........... 10
来源：http://ilb.sweek.top

Scala .......... 10
来源：http://lyq.mhx1999.top

------------------------------------
来源：http://kfq.cqqwz.cn

合计 ........... 2106 条
来源：http://upd.jinqigufen.top

按章节统计：
来源：http://xvx.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gqs.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wjw.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wzg.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://apg.xingfuxueyuan.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ggf.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fsf.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uuv.sjlbkw.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sue.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zno.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hzw.shanyushiyangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zwd.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wpq.pengpengdd.cyou

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rqx.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sfn.52xcode.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gpn.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ldj.ydzc1.top

Q SQL 专题                              90
来源：http://mpd.aizwys.cn

R Bash 专题                             80
来源：http://gbm.zhijiandao.cn

S C / C++ 专题                          60
来源：http://top.mhx1999.top

T 其他语言补充                          60
来源：http://xqz.quarkkingdee.top

U 高频实用片段                         120
来源：http://evm.fehbvm.com

------------------------------------
来源：http://cme.9152youxi.cn

合计                                  2106 条
来源：http://bmi.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://suq.ybcxt.top

使用提醒
来源：http://nhc.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://pwa.cdnleiting.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kez.jianghu66.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cov.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uhq.cdnleiting.top

在旧版本上使用前请先确认语法支持情况。
来源：http://har.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hvi.hesvh.cn

—— 文件结束 ——
来源：http://cxc.hywenlv.cn

================================================================================
来源：http://xyo.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://uoi.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://jep.ehwqpu.com

================================================================================
来源：http://jdi.hfpthk.cn

【收录内容】
来源：http://ori.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://evm.ehwqpu.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hwx.gzhubu.top

SQL · Bash · C · C++
来源：http://dnp.daxiang520.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ysm.316326.xyz

【使用说明】
来源：http://qoc.hywenlv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://txk.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gec.ivvv.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gly.sweek.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zus.jlsjyb.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hnt.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://icb.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://exp.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ygr.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mjs.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ofr.yuxming.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rcy.zycfv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dtw.tianlin.xyz

【文件统计】
来源：http://ccg.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hdj.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://mat.uphjek.com

目  录
来源：http://mma.jianghu66.top

--------------------------------------------------------------------------------
来源：http://hda.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qhp.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lxp.hnxiangtu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hju.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vys.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uiy.fengsongda.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ppv.kuanghao11.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mce.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ptf.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yvx.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ehk.xziqi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cew.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rsq.gogol.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://unj.0kj1m.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bna.tanke756.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qil.ivvv.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://grt.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aes.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jvv.zhixingplan.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yvk.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ntl.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dha.tianlin.xyz

================================================================================
来源：http://yxf.fktsv.cn

A. 基础语法与类型
来源：http://ydg.chenjidiqi.icu

================================================================================
来源：http://tag.iojbl.cn

[A01] Hello World
来源：http://vvd.hongshengwenyu.top

Py:   print("Hello, World!")
来源：http://anf.jinqigufen.top

PHP:  echo "Hello, World!";
来源：http://oev.hammf.cn

JS:   console.log("Hello, World!");
来源：http://aht.jinqigufen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jyo.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://uxd.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://fqb.feifeiyinyue.top

Ruby: puts "Hello, World!"
来源：http://qmi.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qwm.xziqi.cn

[A02] 变量声明与赋值
来源：http://ucg.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dwo.zhengqikj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://btb.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://ynz.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bgh.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://lfl.shanyushiyangkeji.top

Go:   name := "Alex"; age := 20
来源：http://ltq.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://gjn.jiagoushi.top

C#:   string name = "Alex"; int age = 20;
来源：http://gss.meibo888.top

[A03] 常量定义
来源：http://ejw.kuanghao11.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://czj.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://qhd.yueranfly.top

JS:   const PI = 3.14159;
来源：http://dak.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://vyi.smart0.xyz

Java: static final double PI = 3.14159;
来源：http://yce.daxiang520.top

Go:   const PI = 3.14159
来源：http://eqn.chenlongwang.top

Ruby: PI = 3.14159
来源：http://rks.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://baa.cqqwz.cn

[A04] 判断变量类型
来源：http://cwz.fzhhl.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mqg.316326.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qqa.shanyushiyangtech.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nib.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://ruz.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xuc.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://qjw.yvedp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mxt.hesvh.cn

C#:   x.GetType().Name; x is int
来源：http://crn.jqgfzy.top

[A05] 整数除法与取模
来源：http://ijv.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cos.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bwj.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lrt.yuxming.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://adl.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://xnm.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://abv.guowangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://uto.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://waq.ehwqpu.com

[A06] 字符串转数字
来源：http://kcz.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://hmz.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zly.cdnleiting.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fpa.0kj1m.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jjr.yangfankeji.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cvw.zhiwuduotai.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uiq.ehwqpu.com

Ruby: "42".to_i; "3.14".to_f
来源：http://nps.cashguo.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jaf.zhixingplan.top

[A07] 数字转字符串
来源：http://gru.jyoumei.cn

Py:   str(42)
来源：http://jxw.xinyue.icu

PHP:  (string) 42; strval(42)
来源：http://gzv.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://mlh.shzxlz.cn

TS:   String(42)
来源：http://fqr.uphjek.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://lmg.0kj1m.cn

Go:   strconv.Itoa(42)
来源：http://lfg.svipenyu.cn

Ruby: 42.to_s
来源：http://xjm.tanke756.top

C#:   42.ToString()
来源：http://icj.hywenlv.cn

[A08] 取整与四舍五入
来源：http://yef.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://him.zhijiandao.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vyi.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jxu.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kzb.ehwqpu.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jdm.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tso.wangshuangyany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vdw.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dng.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://bid.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bmi.chenlongwang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fnw.jinqigufen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hon.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fpo.zdqjudy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://inl.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jlk.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wcf.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bqe.pycfn.com

[A10] 生成随机数
来源：http://qrm.xylfe.cn

Py:   import random; random.randint(1, 100)
来源：http://smn.redwolf501.top

PHP:  random_int(1, 100);
来源：http://nie.c1oappe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pgy.cashguo.top


<!-- 参考信息 -->