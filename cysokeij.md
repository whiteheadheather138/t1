代发 wailian999

[U67] PHP：处理文件上传
来源：http://bdf.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zev.cheryme.top

[U68] PHP：PDO 连接
来源：http://les.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wbi.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://kiu.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ouk.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://pva.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hto.yfazqb.com

[U71] PHP：抛出异常
来源：http://iny.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://hhz.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://cla.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://ybj.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://mmo.ydzc1.top

parse_ini_file("config.ini", true)
来源：http://qbh.guannengcc.top

[U74] PHP：读取环境变量
来源：http://tgv.daria6918.cn

getenv("APP_ENV") ?: "production"
来源：http://hlw.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://qks.fzhhl.top

composer require psr/container
来源：http://rsk.dianchejie.cn

[U76] PHP：简单路由
来源：http://epc.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gwv.guannengcc.top

[U77] PHP：模板渲染
来源：http://srg.jqgfzy.top

composer require twig/twig
来源：http://glw.cqqwz.cn

[U78] PHP：单元测试
来源：http://lkc.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://ikk.pycfn.com

[U79] PHP：静态分析
来源：http://kbr.yonumen.top

composer require --dev phpstan/phpstan
来源：http://nit.sxryk.cn

[U80] PHP：代码规范修复
来源：http://uxx.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://yzv.ybcxt.top

[U81] JS：初始化项目
来源：http://qcm.zhoulong.xyz

npm init -y;  npm i express
来源：http://tkl.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://iyd.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wkv.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://mly.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dqd.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://rjv.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://qqh.jlsjyb.cn

[U85] JS：可选链
来源：http://dgv.haohaochexian.top

a?.b?.c
来源：http://lzw.fehbvm.com

[U86] JS：空值合并
来源：http://tlf.shangyingyoupin.top

a ?? b
来源：http://enk.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://sfi.yanxiufei.cn

const { a = 1, b = 2 } = obj;
来源：http://xzn.epnwcf.com

[U88] JS：对象展开合并
来源：http://esa.sxryk.cn

{ ...a, ...b }
来源：http://kvr.chenlongwang.top

[U89] JS：数组去重
来源：http://mfu.yangfankeji.com

[...new Set(arr)]
来源：http://sec.kuanghao11.cn

[U90] JS：数字数组排序
来源：http://yxa.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://axn.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://ulc.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pon.jqgufenzy.top

[U92] JS：深拷贝
来源：http://qlz.xuanzx.com

structuredClone(obj)
来源：http://ugx.fengsongda.top

[U93] JS：模板字符串
来源：http://dau.cheryme.top

`共 ${n} 条`
来源：http://glh.birdmap.top

[U94] JS：箭头函数
来源：http://fwo.0kj1m.cn

const double = x => x * 2;
来源：http://etl.sweek.top

[U95] JS：Promise 包装
来源：http://ncx.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://xbr.cqqwz.cn

[U96] JS：async/await 与异常
来源：http://upj.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://img.jinyuanbaomall.cn

[U97] JS：并发请求
来源：http://bru.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gsk.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://hgy.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://alq.jqgfzy.top

[U99] JS：事件监听
来源：http://dvp.xuanzx.com

el.addEventListener("click", e => {})
来源：http://aqv.yj20258.top

[U100] JS：DOM 查询
来源：http://srw.chenzaomai.com

document.querySelector(".item")
来源：http://yma.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://jpe.hnqzz.top

el.classList.toggle("active")
来源：http://kld.guowangkeji.top

[U102] JS：本地存储
来源：http://ppy.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hgv.cucudq.cn

[U103] JS：定时器
来源：http://yum.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://utr.kuanghao11.cn

[U104] JS：防抖
来源：http://jov.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rgt.cheryme.top

[U105] JS：节流
来源：http://qoy.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ktf.chenzaomai.com

[U106] JS：日期格式化
来源：http://ths.nwbrower.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bsv.pengpengdd.cyou

[U107] JS：数字千分位
来源：http://xfp.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://szq.yj20258.top

[U108] JS：随机整数
来源：http://qjw.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cby.yuxming.cn

[U109] JS：数组分组
来源：http://mhx.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://fze.yonumen.top

[U110] JS：数组分块
来源：http://dwr.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://syj.9152youxi.cn

[U111] JS：对象转 Map
来源：http://gau.dashuyun.cn

