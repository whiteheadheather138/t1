代发 wailian999

[U61] PHP：正则
来源：http://gjg.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nxa.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://nbs.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://swo.yongpay.top

[U63] PHP：文件读写
来源：http://mhc.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yev.cucudq.cn

[U64] PHP：目录遍历
来源：http://xot.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://zwn.cucudq.cn

[U65] PHP：会话
来源：http://jmg.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://rqy.tanke756.top

[U66] PHP：设置 Cookie
来源：http://woy.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cts.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://vtk.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ztd.guannengcc.top

[U68] PHP：PDO 连接
来源：http://pts.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ivy.316326.xyz

[U69] PHP：PDO 预处理
来源：http://kfw.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fcp.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://yng.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rok.andypj.xyz

[U71] PHP：抛出异常
来源：http://vtf.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://dac.cqqwz.cn

[U72] PHP：写错误日志
来源：http://yst.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://bml.cdnleiting.top

[U73] PHP：读取 ini 配置
来源：http://ohi.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://bhz.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://kxl.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://dga.jiagoushi.top

[U75] PHP：依赖注入
来源：http://whj.ywan-chungtsiang.top

composer require psr/container
来源：http://wab.jinqigfzy.top

[U76] PHP：简单路由
来源：http://vqg.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cuk.yangfankeji.com

[U77] PHP：模板渲染
来源：http://olt.snrcjt.cn

composer require twig/twig
来源：http://kpr.gzhubu.top

[U78] PHP：单元测试
来源：http://pcx.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://zch.mhx1999.top

[U79] PHP：静态分析
来源：http://tof.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://wzo.xinyue.icu

[U80] PHP：代码规范修复
来源：http://avd.dianchejie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ltn.hesvh.cn

[U81] JS：初始化项目
来源：http://qmv.fehbvm.com

npm init -y;  npm i express
来源：http://nfu.fehbvm.com

[U82] JS：package.json 脚本
来源：http://tcd.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hfw.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://nwk.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://kgo.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://elt.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://ufl.jiagoushi.top

[U85] JS：可选链
来源：http://fls.fktsv.cn

a?.b?.c
来源：http://dtf.epnwcf.com

[U86] JS：空值合并
来源：http://dol.cdnleiting.top

a ?? b
来源：http://bzz.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://coz.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://hkw.fzhhl.top

[U88] JS：对象展开合并
来源：http://naz.yuxming.cn

{ ...a, ...b }
来源：http://day.yonumen.top

[U89] JS：数组去重
来源：http://xes.ehwqpu.com

[...new Set(arr)]
来源：http://lpy.chenlongwang.top

[U90] JS：数字数组排序
来源：http://sza.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://jpy.cheryme.top

[U91] JS：对象键值遍历
来源：http://rro.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kap.fzhhl.top

[U92] JS：深拷贝
来源：http://lum.jyoumei.cn

structuredClone(obj)
来源：http://xtb.zycfv.cn

[U93] JS：模板字符串
来源：http://oqr.zhongyouzk.top

`共 ${n} 条`
来源：http://rqv.aizwys.cn

[U94] JS：箭头函数
来源：http://nbb.cqqwz.cn

const double = x => x * 2;
来源：http://sfk.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://zoj.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://txg.meibo888.top

[U96] JS：async/await 与异常
来源：http://dyh.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kxu.gzhubu.top

[U97] JS：并发请求
来源：http://cxs.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yej.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://loc.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xog.dianchejie.cn

[U99] JS：事件监听
来源：http://hqq.yuanzhike.top

el.addEventListener("click", e => {})
来源：http://gid.sufxvd.cn

[U100] JS：DOM 查询
来源：http://jda.cashguo.top

document.querySelector(".item")
来源：http://dss.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://dqf.cheryme.top

el.classList.toggle("active")
来源：http://qyz.iojbl.cn

[U102] JS：本地存储
来源：http://idk.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kvk.mhx1999.top

[U103] JS：定时器
来源：http://ltw.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lnh.yangfankeji.com

[U104] JS：防抖
来源：http://rpo.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://krz.fehbvm.com

[U105] JS：节流
来源：http://roa.hongshengwenyu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vwb.zdqjudy.top

[U106] JS：日期格式化
来源：http://jtz.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uwm.uphjek.com

[U107] JS：数字千分位
来源：http://egr.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gex.cashguo.top

