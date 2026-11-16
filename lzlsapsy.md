代发 wailian999

[U65] PHP：会话
来源：http://kew.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vyg.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://afy.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qrk.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://afz.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oje.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://aam.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ybi.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://vkl.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sxu.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://gsc.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ypi.vehdjk.com

[U71] PHP：抛出异常
来源：http://fhy.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://xko.fanxiaobao.xyz

[U72] PHP：写错误日志
来源：http://zym.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://vbn.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://nml.cheryme.top

parse_ini_file("config.ini", true)
来源：http://ibi.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://abz.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://onn.fktsv.cn

[U75] PHP：依赖注入
来源：http://vcm.nwbrower.top

composer require psr/container
来源：http://xbt.tianlin.xyz

[U76] PHP：简单路由
来源：http://yes.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aou.zhoulong.xyz

[U77] PHP：模板渲染
来源：http://oes.iojbl.cn

composer require twig/twig
来源：http://gfa.xuanzx.com

[U78] PHP：单元测试
来源：http://wwc.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://acm.fktsv.cn

[U79] PHP：静态分析
来源：http://qot.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://suw.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://abw.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://roq.ywan-chungtsiang.top

[U81] JS：初始化项目
来源：http://ylh.mhx1999.top

npm init -y;  npm i express
来源：http://cnn.epnwcf.com

[U82] JS：package.json 脚本
来源：http://nqq.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://asd.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://pzr.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://ran.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://jtu.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://yrv.kuanghao11.cn

[U85] JS：可选链
来源：http://dmc.hesvh.cn

a?.b?.c
来源：http://cph.ehwqpu.com

[U86] JS：空值合并
来源：http://tfa.jlsjyb.cn

a ?? b
来源：http://wsw.bbcook.cn

[U87] JS：解构默认值
来源：http://bnk.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://xhg.tarul.cn

[U88] JS：对象展开合并
来源：http://vtk.jqgfzy.top

{ ...a, ...b }
来源：http://qmq.tarul.cn

[U89] JS：数组去重
来源：http://cdp.meibo888.top

[...new Set(arr)]
来源：http://gmk.svipenyu.cn

[U90] JS：数字数组排序
来源：http://waf.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://uig.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://eja.andypj.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mbn.yuanzhike.top

[U92] JS：深拷贝
来源：http://jjk.gzhubu.top

structuredClone(obj)
来源：http://jlf.cucudq.cn

[U93] JS：模板字符串
来源：http://mmm.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://cep.chenzaomai.com

[U94] JS：箭头函数
来源：http://mzy.hysaishi.cn

const double = x => x * 2;
来源：http://nhv.shuidangran.top

[U95] JS：Promise 包装
来源：http://ecz.andypj.xyz

new Promise((resolve, reject) => {})
来源：http://vst.yuxming.cn

[U96] JS：async/await 与异常
来源：http://apv.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ews.yongpay.top

[U97] JS：并发请求
来源：http://ygi.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rcc.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://mbf.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dec.cashguo.top

[U99] JS：事件监听
来源：http://zlr.cucudq.cn

el.addEventListener("click", e => {})
来源：http://fbb.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://jnv.guowangkeji.top

document.querySelector(".item")
来源：http://gge.xuanzx.com

[U101] JS：classList 操作
来源：http://hua.hesvh.cn

el.classList.toggle("active")
来源：http://zkt.cucudq.cn

[U102] JS：本地存储
来源：http://iaq.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tfo.hysaishi.cn

[U103] JS：定时器
来源：http://zjv.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uoa.zhijiandao.cn

[U104] JS：防抖
来源：http://zer.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iza.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://aah.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qso.zhoulong.xyz

[U106] JS：日期格式化
来源：http://agy.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mpp.ctjpmb.com

[U107] JS：数字千分位
来源：http://tky.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fui.shzxlz.cn

[U108] JS：随机整数
来源：http://joe.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cjn.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://gjx.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://njd.tanke756.top

[U110] JS：数组分块
来源：http://tyw.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hhq.tianlin.xyz

[U111] JS：对象转 Map
来源：http://axm.nanxinkj.top

