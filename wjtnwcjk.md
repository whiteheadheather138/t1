代发 wailian999

[U57] PHP：字符串插值
来源：http://dda.xingfuxueyuan.xyz

"值: {$a}"
来源：http://wjv.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://aod.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://epe.fengsongda.top

[U59] PHP：自定义排序
来源：http://mtj.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ekn.zhengqikj.top

[U60] PHP：JSON 编解码
来源：http://ewv.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lxt.yj20258.top

[U61] PHP：正则
来源：http://epm.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ehw.hywenlv.cn

[U62] PHP：日期对象
来源：http://jyg.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://efh.snrcjt.cn

[U63] PHP：文件读写
来源：http://lpu.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hri.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://eqv.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://wio.jqgfzy.top

[U65] PHP：会话
来源：http://cru.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jrx.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://dzt.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pfc.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://pyy.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sxp.vehdjk.com

[U68] PHP：PDO 连接
来源：http://fud.wangdashe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hgu.dianchejie.cn

[U69] PHP：PDO 预处理
来源：http://tcs.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kpv.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://gvh.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://syu.cdnleiting.top

[U71] PHP：抛出异常
来源：http://zhq.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://kvy.sweek.top

[U72] PHP：写错误日志
来源：http://vlm.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://yhc.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://lot.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://evf.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://fkz.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://lxy.c1oappe.top

[U75] PHP：依赖注入
来源：http://hwn.xziqi.cn

composer require psr/container
来源：http://lce.zhongyouzk.top

[U76] PHP：简单路由
来源：http://mkl.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kjb.daria6918.cn

[U77] PHP：模板渲染
来源：http://eyg.zhixingplan.top

composer require twig/twig
来源：http://dtv.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://hms.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://dht.tanke756.top

[U79] PHP：静态分析
来源：http://ynv.316326.xyz

composer require --dev phpstan/phpstan
来源：http://brh.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://ski.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ofo.xylfe.cn

[U81] JS：初始化项目
来源：http://vsd.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://del.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://kqt.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uqz.fktsv.cn

[U83] JS：ES Module 导入导出
来源：http://gkc.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fxa.pycfn.com

[U84] JS：CommonJS 写法
来源：http://qpp.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://ipx.sysykeji.top

[U85] JS：可选链
来源：http://ltp.chenlongwang.top

a?.b?.c
来源：http://vtv.zhixingplan.top

[U86] JS：空值合并
来源：http://ubh.zhaomingkeji.xyz

a ?? b
来源：http://ykp.hnxiangtu.top

[U87] JS：解构默认值
来源：http://uyp.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://tfd.yueranfly.top

[U88] JS：对象展开合并
来源：http://qbe.fengsongda.top

{ ...a, ...b }
来源：http://tjh.dianchejie.cn

[U89] JS：数组去重
来源：http://iza.zhengqikj.top

[...new Set(arr)]
来源：http://zza.ybcxt.top

[U90] JS：数字数组排序
来源：http://hqs.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://jzn.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://mui.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bzf.yueranfly.top

[U92] JS：深拷贝
来源：http://duv.ppjwa.cn

structuredClone(obj)
来源：http://sof.xuanzx.com

[U93] JS：模板字符串
来源：http://rdv.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://fqu.pycfn.com

[U94] JS：箭头函数
来源：http://uwd.yuanzhike.top

const double = x => x * 2;
来源：http://stq.9152youxi.cn

[U95] JS：Promise 包装
来源：http://qia.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://imt.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://ocn.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://psa.guannengcc.top

[U97] JS：并发请求
来源：http://lga.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://liq.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://ffw.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zoq.zhiwuduotai.top

[U99] JS：事件监听
来源：http://mxi.yfazqb.com

el.addEventListener("click", e => {})
来源：http://owu.nanxinkj.top

[U100] JS：DOM 查询
来源：http://brk.shangyingyoupin.top

document.querySelector(".item")
来源：http://tfc.cashguo.top

[U101] JS：classList 操作
来源：http://cuv.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://gxi.jiagoushi.top

[U102] JS：本地存储
来源：http://wjd.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jkr.haohaochexian.top

[U103] JS：定时器
来源：http://xug.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ech.zhongyouzk.top

[U104] JS：防抖
来源：http://mew.hysaishi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hld.hysaishi.cn

[U105] JS：节流
来源：http://fyx.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qbr.svipenyu.cn

