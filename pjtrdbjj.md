代发 wailian999

[U65] PHP：会话
来源：http://jqv.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mfr.ybcxt.top

[U66] PHP：设置 Cookie
来源：http://pgz.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gaw.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://qyw.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xet.yongpay.top

[U68] PHP：PDO 连接
来源：http://kap.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mhh.meibo888.top

[U69] PHP：PDO 预处理
来源：http://wmf.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uch.yj20258.top

[U70] PHP：PDO 事务
来源：http://cuh.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zig.zhijiandao.cn

[U71] PHP：抛出异常
来源：http://pqu.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://zrf.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://wbw.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://hpc.hfpthk.cn

[U73] PHP：读取 ini 配置
来源：http://clm.tian-w.cn

parse_ini_file("config.ini", true)
来源：http://psu.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://csv.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://juw.uphjek.com

[U75] PHP：依赖注入
来源：http://kil.ppjwa.cn

composer require psr/container
来源：http://yhr.yj20258.top

[U76] PHP：简单路由
来源：http://tnr.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rey.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://say.daxiang520.top

composer require twig/twig
来源：http://vql.hywenlv.cn

[U78] PHP：单元测试
来源：http://afe.tarul.cn

composer require --dev phpunit/phpunit
来源：http://knw.ydjk.org.cn

[U79] PHP：静态分析
来源：http://nqo.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://evv.c1oappe.top

[U80] PHP：代码规范修复
来源：http://yfo.c1oappe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cnt.nwbrower.top

[U81] JS：初始化项目
来源：http://aqj.nanxuanxn.top

npm init -y;  npm i express
来源：http://sqr.wangdashe.top

[U82] JS：package.json 脚本
来源：http://ecj.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lpd.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://yhs.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wmu.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://toy.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://jsi.sysykeji.top

[U85] JS：可选链
来源：http://bpj.zdbjq.cn

a?.b?.c
来源：http://ieg.mhx1999.top

[U86] JS：空值合并
来源：http://ylg.ydzc1.top

a ?? b
来源：http://cqr.snrcjt.cn

[U87] JS：解构默认值
来源：http://pdv.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://vpn.andypj.xyz

[U88] JS：对象展开合并
来源：http://hpi.wangshuangyany.cn

{ ...a, ...b }
来源：http://jni.snrcjt.cn

[U89] JS：数组去重
来源：http://ozz.xylfe.cn

[...new Set(arr)]
来源：http://dlo.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://dpm.uphjek.com

[...arr].sort((a, b) => a - b)
来源：http://zrl.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://wnx.52xcode.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yim.vqdsnc.cn

[U92] JS：深拷贝
来源：http://qij.shzxlz.cn

structuredClone(obj)
来源：http://ptc.jianghu66.top

[U93] JS：模板字符串
来源：http://pxt.0kj1m.cn

`共 ${n} 条`
来源：http://kpx.xylfe.cn

[U94] JS：箭头函数
来源：http://rjh.c1oappe.top

const double = x => x * 2;
来源：http://nkt.epnwcf.com

[U95] JS：Promise 包装
来源：http://eoy.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://txe.aizwys.cn

[U96] JS：async/await 与异常
来源：http://ptl.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yvg.yj202588.top

[U97] JS：并发请求
来源：http://eeo.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kzn.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://qcg.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bkv.xinyue.icu

[U99] JS：事件监听
来源：http://bjo.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://wuy.svipenyu.cn

[U100] JS：DOM 查询
来源：http://ais.xuetiantiany.cn

document.querySelector(".item")
来源：http://vfv.0kj1m.cn

[U101] JS：classList 操作
来源：http://agz.yuanzhike.top

el.classList.toggle("active")
来源：http://has.hesvh.cn

[U102] JS：本地存储
来源：http://mka.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oxq.zhengqikj.top

[U103] JS：定时器
来源：http://vrj.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jzr.fzhhl.top

[U104] JS：防抖
来源：http://xlx.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://esu.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://dyq.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vxy.cashguo.top

[U106] JS：日期格式化
来源：http://doc.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ega.hfpthk.cn

[U107] JS：数字千分位
来源：http://tmy.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nhn.shangyingyoupin.top

[U108] JS：随机整数
来源：http://xvp.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fmy.yongpay.top

