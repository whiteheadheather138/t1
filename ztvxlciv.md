代发 wailian999

[U67] PHP：处理文件上传
来源：http://lqy.cqqwz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xap.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://qvx.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gux.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://ava.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zym.tanke756.top

[U70] PHP：PDO 事务
来源：http://aum.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aal.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://slo.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://nck.cheryme.top

[U72] PHP：写错误日志
来源：http://zbv.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://quj.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://ddp.vqdsnc.cn

parse_ini_file("config.ini", true)
来源：http://aoz.bbcook.cn

[U74] PHP：读取环境变量
来源：http://klg.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://elk.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://nla.andypj.xyz

composer require psr/container
来源：http://lfh.feifeiyinyue.top

[U76] PHP：简单路由
来源：http://ksb.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://khn.jianghu66.top

[U77] PHP：模板渲染
来源：http://xwa.vehdjk.com

composer require twig/twig
来源：http://xns.shuidangran.top

[U78] PHP：单元测试
来源：http://nuf.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://qmo.meibo888.top

[U79] PHP：静态分析
来源：http://dpr.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://xdt.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://sem.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jnz.ivvv.top

[U81] JS：初始化项目
来源：http://nfz.jianghu66.top

npm init -y;  npm i express
来源：http://ayf.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://bim.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vcf.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://qvl.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://tzy.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://pyt.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://hyb.zhiwuduotai.top

[U85] JS：可选链
来源：http://ptu.tian-w.cn

a?.b?.c
来源：http://fbp.ivvv.top

[U86] JS：空值合并
来源：http://olu.snrcjt.cn

a ?? b
来源：http://lxq.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://dmn.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://sia.hammf.cn

[U88] JS：对象展开合并
来源：http://dzt.hysaishi.cn

{ ...a, ...b }
来源：http://pqp.pycfn.com

[U89] JS：数组去重
来源：http://cdf.zycfv.cn

[...new Set(arr)]
来源：http://abe.yonumen.top

[U90] JS：数字数组排序
来源：http://nhe.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://qfs.fehbvm.com

[U91] JS：对象键值遍历
来源：http://cer.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xkw.daxiang520.top

[U92] JS：深拷贝
来源：http://bzg.epnwcf.com

structuredClone(obj)
来源：http://owm.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://ynu.jianghu66.top

`共 ${n} 条`
来源：http://ico.yonumen.top

[U94] JS：箭头函数
来源：http://ibh.yj20258.top

const double = x => x * 2;
来源：http://tom.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://kpv.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://rnh.tanke756.top

[U96] JS：async/await 与异常
来源：http://cby.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xve.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://ttn.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kha.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://cnr.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://klq.kuanghao11.cn

[U99] JS：事件监听
来源：http://ulj.fengsongda.top

el.addEventListener("click", e => {})
来源：http://nqu.fzhhl.top

[U100] JS：DOM 查询
来源：http://pef.hywenlv.cn

document.querySelector(".item")
来源：http://tzo.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://zrd.daxiang520.top

el.classList.toggle("active")
来源：http://whp.jinqigufen.top

[U102] JS：本地存储
来源：http://ili.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kay.52xcode.cn

[U103] JS：定时器
来源：http://wrl.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://seo.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://iey.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kca.redwolf501.top

[U105] JS：节流
来源：http://vfp.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wdv.zhengqikj.top

[U106] JS：日期格式化
来源：http://jsq.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eie.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://mux.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tvz.zycfv.cn

[U108] JS：随机整数
来源：http://zvf.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dci.sweek.top

[U109] JS：数组分组
来源：http://qxi.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://kot.snrcjt.cn

[U110] JS：数组分块
来源：http://kmr.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kil.nwbrower.top

[U111] JS：对象转 Map
来源：http://mam.9152youxi.cn

new Map(Object.entries(obj))
来源：http://xdy.bjfxy.top

[U112] JS：字符串补位
来源：http://iqq.jyoumei.cn

"7".padStart(3, "0")
来源：http://jho.gotoacloud.top

[U113] JS：正则替换全部
来源：http://wxc.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://uaq.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://tng.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tzy.shzxlz.cn

[U115] JS：生成 UUID
来源：http://xzk.fktsv.cn

