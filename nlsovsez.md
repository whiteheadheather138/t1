代发 wailian999

[U65] PHP：会话
来源：http://htj.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kgu.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://axx.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fcd.cqqwz.cn

[U67] PHP：处理文件上传
来源：http://gcn.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lvs.redwolf501.top

[U68] PHP：PDO 连接
来源：http://gjt.redwolf501.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zbx.cheryme.top

[U69] PHP：PDO 预处理
来源：http://fko.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qom.zdqjudy.top

[U70] PHP：PDO 事务
来源：http://xea.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yvr.wangdashe.top

[U71] PHP：抛出异常
来源：http://nyb.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://lmk.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://etd.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://qrd.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://owo.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://xsz.xinyue.icu

[U74] PHP：读取环境变量
来源：http://qol.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://xxk.smart0.xyz

[U75] PHP：依赖注入
来源：http://zmu.havefunace.top

composer require psr/container
来源：http://qxs.snrcjt.cn

[U76] PHP：简单路由
来源：http://mld.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zhp.hywenlv.cn

[U77] PHP：模板渲染
来源：http://nbm.tianlin.xyz

composer require twig/twig
来源：http://uvz.nanxinkj.top

[U78] PHP：单元测试
来源：http://feq.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://blq.zhongyouzk.top

[U79] PHP：静态分析
来源：http://aft.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://mdi.nwbrower.top

[U80] PHP：代码规范修复
来源：http://fpw.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bzk.cucudq.cn

[U81] JS：初始化项目
来源：http://egt.sweek.top

npm init -y;  npm i express
来源：http://ywr.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://inl.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dku.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://zvp.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://whw.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://pbe.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://qvm.yongpay.top

[U85] JS：可选链
来源：http://ynj.vqdsnc.cn

a?.b?.c
来源：http://dtf.ehwqpu.com

[U86] JS：空值合并
来源：http://lnh.sufxvd.cn

a ?? b
来源：http://kne.dashuyun.cn

[U87] JS：解构默认值
来源：http://rdu.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://ewo.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://swm.316326.xyz

{ ...a, ...b }
来源：http://qzn.smart0.xyz

[U89] JS：数组去重
来源：http://mrl.andypj.xyz

[...new Set(arr)]
来源：http://yoh.hcnkem.com

[U90] JS：数字数组排序
来源：http://nkv.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://xgc.cashguo.top

[U91] JS：对象键值遍历
来源：http://oad.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xpg.yanxiufei.cn

[U92] JS：深拷贝
来源：http://bko.ydjk.org.cn

structuredClone(obj)
来源：http://zsp.xuetiantiany.cn

[U93] JS：模板字符串
来源：http://pmn.chenlongwang.top

`共 ${n} 条`
来源：http://wkt.ydzc1.top

[U94] JS：箭头函数
来源：http://jph.daria6918.cn

const double = x => x * 2;
来源：http://wbh.sysykeji.top

[U95] JS：Promise 包装
来源：http://ftr.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://jdc.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://auh.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rxz.xuanzx.com

[U97] JS：并发请求
来源：http://dmm.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://czx.meibo888.top

[U98] JS：fetch 带 JSON
来源：http://mwc.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hyo.hywenlv.cn

[U99] JS：事件监听
来源：http://hja.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://xbj.birdmap.top

[U100] JS：DOM 查询
来源：http://yqk.jinqigufen.top

document.querySelector(".item")
来源：http://lsj.jiagoushi.top

[U101] JS：classList 操作
来源：http://zfz.yangfankeji.com

el.classList.toggle("active")
来源：http://dcr.shuidangran.top

[U102] JS：本地存储
来源：http://dkj.jianghu66.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qyd.xylfe.cn

[U103] JS：定时器
来源：http://ypm.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lqr.hnqzz.top

[U104] JS：防抖
来源：http://sau.xziqi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxu.yj20258.top

[U105] JS：节流
来源：http://yzn.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hwf.dashuyun.cn

[U106] JS：日期格式化
来源：http://gyr.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rcr.aizwys.cn

[U107] JS：数字千分位
来源：http://eac.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ily.zhijiandao.cn

[U108] JS：随机整数
来源：http://yte.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vev.xylfe.cn

[U109] JS：数组分组
来源：http://sjx.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://cla.bjfxy.top

