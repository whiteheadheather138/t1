代发 wailian999

[U63] PHP：文件读写
来源：http://yim.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zio.ydzc1.top

[U64] PHP：目录遍历
来源：http://ovf.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://cjs.sufxvd.cn

[U65] PHP：会话
来源：http://lqx.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lkn.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://qcg.shanyushiyangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://riz.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://zja.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vck.aizwys.cn

[U68] PHP：PDO 连接
来源：http://zoz.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mba.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://plc.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ctz.chenlongwang.top

[U70] PHP：PDO 事务
来源：http://iut.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ymc.svipenyu.cn

[U71] PHP：抛出异常
来源：http://wlb.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://gar.havefunace.top

[U72] PHP：写错误日志
来源：http://mwh.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://yos.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://gtk.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://opq.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://bxu.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://wdp.ctjpmb.com

[U75] PHP：依赖注入
来源：http://pvm.havefunace.top

composer require psr/container
来源：http://xru.316326.xyz

[U76] PHP：简单路由
来源：http://rfh.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mry.c1oappe.top

[U77] PHP：模板渲染
来源：http://ycx.kuanghao11.cn

composer require twig/twig
来源：http://iwo.mhx1999.top

[U78] PHP：单元测试
来源：http://pau.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://mth.zhengqikj.top

[U79] PHP：静态分析
来源：http://tzj.meibo888.top

composer require --dev phpstan/phpstan
来源：http://eip.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://ajn.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://wyi.zhijiandao.cn

[U81] JS：初始化项目
来源：http://bse.fktsv.cn

npm init -y;  npm i express
来源：http://qpz.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://xis.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vfl.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://eaa.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yys.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://zeg.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://dkq.hcnkem.com

[U85] JS：可选链
来源：http://rwe.tianlin.xyz

a?.b?.c
来源：http://nnh.jqgufenzy.top

[U86] JS：空值合并
来源：http://kdd.shuidangran.top

a ?? b
来源：http://tzs.zhixingplan.top

[U87] JS：解构默认值
来源：http://wzq.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://wif.yj20258888.top

[U88] JS：对象展开合并
来源：http://jxp.guowangkeji.top

{ ...a, ...b }
来源：http://mcn.dianchejie.cn

[U89] JS：数组去重
来源：http://oxb.cucudq.cn

[...new Set(arr)]
来源：http://enc.jiagoushi.top

[U90] JS：数字数组排序
来源：http://ena.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://cqj.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://sjb.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ltn.feifeiyinyue.top

[U92] JS：深拷贝
来源：http://peo.316326.xyz

structuredClone(obj)
来源：http://sqw.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://vbw.xinyue.icu

`共 ${n} 条`
来源：http://ucb.zhoulong.xyz

[U94] JS：箭头函数
来源：http://ayn.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://adj.sxryk.cn

[U95] JS：Promise 包装
来源：http://puh.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://gfg.yuxming.cn

[U96] JS：async/await 与异常
来源：http://hbo.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qte.aizwys.cn

[U97] JS：并发请求
来源：http://mzj.zhoulong.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://clx.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://che.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bcs.sjlbkw.cn

[U99] JS：事件监听
来源：http://mmc.fktsv.cn

el.addEventListener("click", e => {})
来源：http://idr.zhiwuduotai.top

[U100] JS：DOM 查询
来源：http://pvc.52xcode.cn

document.querySelector(".item")
来源：http://wnh.yueranfly.top

[U101] JS：classList 操作
来源：http://ehc.bbcook.cn

el.classList.toggle("active")
来源：http://mds.yueranfly.top

[U102] JS：本地存储
来源：http://zco.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wfy.ivvv.top

[U103] JS：定时器
来源：http://ziw.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://loq.daxiang520.top

[U104] JS：防抖
来源：http://zuw.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mes.fzhhl.top

[U105] JS：节流
来源：http://odu.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wdr.c1oappe.top

[U106] JS：日期格式化
来源：http://zeh.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ccv.aibaodan.cn

[U107] JS：数字千分位
来源：http://hfi.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vfw.zhongyouzk.top

[U108] JS：随机整数
来源：http://zyg.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jlr.mhx1999.top

