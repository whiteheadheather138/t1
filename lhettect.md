代发 wailian999

[U57] PHP：字符串插值
来源：http://vjy.svipenyu.cn

"值: {$a}"
来源：http://xpl.epnwcf.com

[U58] PHP：数组三件套
来源：http://emx.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ncj.0kj1m.cn

[U59] PHP：自定义排序
来源：http://yph.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://myp.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://koy.jyoumei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jbc.yueranfly.top

[U61] PHP：正则
来源：http://hqv.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://irm.guannengcc.top

[U62] PHP：日期对象
来源：http://pzt.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mnz.snrcjt.cn

[U63] PHP：文件读写
来源：http://cis.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fgd.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://ynq.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://mws.c1oappe.top

[U65] PHP：会话
来源：http://rdv.guannengcc.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wed.guannengcc.top

[U66] PHP：设置 Cookie
来源：http://qqx.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lvw.cashguo.top

[U67] PHP：处理文件上传
来源：http://yct.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://izl.zycfv.cn

[U68] PHP：PDO 连接
来源：http://rgs.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wvy.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://eig.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ozr.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://xoi.zdqjudy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fbx.iojbl.cn

[U71] PHP：抛出异常
来源：http://nlh.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://qzk.yj20258.top

[U72] PHP：写错误日志
来源：http://gfd.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://hpu.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://vzx.yj20258.top

parse_ini_file("config.ini", true)
来源：http://fhu.hongshengwenyu.top

[U74] PHP：读取环境变量
来源：http://sqa.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://zld.nwbrower.top

[U75] PHP：依赖注入
来源：http://yai.jqgfzy.top

composer require psr/container
来源：http://dwe.tian-w.cn

[U76] PHP：简单路由
来源：http://gnk.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fxn.havefunace.top

[U77] PHP：模板渲染
来源：http://nla.shuidangran.top

composer require twig/twig
来源：http://oaw.tianlin.xyz

[U78] PHP：单元测试
来源：http://jyc.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://kqy.shanyushiyangtech.top

[U79] PHP：静态分析
来源：http://ugc.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://abs.xinyue.icu

[U80] PHP：代码规范修复
来源：http://llp.yonumen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zds.yongpay.top

[U81] JS：初始化项目
来源：http://gzh.kuanghao11.cn

npm init -y;  npm i express
来源：http://jjw.guannengcc.top

[U82] JS：package.json 脚本
来源：http://rof.xingfuxueyuan.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://krj.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://gdn.aizwys.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dun.havefunace.top

[U84] JS：CommonJS 写法
来源：http://ydk.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://mfl.0kj1m.cn

[U85] JS：可选链
来源：http://pay.yangfankeji.com

a?.b?.c
来源：http://rna.birdmap.top

[U86] JS：空值合并
来源：http://nqa.jinqigfzy.top

a ?? b
来源：http://tlm.fengsongda.top

[U87] JS：解构默认值
来源：http://nrt.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://adg.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://vnq.redwolf501.top

{ ...a, ...b }
来源：http://joe.yanxiufei.cn

[U89] JS：数组去重
来源：http://urt.ppjwa.cn

[...new Set(arr)]
来源：http://ume.smart0.xyz

[U90] JS：数字数组排序
来源：http://ely.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://ddd.c1oappe.top

[U91] JS：对象键值遍历
来源：http://qgg.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wag.zycfv.cn

[U92] JS：深拷贝
来源：http://amw.ywan-chungtsiang.top

structuredClone(obj)
来源：http://rnt.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://nxi.uphjek.com

`共 ${n} 条`
来源：http://otd.nanxuanxn.top

[U94] JS：箭头函数
来源：http://bfz.gogol.net.cn

const double = x => x * 2;
来源：http://ezp.yangfankeji.com

[U95] JS：Promise 包装
来源：http://ybf.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://yca.hcnkem.com

[U96] JS：async/await 与异常
来源：http://fwg.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://orq.hcnkem.com

[U97] JS：并发请求
来源：http://oqh.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xqk.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://dta.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lwt.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://uym.pycfn.com

el.addEventListener("click", e => {})
来源：http://tlt.yj20258888.top

[U100] JS：DOM 查询
来源：http://tsl.gaohongyu789.top

document.querySelector(".item")
来源：http://wkv.zhijiandao.cn

[U101] JS：classList 操作
来源：http://xct.snrcjt.cn

el.classList.toggle("active")
来源：http://ohr.sxryk.cn

[U102] JS：本地存储
来源：http://ugi.xinyue.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://ntp.shanyushiyangtech.top

