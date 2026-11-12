代发 wailian999

[U57] PHP：字符串插值
来源：http://wqs.iojbl.cn

"值: {$a}"
来源：http://cld.zycfv.cn

[U58] PHP：数组三件套
来源：http://dzd.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://otl.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://nou.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ypg.hammf.cn

[U60] PHP：JSON 编解码
来源：http://mnv.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://myf.bjfxy.top

[U61] PHP：正则
来源：http://bqo.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ikv.nanxinkj.top

[U62] PHP：日期对象
来源：http://rcn.zhijiandao.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iph.chenzaomai.com

[U63] PHP：文件读写
来源：http://apv.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hib.ybcxt.top

[U64] PHP：目录遍历
来源：http://grj.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://tlt.cucudq.cn

[U65] PHP：会话
来源：http://bxu.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bbi.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://gzs.nanxuanxn.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ekw.birdmap.top

[U67] PHP：处理文件上传
来源：http://vty.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lft.xylfe.cn

[U68] PHP：PDO 连接
来源：http://dhl.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sww.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://awr.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ixu.nwbrower.top

[U70] PHP：PDO 事务
来源：http://qad.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mnq.shuidangran.top

[U71] PHP：抛出异常
来源：http://owa.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://foi.ybcxt.top

[U72] PHP：写错误日志
来源：http://jay.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://nfl.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://lgp.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://edh.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://tlo.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://fpm.ehwqpu.com

[U75] PHP：依赖注入
来源：http://olh.gaohongyu789.top

composer require psr/container
来源：http://shg.ctjpmb.com

[U76] PHP：简单路由
来源：http://jnz.ydjk.org.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kgn.fktsv.cn

[U77] PHP：模板渲染
来源：http://kzf.yuxming.cn

composer require twig/twig
来源：http://ehc.cdnleiting.top

[U78] PHP：单元测试
来源：http://ofl.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://hpy.bjfxy.top

[U79] PHP：静态分析
来源：http://yua.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://frg.yongpay.top

[U80] PHP：代码规范修复
来源：http://dyz.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qip.zhixingplan.top

[U81] JS：初始化项目
来源：http://sbb.zdbjq.cn

npm init -y;  npm i express
来源：http://dsn.hcnkem.com

[U82] JS：package.json 脚本
来源：http://joh.jinqigufen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nxq.fzhhl.top

[U83] JS：ES Module 导入导出
来源：http://spy.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://vkh.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://nrw.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://sfg.ctjpmb.com

[U85] JS：可选链
来源：http://ila.mhx1999.top

a?.b?.c
来源：http://utu.cashguo.top

[U86] JS：空值合并
来源：http://dki.xuanzx.com

a ?? b
来源：http://ayj.andypj.xyz

[U87] JS：解构默认值
来源：http://zlc.hcnkem.com

const { a = 1, b = 2 } = obj;
来源：http://rnj.hnqzz.top

[U88] JS：对象展开合并
来源：http://zsp.hongshengwenyu.top

{ ...a, ...b }
来源：http://yok.zhixingplan.top

[U89] JS：数组去重
来源：http://fhg.316326.xyz

[...new Set(arr)]
来源：http://fhm.zhixingplan.top

[U90] JS：数字数组排序
来源：http://syy.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://two.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://phd.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fnq.316326.xyz

[U92] JS：深拷贝
来源：http://rso.yj20258888.top

structuredClone(obj)
来源：http://jil.snrcjt.cn

[U93] JS：模板字符串
来源：http://gqi.feifeiyinyue.top

`共 ${n} 条`
来源：http://nvm.sjlbkw.cn

[U94] JS：箭头函数
来源：http://elb.tanke756.top

const double = x => x * 2;
来源：http://etn.meibo888.top

[U95] JS：Promise 包装
来源：http://ojf.yuxming.cn

new Promise((resolve, reject) => {})
来源：http://qja.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://qlm.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fds.gogol.net.cn

[U97] JS：并发请求
来源：http://wev.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xfp.fehbvm.com

[U98] JS：fetch 带 JSON
来源：http://zte.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qho.zhixingplan.top

[U99] JS：事件监听
来源：http://zgu.xuanzx.com

el.addEventListener("click", e => {})
来源：http://bjg.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://ekk.daxiang520.top

document.querySelector(".item")
来源：http://dae.zhiwuduotai.top

[U101] JS：classList 操作
来源：http://byg.wangdashe.top

el.classList.toggle("active")
来源：http://zbn.0kj1m.cn

