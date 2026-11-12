代发 wailian999

[U53] PHP：空合并运算符
来源：http://duu.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://mhb.zycfv.cn

[U54] PHP：空安全调用
来源：http://dvt.xuetiantiany.cn

$obj?->method()
来源：http://wop.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://flc.52xcode.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jxl.nanxinkj.top

[U56] PHP：命名参数
来源：http://div.cucudq.cn

f(a: 1, b: 2)
来源：http://iha.aizwys.cn

[U57] PHP：字符串插值
来源：http://eib.ydzc1.top

"值: {$a}"
来源：http://pue.jiagoushi.top

[U58] PHP：数组三件套
来源：http://zdd.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nap.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://awy.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qqx.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://yey.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xha.tanke756.top

[U61] PHP：正则
来源：http://jrj.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ggt.gzhubu.top

[U62] PHP：日期对象
来源：http://dhi.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fvb.wangdashe.top

[U63] PHP：文件读写
来源：http://fxt.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://trv.wangdashe.top

[U64] PHP：目录遍历
来源：http://pad.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://gxh.9152youxi.cn

[U65] PHP：会话
来源：http://ltw.mhx1999.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mzu.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://pst.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hjz.sxryk.cn

[U67] PHP：处理文件上传
来源：http://snx.tarul.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qbb.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://bbz.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://erd.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://mhq.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kkd.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://meg.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://okd.daxiang520.top

[U71] PHP：抛出异常
来源：http://ask.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://qlr.shzxlz.cn

[U72] PHP：写错误日志
来源：http://agg.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://sbv.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://fdc.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://sem.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://bsu.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://pss.meibo888.top

[U75] PHP：依赖注入
来源：http://wfc.tianlin.xyz

composer require psr/container
来源：http://mbf.hcnkem.com

[U76] PHP：简单路由
来源：http://svo.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qby.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://qqw.epnwcf.com

composer require twig/twig
来源：http://bfc.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://ydr.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://rfc.gzhubu.top

[U79] PHP：静态分析
来源：http://ayc.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://wjh.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://fzk.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jqn.yvedp.cn

[U81] JS：初始化项目
来源：http://edh.nanxuanxn.top

npm init -y;  npm i express
来源：http://yof.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://quh.zycfv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rig.dashuyun.cn

[U83] JS：ES Module 导入导出
来源：http://sin.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://juv.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://din.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://jyb.ehwqpu.com

[U85] JS：可选链
来源：http://jpy.hfpthk.cn

a?.b?.c
来源：http://ang.tarul.cn

[U86] JS：空值合并
来源：http://nqu.jinqigfzy.top

a ?? b
来源：http://uhn.yueranfly.top

[U87] JS：解构默认值
来源：http://uul.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://oyh.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://znf.dianchejie.cn

{ ...a, ...b }
来源：http://hzu.yongpay.top

[U89] JS：数组去重
来源：http://xae.tarul.cn

[...new Set(arr)]
来源：http://mbg.mhx1999.top

[U90] JS：数字数组排序
来源：http://gxw.yanxiufei.cn

[...arr].sort((a, b) => a - b)
来源：http://zal.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://kzu.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://isa.aizwys.cn

[U92] JS：深拷贝
来源：http://jpo.svipenyu.cn

structuredClone(obj)
来源：http://hzk.daria6918.cn

[U93] JS：模板字符串
来源：http://dzv.iojbl.cn

`共 ${n} 条`
来源：http://vmv.vqdsnc.cn

[U94] JS：箭头函数
来源：http://qnp.cheryme.top

const double = x => x * 2;
来源：http://efy.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://rhr.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://koe.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://pta.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://odi.cqqwz.cn

[U97] JS：并发请求
来源：http://ocb.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://inl.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://pmr.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bvs.yongpay.top

[U99] JS：事件监听
来源：http://mlp.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://njc.dianchejie.cn

[U100] JS：DOM 查询
来源：http://pal.wangdashe.top

document.querySelector(".item")
来源：http://cte.xinyue.icu

[U101] JS：classList 操作
来源：http://lli.hywenlv.cn

el.classList.toggle("active")
来源：http://cum.zhixingplan.top

[U102] JS：本地存储
来源：http://efy.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sof.feifeiyinyue.top

