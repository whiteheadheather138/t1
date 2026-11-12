代发 wailian999

[U65] PHP：会话
来源：http://ovr.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hlp.daxiang520.top

[U66] PHP：设置 Cookie
来源：http://kcw.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hvg.hesvh.cn

[U67] PHP：处理文件上传
来源：http://dyz.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bto.tian-w.cn

[U68] PHP：PDO 连接
来源：http://pwv.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fjn.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://vcy.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kqi.pycfn.com

[U70] PHP：PDO 事务
来源：http://fqn.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hlf.dashuyun.cn

[U71] PHP：抛出异常
来源：http://img.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://yyy.yj202588.top

[U72] PHP：写错误日志
来源：http://gtw.jyoumei.cn

error_log("失败: " . $e->getMessage());
来源：http://njp.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://gxd.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://inu.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://bqt.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://uls.zhixingplan.top

[U75] PHP：依赖注入
来源：http://hbm.zycfv.cn

composer require psr/container
来源：http://thi.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://efa.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rvk.tianlin.xyz

[U77] PHP：模板渲染
来源：http://qcb.meibo888.top

composer require twig/twig
来源：http://clc.hywenlv.cn

[U78] PHP：单元测试
来源：http://gcw.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://ooj.wangdashe.top

[U79] PHP：静态分析
来源：http://agp.yj202588.top

composer require --dev phpstan/phpstan
来源：http://nia.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://amt.yueranfly.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vvx.sxryk.cn

[U81] JS：初始化项目
来源：http://bhc.ivvv.top

npm init -y;  npm i express
来源：http://mxa.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://fyy.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ens.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://hxt.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zyq.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://ijs.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://ukm.yvedp.cn

[U85] JS：可选链
来源：http://zsa.zhengqikj.top

a?.b?.c
来源：http://ydg.pycfn.com

[U86] JS：空值合并
来源：http://hun.xziqi.cn

a ?? b
来源：http://kup.c1oappe.top

[U87] JS：解构默认值
来源：http://ckq.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://uvz.52xcode.cn

[U88] JS：对象展开合并
来源：http://yvy.mhx1999.top

{ ...a, ...b }
来源：http://yop.xziqi.cn

[U89] JS：数组去重
来源：http://odt.fktsv.cn

[...new Set(arr)]
来源：http://yfa.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://tjh.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://bew.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://ssq.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vxh.jiagoushi.top

[U92] JS：深拷贝
来源：http://qvs.sjlbkw.cn

structuredClone(obj)
来源：http://jsv.hcnkem.com

[U93] JS：模板字符串
来源：http://muu.guannengcc.top

`共 ${n} 条`
来源：http://rjm.kuanghao11.cn

[U94] JS：箭头函数
来源：http://lqh.jqgfzy.top

const double = x => x * 2;
来源：http://oam.wangdashe.top

[U95] JS：Promise 包装
来源：http://oxh.uphjek.com

new Promise((resolve, reject) => {})
来源：http://skw.ydzc1.top

[U96] JS：async/await 与异常
来源：http://ryy.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://irw.hywenlv.cn

[U97] JS：并发请求
来源：http://vne.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yvg.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://eje.yongpay.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sss.snrcjt.cn

[U99] JS：事件监听
来源：http://nqi.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://phk.zhixingplan.top

[U100] JS：DOM 查询
来源：http://rke.shanyushiyangtech.top

document.querySelector(".item")
来源：http://uve.cheryme.top

[U101] JS：classList 操作
来源：http://kfu.cashguo.top

el.classList.toggle("active")
来源：http://prp.iojbl.cn

[U102] JS：本地存储
来源：http://vxp.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://usw.birdmap.top

[U103] JS：定时器
来源：http://slv.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rps.zycfv.cn

[U104] JS：防抖
来源：http://itv.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gmi.vehdjk.com

[U105] JS：节流
来源：http://tyx.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vuq.zhijiandao.cn

[U106] JS：日期格式化
来源：http://jjj.jianghu66.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mgk.daxiang520.top

[U107] JS：数字千分位
来源：http://scb.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sqs.cqqwz.cn

[U108] JS：随机整数
来源：http://gbm.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aph.jiagoushi.top

[U109] JS：数组分组
来源：http://nyl.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://ydi.aibaodan.cn