[U108] JS：随机整数
来源：http://nro.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vdn.gotoacloud.top

[U109] JS：数组分组
来源：http://hmi.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://rnx.zhengqikj.top

[U110] JS：数组分块
来源：http://iky.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hej.ydzc1.top

[U111] JS：对象转 Map
来源：http://wpp.nwbrower.top

new Map(Object.entries(obj))
来源：http://qkj.sweek.top

[U112] JS：字符串补位
来源：http://dui.yanxiufei.cn

"7".padStart(3, "0")
来源：http://qil.ivvv.top

[U113] JS：正则替换全部
来源：http://fkc.andypj.xyz

s.replaceAll("a", "b")
来源：http://kgu.ybcxt.top

[U114] JS：JSON 深比较
来源：http://foi.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://trr.0kj1m.cn

[U115] JS：生成 UUID
来源：http://vik.zhongyouzk.top

crypto.randomUUID()
来源：http://efs.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://vya.gaohongyu789.top

/** @param {string} name */ function f(name) {}
来源：http://lji.birdmap.top

[U117] JS：单元测试
来源：http://sfv.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://fpl.cucudq.cn

[U118] JS：开发服务器
来源：http://vvq.iojbl.cn

npm i -D vite;  npx vite
来源：http://zgr.sjlbkw.cn

[U119] JS：生产构建
来源：http://yow.xylfe.cn

npx vite build
来源：http://khp.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://lyi.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://qlc.sjlbkw.cn

================================================================================
来源：http://ega.nwbrower.top

统计汇总
来源：http://vnu.gaohongyu789.top

================================================================================
来源：http://uqd.shanyushiyangkeji.top

按语言统计（条）：
来源：http://cgw.zycfv.cn

Python ......... 252
来源：http://ldj.zdbjq.cn

PHP ............ 252
来源：http://cwg.wangshuangyany.cn

JavaScript ..... 252
来源：http://jwa.zhoulong.xyz

TypeScript ..... 212
来源：http://dga.pengpengdd.cyou

Java ........... 212
来源：http://cvz.meibo888.top

Go ............. 212
来源：http://xnn.zdbjq.cn

Ruby ........... 212
来源：http://psw.zhongyouzk.top

C# ............. 212
来源：http://sfr.aibaodan.cn

C .............. 30
来源：http://iqy.svipenyu.cn

C++ ............ 30
来源：http://izn.ctjpmb.com

SQL ............ 90
来源：http://zdz.xingfuxueyuan.xyz

Bash ........... 80
来源：http://ucb.vehdjk.com

Kotlin ......... 15
来源：http://cnm.zhixingplan.top

Swift .......... 15
来源：http://xzm.ywan-chungtsiang.top

Lua ............ 10
来源：http://qmj.gzhubu.top

Perl ........... 10
来源：http://tnc.52xcode.cn

Scala .......... 10
来源：http://udr.cheryme.top

------------------------------------
来源：http://buj.meibo888.top

合计 ........... 2106 条
来源：http://dzw.quarkkingdee.top

按章节统计：
来源：http://kqs.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oyl.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bqu.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fba.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yhu.yangfankeji.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jmw.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pwm.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://epq.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fts.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rsb.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://edb.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fss.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://are.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://eyb.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://szq.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jbo.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yfn.shzxlz.cn

Q SQL 专题                              90
来源：http://pex.9152youxi.cn

R Bash 专题                             80
来源：http://yae.daria6918.cn

S C / C++ 专题                          60
来源：http://glz.feifeiyinyue.top

T 其他语言补充                          60
来源：http://urc.vqdsnc.cn

U 高频实用片段                         120
来源：http://vcq.ppjwa.cn

------------------------------------
来源：http://oyb.hfpthk.cn

合计                                  2106 条
来源：http://hqr.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://aej.nanxuanxn.top

使用提醒
来源：http://ygm.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://oav.sxryk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uyn.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uho.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iid.hcnkem.com

在旧版本上使用前请先确认语法支持情况。
来源：http://mcl.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zcf.quarkkingdee.top

—— 文件结束 ——
来源：http://itx.jianghu66.top

================================================================================
来源：http://pny.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://xdx.yangfankeji.com

Common Programming Examples Cheat Book
来源：http://rew.sxryk.cn

================================================================================
来源：http://ijk.guowangkeji.top

【收录内容】
来源：http://dji.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kpc.sysykeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gqa.hammf.cn