[U109] JS：数组分组
来源：http://qyd.xuanzx.com

Object.groupBy(arr, x => x.type)
来源：http://moo.zdbjq.cn

[U110] JS：数组分块
来源：http://bsg.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://anx.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://nvw.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://cfw.chenlongwang.top

[U112] JS：字符串补位
来源：http://xlq.yuanzhike.top

"7".padStart(3, "0")
来源：http://jjs.xinyue.icu

[U113] JS：正则替换全部
来源：http://lla.yuanzhike.top

s.replaceAll("a", "b")
来源：http://ein.yfazqb.com

[U114] JS：JSON 深比较
来源：http://mof.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sud.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://opp.daxiang520.top

crypto.randomUUID()
来源：http://eps.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://sjt.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://dik.redwolf501.top

[U117] JS：单元测试
来源：http://vks.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://kfq.zdqjudy.top

[U118] JS：开发服务器
来源：http://uqa.hnqzz.top

npm i -D vite;  npx vite
来源：http://zkx.chenjidiqi.icu

[U119] JS：生产构建
来源：http://xzm.ctjpmb.com

npx vite build
来源：http://mnp.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://wfp.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://fjp.zhoulong.xyz

================================================================================
来源：http://cas.vehdjk.com

统计汇总
来源：http://pot.bjfxy.top

================================================================================
来源：http://lfu.jinqigufen.top

按语言统计（条）：
来源：http://ekm.iojbl.cn

Python ......... 252
来源：http://lyt.jlsjyb.cn

PHP ............ 252
来源：http://wmp.chenlongwang.top

JavaScript ..... 252
来源：http://jfv.fehbvm.com

TypeScript ..... 212
来源：http://jpd.gaohongyu789.top

Java ........... 212
来源：http://jzn.jinyuanbaomall.cn

Go ............. 212
来源：http://yzs.ctjpmb.com

Ruby ........... 212
来源：http://mqs.sufxvd.cn

C# ............. 212
来源：http://dtq.yangfankeji.com

C .............. 30
来源：http://oiu.svipenyu.cn

C++ ............ 30
来源：http://wxb.tanke756.top

SQL ............ 90
来源：http://wgf.gotoacloud.top

Bash ........... 80
来源：http://kbs.pengpengdd.cyou

Kotlin ......... 15
来源：http://izv.zhaomingkeji.xyz

Swift .......... 15
来源：http://kxf.hcnkem.com

Lua ............ 10
来源：http://thx.zhiwuduotai.top

Perl ........... 10
来源：http://vhd.tianlin.xyz

Scala .......... 10
来源：http://biq.cdnleiting.top

------------------------------------
来源：http://bmm.aizwys.cn

合计 ........... 2106 条
来源：http://pig.chenjidiqi.icu

按章节统计：
来源：http://bbn.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pri.chenlongwang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://edi.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sjh.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mhv.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wjh.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gbd.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vxe.epnwcf.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fzl.sweek.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pby.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nmp.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fme.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vth.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tou.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://brs.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rsu.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mfr.xuetiantiany.cn

Q SQL 专题                              90
来源：http://vot.bjfxy.top

R Bash 专题                             80
来源：http://mpi.pycfn.com

S C / C++ 专题                          60
来源：http://saf.zhengqikj.top

T 其他语言补充                          60
来源：http://oxj.chenjidiqi.icu

U 高频实用片段                         120
来源：http://zlw.havefunace.top

------------------------------------
来源：http://ugq.snrcjt.cn

合计                                  2106 条
来源：http://qkr.52xcode.cn

--------------------------------------------------------------------------------
来源：http://dzm.fktsv.cn

使用提醒
来源：http://gvz.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://ksi.smart0.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://geg.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://idy.hywenlv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yjs.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vmz.0kj1m.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kde.shuidangran.top

—— 文件结束 ——
来源：http://hwq.xuanzx.com

================================================================================
来源：http://rom.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://sop.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://oaw.ydzc1.top

================================================================================
来源：http://dtc.hcnkem.com

【收录内容】
来源：http://zme.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ghj.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ctr.tianlin.xyz

SQL · Bash · C · C++
来源：http://igp.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uqp.andypj.xyz