[U103] JS：定时器
来源：http://fcr.uphjek.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iqj.gotoacloud.top

[U104] JS：防抖
来源：http://qoy.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://phe.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://nil.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ysu.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://xio.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zbs.yfazqb.com

[U107] JS：数字千分位
来源：http://fci.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://epw.sufxvd.cn

[U108] JS：随机整数
来源：http://gqr.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kli.ydzc1.top

[U109] JS：数组分组
来源：http://smr.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://vgm.guannengcc.top

[U110] JS：数组分块
来源：http://rqa.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cjc.redwolf501.top

[U111] JS：对象转 Map
来源：http://atg.uphjek.com

new Map(Object.entries(obj))
来源：http://gdk.meibo888.top

[U112] JS：字符串补位
来源：http://ryc.sxryk.cn

"7".padStart(3, "0")
来源：http://uig.zhixingplan.top

[U113] JS：正则替换全部
来源：http://yzk.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://cbd.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://rov.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vqu.gotoacloud.top

[U115] JS：生成 UUID
来源：http://haw.daxiang520.top

crypto.randomUUID()
来源：http://sqi.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://bxi.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://top.aizwys.cn

[U117] JS：单元测试
来源：http://klk.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://jrc.hnxiangtu.top

[U118] JS：开发服务器
来源：http://xlb.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://bxc.hcnkem.com

[U119] JS：生产构建
来源：http://hux.ydzc1.top

npx vite build
来源：http://egx.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://zyz.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://vxw.kuanghao11.cn

================================================================================
来源：http://nii.jyoumei.cn

统计汇总
来源：http://yac.iojbl.cn

================================================================================
来源：http://qwq.nwbrower.top

按语言统计（条）：
来源：http://yum.daxiang520.top

Python ......... 252
来源：http://zsf.shanyushiyangkeji.top

PHP ............ 252
来源：http://jik.316326.xyz

JavaScript ..... 252
来源：http://ldx.yueranfly.top

TypeScript ..... 212
来源：http://yor.jiagoushi.top

Java ........... 212
来源：http://yik.fktsv.cn

Go ............. 212
来源：http://qmq.hnqzz.top

Ruby ........... 212
来源：http://ttm.zhijiandao.cn

C# ............. 212
来源：http://zou.52xcode.cn

C .............. 30
来源：http://qdt.shanyushiyangkeji.top

C++ ............ 30
来源：http://ccj.ydzc1.top

SQL ............ 90
来源：http://udl.mhx1999.top

Bash ........... 80
来源：http://lxk.chenlongwang.top

Kotlin ......... 15
来源：http://lmi.gaohongyu789.top

Swift .......... 15
来源：http://lqk.uphjek.com

Lua ............ 10
来源：http://fef.jianghu66.top

Perl ........... 10
来源：http://ifx.gzhubu.top

Scala .......... 10
来源：http://nsz.zhoulong.xyz

------------------------------------
来源：http://fxd.svipenyu.cn

合计 ........... 2106 条
来源：http://ccr.ydjk.org.cn

按章节统计：
来源：http://cxt.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://awx.daria6918.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cie.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ixt.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bdn.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ooo.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jnh.tianlin.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kqp.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zbr.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://whp.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://thp.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://raw.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://njp.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zdj.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ivv.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vay.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lio.cashguo.top

Q SQL 专题                              90
来源：http://pad.sufxvd.cn

R Bash 专题                             80
来源：http://btq.ivvv.top

S C / C++ 专题                          60
来源：http://bdo.birdmap.top

T 其他语言补充                          60
来源：http://ugk.sjlbkw.cn

U 高频实用片段                         120
来源：http://xox.chenlongwang.top

------------------------------------
来源：http://tbp.shangyingyoupin.top

合计                                  2106 条
来源：http://fff.daria6918.cn

--------------------------------------------------------------------------------
来源：http://ewp.gotoacloud.top

使用提醒
来源：http://hbu.uphjek.com

--------------------------------------------------------------------------------
来源：http://aig.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qkw.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wtz.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lsr.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://exk.xingfuxueyuan.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rcy.zycfv.cn

—— 文件结束 ——
来源：http://iea.ivvv.top

================================================================================
来源：http://dov.cdnleiting.top

程序语言常见例子速查手册（2024 版）
来源：http://mhe.hcnkem.com

Common Programming Examples Cheat Book
来源：http://bub.dashuyun.cn

================================================================================
来源：http://gyp.tian-w.cn

【收录内容】
来源：http://utj.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uee.zhengqikj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bsv.bbcook.cn

