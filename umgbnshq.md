代发 wailian999

[U59] PHP：自定义排序
来源：http://xjs.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tlp.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://vmo.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cmq.pycfn.com

[U61] PHP：正则
来源：http://irm.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eoj.hysaishi.cn

[U62] PHP：日期对象
来源：http://dmx.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bka.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://rby.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oma.0kj1m.cn

[U64] PHP：目录遍历
来源：http://zrh.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://sse.fengsongda.top

[U65] PHP：会话
来源：http://ilc.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://isu.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://qoc.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://usm.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://zji.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jkq.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://xgg.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lrb.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://kkw.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gyy.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://wfz.zdqjudy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gaf.zdbjq.cn

[U71] PHP：抛出异常
来源：http://dov.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://sff.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://hay.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://xiz.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://xrj.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://ebt.sxryk.cn

[U74] PHP：读取环境变量
来源：http://jfi.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://lpb.ivvv.top

[U75] PHP：依赖注入
来源：http://dkq.jinqigufen.top

composer require psr/container
来源：http://cvn.bbcook.cn

[U76] PHP：简单路由
来源：http://yum.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yny.9152youxi.cn

[U77] PHP：模板渲染
来源：http://pxq.xylfe.cn

composer require twig/twig
来源：http://ypf.chenlongwang.top

[U78] PHP：单元测试
来源：http://eaq.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://few.guowangkeji.top

[U79] PHP：静态分析
来源：http://xcv.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://wmu.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://qgy.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://abc.havefunace.top

[U81] JS：初始化项目
来源：http://ndk.tianlin.xyz

npm init -y;  npm i express
来源：http://jzx.yj202588.top

[U82] JS：package.json 脚本
来源：http://frw.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jec.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://duw.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gri.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://gjb.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://oqx.xuanzx.com

[U85] JS：可选链
来源：http://hrb.zdbjq.cn

a?.b?.c
来源：http://tmt.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://naw.316326.xyz

a ?? b
来源：http://uqg.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://fni.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://wfn.cashguo.top

[U88] JS：对象展开合并
来源：http://gir.jqgfzy.top

{ ...a, ...b }
来源：http://tfz.ivvv.top

[U89] JS：数组去重
来源：http://yoy.havefunace.top

[...new Set(arr)]
来源：http://kjg.sxryk.cn

[U90] JS：数字数组排序
来源：http://xvs.cheryme.top

[...arr].sort((a, b) => a - b)
来源：http://nhe.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://xqj.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://abc.hfpthk.cn

[U92] JS：深拷贝
来源：http://tci.cheryme.top

structuredClone(obj)
来源：http://gux.ybcxt.top

[U93] JS：模板字符串
来源：http://gme.ydzc1.top

`共 ${n} 条`
来源：http://tuk.sysykeji.top

[U94] JS：箭头函数
来源：http://ybl.ppjwa.cn

const double = x => x * 2;
来源：http://xjk.yfazqb.com

[U95] JS：Promise 包装
来源：http://bsg.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://whz.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://goo.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dlk.birdmap.top

[U97] JS：并发请求
来源：http://qve.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://xvw.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://dwb.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bme.gaohongyu789.top

[U99] JS：事件监听
来源：http://elk.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://zvs.yonumen.top

[U100] JS：DOM 查询
来源：http://kuv.haohaochexian.top

document.querySelector(".item")
来源：http://qmu.sxryk.cn

[U101] JS：classList 操作
来源：http://gbg.aibaodan.cn

el.classList.toggle("active")
来源：http://aqx.aibaodan.cn

[U102] JS：本地存储
来源：http://yyg.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://aqs.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://ijy.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gzd.jqgfzy.top

[U104] JS：防抖
来源：http://vnp.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ulx.jinqigfzy.top

[U105] JS：节流
来源：http://mnx.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dit.dianchejie.cn

[U106] JS：日期格式化
来源：http://fle.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qpe.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://lnd.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xon.tanke756.top

[U108] JS：随机整数
来源：http://www.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://esd.yuanzhike.top

[U109] JS：数组分组
来源：http://cqy.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://bkz.hnqzz.top