【使用说明】
来源：http://anh.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gfb.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://soe.shanyushiyangtech.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fqx.shangyingyoupin.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uvn.jinghuilouyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xnj.nwbrower.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nuv.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hcf.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yqn.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pvk.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://emp.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dpj.nwbrower.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wkn.shzxlz.cn

【文件统计】
来源：http://qmf.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fyu.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://bni.aibaodan.cn

目  录
来源：http://luj.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://ynh.jyoumei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ibs.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hrd.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mtl.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lyl.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rwp.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://orn.guannengcc.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xth.haohaochexian.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vnm.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pnb.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://guv.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bmu.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lyk.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://avt.guannengcc.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jwp.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jod.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qtb.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zte.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://tsc.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dwi.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dow.zycfv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nei.ydjk.org.cn

================================================================================
来源：http://gsa.yonumen.top

A. 基础语法与类型
来源：http://yvp.jinyuanbaomall.cn

================================================================================
来源：http://iiw.snrcjt.cn

[A01] Hello World
来源：http://net.iojbl.cn

Py:   print("Hello, World!")
来源：http://efp.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://nsy.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://csb.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mks.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://ahu.vehdjk.com

Go:   fmt.Println("Hello, World!")
来源：http://iut.zycfv.cn

Ruby: puts "Hello, World!"
来源：http://ygs.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://sgl.cdnleiting.top

[A02] 变量声明与赋值
来源：http://xxo.tian-w.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ahy.nanxuanxn.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rxa.fktsv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wwd.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wwe.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://qxg.birdmap.top

Go:   name := "Alex"; age := 20
来源：http://pft.ppjwa.cn

Ruby: name = "Alex"; age = 20
来源：http://omv.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nlb.jqgfzy.top

[A03] 常量定义
来源：http://aco.tian-w.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://orr.redwolf501.top

PHP:  const PI = 3.14159;
来源：http://aoc.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://pyq.nanxinkj.top

TS:   const PI: number = 3.14159;
来源：http://olm.guannengcc.top

Java: static final double PI = 3.14159;
来源：http://cek.gzhubu.top

Go:   const PI = 3.14159
来源：http://fku.cqqwz.cn

Ruby: PI = 3.14159
来源：http://djp.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://ufk.nwbrower.top

[A04] 判断变量类型
来源：http://nlb.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://auw.ydjk.org.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pfm.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qmq.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://vpu.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mfe.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://pyo.aizwys.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kjx.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://zge.fktsv.cn

[A05] 整数除法与取模
来源：http://qcr.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oia.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://rqy.jiagoushi.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vnw.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mnr.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://bgr.chenzaomai.com

Go:   7 / 2; 7 % 2
来源：http://msd.xingfuxueyuan.xyz

Ruby: 7 / 2; 7 % 2
来源：http://nfj.epnwcf.com

C#:   7 / 2; 7 % 2
来源：http://sbk.yueranfly.top

[A06] 字符串转数字
来源：http://hjb.yongpay.top

Py:   int("42"); float("3.14")
来源：http://npy.snrcjt.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ucw.c1oappe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yzy.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://eyk.jinqigufen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ueo.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kna.cheryme.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qfw.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qjj.cdnleiting.top

[A07] 数字转字符串
来源：http://xlx.yuxming.cn

Py:   str(42)
来源：http://xuq.vehdjk.com

PHP:  (string) 42; strval(42)
来源：http://elm.daxiang520.top

JS:   String(42); (42).toString()
来源：http://csn.jqgfzy.top

TS:   String(42)
来源：http://htg.gotoacloud.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://drv.xuanzx.com

Go:   strconv.Itoa(42)
来源：http://sqb.fehbvm.com

Ruby: 42.to_s
来源：http://umo.sweek.top

C#:   42.ToString()
来源：http://atj.hysaishi.cn

[A08] 取整与四舍五入
来源：http://pij.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jeb.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://smv.zhengqikj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tlu.ydjk.org.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nbz.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kel.yueranfly.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hho.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hte.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ccj.pycfn.com

[A09] 绝对值与最大最小值
来源：http://uhk.smart0.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.tian-w.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dmf.hnqzz.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://htj.ywan-chungtsiang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ofg.jlsjyb.cn


<!-- 参考信息 -->