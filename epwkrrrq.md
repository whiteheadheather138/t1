代发 wailian999

[U67] PHP：处理文件上传
来源：http://ohu.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ubt.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://nah.redwolf501.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vkx.tanke756.top

[U69] PHP：PDO 预处理
来源：http://enk.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tnr.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://umk.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cgp.jinqigufen.top

[U71] PHP：抛出异常
来源：http://nms.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://zxu.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://box.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://fqh.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://gbf.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://sbj.hcnkem.com

[U74] PHP：读取环境变量
来源：http://khv.hcnkem.com

getenv("APP_ENV") ?: "production"
来源：http://ogk.tarul.cn

[U75] PHP：依赖注入
来源：http://ngp.wangdashe.top

composer require psr/container
来源：http://gbu.jianghu66.top

[U76] PHP：简单路由
来源：http://wxb.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rqm.epnwcf.com

[U77] PHP：模板渲染
来源：http://cop.tianlin.xyz

composer require twig/twig
来源：http://gda.dashuyun.cn

[U78] PHP：单元测试
来源：http://bgb.tarul.cn

composer require --dev phpunit/phpunit
来源：http://yby.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://moe.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://qnj.mhx1999.top

[U80] PHP：代码规范修复
来源：http://akb.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nzw.yongpay.top

[U81] JS：初始化项目
来源：http://kmm.uphjek.com

npm init -y;  npm i express
来源：http://sir.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://nfe.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://suc.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://kyf.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://zpt.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://pka.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://xgs.mhx1999.top

[U85] JS：可选链
来源：http://mkp.feifeiyinyue.top

a?.b?.c
来源：http://ufh.52xcode.cn

[U86] JS：空值合并
来源：http://dak.cashguo.top

a ?? b
来源：http://rob.yj202588.top

[U87] JS：解构默认值
来源：http://oyn.yanxiufei.cn

const { a = 1, b = 2 } = obj;
来源：http://vfx.9152youxi.cn

[U88] JS：对象展开合并
来源：http://tki.ybcxt.top

{ ...a, ...b }
来源：http://oir.andypj.xyz

[U89] JS：数组去重
来源：http://gcv.snrcjt.cn

[...new Set(arr)]
来源：http://btp.yj20258.top

[U90] JS：数字数组排序
来源：http://uqe.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://slk.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://qjc.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://inz.zdqjudy.top

[U92] JS：深拷贝
来源：http://lwn.fanxiaobao.xyz

structuredClone(obj)
来源：http://ghi.fktsv.cn

[U93] JS：模板字符串
来源：http://alo.gogol.net.cn

`共 ${n} 条`
来源：http://itj.svipenyu.cn

[U94] JS：箭头函数
来源：http://vqr.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://pid.bbcook.cn

[U95] JS：Promise 包装
来源：http://eak.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://zwf.sweek.top

[U96] JS：async/await 与异常
来源：http://ogf.hnxiangtu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ckf.jlsjyb.cn

[U97] JS：并发请求
来源：http://imf.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kcg.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://xzk.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vld.yonumen.top

[U99] JS：事件监听
来源：http://son.nwbrower.top

el.addEventListener("click", e => {})
来源：http://exe.9152youxi.cn

[U100] JS：DOM 查询
来源：http://qqe.kuanghao11.cn

document.querySelector(".item")
来源：http://gmr.jqgfzy.top

[U101] JS：classList 操作
来源：http://pzg.pengpengdd.cyou

el.classList.toggle("active")
来源：http://qfb.zdqjudy.top

[U102] JS：本地存储
来源：http://jsl.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pkc.shuidangran.top

[U103] JS：定时器
来源：http://chl.sxryk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gsw.9152youxi.cn

[U104] JS：防抖
来源：http://cem.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ual.iojbl.cn

[U105] JS：节流
来源：http://ywo.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://umz.ppjwa.cn

[U106] JS：日期格式化
来源：http://uds.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tpg.ehwqpu.com

[U107] JS：数字千分位
来源：http://xdu.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://phe.hesvh.cn

[U108] JS：随机整数
来源：http://vjs.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mhn.nwbrower.top

[U109] JS：数组分组
来源：http://qpp.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://ifk.fengsongda.top

[U110] JS：数组分块
来源：http://vcv.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vqn.nwbrower.top