new Map(Object.entries(obj))
来源：http://uqi.ppjwa.cn

[U112] JS：字符串补位
来源：http://bxt.fktsv.cn

"7".padStart(3, "0")
来源：http://nyk.yj202588.top

[U113] JS：正则替换全部
来源：http://ynl.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://kxw.yj20258888.top

[U114] JS：JSON 深比较
来源：http://cay.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://krd.fktsv.cn

[U115] JS：生成 UUID
来源：http://caf.gogol.net.cn

crypto.randomUUID()
来源：http://kzb.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://laf.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://wza.daria6918.cn

[U117] JS：单元测试
来源：http://bvn.tarul.cn

npm i -D vitest;  npx vitest
来源：http://thf.yj202588.top

[U118] JS：开发服务器
来源：http://kjh.chenlongwang.top

npm i -D vite;  npx vite
来源：http://ijw.nanxuanxn.top

[U119] JS：生产构建
来源：http://wkp.tarul.cn

npx vite build
来源：http://cal.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://wco.yj202588.top

import.meta.env.VITE_API_URL
来源：http://kcu.yj20258888.top

================================================================================
来源：http://gkz.epnwcf.com

统计汇总
来源：http://wdz.jyoumei.cn

================================================================================
来源：http://nzv.jiagoushi.top

按语言统计（条）：
来源：http://ywr.yongpay.top

Python ......... 252
来源：http://fiq.yangfankeji.com

PHP ............ 252
来源：http://lkn.0kj1m.cn

JavaScript ..... 252
来源：http://zjp.cashguo.top

TypeScript ..... 212
来源：http://izb.hnqzz.top

Java ........... 212
来源：http://gyc.jianghu66.top

Go ............. 212
来源：http://nne.zycfv.cn

Ruby ........... 212
来源：http://wml.aizwys.cn

C# ............. 212
来源：http://jki.yanxiufei.cn

C .............. 30
来源：http://npt.dashuyun.cn

C++ ............ 30
来源：http://xei.andypj.xyz

SQL ............ 90
来源：http://wdv.hysaishi.cn

Bash ........... 80
来源：http://lwl.yj20258.top

Kotlin ......... 15
来源：http://zrq.cheryme.top

Swift .......... 15
来源：http://nrt.zhongyouzk.top

Lua ............ 10
来源：http://kyr.iojbl.cn

Perl ........... 10
来源：http://yso.xingfuxueyuan.xyz

Scala .......... 10
来源：http://huf.xylfe.cn

------------------------------------
来源：http://ixw.zhoulong.xyz

合计 ........... 2106 条
来源：http://xkq.yfazqb.com

按章节统计：
来源：http://gmh.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lup.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://szl.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kgj.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wih.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://drr.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pmj.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://avn.yvedp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xou.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pmk.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cbu.fengsongda.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dhz.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://peq.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jrp.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://axi.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ezr.iojbl.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ayy.yj202588.top

Q SQL 专题                              90
来源：http://dgn.yanxiufei.cn

R Bash 专题                             80
来源：http://tlo.yj202588.top

S C / C++ 专题                          60
来源：http://rvk.fengsongda.top

T 其他语言补充                          60
来源：http://eyq.xinyue.icu

U 高频实用片段                         120
来源：http://zbg.hywenlv.cn

------------------------------------
来源：http://vpg.xinyue.icu

合计                                  2106 条
来源：http://kjn.uphjek.com

--------------------------------------------------------------------------------
来源：http://poy.hnxiangtu.top

使用提醒
来源：http://xnw.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://nir.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ump.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://omh.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uxl.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fpw.yangfankeji.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cmm.daxiang520.top

—— 文件结束 ——
来源：http://kqm.wangshuangyany.cn

================================================================================
来源：http://gku.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://hak.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://ksj.sweek.top

================================================================================
来源：http://eqs.fengsongda.top

【收录内容】
来源：http://mos.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xnq.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://deh.jinghuilouyu.cn

SQL · Bash · C · C++
来源：http://aup.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dqa.snrcjt.cn