[U110] JS：数组分块
来源：http://gmk.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lbf.shzxlz.cn

[U111] JS：对象转 Map
来源：http://xhj.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://hcs.uphjek.com

[U112] JS：字符串补位
来源：http://lzw.smart0.xyz

"7".padStart(3, "0")
来源：http://xrd.smart0.xyz

[U113] JS：正则替换全部
来源：http://tpn.nanxinkj.top

s.replaceAll("a", "b")
来源：http://zvj.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://itr.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://smc.fehbvm.com

[U115] JS：生成 UUID
来源：http://amz.pengpengdd.cyou

crypto.randomUUID()
来源：http://lql.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://naw.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://hfx.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://jhy.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://ckw.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://rte.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://daj.meibo888.top

[U119] JS：生产构建
来源：http://heg.yfazqb.com

npx vite build
来源：http://muw.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://hqy.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://eou.ybcxt.top

================================================================================
来源：http://cay.fktsv.cn

统计汇总
来源：http://ass.chenzaomai.com

================================================================================
来源：http://zal.vqdsnc.cn

按语言统计（条）：
来源：http://oxi.ywan-chungtsiang.top

Python ......... 252
来源：http://zve.c1oappe.top

PHP ............ 252
来源：http://maw.guowangkeji.top

JavaScript ..... 252
来源：http://npb.guowangkeji.top

TypeScript ..... 212
来源：http://ezj.hammf.cn

Java ........... 212
来源：http://nup.iojbl.cn

Go ............. 212
来源：http://rfo.shangyingyoupin.top

Ruby ........... 212
来源：http://cnr.daxiang520.top

C# ............. 212
来源：http://lcx.xylfe.cn

C .............. 30
来源：http://akn.zhaomingkeji.xyz

C++ ............ 30
来源：http://bhe.wangdashe.top

SQL ............ 90
来源：http://yhj.nanxinkj.top

Bash ........... 80
来源：http://iha.ehwqpu.com

Kotlin ......... 15
来源：http://vab.hysaishi.cn

Swift .......... 15
来源：http://ytf.ydzc1.top

Lua ............ 10
来源：http://dkc.316326.xyz

Perl ........... 10
来源：http://nmv.yj202588.top

Scala .......... 10
来源：http://ooz.0kj1m.cn

------------------------------------
来源：http://mxh.hnqzz.top

合计 ........... 2106 条
来源：http://zfd.ppjwa.cn

按章节统计：
来源：http://odo.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nuq.daria6918.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iqk.cashguo.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lor.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vze.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xdr.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aem.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hxd.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://evp.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iiw.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ywa.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nbt.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kww.jqgufenzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bio.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ngr.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://syv.andypj.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wkc.hcnkem.com

Q SQL 专题                              90
来源：http://esc.xylfe.cn

R Bash 专题                             80
来源：http://kah.guannengcc.top

S C / C++ 专题                          60
来源：http://vtr.ydjk.org.cn

T 其他语言补充                          60
来源：http://irr.redwolf501.top

U 高频实用片段                         120
来源：http://zys.yvedp.cn

------------------------------------
来源：http://jxz.fehbvm.com

合计                                  2106 条
来源：http://vwt.fengsongda.top

--------------------------------------------------------------------------------
来源：http://jcj.snrcjt.cn

使用提醒
来源：http://zyr.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://xyj.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vsq.mhx1999.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ixx.yj20258888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tbh.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ahl.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qwi.aizwys.cn

—— 文件结束 ——
来源：http://qbh.xingfuxueyuan.xyz

================================================================================
来源：http://tmy.ydjk.org.cn

程序语言常见例子速查手册（2024 版）
来源：http://evs.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://wot.zhengqikj.top

================================================================================
来源：http://eqn.feifeiyinyue.top

【收录内容】
来源：http://fcg.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lcm.pengpengdd.cyou

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qjg.shzxlz.cn

SQL · Bash · C · C++
来源：http://wtm.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zcf.aizwys.cn

【使用说明】
来源：http://iqd.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mkz.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dal.jqgfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dhl.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tfj.sufxvd.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ajh.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cye.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://etb.snrcjt.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fdb.sweek.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ojf.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rwa.mhx1999.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://njg.aibaodan.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fjz.uphjek.com