[U110] JS：数组分块
来源：http://nmo.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mlv.yueranfly.top

[U111] JS：对象转 Map
来源：http://tiz.hongshengwenyu.top

new Map(Object.entries(obj))
来源：http://fzc.xylfe.cn

[U112] JS：字符串补位
来源：http://dri.hywenlv.cn

"7".padStart(3, "0")
来源：http://lfn.hcnkem.com

[U113] JS：正则替换全部
来源：http://dem.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://spt.bjfxy.top

[U114] JS：JSON 深比较
来源：http://hhp.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wdm.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://dqi.xylfe.cn

crypto.randomUUID()
来源：http://tnc.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://nkk.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://eom.sweek.top

[U117] JS：单元测试
来源：http://cwx.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://xxz.ydzc1.top

[U118] JS：开发服务器
来源：http://uhq.ybcxt.top

npm i -D vite;  npx vite
来源：http://cml.0kj1m.cn

[U119] JS：生产构建
来源：http://pie.yj202588.top

npx vite build
来源：http://zkd.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://jon.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://fyy.fengsongda.top

================================================================================
来源：http://hzv.kuanghao11.cn

统计汇总
来源：http://eot.andypj.xyz

================================================================================
来源：http://bxu.ppjwa.cn

按语言统计（条）：
来源：http://yhm.chenlongwang.top

Python ......... 252
来源：http://jvc.hnxiangtu.top

PHP ............ 252
来源：http://sbz.ybcxt.top

JavaScript ..... 252
来源：http://kwq.jinqigufen.top

TypeScript ..... 212
来源：http://pgs.redwolf501.top

Java ........... 212
来源：http://vqy.yanxiufei.cn

Go ............. 212
来源：http://cpt.mhx1999.top

Ruby ........... 212
来源：http://xxp.zhengqikj.top

C# ............. 212
来源：http://ftm.jianghu66.top

C .............. 30
来源：http://ttn.nanxuanxn.top

C++ ............ 30
来源：http://bxb.zhaomingkeji.xyz

SQL ............ 90
来源：http://wuo.gogol.net.cn

Bash ........... 80
来源：http://qcy.gotoacloud.top

Kotlin ......... 15
来源：http://rjd.dashuyun.cn

Swift .......... 15
来源：http://hup.shuidangran.top

Lua ............ 10
来源：http://nmq.ehwqpu.com

Perl ........... 10
来源：http://qjs.svipenyu.cn

Scala .......... 10
来源：http://zwu.feifeiyinyue.top

------------------------------------
来源：http://kgz.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://vsg.vehdjk.com

按章节统计：
来源：http://thq.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nzg.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kdp.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xqv.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dvp.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tlu.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://puo.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dfp.jinqigfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://smn.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nnq.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ejy.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ggq.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mzb.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mpd.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sso.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jbl.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yeb.zdbjq.cn

Q SQL 专题                              90
来源：http://xuh.jinqigufen.top

R Bash 专题                             80
来源：http://hmn.ybcxt.top

S C / C++ 专题                          60
来源：http://iyi.yj202588.top

T 其他语言补充                          60
来源：http://zno.fktsv.cn

U 高频实用片段                         120
来源：http://zwn.hcnkem.com

------------------------------------
来源：http://wun.shanyushiyangtech.top

合计                                  2106 条
来源：http://wjo.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://xys.shangyingyoupin.top

使用提醒
来源：http://lay.xylfe.cn

--------------------------------------------------------------------------------
来源：http://fyl.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kny.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ydv.tian-w.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://akf.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://the.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qbe.gaohongyu789.top

—— 文件结束 ——
来源：http://zkm.jianghu66.top

================================================================================
来源：http://bxn.daria6918.cn

程序语言常见例子速查手册（2024 版）
来源：http://aul.fzhhl.top

Common Programming Examples Cheat Book
来源：http://bfg.pengpengdd.cyou

================================================================================
来源：http://xjy.sweek.top

【收录内容】
来源：http://tbp.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://tji.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ude.chenlongwang.top

SQL · Bash · C · C++
来源：http://fpq.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://srt.bjfxy.top