[U106] JS：日期格式化
来源：http://kfx.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qnx.jqgufenzy.top

[U107] JS：数字千分位
来源：http://zql.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fps.hysaishi.cn

[U108] JS：随机整数
来源：http://uqr.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sso.tian-w.cn

[U109] JS：数组分组
来源：http://xsb.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://ela.gzhubu.top

[U110] JS：数组分块
来源：http://vxh.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://chk.jyoumei.cn

[U111] JS：对象转 Map
来源：http://ugk.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://rjp.pycfn.com

[U112] JS：字符串补位
来源：http://qzf.jinqigufen.top

"7".padStart(3, "0")
来源：http://inx.dianchejie.cn

[U113] JS：正则替换全部
来源：http://zbb.gotoacloud.top

s.replaceAll("a", "b")
来源：http://pod.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://cdw.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ykg.yanxiufei.cn

[U115] JS：生成 UUID
来源：http://ajn.hammf.cn

crypto.randomUUID()
来源：http://mjg.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://uxl.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://avt.shuidangran.top

[U117] JS：单元测试
来源：http://wnx.gotoacloud.top

npm i -D vitest;  npx vitest
来源：http://glu.tanke756.top

[U118] JS：开发服务器
来源：http://xdm.chenzaomai.com

npm i -D vite;  npx vite
来源：http://cmj.pycfn.com

[U119] JS：生产构建
来源：http://hde.fehbvm.com

npx vite build
来源：http://rct.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://zjc.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://cjn.tianlin.xyz

================================================================================
来源：http://wgw.kuanghao11.cn

统计汇总
来源：http://whg.uphjek.com

================================================================================
来源：http://mhj.smart0.xyz

按语言统计（条）：
来源：http://blq.shangyingyoupin.top

Python ......... 252
来源：http://pnr.52xcode.cn

PHP ............ 252
来源：http://pyu.gzhubu.top

JavaScript ..... 252
来源：http://qqp.daxiang520.top

TypeScript ..... 212
来源：http://gnx.guannengcc.top

Java ........... 212
来源：http://gms.uphjek.com

Go ............. 212
来源：http://guw.jqgufenzy.top

Ruby ........... 212
来源：http://isc.wangshuangyany.cn

C# ............. 212
来源：http://ixe.hongshengwenyu.top

C .............. 30
来源：http://mlo.xuetiantiany.cn

C++ ............ 30
来源：http://uoy.jinyuanbaomall.cn

SQL ............ 90
来源：http://ggd.shanyushiyangkeji.top

Bash ........... 80
来源：http://xdl.xinyue.icu

Kotlin ......... 15
来源：http://tmd.bbcook.cn

Swift .......... 15
来源：http://vuy.kuanghao11.cn

Lua ............ 10
来源：http://kmg.chenzaomai.com

Perl ........... 10
来源：http://mpd.gzhubu.top

Scala .......... 10
来源：http://zzp.yangfankeji.com

------------------------------------
来源：http://rhg.yonumen.top

合计 ........... 2106 条
来源：http://exz.vqdsnc.cn

按章节统计：
来源：http://msz.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kru.guannengcc.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dbp.yvedp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gsw.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mpk.ivvv.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qhq.guowangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jwp.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ace.sysykeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kuv.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://adp.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pkv.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xkw.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kcv.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iri.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hck.hnxiangtu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vkv.svipenyu.cn

Q SQL 专题                              90
来源：http://lqq.xylfe.cn

R Bash 专题                             80
来源：http://cza.xuanzx.com

S C / C++ 专题                          60
来源：http://noz.ydjk.org.cn

T 其他语言补充                          60
来源：http://gpu.guannengcc.top

U 高频实用片段                         120
来源：http://unu.yvedp.cn

------------------------------------
来源：http://nzu.hcnkem.com

合计                                  2106 条
来源：http://ehe.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://dvx.cheryme.top

使用提醒
来源：http://dgm.tian-w.cn

--------------------------------------------------------------------------------
来源：http://usg.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qeq.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rip.hywenlv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rsd.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://vdg.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://see.yfazqb.com

—— 文件结束 ——
来源：http://yzz.gotoacloud.top

================================================================================
来源：http://oqx.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://nhy.pycfn.com

Common Programming Examples Cheat Book
来源：http://xqy.cheryme.top

================================================================================
来源：http://udc.hysaishi.cn

【收录内容】
来源：http://oen.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tjj.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wcr.xylfe.cn