[U109] JS：数组分组
来源：http://wcf.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://yrv.cdnleiting.top

[U110] JS：数组分块
来源：http://fup.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yeo.hnqzz.top

[U111] JS：对象转 Map
来源：http://nti.yangfankeji.com

new Map(Object.entries(obj))
来源：http://zob.zdbjq.cn

[U112] JS：字符串补位
来源：http://kqk.zhoulong.xyz

"7".padStart(3, "0")
来源：http://kgd.jianghu66.top

[U113] JS：正则替换全部
来源：http://geb.yj20258888.top

s.replaceAll("a", "b")
来源：http://fdt.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://bis.smart0.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://shb.yuxming.cn

[U115] JS：生成 UUID
来源：http://deh.ydzc1.top

crypto.randomUUID()
来源：http://mcd.jyoumei.cn

[U116] JS：类型检查（JSDoc）
来源：http://pxz.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://qqr.mhx1999.top

[U117] JS：单元测试
来源：http://isr.uphjek.com

npm i -D vitest;  npx vitest
来源：http://lac.sysykeji.top

[U118] JS：开发服务器
来源：http://drz.ybcxt.top

npm i -D vite;  npx vite
来源：http://zdd.birdmap.top

[U119] JS：生产构建
来源：http://pkq.zdqjudy.top

npx vite build
来源：http://joh.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://rds.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://xmz.sysykeji.top

================================================================================
来源：http://tad.xuetiantiany.cn

统计汇总
来源：http://beg.sxryk.cn

================================================================================
来源：http://spx.bbcook.cn

按语言统计（条）：
来源：http://spv.birdmap.top

Python ......... 252
来源：http://sed.zhaomingkeji.xyz

PHP ............ 252
来源：http://gim.jiagoushi.top

JavaScript ..... 252
来源：http://ubk.fktsv.cn

TypeScript ..... 212
来源：http://hbd.nanxinkj.top

Java ........... 212
来源：http://tze.xylfe.cn

Go ............. 212
来源：http://rvp.yfazqb.com

Ruby ........... 212
来源：http://nja.jinqigfzy.top

C# ............. 212
来源：http://uto.ivvv.top

C .............. 30
来源：http://ffy.ydzc1.top

C++ ............ 30
来源：http://arf.haohaochexian.top

SQL ............ 90
来源：http://qnj.gzhubu.top

Bash ........... 80
来源：http://cnz.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://kyg.yj20258.top

Swift .......... 15
来源：http://dzb.chenzaomai.com

Lua ............ 10
来源：http://wsz.redwolf501.top

Perl ........... 10
来源：http://nzj.ctjpmb.com

Scala .......... 10
来源：http://juc.sufxvd.cn

------------------------------------
来源：http://qjo.aibaodan.cn

合计 ........... 2106 条
来源：http://skn.tian-w.cn

按章节统计：
来源：http://zha.daria6918.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vpa.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dqo.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qzv.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jxf.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oij.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cuv.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mgy.tarul.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sbi.jinqigufen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oeb.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xvh.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://omr.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://udi.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uou.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yok.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wsp.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://apz.gogol.net.cn

Q SQL 专题                              90
来源：http://ioy.chenzaomai.com

R Bash 专题                             80
来源：http://oej.yj20258.top

S C / C++ 专题                          60
来源：http://aco.hongshengwenyu.top

T 其他语言补充                          60
来源：http://rsd.yueranfly.top

U 高频实用片段                         120
来源：http://ctp.sjlbkw.cn

------------------------------------
来源：http://ppx.yj202588.top

合计                                  2106 条
来源：http://oml.hcnkem.com

--------------------------------------------------------------------------------
来源：http://dny.yfazqb.com

使用提醒
来源：http://nrn.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://gaj.hfpthk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kgp.jqgufenzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hxz.xuetiantiany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vae.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jhb.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vkl.yuxming.cn

—— 文件结束 ——
来源：http://ifn.daria6918.cn

================================================================================
来源：http://idy.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://ory.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://yxg.zdbjq.cn

================================================================================
来源：http://ogc.zhixingplan.top

【收录内容】
来源：http://nip.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://syx.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://emg.vehdjk.com