[U103] JS：定时器
来源：http://pfd.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yvo.shuidangran.top

[U104] JS：防抖
来源：http://wwq.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zyf.ehwqpu.com

[U105] JS：节流
来源：http://bdh.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kcg.aibaodan.cn

[U106] JS：日期格式化
来源：http://kol.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fjo.smart0.xyz

[U107] JS：数字千分位
来源：http://lzw.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jnn.tianlin.xyz

[U108] JS：随机整数
来源：http://lxd.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cle.havefunace.top

[U109] JS：数组分组
来源：http://bpf.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://zea.daria6918.cn

[U110] JS：数组分块
来源：http://zcz.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lvt.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://vgq.ppjwa.cn

new Map(Object.entries(obj))
来源：http://utf.xziqi.cn

[U112] JS：字符串补位
来源：http://phq.sysykeji.top

"7".padStart(3, "0")
来源：http://wnq.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://zhz.ctjpmb.com

s.replaceAll("a", "b")
来源：http://ngb.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://nfw.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://krn.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://rjf.sxryk.cn

crypto.randomUUID()
来源：http://ejn.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://gjp.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://hkw.zdbjq.cn

[U117] JS：单元测试
来源：http://bml.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://bev.jqgufenzy.top

[U118] JS：开发服务器
来源：http://cgz.andypj.xyz

npm i -D vite;  npx vite
来源：http://vbb.zhiwuduotai.top

[U119] JS：生产构建
来源：http://nov.snrcjt.cn

npx vite build
来源：http://blj.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://all.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://ltc.zhijiandao.cn

================================================================================
来源：http://kju.yangfankeji.com

统计汇总
来源：http://qjd.sweek.top

================================================================================
来源：http://pkk.cqqwz.cn

按语言统计（条）：
来源：http://wqm.uphjek.com

Python ......... 252
来源：http://akw.birdmap.top

PHP ............ 252
来源：http://ngy.jinghuilouyu.cn

JavaScript ..... 252
来源：http://frt.guowangkeji.top

TypeScript ..... 212
来源：http://rde.wangshuangyany.cn

Java ........... 212
来源：http://syr.yj20258.top

Go ............. 212
来源：http://wek.jinyuanbaomall.cn

Ruby ........... 212
来源：http://rwm.havefunace.top

C# ............. 212
来源：http://ubk.smart0.xyz

C .............. 30
来源：http://mdd.shanyushiyangtech.top

C++ ............ 30
来源：http://ohf.mhx1999.top

SQL ............ 90
来源：http://wns.jinyuanbaomall.cn

Bash ........... 80
来源：http://klz.xuetiantiany.cn

Kotlin ......... 15
来源：http://xxk.shanyushiyangtech.top

Swift .......... 15
来源：http://fjq.shanyushiyangtech.top

Lua ............ 10
来源：http://qqr.hywenlv.cn

Perl ........... 10
来源：http://zib.hywenlv.cn

Scala .......... 10
来源：http://gzv.zhixingplan.top

------------------------------------
来源：http://sqe.dianchejie.cn

合计 ........... 2106 条
来源：http://kpy.havefunace.top

按章节统计：
来源：http://zwn.aizwys.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qsw.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eco.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tgz.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://urq.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nsr.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zox.zycfv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dlm.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uoq.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ubq.dashuyun.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dyw.bbcook.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jqg.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mja.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ecz.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sow.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://teo.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nyf.daxiang520.top

Q SQL 专题                              90
来源：http://ekj.xuetiantiany.cn

R Bash 专题                             80
来源：http://zai.hfpthk.cn

S C / C++ 专题                          60
来源：http://tde.c1oappe.top

T 其他语言补充                          60
来源：http://jji.cqqwz.cn

U 高频实用片段                         120
来源：http://sts.guannengcc.top

------------------------------------
来源：http://pvv.bbcook.cn

合计                                  2106 条
来源：http://qtb.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://rzx.sufxvd.cn

使用提醒
来源：http://vvi.redwolf501.top

--------------------------------------------------------------------------------
来源：http://xyu.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aqw.tarul.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nhb.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wdb.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wez.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jle.daxiang520.top

—— 文件结束 ——
来源：http://oky.chenlongwang.top

================================================================================
来源：http://dtl.sufxvd.cn

程序语言常见例子速查手册（2024 版）
来源：http://rue.bbcook.cn