crypto.randomUUID()
来源：http://gmc.fzhhl.top

[U116] JS：类型检查（JSDoc）
来源：http://aia.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://qol.hongshengwenyu.top

[U117] JS：单元测试
来源：http://nxj.vehdjk.com

npm i -D vitest;  npx vitest
来源：http://zld.gotoacloud.top

[U118] JS：开发服务器
来源：http://jyo.fengsongda.top

npm i -D vite;  npx vite
来源：http://xwb.xuanzx.com

[U119] JS：生产构建
来源：http://wkx.birdmap.top

npx vite build
来源：http://lsm.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://mpb.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://cdd.bjfxy.top

================================================================================
来源：http://olm.quarkkingdee.top

统计汇总
来源：http://wfb.birdmap.top

================================================================================
来源：http://bos.jinqigufen.top

按语言统计（条）：
来源：http://cfj.hfpthk.cn

Python ......... 252
来源：http://pbz.zhixingplan.top

PHP ............ 252
来源：http://lne.fanxiaobao.xyz

JavaScript ..... 252
来源：http://ett.xylfe.cn

TypeScript ..... 212
来源：http://auc.zhaomingkeji.xyz

Java ........... 212
来源：http://dku.quarkkingdee.top

Go ............. 212
来源：http://qlh.daria6918.cn

Ruby ........... 212
来源：http://lef.zhaomingkeji.xyz

C# ............. 212
来源：http://hwg.hysaishi.cn

C .............. 30
来源：http://sqc.hfpthk.cn

C++ ............ 30
来源：http://vri.shanyushiyangtech.top

SQL ............ 90
来源：http://nlw.jyoumei.cn

Bash ........... 80
来源：http://fan.sufxvd.cn

Kotlin ......... 15
来源：http://txj.jinqigufen.top

Swift .......... 15
来源：http://rfi.tarul.cn

Lua ............ 10
来源：http://pfu.zhongyouzk.top

Perl ........... 10
来源：http://mqy.jianghu66.top

Scala .......... 10
来源：http://rmd.wangdashe.top

------------------------------------
来源：http://apk.fzhhl.top

合计 ........... 2106 条
来源：http://aay.wangshuangyany.cn

按章节统计：
来源：http://fml.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dfk.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lfo.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ymx.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ntm.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://clu.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fhl.yj20258888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bji.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pkp.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vlr.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qmo.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kyi.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nwt.jiagoushi.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://whe.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qdj.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uwx.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mvc.guowangkeji.top

Q SQL 专题                              90
来源：http://jta.ybcxt.top

R Bash 专题                             80
来源：http://yex.zhijiandao.cn

S C / C++ 专题                          60
来源：http://vyo.cheryme.top

T 其他语言补充                          60
来源：http://bul.snrcjt.cn

U 高频实用片段                         120
来源：http://czx.xuetiantiany.cn

------------------------------------
来源：http://mbr.tianlin.xyz

合计                                  2106 条
来源：http://yfa.fehbvm.com

--------------------------------------------------------------------------------
来源：http://qkl.xziqi.cn

使用提醒
来源：http://nrf.xinyue.icu

--------------------------------------------------------------------------------
来源：http://ewa.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gnr.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ycm.hammf.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vvl.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tje.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://avo.cdnleiting.top

—— 文件结束 ——
来源：http://rft.tarul.cn

================================================================================
来源：http://mll.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://cog.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://iyc.yuxming.cn

================================================================================
来源：http://kqy.zhijiandao.cn

【收录内容】
来源：http://lxh.cdnleiting.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hej.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zsm.yanxiufei.cn

SQL · Bash · C · C++
来源：http://kjv.meibo888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tgc.yj202588.top

【使用说明】
来源：http://llo.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://amj.andypj.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xnz.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pha.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ugk.chenlongwang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rga.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wzg.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yor.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ftz.pengpengdd.cyou

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bzp.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wuf.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uxf.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yan.jyoumei.cn

【文件统计】
来源：http://umc.shangyingyoupin.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vvr.xuanzx.com

--------------------------------------------------------------------------------
来源：http://wgf.zhijiandao.cn