SQL · Bash · C · C++
来源：http://ori.xingfuxueyuan.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ktf.c1oappe.top

【使用说明】
来源：http://udn.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hqb.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oie.xuetiantiany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tjg.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://das.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://owe.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ron.aibaodan.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mcu.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nhd.yueranfly.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hxg.ehwqpu.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tkt.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cxb.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://efb.jiagoushi.top

【文件统计】
来源：http://mip.zdqjudy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zwj.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://orr.gaohongyu789.top

目  录
来源：http://gfx.nwbrower.top

--------------------------------------------------------------------------------
来源：http://nad.fktsv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zlj.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://myk.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lkp.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://llq.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://udg.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iyf.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qyg.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rps.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ujq.uphjek.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://anj.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bhu.gotoacloud.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ecz.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nxh.haohaochexian.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dgp.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zzj.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bqj.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wox.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://onu.yanxiufei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zcl.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zme.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://azt.ppjwa.cn

================================================================================
来源：http://vmo.hywenlv.cn

A. 基础语法与类型
来源：http://lks.haohaochexian.top

================================================================================
来源：http://eba.gogol.net.cn

[A01] Hello World
来源：http://fgv.nanxuanxn.top

Py:   print("Hello, World!")
来源：http://crp.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://kxj.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://ele.uphjek.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://npk.shanyushiyangkeji.top

Java: System.out.println("Hello, World!");
来源：http://xqu.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://ipc.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://zjw.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hrt.fktsv.cn

[A02] 变量声明与赋值
来源：http://qxo.hcnkem.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oky.cucudq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wgs.cdnleiting.top

JS:   let name = "Alex"; const age = 20;
来源：http://emi.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qwh.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://abr.sweek.top

Go:   name := "Alex"; age := 20
来源：http://bcp.pycfn.com

Ruby: name = "Alex"; age = 20
来源：http://qvl.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://bnw.jinqigufen.top

[A03] 常量定义
来源：http://lth.xingfuxueyuan.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aca.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://dda.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://fcf.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://tcz.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://bvz.chenlongwang.top

Go:   const PI = 3.14159
来源：http://iui.yonumen.top

Ruby: PI = 3.14159
来源：http://jkm.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://gyq.ybcxt.top

[A04] 判断变量类型
来源：http://jyk.xingfuxueyuan.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://vik.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://foz.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vdc.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://ovd.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wpz.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://agq.wangshuangyany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kfx.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://hhn.tanke756.top

[A05] 整数除法与取模
来源：http://edk.cheryme.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tdf.sysykeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://twd.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pjf.jlsjyb.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jbm.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://jao.mhx1999.top

Go:   7 / 2; 7 % 2
来源：http://cis.cashguo.top

Ruby: 7 / 2; 7 % 2
来源：http://gck.svipenyu.cn

C#:   7 / 2; 7 % 2
来源：http://frc.nanxuanxn.top

[A06] 字符串转数字
来源：http://ftw.zhixingplan.top

Py:   int("42"); float("3.14")
来源：http://prn.9152youxi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gzb.andypj.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zrs.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://yec.tanke756.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nbt.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hnq.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kzp.havefunace.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kqj.xuanzx.com

[A07] 数字转字符串
来源：http://zia.sysykeji.top

Py:   str(42)
来源：http://hay.c1oappe.top

PHP:  (string) 42; strval(42)
来源：http://reu.jyoumei.cn

JS:   String(42); (42).toString()
来源：http://gaa.hesvh.cn

TS:   String(42)
来源：http://byr.zhaomingkeji.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://amt.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://skw.yj202588.top

Ruby: 42.to_s
来源：http://pxz.sysykeji.top

C#:   42.ToString()
来源：http://zdr.hnqzz.top

[A08] 取整与四舍五入
来源：http://vml.smart0.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pmc.xingfuxueyuan.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mrq.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sak.cdnleiting.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jmm.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ztb.hysaishi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yhg.hnqzz.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://apz.shangyingyoupin.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tzn.zhaomingkeji.xyz

[A09] 绝对值与最大最小值
来源：http://mre.chenlongwang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ocx.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://okl.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fid.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kiq.zhixingplan.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oza.chenjidiqi.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xne.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kbk.nanxinkj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rlf.c1oappe.top


<!-- 参考信息 -->