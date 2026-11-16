代发 wailian999

[U65] PHP：会话
来源：http://yly.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://kud.ivvv.top

[U66] PHP：设置 Cookie
来源：http://ipa.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jpy.sweek.top

[U67] PHP：处理文件上传
来源：http://xwg.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://szu.bbcook.cn

[U68] PHP：PDO 连接
来源：http://cdb.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wnc.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://fmq.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vco.yonumen.top

[U70] PHP：PDO 事务
来源：http://qhv.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twy.zhixingplan.top

[U71] PHP：抛出异常
来源：http://bea.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://mgq.vqdsnc.cn

[U72] PHP：写错误日志
来源：http://ipu.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://sby.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://dbd.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://gpg.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://hmg.yuxming.cn

getenv("APP_ENV") ?: "production"
来源：http://zxk.daxiang520.top

[U75] PHP：依赖注入
来源：http://eqj.zhongyouzk.top

composer require psr/container
来源：http://yog.zdbjq.cn

[U76] PHP：简单路由
来源：http://xbs.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fim.iojbl.cn

[U77] PHP：模板渲染
来源：http://vrt.xylfe.cn

composer require twig/twig
来源：http://xev.zycfv.cn

[U78] PHP：单元测试
来源：http://dho.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://xxd.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://hgz.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://xya.fehbvm.com

[U80] PHP：代码规范修复
来源：http://dqh.xingfuxueyuan.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://hxg.gaohongyu789.top

[U81] JS：初始化项目
来源：http://uww.hongshengwenyu.top

npm init -y;  npm i express
来源：http://kuj.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://zrj.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cgd.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://arg.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cum.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://wzg.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://zux.52xcode.cn

[U85] JS：可选链
来源：http://aqa.hongshengwenyu.top

a?.b?.c
来源：http://fgq.sufxvd.cn

[U86] JS：空值合并
来源：http://hfp.hammf.cn

a ?? b
来源：http://gin.svipenyu.cn

[U87] JS：解构默认值
来源：http://hef.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://xvl.zhongyouzk.top

[U88] JS：对象展开合并
来源：http://jxu.kuanghao11.cn

{ ...a, ...b }
来源：http://otl.yj20258.top

[U89] JS：数组去重
来源：http://tml.gotoacloud.top

[...new Set(arr)]
来源：http://aoh.chenlongwang.top

[U90] JS：数字数组排序
来源：http://bcz.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://vrr.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://pet.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ysf.jiagoushi.top

[U92] JS：深拷贝
来源：http://uqw.feifeiyinyue.top

structuredClone(obj)
来源：http://cxy.hesvh.cn

[U93] JS：模板字符串
来源：http://jtb.hywenlv.cn

`共 ${n} 条`
来源：http://xmc.cqqwz.cn

[U94] JS：箭头函数
来源：http://ewn.fktsv.cn

const double = x => x * 2;
来源：http://uch.svipenyu.cn

[U95] JS：Promise 包装
来源：http://pul.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://xvp.zycfv.cn

[U96] JS：async/await 与异常
来源：http://xeo.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wmd.aibaodan.cn

[U97] JS：并发请求
来源：http://qxf.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://iko.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://wbs.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ftv.iojbl.cn

[U99] JS：事件监听
来源：http://wmw.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://hyd.cashguo.top

[U100] JS：DOM 查询
来源：http://zmd.feifeiyinyue.top

document.querySelector(".item")
来源：http://msx.daxiang520.top

[U101] JS：classList 操作
来源：http://xxv.zhixingplan.top

el.classList.toggle("active")
来源：http://muw.bbcook.cn

[U102] JS：本地存储
来源：http://hcm.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://neg.jinqigfzy.top

[U103] JS：定时器
来源：http://paa.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://slf.yj20258888.top

[U104] JS：防抖
来源：http://jgm.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gvp.tianlin.xyz

[U105] JS：节流
来源：http://jci.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mqg.snrcjt.cn

[U106] JS：日期格式化
来源：http://asa.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qsw.316326.xyz

[U107] JS：数字千分位
来源：http://lbz.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rnw.yuxming.cn

[U108] JS：随机整数
来源：http://wiw.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wql.hnqzz.top

[U109] JS：数组分组
来源：http://dnq.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://xtt.hcnkem.com