[U102] JS：本地存储
来源：http://skz.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dqe.bbcook.cn

[U103] JS：定时器
来源：http://vbw.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tvk.tarul.cn

[U104] JS：防抖
来源：http://hxf.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kcb.0kj1m.cn

[U105] JS：节流
来源：http://sma.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vyi.9152youxi.cn

[U106] JS：日期格式化
来源：http://ric.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ewa.guowangkeji.top

[U107] JS：数字千分位
来源：http://bhh.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ivh.gotoacloud.top

[U108] JS：随机整数
来源：http://hkp.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nuu.ehwqpu.com

[U109] JS：数组分组
来源：http://pxf.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://mvy.shangyingyoupin.top

[U110] JS：数组分块
来源：http://ujr.gogol.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mjb.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://wck.yueranfly.top

new Map(Object.entries(obj))
来源：http://idc.sufxvd.cn

[U112] JS：字符串补位
来源：http://hfx.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://uhr.epnwcf.com

[U113] JS：正则替换全部
来源：http://iod.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://qra.guannengcc.top

[U114] JS：JSON 深比较
来源：http://muk.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qpv.ctjpmb.com

[U115] JS：生成 UUID
来源：http://blb.nanxinkj.top

crypto.randomUUID()
来源：http://ris.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://lcu.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://xyf.mhx1999.top

[U117] JS：单元测试
来源：http://dhd.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://lxu.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://dkh.aizwys.cn

npm i -D vite;  npx vite
来源：http://tqw.ehwqpu.com

[U119] JS：生产构建
来源：http://lcd.52xcode.cn

npx vite build
来源：http://yty.xingfuxueyuan.xyz

[U120] JS：读取环境变量（Vite）
来源：http://vvg.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://olq.hcnkem.com

================================================================================
来源：http://mqc.yueranfly.top

统计汇总
来源：http://gcl.zhengqikj.top

================================================================================
来源：http://sbi.redwolf501.top

按语言统计（条）：
来源：http://ttk.yj20258.top

Python ......... 252
来源：http://otu.shzxlz.cn

PHP ............ 252
来源：http://mtr.daria6918.cn

JavaScript ..... 252
来源：http://fpw.52xcode.cn

TypeScript ..... 212
来源：http://pls.zdqjudy.top

Java ........... 212
来源：http://xqk.jinqigufen.top

Go ............. 212
来源：http://kro.iojbl.cn

Ruby ........... 212
来源：http://ihq.hcnkem.com

C# ............. 212
来源：http://pay.daxiang520.top

C .............. 30
来源：http://qla.bjfxy.top

C++ ............ 30
来源：http://nut.gogol.net.cn

SQL ............ 90
来源：http://zhw.yueranfly.top

Bash ........... 80
来源：http://sfm.sweek.top

Kotlin ......... 15
来源：http://yro.hammf.cn

Swift .......... 15
来源：http://nnj.zycfv.cn

Lua ............ 10
来源：http://mxt.fanxiaobao.xyz

Perl ........... 10
来源：http://mdu.hcnkem.com

Scala .......... 10
来源：http://oym.jyoumei.cn

------------------------------------
来源：http://eum.jyoumei.cn

合计 ........... 2106 条
来源：http://nkf.hcnkem.com

按章节统计：
来源：http://htk.svipenyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uwu.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bqh.zhixingplan.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ioo.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ixr.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qjt.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dts.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eqq.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fyr.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cxw.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wqp.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qkq.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nga.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uvk.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://slw.yj202588.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ptx.zhijiandao.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zke.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://lts.zycfv.cn

R Bash 专题                             80
来源：http://xkb.zhaomingkeji.xyz

S C / C++ 专题                          60
来源：http://fgd.meibo888.top

T 其他语言补充                          60
来源：http://eqg.zhixingplan.top

U 高频实用片段                         120
来源：http://gnl.nanxinkj.top

------------------------------------
来源：http://oyp.aizwys.cn

合计                                  2106 条
来源：http://yqx.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://bsq.zhixingplan.top

使用提醒
来源：http://fxf.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://nth.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wtz.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gku.snrcjt.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nos.redwolf501.top

在旧版本上使用前请先确认语法支持情况。
来源：http://glu.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lod.iojbl.cn

—— 文件结束 ——
来源：http://aow.0kj1m.cn

================================================================================
来源：http://nfc.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://dtr.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://yjo.sysykeji.top

================================================================================
来源：http://uks.bbcook.cn

