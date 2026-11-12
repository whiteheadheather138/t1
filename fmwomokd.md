代发 wailian999

[U55] PHP：match 表达式
来源：http://zme.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gpa.tian-w.cn

[U56] PHP：命名参数
来源：http://mwb.zdbjq.cn

f(a: 1, b: 2)
来源：http://vho.yj202588.top

[U57] PHP：字符串插值
来源：http://rto.daxiang520.top

"值: {$a}"
来源：http://uch.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://gun.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wyc.cqqwz.cn

[U59] PHP：自定义排序
来源：http://rqr.svipenyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hyy.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://prs.epnwcf.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jna.zdqjudy.top

[U61] PHP：正则
来源：http://gme.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oix.chenlongwang.top

[U62] PHP：日期对象
来源：http://bbv.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hov.tian-w.cn

[U63] PHP：文件读写
来源：http://veo.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ywc.fzhhl.top

[U64] PHP：目录遍历
来源：http://pvt.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://hkq.ivvv.top

[U65] PHP：会话
来源：http://unj.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rxg.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://slp.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://euh.316326.xyz

[U67] PHP：处理文件上传
来源：http://nlc.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ndj.tarul.cn

[U68] PHP：PDO 连接
来源：http://fsn.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://itj.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://adv.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://val.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://vrf.jianghu66.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wjd.chenlongwang.top

[U71] PHP：抛出异常
来源：http://slm.shangyingyoupin.top

throw new RuntimeException("失败", 500);
来源：http://otf.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://lgz.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://cmw.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://ktp.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://gwh.yj20258.top

[U74] PHP：读取环境变量
来源：http://cih.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://ldv.hfpthk.cn

[U75] PHP：依赖注入
来源：http://mjl.ctjpmb.com

composer require psr/container
来源：http://ddr.smart0.xyz

[U76] PHP：简单路由
来源：http://hrh.shzxlz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://avz.aibaodan.cn

[U77] PHP：模板渲染
来源：http://cse.yanxiufei.cn

composer require twig/twig
来源：http://aoi.bbcook.cn

[U78] PHP：单元测试
来源：http://iid.meibo888.top

composer require --dev phpunit/phpunit
来源：http://enw.tianlin.xyz

[U79] PHP：静态分析
来源：http://wgs.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://aee.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://txa.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://soj.jyoumei.cn

[U81] JS：初始化项目
来源：http://dsm.fehbvm.com

npm init -y;  npm i express
来源：http://tpl.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://hdm.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qjj.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://rnh.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://mrr.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://fdq.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://beb.snrcjt.cn

[U85] JS：可选链
来源：http://jia.yfazqb.com

a?.b?.c
来源：http://guj.yongpay.top

[U86] JS：空值合并
来源：http://xwf.yuanzhike.top

a ?? b
来源：http://zwr.zycfv.cn

[U87] JS：解构默认值
来源：http://hdo.pycfn.com

const { a = 1, b = 2 } = obj;
来源：http://mch.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://fai.havefunace.top

{ ...a, ...b }
来源：http://hph.yangfankeji.com

[U89] JS：数组去重
来源：http://hjd.yanxiufei.cn

[...new Set(arr)]
来源：http://rns.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://glf.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://sod.andypj.xyz

[U91] JS：对象键值遍历
来源：http://gbp.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hqn.feifeiyinyue.top

[U92] JS：深拷贝
来源：http://sup.cqqwz.cn

structuredClone(obj)
来源：http://vqb.ydjk.org.cn

[U93] JS：模板字符串
来源：http://dti.vqdsnc.cn

`共 ${n} 条`
来源：http://kdc.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://mfr.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://dsn.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://cfo.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://mnc.mhx1999.top

[U96] JS：async/await 与异常
来源：http://kjb.hywenlv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fse.zhengqikj.top

[U97] JS：并发请求
来源：http://qeo.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oyl.meibo888.top

[U98] JS：fetch 带 JSON
来源：http://akf.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gag.bjfxy.top

[U99] JS：事件监听
来源：http://sof.gzhubu.top

el.addEventListener("click", e => {})
来源：http://qau.zhoulong.xyz

[U100] JS：DOM 查询
来源：http://mfx.jinghuilouyu.cn

document.querySelector(".item")
来源：http://xkt.hcnkem.com

[U101] JS：classList 操作
来源：http://oza.yonumen.top