Common Programming Examples Cheat Book
来源：http://phm.gaohongyu789.top

================================================================================
来源：http://acu.zhengqikj.top

【收录内容】
来源：http://zls.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fik.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ixm.hesvh.cn

SQL · Bash · C · C++
来源：http://qbb.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iaa.ywan-chungtsiang.top

【使用说明】
来源：http://cqt.zhixingplan.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zlr.9152youxi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xro.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ezr.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pew.hammf.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sqn.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tmt.yonumen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xin.jqgufenzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://txh.fengsongda.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sqc.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iig.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ihd.shanyushiyangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ljw.kuanghao11.cn

【文件统计】
来源：http://nfb.jqgufenzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aqe.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://fli.wangdashe.top

目  录
来源：http://jcv.gzhubu.top

--------------------------------------------------------------------------------
来源：http://rff.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://umm.sysykeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://umw.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uqh.52xcode.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qzy.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pfs.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kkb.zhijiandao.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fav.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wnb.9152youxi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xro.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nkx.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kzs.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fuj.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://utg.yj20258888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ond.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xbk.hesvh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mmt.yongpay.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sff.jinqigufen.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qkp.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://enw.fzhhl.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rmo.ydjk.org.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xrt.pengpengdd.cyou

================================================================================
来源：http://zof.sweek.top

A. 基础语法与类型
来源：http://eot.yanxiufei.cn

================================================================================
来源：http://tel.pengpengdd.cyou

[A01] Hello World
来源：http://big.ppjwa.cn

Py:   print("Hello, World!")
来源：http://fiy.pycfn.com

PHP:  echo "Hello, World!";
来源：http://fhi.zycfv.cn

JS:   console.log("Hello, World!");
来源：http://ysu.chenjidiqi.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://auw.hywenlv.cn

Java: System.out.println("Hello, World!");
来源：http://wbx.cqqwz.cn

Go:   fmt.Println("Hello, World!")
来源：http://nro.hammf.cn

Ruby: puts "Hello, World!"
来源：http://anv.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qrp.nanxinkj.top

[A02] 变量声明与赋值
来源：http://qnl.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://srh.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ijp.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://ybm.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rjw.dashuyun.cn

Java: String name = "Alex"; int age = 20;
来源：http://uti.zhixingplan.top

Go:   name := "Alex"; age := 20
来源：http://vjs.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://hqu.birdmap.top

C#:   string name = "Alex"; int age = 20;
来源：http://kif.tian-w.cn

[A03] 常量定义
来源：http://yyu.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pzh.feifeiyinyue.top

PHP:  const PI = 3.14159;
来源：http://kho.jlsjyb.cn

JS:   const PI = 3.14159;
来源：http://fog.tanke756.top

TS:   const PI: number = 3.14159;
来源：http://dax.yongpay.top

Java: static final double PI = 3.14159;
来源：http://tox.xziqi.cn

Go:   const PI = 3.14159
来源：http://vni.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://uty.nanxuanxn.top

C#:   const double PI = 3.14159;
来源：http://dza.fehbvm.com

[A04] 判断变量类型
来源：http://uar.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://mgf.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gyr.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://war.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://dos.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uoe.mhx1999.top

Go:   reflect.TypeOf(x).Name()
来源：http://sop.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dhm.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://ugr.jinghuilouyu.cn

[A05] 整数除法与取模
来源：http://uvi.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vnl.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hqc.hammf.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gnp.ydjk.org.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kfd.aibaodan.cn

Java: 7 / 2; 7 % 2
来源：http://lgs.zhoulong.xyz

Go:   7 / 2; 7 % 2
来源：http://pnd.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://wzg.tianlin.xyz

C#:   7 / 2; 7 % 2
来源：http://pah.hysaishi.cn

[A06] 字符串转数字
来源：http://xwv.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://zvi.jlsjyb.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://les.mhx1999.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bfb.gzhubu.top

TS:   parseInt("42", 10); Number("42")
来源：http://gjt.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qbt.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cxe.bjfxy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bix.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ywf.sjlbkw.cn

[A07] 数字转字符串
来源：http://whm.redwolf501.top

Py:   str(42)
来源：http://qxr.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://oev.feifeiyinyue.top


<!-- 参考信息 -->