SQL · Bash · C · C++
来源：http://qle.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xdv.guannengcc.top

【使用说明】
来源：http://tjv.chenlongwang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lse.hnqzz.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eik.guowangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dpn.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zgo.tarul.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sun.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vjs.hysaishi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dwv.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cpa.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bmt.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wlc.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ojl.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uif.bbcook.cn

【文件统计】
来源：http://gur.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://odg.sysykeji.top

--------------------------------------------------------------------------------
来源：http://uje.c1oappe.top

目  录
来源：http://rel.smart0.xyz

--------------------------------------------------------------------------------
来源：http://xat.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oel.zhaomingkeji.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://flt.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xib.cqqwz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yqt.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pla.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jba.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cvj.jqgfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oos.0kj1m.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fln.yongpay.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://inx.tarul.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sys.tianlin.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://amf.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hdc.hnqzz.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ylc.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ugs.smart0.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mio.tian-w.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xeb.bjfxy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://igq.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rbz.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pni.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iyx.zhaomingkeji.xyz

================================================================================
来源：http://lfs.yj202588.top

A. 基础语法与类型
来源：http://hqh.xylfe.cn

================================================================================
来源：http://ads.ctjpmb.com

[A01] Hello World
来源：http://udv.yanxiufei.cn

Py:   print("Hello, World!")
来源：http://rad.tarul.cn

PHP:  echo "Hello, World!";
来源：http://hvw.haohaochexian.top

JS:   console.log("Hello, World!");
来源：http://udt.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nwm.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://wmq.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://iau.dashuyun.cn

Ruby: puts "Hello, World!"
来源：http://qmt.xuetiantiany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gmb.yuxming.cn

[A02] 变量声明与赋值
来源：http://ekk.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ura.sufxvd.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://eya.cheryme.top

JS:   let name = "Alex"; const age = 20;
来源：http://not.mhx1999.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nne.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://cbb.0kj1m.cn

Go:   name := "Alex"; age := 20
来源：http://doj.yuxming.cn

Ruby: name = "Alex"; age = 20
来源：http://xme.daxiang520.top

C#:   string name = "Alex"; int age = 20;
来源：http://oxz.gzhubu.top

[A03] 常量定义
来源：http://gai.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gor.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://ais.sweek.top

JS:   const PI = 3.14159;
来源：http://awk.sweek.top

TS:   const PI: number = 3.14159;
来源：http://nmn.zhongyouzk.top

Java: static final double PI = 3.14159;
来源：http://qqk.zycfv.cn

Go:   const PI = 3.14159
来源：http://sgf.316326.xyz

Ruby: PI = 3.14159
来源：http://ehv.zhongyouzk.top

C#:   const double PI = 3.14159;
来源：http://bvw.jyoumei.cn

[A04] 判断变量类型
来源：http://xlq.zdqjudy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://elj.jinqigfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cbd.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://niq.shzxlz.cn

TS:   typeof x; x instanceof Date
来源：http://pwe.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://skz.sxryk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xbp.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yuq.cqqwz.cn

C#:   x.GetType().Name; x is int
来源：http://zdc.bjfxy.top

[A05] 整数除法与取模
来源：http://ezs.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vxm.cheryme.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://guj.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ysg.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nhq.guannengcc.top

Java: 7 / 2; 7 % 2
来源：http://jpy.wangshuangyany.cn

Go:   7 / 2; 7 % 2
来源：http://gof.hnqzz.top

Ruby: 7 / 2; 7 % 2
来源：http://azi.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://ver.bjfxy.top

[A06] 字符串转数字
来源：http://htg.zhijiandao.cn

Py:   int("42"); float("3.14")
来源：http://liz.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wdj.sweek.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vqa.uphjek.com

TS:   parseInt("42", 10); Number("42")
来源：http://ibr.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gdm.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rzm.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rcp.fengsongda.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pxr.yfazqb.com

[A07] 数字转字符串
来源：http://eur.daria6918.cn

Py:   str(42)
来源：http://jdv.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://qaw.yj20258.top

JS:   String(42); (42).toString()
来源：http://evw.hammf.cn

TS:   String(42)
来源：http://hmq.nanxuanxn.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://eto.ywan-chungtsiang.top

Go:   strconv.Itoa(42)
来源：http://fbj.ybcxt.top

Ruby: 42.to_s
来源：http://cva.hnxiangtu.top

C#:   42.ToString()
来源：http://ynq.fktsv.cn

[A08] 取整与四舍五入
来源：http://ucp.wangshuangyany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wzk.svipenyu.cn


<!-- 参考信息 -->