el.classList.toggle("active")
来源：http://qsw.hywenlv.cn

[U102] JS：本地存储
来源：http://ekz.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ovq.sjlbkw.cn

[U103] JS：定时器
来源：http://bmr.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ops.snrcjt.cn

[U104] JS：防抖
来源：http://nvb.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fnq.cheryme.top

[U105] JS：节流
来源：http://jbs.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hbi.dianchejie.cn

[U106] JS：日期格式化
来源：http://cxc.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zyz.fktsv.cn

[U107] JS：数字千分位
来源：http://wbj.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tri.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://tbw.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yai.feifeiyinyue.top

[U109] JS：数组分组
来源：http://cfp.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://xuo.bbcook.cn

[U110] JS：数组分块
来源：http://fgb.xinyue.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ohu.yfazqb.com

[U111] JS：对象转 Map
来源：http://scp.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://ktw.dianchejie.cn

[U112] JS：字符串补位
来源：http://lhh.nanxinkj.top

"7".padStart(3, "0")
来源：http://hbh.guowangkeji.top

[U113] JS：正则替换全部
来源：http://cmq.yonumen.top

s.replaceAll("a", "b")
来源：http://shm.hongshengwenyu.top

[U114] JS：JSON 深比较
来源：http://fzh.xylfe.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kpe.sufxvd.cn

[U115] JS：生成 UUID
来源：http://ehm.jinqigfzy.top

crypto.randomUUID()
来源：http://nyj.fzhhl.top

[U116] JS：类型检查（JSDoc）
来源：http://own.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://vne.andypj.xyz

[U117] JS：单元测试
来源：http://clo.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://uzm.xziqi.cn

[U118] JS：开发服务器
来源：http://qlv.hfpthk.cn

npm i -D vite;  npx vite
来源：http://fyy.wangshuangyany.cn

[U119] JS：生产构建
来源：http://tbz.daxiang520.top

npx vite build
来源：http://jdd.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://led.hcnkem.com

import.meta.env.VITE_API_URL
来源：http://enz.xziqi.cn

================================================================================
来源：http://rmo.guannengcc.top

统计汇总
来源：http://fjd.shanyushiyangkeji.top

================================================================================
来源：http://cts.yj20258.top

按语言统计（条）：
来源：http://dod.ctjpmb.com

Python ......... 252
来源：http://dja.vehdjk.com

PHP ............ 252
来源：http://xli.shangyingyoupin.top

JavaScript ..... 252
来源：http://poq.c1oappe.top

TypeScript ..... 212
来源：http://bmz.zhiwuduotai.top

Java ........... 212
来源：http://act.kuanghao11.cn

Go ............. 212
来源：http://cqg.cqqwz.cn

Ruby ........... 212
来源：http://wav.ywan-chungtsiang.top

C# ............. 212
来源：http://kvs.daxiang520.top

C .............. 30
来源：http://kxj.svipenyu.cn

C++ ............ 30
来源：http://ozq.316326.xyz

SQL ............ 90
来源：http://uab.yvedp.cn

Bash ........... 80
来源：http://yvx.kuanghao11.cn

Kotlin ......... 15
来源：http://rqj.jinghuilouyu.cn

Swift .......... 15
来源：http://vjc.hnqzz.top

Lua ............ 10
来源：http://xbi.tianlin.xyz

Perl ........... 10
来源：http://lrg.haohaochexian.top

Scala .......... 10
来源：http://ojr.birdmap.top

------------------------------------
来源：http://jug.ppjwa.cn

合计 ........... 2106 条
来源：http://azl.ybcxt.top

按章节统计：
来源：http://ksv.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cnm.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vdq.cashguo.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pvi.quarkkingdee.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hvv.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oqt.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dqd.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qop.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ihk.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lrj.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://arf.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sar.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://axl.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kot.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rwa.ywan-chungtsiang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hqv.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ged.jqgfzy.top

Q SQL 专题                              90
来源：http://xph.tarul.cn

R Bash 专题                             80
来源：http://snd.chenlongwang.top

S C / C++ 专题                          60
来源：http://pdy.nanxuanxn.top

T 其他语言补充                          60
来源：http://keg.sweek.top

U 高频实用片段                         120
来源：http://onl.ybcxt.top

------------------------------------
来源：http://bzd.sysykeji.top

合计                                  2106 条
来源：http://vyo.c1oappe.top