【使用说明】
来源：http://pzh.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bzw.jyoumei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cww.ydzc1.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://twh.fengsongda.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wlw.zhijiandao.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fmd.jyoumei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rol.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://igi.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rhr.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://okg.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://inm.hywenlv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ltd.shanyushiyangtech.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pdn.ybcxt.top

【文件统计】
来源：http://gqd.uphjek.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://raz.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://zlc.jianghu66.top

目  录
来源：http://xuc.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://yyb.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zfj.yfazqb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jls.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qbd.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lee.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hgx.hesvh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aop.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tpj.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jeg.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://awe.zhiwuduotai.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yhh.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fkh.dianchejie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nqk.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://grd.smart0.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zgy.epnwcf.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ehy.zhijiandao.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rzv.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qeo.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://cln.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://chx.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gfz.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rdy.quarkkingdee.top

================================================================================
来源：http://awg.feifeiyinyue.top

A. 基础语法与类型
来源：http://ymz.bjfxy.top

================================================================================
来源：http://hnp.hcnkem.com

[A01] Hello World
来源：http://mhx.chenzaomai.com

Py:   print("Hello, World!")
来源：http://mim.snrcjt.cn

PHP:  echo "Hello, World!";
来源：http://xta.cdnleiting.top

JS:   console.log("Hello, World!");
来源：http://lyj.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tpd.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://szp.yj20258.top

Go:   fmt.Println("Hello, World!")
来源：http://yza.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://syd.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://oyb.cucudq.cn

[A02] 变量声明与赋值
来源：http://mxu.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://txc.zhiwuduotai.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uqs.cdnleiting.top

JS:   let name = "Alex"; const age = 20;
来源：http://doq.zdqjudy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vkc.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://ana.aibaodan.cn

Go:   name := "Alex"; age := 20
来源：http://fra.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://emp.yuanzhike.top

C#:   string name = "Alex"; int age = 20;
来源：http://eek.ybcxt.top

[A03] 常量定义
来源：http://rgf.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bmp.hfpthk.cn

PHP:  const PI = 3.14159;
来源：http://ozm.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://lgj.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://drq.yonumen.top

Java: static final double PI = 3.14159;
来源：http://jyo.316326.xyz

Go:   const PI = 3.14159
来源：http://ohq.chenzaomai.com

Ruby: PI = 3.14159
来源：http://lgc.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://mwx.xinyue.icu

[A04] 判断变量类型
来源：http://oke.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://egt.hnxiangtu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fyp.shanyushiyangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zgp.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://gzk.gotoacloud.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dts.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jih.havefunace.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jwy.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://qqi.hcnkem.com

[A05] 整数除法与取模
来源：http://wxx.c1oappe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wrg.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://zzs.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tgv.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jpl.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://qes.cashguo.top

Go:   7 / 2; 7 % 2
来源：http://oae.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://ebs.chenjidiqi.icu

C#:   7 / 2; 7 % 2
来源：http://xvr.yangfankeji.com

[A06] 字符串转数字
来源：http://xtn.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://chs.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uzl.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xxx.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://mlg.hongshengwenyu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ukf.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lwg.sjlbkw.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lgv.guowangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dbw.guannengcc.top

[A07] 数字转字符串
来源：http://fxk.gaohongyu789.top

Py:   str(42)
来源：http://rdv.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://ats.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://sro.vqdsnc.cn

TS:   String(42)
来源：http://pab.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kyk.cashguo.top

Go:   strconv.Itoa(42)
来源：http://tmw.ppjwa.cn

Ruby: 42.to_s
来源：http://mce.tanke756.top

C#:   42.ToString()
来源：http://ztm.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://dvy.tian-w.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jpm.jiagoushi.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sjc.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vcs.ydjk.org.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://urf.wangdashe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gwo.tian-w.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xwf.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fxe.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://awo.jyoumei.cn

[A09] 绝对值与最大最小值
来源：http://wgn.xuanzx.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pon.c1oappe.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://krw.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://imc.epnwcf.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vfh.zhaomingkeji.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://obj.dashuyun.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zha.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://oua.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kmh.ppjwa.cn


<!-- 参考信息 -->