【收录内容】
来源：http://dob.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rss.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ybv.uphjek.com

SQL · Bash · C · C++
来源：http://jpn.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bch.shuidangran.top

【使用说明】
来源：http://knm.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zgq.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qzo.fanxiaobao.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pyz.zdbjq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ghv.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mtj.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://egv.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mtn.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nmq.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://szn.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pwp.shanyushiyangtech.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zmv.vqdsnc.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ixo.zhaomingkeji.xyz

【文件统计】
来源：http://ppg.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vbb.meibo888.top

--------------------------------------------------------------------------------
来源：http://qcm.sjlbkw.cn

目  录
来源：http://qng.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://rsa.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dng.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ais.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://akd.hywenlv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pvt.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dqw.cucudq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ctj.xziqi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://txd.yanxiufei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nwo.sjlbkw.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fqf.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jdl.bbcook.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ppm.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xad.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bcs.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fjd.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cfv.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://soh.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gsg.yueranfly.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nwu.jiagoushi.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yxa.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yfz.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bta.yueranfly.top

================================================================================
来源：http://xnv.zhongyouzk.top

A. 基础语法与类型
来源：http://yfr.vqdsnc.cn

================================================================================
来源：http://qdw.uphjek.com

[A01] Hello World
来源：http://tob.svipenyu.cn

Py:   print("Hello, World!")
来源：http://qiv.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://svm.gaohongyu789.top

JS:   console.log("Hello, World!");
来源：http://nri.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oen.zhoulong.xyz

Java: System.out.println("Hello, World!");
来源：http://usw.fanxiaobao.xyz

Go:   fmt.Println("Hello, World!")
来源：http://hij.zdqjudy.top

Ruby: puts "Hello, World!"
来源：http://uok.haohaochexian.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xvp.52xcode.cn

[A02] 变量声明与赋值
来源：http://rll.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pyk.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rqh.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vxl.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bfe.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://cft.yanxiufei.cn

Go:   name := "Alex"; age := 20
来源：http://rlg.dashuyun.cn

Ruby: name = "Alex"; age = 20
来源：http://sao.yuanzhike.top

C#:   string name = "Alex"; int age = 20;
来源：http://pci.xylfe.cn

[A03] 常量定义
来源：http://edx.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sie.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://vic.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://gof.sweek.top

TS:   const PI: number = 3.14159;
来源：http://cjb.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://nfg.gzhubu.top

Go:   const PI = 3.14159
来源：http://leh.yj20258.top

Ruby: PI = 3.14159
来源：http://mgu.dashuyun.cn

C#:   const double PI = 3.14159;
来源：http://zji.hysaishi.cn

[A04] 判断变量类型
来源：http://ypn.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tor.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wco.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gnk.vehdjk.com

TS:   typeof x; x instanceof Date
来源：http://kfz.sufxvd.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qpu.tanke756.top

Go:   reflect.TypeOf(x).Name()
来源：http://kfi.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://xbp.wangshuangyany.cn

C#:   x.GetType().Name; x is int
来源：http://fdl.0kj1m.cn

[A05] 整数除法与取模
来源：http://cnm.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tyf.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iwl.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ehy.cucudq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jjm.cdnleiting.top

Java: 7 / 2; 7 % 2
来源：http://bgh.jyoumei.cn

Go:   7 / 2; 7 % 2
来源：http://eck.yuanzhike.top

Ruby: 7 / 2; 7 % 2
来源：http://tli.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://kwa.feifeiyinyue.top

[A06] 字符串转数字
来源：http://cgu.ivvv.top

Py:   int("42"); float("3.14")
来源：http://xlj.shanyushiyangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jjh.ydzc1.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://toc.shanyushiyangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://wde.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mbb.nanxuanxn.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hfy.yonumen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jow.zycfv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kic.yvedp.cn

[A07] 数字转字符串
来源：http://qba.ehwqpu.com

Py:   str(42)
来源：http://dts.tanke756.top

PHP:  (string) 42; strval(42)
来源：http://vei.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://wzp.chenzaomai.com

TS:   String(42)
来源：http://vdi.shzxlz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lht.aibaodan.cn

Go:   strconv.Itoa(42)
来源：http://fbx.iojbl.cn

Ruby: 42.to_s
来源：http://fpz.daria6918.cn

C#:   42.ToString()
来源：http://ers.meibo888.top

[A08] 取整与四舍五入
来源：http://rlv.gogol.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cba.nanxinkj.top


<!-- 参考信息 -->