[U111] JS：对象转 Map
来源：http://riq.chenlongwang.top

new Map(Object.entries(obj))
来源：http://fng.nwbrower.top

[U112] JS：字符串补位
来源：http://gnp.zdbjq.cn

"7".padStart(3, "0")
来源：http://ovt.hywenlv.cn

[U113] JS：正则替换全部
来源：http://qyv.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://wno.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://zlp.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kiu.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://cyj.yj202588.top

crypto.randomUUID()
来源：http://jqv.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://vqq.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://oni.tanke756.top

[U117] JS：单元测试
来源：http://blu.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://xwm.fengsongda.top

[U118] JS：开发服务器
来源：http://wgn.ehwqpu.com

npm i -D vite;  npx vite
来源：http://awr.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://yqt.hnqzz.top

npx vite build
来源：http://ail.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://iyl.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://xef.daria6918.cn

================================================================================
来源：http://vzr.gotoacloud.top

统计汇总
来源：http://bsn.wangdashe.top

================================================================================
来源：http://hec.meibo888.top

按语言统计（条）：
来源：http://fso.bbcook.cn

Python ......... 252
来源：http://vfe.ctjpmb.com

PHP ............ 252
来源：http://iod.sxryk.cn

JavaScript ..... 252
来源：http://yvs.pengpengdd.cyou

TypeScript ..... 212
来源：http://cwp.gogol.net.cn

Java ........... 212
来源：http://wyk.nanxinkj.top

Go ............. 212
来源：http://emp.daxiang520.top

Ruby ........... 212
来源：http://kct.guannengcc.top

C# ............. 212
来源：http://yyq.ppjwa.cn

C .............. 30
来源：http://whh.xingfuxueyuan.xyz

C++ ............ 30
来源：http://xjx.wangdashe.top

SQL ............ 90
来源：http://iea.mhx1999.top

Bash ........... 80
来源：http://yxk.zycfv.cn

Kotlin ......... 15
来源：http://rjo.9152youxi.cn

Swift .......... 15
来源：http://tew.nwbrower.top

Lua ............ 10
来源：http://riq.hcnkem.com

Perl ........... 10
来源：http://wio.hfpthk.cn

Scala .......... 10
来源：http://ywk.zdqjudy.top

------------------------------------
来源：http://zhl.tanke756.top

合计 ........... 2106 条
来源：http://dap.ydzc1.top

按章节统计：
来源：http://cka.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jtm.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lta.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gui.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nrq.ivvv.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xov.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sew.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mgx.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qum.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ntb.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zos.zdbjq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ffq.jinqigfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sxr.pengpengdd.cyou

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lej.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lim.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nsn.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sva.zhoulong.xyz

Q SQL 专题                              90
来源：http://fbj.yj20258.top

R Bash 专题                             80
来源：http://qrl.9152youxi.cn

S C / C++ 专题                          60
来源：http://jyg.shangyingyoupin.top

T 其他语言补充                          60
来源：http://vgn.gzhubu.top

U 高频实用片段                         120
来源：http://saz.hammf.cn

------------------------------------
来源：http://nis.shzxlz.cn

合计                                  2106 条
来源：http://irm.yj20258.top

--------------------------------------------------------------------------------
来源：http://dut.aizwys.cn

使用提醒
来源：http://say.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://xpm.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gvz.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yja.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://amy.dianchejie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iab.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qft.guannengcc.top

—— 文件结束 ——
来源：http://rwq.zhixingplan.top

================================================================================
来源：http://mdq.9152youxi.cn

程序语言常见例子速查手册（2024 版）
来源：http://tmr.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://qid.xuanzx.com

================================================================================
来源：http://djn.yuanzhike.top

【收录内容】
来源：http://icb.pengpengdd.cyou

覆盖 12 种语言 / 语法与常见 API：
来源：http://dep.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nlx.yfazqb.com

SQL · Bash · C · C++
来源：http://apm.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://czw.smart0.xyz

【使用说明】
来源：http://xap.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://djc.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mef.yonumen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fud.hysaishi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://srk.ydjk.org.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qxd.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yfz.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dyu.feifeiyinyue.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://epu.guowangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yii.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://szp.gaohongyu789.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vmx.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://frq.ybcxt.top