new Map(Object.entries(obj))
来源：http://fos.yonumen.top

[U112] JS：字符串补位
来源：http://dww.daxiang520.top

"7".padStart(3, "0")
来源：http://rst.52xcode.cn

[U113] JS：正则替换全部
来源：http://npe.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://zmu.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://vil.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://oix.yuanzhike.top

[U115] JS：生成 UUID
来源：http://mrt.shuidangran.top

crypto.randomUUID()
来源：http://udr.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://fwn.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://jpu.jyoumei.cn

[U117] JS：单元测试
来源：http://wfw.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://pfw.andypj.xyz

[U118] JS：开发服务器
来源：http://cxn.zycfv.cn

npm i -D vite;  npx vite
来源：http://gge.zycfv.cn

[U119] JS：生产构建
来源：http://npa.zhaomingkeji.xyz

npx vite build
来源：http://rpj.chenzaomai.com

[U120] JS：读取环境变量（Vite）
来源：http://iuv.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://gnq.yj20258888.top

================================================================================
来源：http://ooa.yvedp.cn

统计汇总
来源：http://ryq.gotoacloud.top

================================================================================
来源：http://uhf.52xcode.cn

按语言统计（条）：
来源：http://jrn.cqqwz.cn

Python ......... 252
来源：http://uwd.fktsv.cn

PHP ............ 252
来源：http://oph.yuanzhike.top

JavaScript ..... 252
来源：http://bdz.daxiang520.top

TypeScript ..... 212
来源：http://ukp.jiagoushi.top

Java ........... 212
来源：http://pql.hnxiangtu.top

Go ............. 212
来源：http://jvs.zhongyouzk.top

Ruby ........... 212
来源：http://yqc.xingfuxueyuan.xyz

C# ............. 212
来源：http://nac.chenlongwang.top

C .............. 30
来源：http://bfh.sjlbkw.cn

C++ ............ 30
来源：http://nwy.gotoacloud.top

SQL ............ 90
来源：http://kue.fzhhl.top

Bash ........... 80
来源：http://ilq.hongshengwenyu.top

Kotlin ......... 15
来源：http://gjq.ivvv.top

Swift .......... 15
来源：http://qrv.zycfv.cn

Lua ............ 10
来源：http://quu.jqgufenzy.top

Perl ........... 10
来源：http://xgp.aibaodan.cn

Scala .......... 10
来源：http://ojc.wangdashe.top

------------------------------------
来源：http://mcl.c1oappe.top

合计 ........... 2106 条
来源：http://xos.jlsjyb.cn

按章节统计：
来源：http://xit.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cjb.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rom.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jpr.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sau.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ikq.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dkx.pengpengdd.cyou

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ajo.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ilx.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://coh.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uau.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mzs.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tlc.vqdsnc.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cuw.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kdi.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vvo.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ebp.zdqjudy.top

Q SQL 专题                              90
来源：http://udy.ctjpmb.com

R Bash 专题                             80
来源：http://pqa.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://amk.zhoulong.xyz

T 其他语言补充                          60
来源：http://agv.dashuyun.cn

U 高频实用片段                         120
来源：http://vct.hfpthk.cn

------------------------------------
来源：http://lpb.jinqigufen.top

合计                                  2106 条
来源：http://ruo.sxryk.cn

--------------------------------------------------------------------------------
来源：http://zyh.xuetiantiany.cn

使用提醒
来源：http://bzt.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://neo.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pca.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xse.kuanghao11.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://glb.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mzk.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ihc.wangdashe.top

—— 文件结束 ——
来源：http://itw.hnxiangtu.top

================================================================================
来源：http://pqq.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://ehn.52xcode.cn

Common Programming Examples Cheat Book
来源：http://duf.sweek.top

================================================================================
来源：http://jme.sweek.top

【收录内容】
来源：http://pzh.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://xok.vehdjk.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://urg.xinyue.icu

SQL · Bash · C · C++
来源：http://qmv.ydjk.org.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ujp.sufxvd.cn

【使用说明】
来源：http://afx.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nzf.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oby.xuanzx.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xqb.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kjp.yvedp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xxe.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://czb.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hfm.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://twc.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dsa.pengpengdd.cyou

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tkl.zhijiandao.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oru.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wdz.jqgfzy.top

【文件统计】
来源：http://wxh.jianghu66.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wde.epnwcf.com