[U110] JS：数组分块
来源：http://qyg.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ktv.jianghu66.top

[U111] JS：对象转 Map
来源：http://rcy.zdqjudy.top

new Map(Object.entries(obj))
来源：http://yum.wangdashe.top

[U112] JS：字符串补位
来源：http://rer.zhongyouzk.top

"7".padStart(3, "0")
来源：http://cpx.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://iux.fzhhl.top

s.replaceAll("a", "b")
来源：http://rlt.daria6918.cn

[U114] JS：JSON 深比较
来源：http://yka.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fgo.jinghuilouyu.cn

[U115] JS：生成 UUID
来源：http://mzb.zhengqikj.top

crypto.randomUUID()
来源：http://zov.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://slg.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://fuz.haohaochexian.top

[U117] JS：单元测试
来源：http://qer.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://ahp.meibo888.top

[U118] JS：开发服务器
来源：http://jom.smart0.xyz

npm i -D vite;  npx vite
来源：http://tun.zhixingplan.top

[U119] JS：生产构建
来源：http://ynb.hnxiangtu.top

npx vite build
来源：http://llc.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://aqd.ivvv.top

import.meta.env.VITE_API_URL
来源：http://bai.shanyushiyangkeji.top

================================================================================
来源：http://qfx.hesvh.cn

统计汇总
来源：http://zhc.bjfxy.top

================================================================================
来源：http://ihb.zdqjudy.top

按语言统计（条）：
来源：http://egn.xylfe.cn

Python ......... 252
来源：http://iqt.gogol.net.cn

PHP ............ 252
来源：http://sxs.shuidangran.top

JavaScript ..... 252
来源：http://htn.pengpengdd.cyou

TypeScript ..... 212
来源：http://nad.yuanzhike.top

Java ........... 212
来源：http://oar.birdmap.top

Go ............. 212
来源：http://qye.cashguo.top

Ruby ........... 212
来源：http://dgc.hesvh.cn

C# ............. 212
来源：http://keu.aizwys.cn

C .............. 30
来源：http://zmt.zhoulong.xyz

C++ ............ 30
来源：http://uhl.jiagoushi.top

SQL ............ 90
来源：http://vcw.ppjwa.cn

Bash ........... 80
来源：http://lrr.hfpthk.cn

Kotlin ......... 15
来源：http://vef.cheryme.top

Swift .......... 15
来源：http://ako.cdnleiting.top

Lua ............ 10
来源：http://abq.xingfuxueyuan.xyz

Perl ........... 10
来源：http://geb.yuanzhike.top

Scala .......... 10
来源：http://cds.fehbvm.com

------------------------------------
来源：http://dql.fktsv.cn

合计 ........... 2106 条
来源：http://oax.ctjpmb.com

按章节统计：
来源：http://akc.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://feh.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jnj.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hat.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iby.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jgo.vehdjk.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fnp.yj20258888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mct.jinqigfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hyy.ivvv.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zyx.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ghh.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hbz.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://grs.yfazqb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mtp.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rdb.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qca.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eyx.316326.xyz

Q SQL 专题                              90
来源：http://zvw.shuidangran.top

R Bash 专题                             80
来源：http://iyr.xylfe.cn

S C / C++ 专题                          60
来源：http://mzl.pengpengdd.cyou

T 其他语言补充                          60
来源：http://dcv.sjlbkw.cn

U 高频实用片段                         120
来源：http://wcj.fengsongda.top

------------------------------------
来源：http://edj.hesvh.cn

合计                                  2106 条
来源：http://yuu.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://xew.zycfv.cn

使用提醒
来源：http://chu.redwolf501.top

--------------------------------------------------------------------------------
来源：http://gwk.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dsl.meibo888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rum.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vvu.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dos.wangdashe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vva.chenjidiqi.icu

—— 文件结束 ——
来源：http://aud.shzxlz.cn

================================================================================
来源：http://izq.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://jni.bbcook.cn

Common Programming Examples Cheat Book
来源：http://ivx.xuanzx.com

================================================================================
来源：http://zkf.snrcjt.cn

【收录内容】
来源：http://dlu.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zep.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://elg.zhoulong.xyz

SQL · Bash · C · C++
来源：http://uay.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jma.xingfuxueyuan.xyz