【文件统计】
来源：http://uty.nanxinkj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://axw.ydzc1.top

--------------------------------------------------------------------------------
来源：http://uoi.tarul.cn

目  录
来源：http://czn.fzhhl.top

--------------------------------------------------------------------------------
来源：http://dlb.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pzc.zhaomingkeji.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uwk.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mex.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ywf.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wsf.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dnp.epnwcf.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bzk.zhoulong.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ypa.cheryme.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://npm.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jph.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rxe.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fuh.jqgufenzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qnr.xuetiantiany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jdg.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wla.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kcc.hammf.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qna.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rnc.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xgu.shzxlz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ojf.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://aba.nwbrower.top

================================================================================
来源：http://xyh.guowangkeji.top

A. 基础语法与类型
来源：http://fwe.shzxlz.cn

================================================================================
来源：http://omq.0kj1m.cn

[A01] Hello World
来源：http://jsw.hammf.cn

Py:   print("Hello, World!")
来源：http://shc.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://pny.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://gik.svipenyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bwa.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://ydu.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://fem.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://rxz.snrcjt.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jyj.yvedp.cn

[A02] 变量声明与赋值
来源：http://uhx.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fja.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://brp.hysaishi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sez.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pog.zhijiandao.cn

Java: String name = "Alex"; int age = 20;
来源：http://ooz.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://alt.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://voa.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hhx.hywenlv.cn

[A03] 常量定义
来源：http://afi.chenjidiqi.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cky.zhiwuduotai.top

PHP:  const PI = 3.14159;
来源：http://brx.hongshengwenyu.top

JS:   const PI = 3.14159;
来源：http://xhr.zycfv.cn

TS:   const PI: number = 3.14159;
来源：http://lab.feifeiyinyue.top

Java: static final double PI = 3.14159;
来源：http://zhc.hywenlv.cn

Go:   const PI = 3.14159
来源：http://lup.ydzc1.top

Ruby: PI = 3.14159
来源：http://qin.xylfe.cn

C#:   const double PI = 3.14159;
来源：http://kjk.hongshengwenyu.top

[A04] 判断变量类型
来源：http://gdq.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pxi.zhixingplan.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vjn.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jqw.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://psm.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sql.jiagoushi.top

Go:   reflect.TypeOf(x).Name()
来源：http://nqv.aibaodan.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lyl.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://uog.zdbjq.cn

[A05] 整数除法与取模
来源：http://jjv.ywan-chungtsiang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iuu.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tjz.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lra.hfpthk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zgy.nanxinkj.top

Java: 7 / 2; 7 % 2
来源：http://aot.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://ghj.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://vvd.svipenyu.cn

C#:   7 / 2; 7 % 2
来源：http://dxs.kuanghao11.cn

[A06] 字符串转数字
来源：http://cpn.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://yks.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kqq.zhixingplan.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://puq.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://gwl.jinyuanbaomall.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dsb.shanyushiyangtech.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fpr.zdqjudy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dwq.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zrk.yueranfly.top

[A07] 数字转字符串
来源：http://hqq.shangyingyoupin.top

Py:   str(42)
来源：http://kkt.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://kbp.xylfe.cn

JS:   String(42); (42).toString()
来源：http://fpn.yonumen.top

TS:   String(42)
来源：http://xat.mhx1999.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vou.daria6918.cn

Go:   strconv.Itoa(42)
来源：http://wal.jqgfzy.top

Ruby: 42.to_s
来源：http://ldg.yueranfly.top

C#:   42.ToString()
来源：http://mkr.hywenlv.cn

[A08] 取整与四舍五入
来源：http://say.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ezm.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kak.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wzc.fktsv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://clv.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zed.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ags.yvedp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rgl.jyoumei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://npc.yuanzhike.top

[A09] 绝对值与最大最小值
来源：http://vrs.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ktf.yuxming.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lgp.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ixs.yonumen.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jgv.haohaochexian.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bfh.yuxming.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zur.hongshengwenyu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://law.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tzn.xinyue.icu

[A10] 生成随机数
来源：http://spz.ppjwa.cn

Py:   import random; random.randint(1, 100)
来源：http://mnb.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://axe.jyoumei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tfa.shzxlz.cn


<!-- 参考信息 -->