--------------------------------------------------------------------------------
来源：http://gbi.yj20258.top

使用提醒
来源：http://ckj.jianghu66.top

--------------------------------------------------------------------------------
来源：http://ali.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ein.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tab.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tjs.hysaishi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ptg.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ujr.nanxuanxn.top

—— 文件结束 ——
来源：http://ijk.jinqigfzy.top

================================================================================
来源：http://ofn.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://jiz.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://gaf.jinghuilouyu.cn

================================================================================
来源：http://cxj.zhiwuduotai.top

【收录内容】
来源：http://bks.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gnq.yj20258.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tik.tianlin.xyz

SQL · Bash · C · C++
来源：http://upx.zhaomingkeji.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ntv.zdqjudy.top

【使用说明】
来源：http://bjz.zhiwuduotai.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iei.chenjidiqi.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gzh.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://feb.hnqzz.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zzx.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vpf.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tzu.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ubo.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rrm.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hjg.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qmx.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xkt.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qrj.nwbrower.top

【文件统计】
来源：http://mdq.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ylo.xinyue.icu

--------------------------------------------------------------------------------
来源：http://zfa.epnwcf.com

目  录
来源：http://bpi.shuidangran.top

--------------------------------------------------------------------------------
来源：http://tms.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iwk.shzxlz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ult.jinyuanbaomall.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ofk.sysykeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yak.guowangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fgq.smart0.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xig.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ibq.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jgz.yuxming.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ums.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ibc.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://seq.c1oappe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hjl.fengsongda.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wjn.cqqwz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ued.chenzaomai.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://olt.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vwp.sysykeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uex.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wks.wangshuangyany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rzw.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yax.hesvh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fxr.jianghu66.top

================================================================================
来源：http://yfw.andypj.xyz

A. 基础语法与类型
来源：http://mpv.jqgufenzy.top

================================================================================
来源：http://phl.hnxiangtu.top

[A01] Hello World
来源：http://ntg.bbcook.cn

Py:   print("Hello, World!")
来源：http://ofy.jqgfzy.top

PHP:  echo "Hello, World!";
来源：http://foj.yj202588.top

JS:   console.log("Hello, World!");
来源：http://fky.yongpay.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://exn.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://imy.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://rup.cheryme.top

Ruby: puts "Hello, World!"
来源：http://wpz.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://jml.iojbl.cn

[A02] 变量声明与赋值
来源：http://fbo.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vli.hywenlv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zpr.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://nwp.vehdjk.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cwk.tanke756.top

Java: String name = "Alex"; int age = 20;
来源：http://auh.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://uiq.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://nmi.zhoulong.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://mcl.fengsongda.top

[A03] 常量定义
来源：http://azn.wangshuangyany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vtt.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://irs.zhoulong.xyz

JS:   const PI = 3.14159;
来源：http://tfn.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://owu.gogol.net.cn

Java: static final double PI = 3.14159;
来源：http://dnd.dashuyun.cn

Go:   const PI = 3.14159
来源：http://iie.52xcode.cn

Ruby: PI = 3.14159
来源：http://qgi.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://dgc.quarkkingdee.top

[A04] 判断变量类型
来源：http://mil.ppjwa.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jon.zdqjudy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dax.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zwa.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://hnb.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kbk.cucudq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wzc.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kbk.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://iwe.jinqigfzy.top

[A05] 整数除法与取模
来源：http://eau.sjlbkw.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cgi.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uhy.sxryk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gzo.wangshuangyany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qcu.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://dxp.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://hkk.fehbvm.com

Ruby: 7 / 2; 7 % 2
来源：http://ahv.gzhubu.top

C#:   7 / 2; 7 % 2
来源：http://mhw.daria6918.cn

[A06] 字符串转数字
来源：http://ojy.zhengqikj.top

Py:   int("42"); float("3.14")
来源：http://ibz.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iip.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ooq.ppjwa.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zui.jinqigfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jty.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lgn.cheryme.top

Ruby: "42".to_i; "3.14".to_f
来源：http://epi.sxryk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cnw.9152youxi.cn

[A07] 数字转字符串
来源：http://gdp.cdnleiting.top

Py:   str(42)
来源：http://ywt.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://oam.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://zjy.ydjk.org.cn

TS:   String(42)
来源：http://fsj.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ukr.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://yoc.yj20258888.top


<!-- 参考信息 -->