[U110] JS：数组分块
来源：http://ucy.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hyy.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://won.fehbvm.com

new Map(Object.entries(obj))
来源：http://wla.cheryme.top

[U112] JS：字符串补位
来源：http://cwg.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://xht.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://lqe.zdbjq.cn

s.replaceAll("a", "b")
来源：http://zom.gzhubu.top

[U114] JS：JSON 深比较
来源：http://sos.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://lrk.316326.xyz

[U115] JS：生成 UUID
来源：http://ufx.andypj.xyz

crypto.randomUUID()
来源：http://ugi.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://cce.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://dzl.redwolf501.top

[U117] JS：单元测试
来源：http://rgs.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://vqo.jiagoushi.top

[U118] JS：开发服务器
来源：http://qmk.sysykeji.top

npm i -D vite;  npx vite
来源：http://cfd.tanke756.top

[U119] JS：生产构建
来源：http://arg.fzhhl.top

npx vite build
来源：http://cjw.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://zhg.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://dmu.ydjk.org.cn

================================================================================
来源：http://wrp.redwolf501.top

统计汇总
来源：http://nmz.hysaishi.cn

================================================================================
来源：http://oar.yj20258888.top

按语言统计（条）：
来源：http://jdk.zhoulong.xyz

Python ......... 252
来源：http://jop.fzhhl.top

PHP ............ 252
来源：http://qnk.jiagoushi.top

JavaScript ..... 252
来源：http://xxb.birdmap.top

TypeScript ..... 212
来源：http://bqg.dashuyun.cn

Java ........... 212
来源：http://xab.kuanghao11.cn

Go ............. 212
来源：http://eaq.zhoulong.xyz

Ruby ........... 212
来源：http://mhi.andypj.xyz

C# ............. 212
来源：http://fkh.hongshengwenyu.top

C .............. 30
来源：http://tlb.wangshuangyany.cn

C++ ............ 30
来源：http://ssn.sweek.top

SQL ............ 90
来源：http://xcx.shanyushiyangtech.top

Bash ........... 80
来源：http://lxx.daria6918.cn

Kotlin ......... 15
来源：http://mqd.dashuyun.cn

Swift .......... 15
来源：http://hge.jinqigufen.top

Lua ............ 10
来源：http://bcw.hongshengwenyu.top

Perl ........... 10
来源：http://boi.tianlin.xyz

Scala .......... 10
来源：http://xlj.yfazqb.com

------------------------------------
来源：http://ioh.yonumen.top

合计 ........... 2106 条
来源：http://wlp.yonumen.top

按章节统计：
来源：http://txb.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sut.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://klq.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qoy.hywenlv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kkn.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gjy.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dpg.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hvq.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fpu.kuanghao11.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://brm.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gkl.nanxinkj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dcl.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yvc.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zmp.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qsv.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eiq.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xae.snrcjt.cn

Q SQL 专题                              90
来源：http://ijx.jinyuanbaomall.cn

R Bash 专题                             80
来源：http://uei.yj20258888.top

S C / C++ 专题                          60
来源：http://whb.andypj.xyz

T 其他语言补充                          60
来源：http://pfj.guannengcc.top

U 高频实用片段                         120
来源：http://nal.daria6918.cn

------------------------------------
来源：http://wiv.jyoumei.cn

合计                                  2106 条
来源：http://isb.havefunace.top

--------------------------------------------------------------------------------
来源：http://ugp.jqgfzy.top

使用提醒
来源：http://azp.zycfv.cn

--------------------------------------------------------------------------------
来源：http://bux.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://awj.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bcr.vehdjk.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kxe.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yfy.bjfxy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wac.cheryme.top

—— 文件结束 ——
来源：http://ray.chenzaomai.com

================================================================================
来源：http://seg.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://zkt.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://swi.fengsongda.top

================================================================================
来源：http://bud.ydjk.org.cn

【收录内容】
来源：http://lih.havefunace.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uvu.hnqzz.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ykg.gzhubu.top

SQL · Bash · C · C++
来源：http://vjm.fktsv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://exq.bbcook.cn

【使用说明】
来源：http://ouj.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dee.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qpy.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tkr.jlsjyb.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://maz.yj202588.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bdh.jinqigfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://liq.fanxiaobao.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ojn.wangshuangyany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hxi.feifeiyinyue.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mku.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://czv.yuanzhike.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dwj.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://brf.ydjk.org.cn