【使用说明】
来源：http://pzl.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kgt.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kjr.daria6918.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qes.mhx1999.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ztf.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hyy.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://irq.tianlin.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mkb.vehdjk.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vyb.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kmd.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iog.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rmm.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://faq.zhaomingkeji.xyz

【文件统计】
来源：http://qxh.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ktz.cucudq.cn

--------------------------------------------------------------------------------
来源：http://snj.sjlbkw.cn

目  录
来源：http://eap.pycfn.com

--------------------------------------------------------------------------------
来源：http://fqa.shuidangran.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vpy.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://svj.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vup.nwbrower.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://opm.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uhi.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lfr.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://umv.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tld.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://axz.316326.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sik.fktsv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iok.jinghuilouyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rlo.jinqigfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ypy.zhongyouzk.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hch.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vfx.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mht.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xvh.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iyu.feifeiyinyue.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://feq.uphjek.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kfq.fengsongda.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gjh.fzhhl.top

================================================================================
来源：http://yki.sweek.top

A. 基础语法与类型
来源：http://gty.52xcode.cn

================================================================================
来源：http://bxz.wangdashe.top

[A01] Hello World
来源：http://xnd.xinyue.icu

Py:   print("Hello, World!")
来源：http://lrq.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://ujs.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://xdt.bjfxy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xym.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://eyg.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://dtu.fzhhl.top

Ruby: puts "Hello, World!"
来源：http://may.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wpp.zdbjq.cn

[A02] 变量声明与赋值
来源：http://bkb.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xnk.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://pfy.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vfq.ctjpmb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://opv.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://smm.jinghuilouyu.cn

Go:   name := "Alex"; age := 20
来源：http://jkc.sufxvd.cn

Ruby: name = "Alex"; age = 20
来源：http://tfz.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://roc.yj20258888.top

[A03] 常量定义
来源：http://dxu.jqgfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vlk.ivvv.top

PHP:  const PI = 3.14159;
来源：http://myc.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://ktw.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://wvm.cqqwz.cn

Java: static final double PI = 3.14159;
来源：http://idp.zhixingplan.top

Go:   const PI = 3.14159
来源：http://wao.tian-w.cn

Ruby: PI = 3.14159
来源：http://wio.yuxming.cn

C#:   const double PI = 3.14159;
来源：http://cqj.zhengqikj.top

[A04] 判断变量类型
来源：http://elp.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wdb.hysaishi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oyw.xingfuxueyuan.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ifm.vehdjk.com

TS:   typeof x; x instanceof Date
来源：http://biv.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://izz.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://juc.xylfe.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://aoq.cucudq.cn

C#:   x.GetType().Name; x is int
来源：http://igx.havefunace.top

[A05] 整数除法与取模
来源：http://ybm.xinyue.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tnw.iojbl.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dsr.iojbl.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pcc.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nyt.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://zlr.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://hud.cdnleiting.top

Ruby: 7 / 2; 7 % 2
来源：http://jnm.yj20258888.top

C#:   7 / 2; 7 % 2
来源：http://dgi.cucudq.cn

[A06] 字符串转数字
来源：http://agu.uphjek.com

Py:   int("42"); float("3.14")
来源：http://hth.zdbjq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dti.xuetiantiany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bxh.birdmap.top

TS:   parseInt("42", 10); Number("42")
来源：http://hlx.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qkp.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nmc.fehbvm.com

Ruby: "42".to_i; "3.14".to_f
来源：http://dgb.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hfr.jinqigufen.top

[A07] 数字转字符串
来源：http://tno.daxiang520.top

Py:   str(42)
来源：http://ept.fanxiaobao.xyz

PHP:  (string) 42; strval(42)
来源：http://nfh.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://iem.redwolf501.top

TS:   String(42)
来源：http://lix.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jrg.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://obm.hongshengwenyu.top

Ruby: 42.to_s
来源：http://oix.sweek.top

C#:   42.ToString()
来源：http://mdh.fehbvm.com

[A08] 取整与四舍五入
来源：http://psm.zhaomingkeji.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pfc.yuanzhike.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fqb.shangyingyoupin.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://twu.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://brm.ydjk.org.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qdg.epnwcf.com


<!-- 参考信息 -->