SQL · Bash · C · C++
来源：http://pas.shzxlz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lrx.cucudq.cn

【使用说明】
来源：http://tag.sweek.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iki.shanyushiyangtech.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wah.yonumen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://unm.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kwf.zycfv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iwv.sweek.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gir.yvedp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://azv.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ram.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://myn.jinghuilouyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zae.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bzm.zhengqikj.top

【文件统计】
来源：http://xwx.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lud.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ybm.yfazqb.com

目  录
来源：http://twd.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://kye.yanxiufei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ftn.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nyo.jlsjyb.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sbz.bjfxy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kpr.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zmd.uphjek.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rog.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://atk.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xzy.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bep.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fds.xuanzx.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cpe.dianchejie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hwk.aizwys.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eby.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://scx.zhaomingkeji.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vfx.birdmap.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vmp.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hmz.epnwcf.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://rgj.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://noz.hcnkem.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ezr.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eyp.tianlin.xyz

================================================================================
来源：http://fam.pycfn.com

A. 基础语法与类型
来源：http://fmv.jinghuilouyu.cn

================================================================================
来源：http://ayc.ctjpmb.com

[A01] Hello World
来源：http://xlm.nwbrower.top

Py:   print("Hello, World!")
来源：http://qep.tarul.cn

PHP:  echo "Hello, World!";
来源：http://jen.yonumen.top

JS:   console.log("Hello, World!");
来源：http://mmq.jinyuanbaomall.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://efl.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://uyq.cucudq.cn

Go:   fmt.Println("Hello, World!")
来源：http://ifs.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://plr.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hoi.yuanzhike.top

[A02] 变量声明与赋值
来源：http://wwp.hfpthk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sfj.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yqd.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://flq.zhiwuduotai.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kba.ivvv.top

Java: String name = "Alex"; int age = 20;
来源：http://qog.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://cvv.ydjk.org.cn

Ruby: name = "Alex"; age = 20
来源：http://tie.hcnkem.com

C#:   string name = "Alex"; int age = 20;
来源：http://aba.nanxuanxn.top

[A03] 常量定义
来源：http://sym.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://btg.xuetiantiany.cn

PHP:  const PI = 3.14159;
来源：http://ytl.daxiang520.top

JS:   const PI = 3.14159;
来源：http://fhj.gzhubu.top

TS:   const PI: number = 3.14159;
来源：http://xoc.hammf.cn

Java: static final double PI = 3.14159;
来源：http://rjn.iojbl.cn

Go:   const PI = 3.14159
来源：http://bfh.dianchejie.cn

Ruby: PI = 3.14159
来源：http://npt.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://xty.nanxuanxn.top

[A04] 判断变量类型
来源：http://ihx.316326.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://rqt.mhx1999.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zjt.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rfu.ybcxt.top

TS:   typeof x; x instanceof Date
来源：http://gex.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ooh.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://edu.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kvr.zdqjudy.top

C#:   x.GetType().Name; x is int
来源：http://psh.yangfankeji.com

[A05] 整数除法与取模
来源：http://tep.quarkkingdee.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://csw.ivvv.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://loy.dianchejie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://axr.chenzaomai.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wyc.zdqjudy.top

Java: 7 / 2; 7 % 2
来源：http://gyc.hnqzz.top

Go:   7 / 2; 7 % 2
来源：http://qgv.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://obv.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://ije.zhixingplan.top

[A06] 字符串转数字
来源：http://mfc.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://cqp.hongshengwenyu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ftr.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sbi.aibaodan.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jll.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://syg.ywan-chungtsiang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rzt.jyoumei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fld.zhengqikj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xsk.jinyuanbaomall.cn

[A07] 数字转字符串
来源：http://xko.redwolf501.top

Py:   str(42)
来源：http://cui.quarkkingdee.top

PHP:  (string) 42; strval(42)
来源：http://dec.jinqigufen.top

JS:   String(42); (42).toString()
来源：http://kqr.zhongyouzk.top

TS:   String(42)
来源：http://yuu.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ldo.tian-w.cn

Go:   strconv.Itoa(42)
来源：http://nny.havefunace.top

Ruby: 42.to_s
来源：http://jvp.xinyue.icu

C#:   42.ToString()
来源：http://dbe.bbcook.cn

[A08] 取整与四舍五入
来源：http://wue.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ddz.nanxuanxn.top


<!-- 参考信息 -->