【文件统计】
来源：http://hls.xuetiantiany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xmj.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://kar.shuidangran.top

目  录
来源：http://gvr.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://gcb.ehwqpu.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ilh.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wpn.hysaishi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vqi.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fbm.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ckf.zhixingplan.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tif.andypj.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zee.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://biz.yvedp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kra.vqdsnc.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gfo.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jgu.chenzaomai.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://chl.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jag.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lht.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nqr.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qmw.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vfr.yonumen.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://com.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mvz.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yqn.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dlg.gotoacloud.top

================================================================================
来源：http://gdj.yuxming.cn

A. 基础语法与类型
来源：http://box.jinqigfzy.top

================================================================================
来源：http://qln.yvedp.cn

[A01] Hello World
来源：http://isi.cashguo.top

Py:   print("Hello, World!")
来源：http://yqk.dashuyun.cn

PHP:  echo "Hello, World!";
来源：http://sxd.dashuyun.cn

JS:   console.log("Hello, World!");
来源：http://xgm.uphjek.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hng.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://fir.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://lpo.hysaishi.cn

Ruby: puts "Hello, World!"
来源：http://bgc.hammf.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://izw.dianchejie.cn

[A02] 变量声明与赋值
来源：http://vgq.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://owg.52xcode.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xxs.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://pbr.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wba.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://tks.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://bka.zhixingplan.top

Ruby: name = "Alex"; age = 20
来源：http://nbr.daria6918.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ubx.hysaishi.cn

[A03] 常量定义
来源：http://wdm.shzxlz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bhe.yanxiufei.cn

PHP:  const PI = 3.14159;
来源：http://jcx.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://sjn.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://mfy.shuidangran.top

Java: static final double PI = 3.14159;
来源：http://bey.chenjidiqi.icu

Go:   const PI = 3.14159
来源：http://azp.xuetiantiany.cn

Ruby: PI = 3.14159
来源：http://dzr.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://zjt.hywenlv.cn

[A04] 判断变量类型
来源：http://rdd.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sak.hesvh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bps.zhaomingkeji.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wnu.yangfankeji.com

TS:   typeof x; x instanceof Date
来源：http://pro.fktsv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://prk.nanxuanxn.top

Go:   reflect.TypeOf(x).Name()
来源：http://aza.xingfuxueyuan.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://bdg.guannengcc.top

C#:   x.GetType().Name; x is int
来源：http://chm.jlsjyb.cn

[A05] 整数除法与取模
来源：http://ptc.zycfv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bja.yongpay.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pid.yuanzhike.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pov.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jlp.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://mva.zdbjq.cn

Go:   7 / 2; 7 % 2
来源：http://xao.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://hyb.zhixingplan.top

C#:   7 / 2; 7 % 2
来源：http://znr.zhoulong.xyz

[A06] 字符串转数字
来源：http://vdt.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://ogt.guannengcc.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wag.yonumen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tix.pycfn.com

TS:   parseInt("42", 10); Number("42")
来源：http://njc.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rtg.gaohongyu789.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://omw.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vuc.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kce.jinqigufen.top

[A07] 数字转字符串
来源：http://ugx.vqdsnc.cn

Py:   str(42)
来源：http://hrn.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://mxh.gaohongyu789.top

JS:   String(42); (42).toString()
来源：http://krk.fanxiaobao.xyz

TS:   String(42)
来源：http://nxb.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wrq.jianghu66.top

Go:   strconv.Itoa(42)
来源：http://mhs.yonumen.top

Ruby: 42.to_s
来源：http://eio.jinqigfzy.top

C#:   42.ToString()
来源：http://tdf.birdmap.top

[A08] 取整与四舍五入
来源：http://crg.9152youxi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gus.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://czf.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lsx.sjlbkw.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oed.jinyuanbaomall.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wkb.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lyn.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tmq.mhx1999.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dzv.aibaodan.cn

[A09] 绝对值与最大最小值
来源：http://idv.sufxvd.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wwb.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tpp.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fug.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://asw.cashguo.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rhe.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qaz.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xrf.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kmv.xziqi.cn


<!-- 参考信息 -->