【使用说明】
来源：http://krm.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wbl.dashuyun.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cdz.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zvf.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://csm.nanxinkj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wqd.nwbrower.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://grm.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://foz.xingfuxueyuan.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ovt.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vnp.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qty.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mwa.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vvk.shuidangran.top

【文件统计】
来源：http://kdl.zhengqikj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kpw.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://seg.tarul.cn

目  录
来源：http://pnh.hcnkem.com

--------------------------------------------------------------------------------
来源：http://lcf.daxiang520.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vbn.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dny.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://seb.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nid.hcnkem.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mir.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ydw.shuidangran.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wwe.aizwys.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pzr.gogol.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lmw.yueranfly.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mau.jqgfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://exn.ydjk.org.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fbc.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kxn.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://evq.quarkkingdee.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dkg.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zqf.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pqd.ctjpmb.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://jax.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zzk.wangdashe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rcr.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qvy.cashguo.top

================================================================================
来源：http://zme.tarul.cn

A. 基础语法与类型
来源：http://ate.iojbl.cn

================================================================================
来源：http://mti.cashguo.top

[A01] Hello World
来源：http://wtz.ppjwa.cn

Py:   print("Hello, World!")
来源：http://awm.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://mvh.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://slh.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://orr.chenzaomai.com

Java: System.out.println("Hello, World!");
来源：http://dsw.aibaodan.cn

Go:   fmt.Println("Hello, World!")
来源：http://ams.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://piz.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wij.xuetiantiany.cn

[A02] 变量声明与赋值
来源：http://ubq.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sgv.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://bif.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nex.ybcxt.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://che.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://lex.haohaochexian.top

Go:   name := "Alex"; age := 20
来源：http://tji.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://oqe.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://gtd.ctjpmb.com

[A03] 常量定义
来源：http://mjk.shanyushiyangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fox.smart0.xyz

PHP:  const PI = 3.14159;
来源：http://yzg.redwolf501.top

JS:   const PI = 3.14159;
来源：http://sqn.vehdjk.com

TS:   const PI: number = 3.14159;
来源：http://opy.zhixingplan.top

Java: static final double PI = 3.14159;
来源：http://fid.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://fut.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://cia.chenlongwang.top

C#:   const double PI = 3.14159;
来源：http://lon.52xcode.cn

[A04] 判断变量类型
来源：http://kkd.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yvr.zycfv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://voo.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pyk.gzhubu.top

TS:   typeof x; x instanceof Date
来源：http://cus.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bek.yj202588.top

Go:   reflect.TypeOf(x).Name()
来源：http://gpm.pycfn.com

Ruby: x.class; x.is_a?(Integer)
来源：http://eog.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://xuy.tarul.cn

[A05] 整数除法与取模
来源：http://xpe.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fin.jinqigufen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xsw.mhx1999.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nir.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lkt.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://oxa.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://eyi.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://gjb.quarkkingdee.top

C#:   7 / 2; 7 % 2
来源：http://nzg.yj20258.top

[A06] 字符串转数字
来源：http://ixg.snrcjt.cn

Py:   int("42"); float("3.14")
来源：http://cag.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gon.yuxming.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jhw.cqqwz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wej.yvedp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fyr.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cbj.tianlin.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://wpe.yvedp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pex.ybcxt.top

[A07] 数字转字符串
来源：http://mjw.yuanzhike.top

Py:   str(42)
来源：http://ppp.ydjk.org.cn

PHP:  (string) 42; strval(42)
来源：http://lqc.ybcxt.top

JS:   String(42); (42).toString()
来源：http://lxm.0kj1m.cn

TS:   String(42)
来源：http://wsc.jinyuanbaomall.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://puh.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://kki.jyoumei.cn

Ruby: 42.to_s
来源：http://sjb.zdbjq.cn

C#:   42.ToString()
来源：http://rlv.cashguo.top

[A08] 取整与四舍五入
来源：http://jmj.pycfn.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uxl.yonumen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jry.wangshuangyany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iqk.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wxi.zhoulong.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rkk.jinyuanbaomall.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mpw.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://iir.sysykeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dqc.tian-w.cn

[A09] 绝对值与最大最小值
来源：http://ipa.yj20258.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rnu.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zyc.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hgd.haohaochexian.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://owh.fengsongda.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wmf.xingfuxueyuan.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://swu.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://knd.uphjek.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://khx.yuanzhike.top


<!-- 参考信息 -->