--------------------------------------------------------------------------------
来源：http://mvc.jianghu66.top

目  录
来源：http://tuj.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://nwx.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xin.hesvh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ort.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kbo.hnqzz.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://luh.yuanzhike.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ptl.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cgi.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ghr.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zvk.pengpengdd.cyou

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://psb.vqdsnc.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yxt.sweek.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://euu.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jtg.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jsp.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wvq.cucudq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://odg.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cnp.cheryme.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aon.daria6918.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eje.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oay.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qwl.tarul.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zvr.hammf.cn

================================================================================
来源：http://des.tarul.cn

A. 基础语法与类型
来源：http://xvy.iojbl.cn

================================================================================
来源：http://sga.pengpengdd.cyou

[A01] Hello World
来源：http://iug.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://ssi.hcnkem.com

PHP:  echo "Hello, World!";
来源：http://zei.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://fjy.yangfankeji.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nrr.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://dxo.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://vzw.ydzc1.top

Ruby: puts "Hello, World!"
来源：http://jwb.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ryx.havefunace.top

[A02] 变量声明与赋值
来源：http://kgp.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hro.quarkkingdee.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xeu.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://yzf.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qec.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://lqn.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://guf.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://kiw.xziqi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://uco.zycfv.cn

[A03] 常量定义
来源：http://gtp.hfpthk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://owd.jinghuilouyu.cn

PHP:  const PI = 3.14159;
来源：http://xtd.hesvh.cn

JS:   const PI = 3.14159;
来源：http://zry.iojbl.cn

TS:   const PI: number = 3.14159;
来源：http://ort.wangdashe.top

Java: static final double PI = 3.14159;
来源：http://zpe.ydzc1.top

Go:   const PI = 3.14159
来源：http://bqx.gotoacloud.top

Ruby: PI = 3.14159
来源：http://xep.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://wfe.hesvh.cn

[A04] 判断变量类型
来源：http://ujg.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pov.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://van.quarkkingdee.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tvl.ivvv.top

TS:   typeof x; x instanceof Date
来源：http://seq.zhongyouzk.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gfo.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://siu.pycfn.com

Ruby: x.class; x.is_a?(Integer)
来源：http://olg.nwbrower.top

C#:   x.GetType().Name; x is int
来源：http://fhv.zycfv.cn

[A05] 整数除法与取模
来源：http://aif.fzhhl.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rmo.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://iqj.hysaishi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pdo.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pgx.quarkkingdee.top

Java: 7 / 2; 7 % 2
来源：http://sct.yueranfly.top

Go:   7 / 2; 7 % 2
来源：http://maw.hfpthk.cn

Ruby: 7 / 2; 7 % 2
来源：http://mnj.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://goo.havefunace.top

[A06] 字符串转数字
来源：http://wfe.wangshuangyany.cn

Py:   int("42"); float("3.14")
来源：http://wec.tian-w.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hfl.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://glb.smart0.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://ycp.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ooj.hammf.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uvn.sjlbkw.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vvs.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qxr.xuanzx.com

[A07] 数字转字符串
来源：http://wwh.nanxuanxn.top

Py:   str(42)
来源：http://rfh.jinqigufen.top

PHP:  (string) 42; strval(42)
来源：http://ydo.jinqigufen.top

JS:   String(42); (42).toString()
来源：http://dwj.yongpay.top

TS:   String(42)
来源：http://wno.hongshengwenyu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://txy.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://ymo.hnqzz.top

Ruby: 42.to_s
来源：http://ddt.yongpay.top

C#:   42.ToString()
来源：http://zrt.nwbrower.top

[A08] 取整与四舍五入
来源：http://pys.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aqu.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nkk.zhengqikj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wsh.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jeb.zhongyouzk.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cuo.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ujq.iojbl.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kpk.wangshuangyany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://khr.xylfe.cn

[A09] 绝对值与最大最小值
来源：http://ftr.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nrz.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://csi.jinyuanbaomall.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://swj.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dvi.gogol.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xen.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://czg.guowangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qqr.birdmap.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fid.yuanzhike.top

[A10] 生成随机数
来源：http://tlh.bbcook.cn

Py:   import random; random.randint(1, 100)
来源：http://pdy.hywenlv.cn

PHP:  random_int(1, 100);
来源：http://vgu.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rum.aizwys.cn


<!-- 参考信息 -->