【文件统计】
来源：http://mvd.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hmi.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://mty.tarul.cn

目  录
来源：http://vib.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://yoh.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xgd.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tdl.dashuyun.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kca.cdnleiting.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yew.chenzaomai.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ttn.sjlbkw.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xbs.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kfg.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zbb.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vai.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://enk.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rkz.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xma.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rjt.gogol.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gep.yfazqb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hps.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mnn.shanyushiyangtech.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kcq.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://tzc.ydzc1.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ckx.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ejv.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zgq.xinyue.icu

================================================================================
来源：http://lax.dianchejie.cn

A. 基础语法与类型
来源：http://emu.wangdashe.top

================================================================================
来源：http://qyh.iojbl.cn

[A01] Hello World
来源：http://bcs.uphjek.com

Py:   print("Hello, World!")
来源：http://iyr.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://dpu.nwbrower.top

JS:   console.log("Hello, World!");
来源：http://tcl.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tec.chenzaomai.com

Java: System.out.println("Hello, World!");
来源：http://ipw.0kj1m.cn

Go:   fmt.Println("Hello, World!")
来源：http://hax.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://low.yonumen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xrh.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://xva.xinyue.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iwa.smart0.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://amx.pengpengdd.cyou

JS:   let name = "Alex"; const age = 20;
来源：http://twn.yuxming.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ywy.fanxiaobao.xyz

Java: String name = "Alex"; int age = 20;
来源：http://hxj.gzhubu.top

Go:   name := "Alex"; age := 20
来源：http://xwj.jinqigufen.top

Ruby: name = "Alex"; age = 20
来源：http://vae.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gzy.wangdashe.top

[A03] 常量定义
来源：http://skb.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://emj.shzxlz.cn

PHP:  const PI = 3.14159;
来源：http://ubn.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://avb.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://fjh.yfazqb.com

Java: static final double PI = 3.14159;
来源：http://wdl.fzhhl.top

Go:   const PI = 3.14159
来源：http://pen.feifeiyinyue.top

Ruby: PI = 3.14159
来源：http://jnj.hywenlv.cn

C#:   const double PI = 3.14159;
来源：http://gam.gogol.net.cn

[A04] 判断变量类型
来源：http://hjh.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gcn.shanyushiyangtech.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zqr.xinyue.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ddv.jiagoushi.top

TS:   typeof x; x instanceof Date
来源：http://npv.iojbl.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tnz.chenjidiqi.icu

Go:   reflect.TypeOf(x).Name()
来源：http://rbs.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://and.yangfankeji.com

C#:   x.GetType().Name; x is int
来源：http://hhh.zhongyouzk.top

[A05] 整数除法与取模
来源：http://ujf.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://asp.ivvv.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fqz.zdqjudy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://piu.xingfuxueyuan.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://goe.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://vkr.aibaodan.cn

Go:   7 / 2; 7 % 2
来源：http://bwx.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://gfc.jinqigfzy.top

C#:   7 / 2; 7 % 2
来源：http://opr.dianchejie.cn

[A06] 字符串转数字
来源：http://qjl.yanxiufei.cn

Py:   int("42"); float("3.14")
来源：http://zqu.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://erf.hysaishi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gaz.shangyingyoupin.top

TS:   parseInt("42", 10); Number("42")
来源：http://xrn.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gqc.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cjy.ydjk.org.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hdf.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ntg.jiagoushi.top

[A07] 数字转字符串
来源：http://req.ywan-chungtsiang.top

Py:   str(42)
来源：http://sec.xuanzx.com

PHP:  (string) 42; strval(42)
来源：http://ssb.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://czd.shanyushiyangtech.top

TS:   String(42)
来源：http://zih.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qlj.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://cec.cheryme.top

Ruby: 42.to_s
来源：http://vkk.yj202588.top

C#:   42.ToString()
来源：http://mdt.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://bob.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nxp.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gju.zhoulong.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vzs.jyoumei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eif.andypj.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ztx.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dhb.mhx1999.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lky.guannengcc.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tsj.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://mgh.mhx1999.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wdb.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ivj.chenjidiqi.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gpz.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rai.yj20258.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xvg.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nxm.shanyushiyangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://taa.yj20258888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zdw.jlsjyb.cn


<!-- 参考信息 -->