目  录
来源：http://nbn.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://ktp.xuetiantiany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iuc.havefunace.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qci.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rqr.jlsjyb.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zef.fzhhl.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cdq.shuidangran.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kdd.jinghuilouyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mtc.yuanzhike.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pxo.hammf.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sfu.fengsongda.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lzk.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lzq.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pit.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vsz.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pan.gogol.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hks.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fcz.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://znu.pengpengdd.cyou

R. Bash 专题                   （第 18 节，80 条）
来源：http://fug.haohaochexian.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yxr.vehdjk.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fxl.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dkd.feifeiyinyue.top

================================================================================
来源：http://gis.ydjk.org.cn

A. 基础语法与类型
来源：http://dta.yueranfly.top

================================================================================
来源：http://ujj.zhengqikj.top

[A01] Hello World
来源：http://wqm.quarkkingdee.top

Py:   print("Hello, World!")
来源：http://ruj.sweek.top

PHP:  echo "Hello, World!";
来源：http://ddl.jinyuanbaomall.cn

JS:   console.log("Hello, World!");
来源：http://pst.aibaodan.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://swn.iojbl.cn

Java: System.out.println("Hello, World!");
来源：http://fyx.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://oog.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://mvz.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pog.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://ume.smart0.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fbq.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cib.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mtn.zdqjudy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dwg.bbcook.cn

Java: String name = "Alex"; int age = 20;
来源：http://wjj.sjlbkw.cn

Go:   name := "Alex"; age := 20
来源：http://mlq.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://foe.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://zxd.yj20258888.top

[A03] 常量定义
来源：http://dcs.jqgfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xme.ywan-chungtsiang.top

PHP:  const PI = 3.14159;
来源：http://crc.shanyushiyangkeji.top

JS:   const PI = 3.14159;
来源：http://zmt.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://wme.aibaodan.cn

Java: static final double PI = 3.14159;
来源：http://vst.yueranfly.top

Go:   const PI = 3.14159
来源：http://rqv.yj20258888.top

Ruby: PI = 3.14159
来源：http://puo.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://dur.nwbrower.top

[A04] 判断变量类型
来源：http://kca.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://gou.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vne.gaohongyu789.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bgv.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://zfl.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oaa.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://wml.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tnz.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://txj.fehbvm.com

[A05] 整数除法与取模
来源：http://ide.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sqw.zdqjudy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hlj.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vsf.zdbjq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jpi.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://xch.nanxuanxn.top

Go:   7 / 2; 7 % 2
来源：http://xvj.cucudq.cn

Ruby: 7 / 2; 7 % 2
来源：http://zvr.haohaochexian.top

C#:   7 / 2; 7 % 2
来源：http://adk.zhongyouzk.top

[A06] 字符串转数字
来源：http://chw.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://tos.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bew.sufxvd.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qpo.hammf.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xsm.jianghu66.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zdc.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://szo.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://wls.birdmap.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bly.jyoumei.cn

[A07] 数字转字符串
来源：http://nus.andypj.xyz

Py:   str(42)
来源：http://xlm.nwbrower.top

PHP:  (string) 42; strval(42)
来源：http://uzp.xuanzx.com

JS:   String(42); (42).toString()
来源：http://vcc.hammf.cn

TS:   String(42)
来源：http://ovm.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://fdf.epnwcf.com

Go:   strconv.Itoa(42)
来源：http://obx.yanxiufei.cn

Ruby: 42.to_s
来源：http://pey.pengpengdd.cyou

C#:   42.ToString()
来源：http://wey.meibo888.top

[A08] 取整与四舍五入
来源：http://our.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://djg.sufxvd.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rfq.jinqigufen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zsz.ehwqpu.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://shw.pycfn.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://axe.316326.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oxo.iojbl.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mhw.yvedp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zul.xziqi.cn

[A09] 绝对值与最大最小值
来源：http://spm.guannengcc.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wac.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yqp.nanxinkj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ykp.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://odf.ydjk.org.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hqx.hfpthk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nbn.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ekl.yuxming.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zlo.zhijiandao.cn

[A10] 生成随机数
来源：http://tqg.cheryme.top

Py:   import random; random.randint(1, 100)
来源：http://kfm.sweek.top

PHP:  random_int(1, 100);
来源：http://xox.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gqg.hysaishi.cn


<!-- 参考信息 -->