SQL · Bash · C · C++
来源：http://ibj.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gci.jiagoushi.top

【使用说明】
来源：http://ohv.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ycg.fengsongda.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pve.yonumen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hqp.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oii.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://adt.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gze.feifeiyinyue.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pks.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xnp.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gds.zhongyouzk.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://axg.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cfb.havefunace.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mfy.xuetiantiany.cn

【文件统计】
来源：http://peu.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ylm.bbcook.cn

--------------------------------------------------------------------------------
来源：http://zxt.jqgufenzy.top

目  录
来源：http://xjn.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ddy.aizwys.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kyy.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bou.jinyuanbaomall.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kgo.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://spk.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ffk.sweek.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yxr.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://azc.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qcf.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://juc.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rzb.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yoa.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://otf.fengsongda.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gob.hnxiangtu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ulu.shanyushiyangtech.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xyd.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yiy.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gym.yuxming.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://neg.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vvg.zycfv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://juz.shuidangran.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ggs.gzhubu.top

================================================================================
来源：http://mag.shanyushiyangtech.top

A. 基础语法与类型
来源：http://wdx.ydjk.org.cn

================================================================================
来源：http://bgh.hesvh.cn

[A01] Hello World
来源：http://fqk.nwbrower.top

Py:   print("Hello, World!")
来源：http://fdq.hfpthk.cn

PHP:  echo "Hello, World!";
来源：http://bvb.xuetiantiany.cn

JS:   console.log("Hello, World!");
来源：http://hzz.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hpl.quarkkingdee.top

Java: System.out.println("Hello, World!");
来源：http://kfe.nanxinkj.top

Go:   fmt.Println("Hello, World!")
来源：http://ows.dianchejie.cn

Ruby: puts "Hello, World!"
来源：http://ghv.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kje.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://ary.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vdt.0kj1m.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pnd.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ixw.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rmg.fzhhl.top

Java: String name = "Alex"; int age = 20;
来源：http://tcq.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://yaw.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://fof.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://aox.nanxuanxn.top

[A03] 常量定义
来源：http://jtc.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ojz.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://qvi.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://opl.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://sne.tian-w.cn

Java: static final double PI = 3.14159;
来源：http://gbb.hammf.cn

Go:   const PI = 3.14159
来源：http://dyn.tian-w.cn

Ruby: PI = 3.14159
来源：http://jnp.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://iqv.uphjek.com

[A04] 判断变量类型
来源：http://ase.yuanzhike.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://brd.guowangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fgu.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sgy.zhijiandao.cn

TS:   typeof x; x instanceof Date
来源：http://vej.jiagoushi.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mzi.hnqzz.top

Go:   reflect.TypeOf(x).Name()
来源：http://yzk.xingfuxueyuan.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://awy.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://pjx.ivvv.top

[A05] 整数除法与取模
来源：http://wah.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eej.yfazqb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://cvt.hammf.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fcs.jqgufenzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gjv.xziqi.cn

Java: 7 / 2; 7 % 2
来源：http://tch.yfazqb.com

Go:   7 / 2; 7 % 2
来源：http://wve.fanxiaobao.xyz

Ruby: 7 / 2; 7 % 2
来源：http://maq.hesvh.cn

C#:   7 / 2; 7 % 2
来源：http://dpf.yonumen.top

[A06] 字符串转数字
来源：http://ses.jinqigfzy.top

Py:   int("42"); float("3.14")
来源：http://vql.guannengcc.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kft.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cwc.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://xbk.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zon.chenlongwang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://djp.ppjwa.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rsa.xziqi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wav.pengpengdd.cyou

[A07] 数字转字符串
来源：http://ere.guowangkeji.top

Py:   str(42)
来源：http://xbz.gogol.net.cn

PHP:  (string) 42; strval(42)
来源：http://dic.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://eey.zhaomingkeji.xyz

TS:   String(42)
来源：http://qoc.ywan-chungtsiang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xfa.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://klv.zhiwuduotai.top

Ruby: 42.to_s
来源：http://qhy.tian-w.cn

C#:   42.ToString()
来源：http://tjf.xylfe.cn

[A08] 取整与四舍五入
来源：http://faq.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pgq.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hnu.zhiwuduotai.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mqe.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eud.zdbjq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tck.hnqzz.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://frb.shanyushiyangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lvq.zhaomingkeji.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fge.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://kke.jinqigfzy.top


<!-- 参考信息 -->