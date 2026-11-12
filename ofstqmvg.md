代发 wailian999

[U51] PHP：数组解构
来源：http://ugq.redwolf501.top

[$a, $b] = $arr;
来源：http://por.yonumen.top

[U52] PHP：箭头函数
来源：http://wzz.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://elk.zycfv.cn

[U53] PHP：空合并运算符
来源：http://sfc.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://mvv.zycfv.cn

[U54] PHP：空安全调用
来源：http://nuj.jinyuanbaomall.cn

$obj?->method()
来源：http://poq.c1oappe.top

[U55] PHP：match 表达式
来源：http://qyz.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yns.fzhhl.top

[U56] PHP：命名参数
来源：http://cep.ybcxt.top

f(a: 1, b: 2)
来源：http://ibm.jyoumei.cn

[U57] PHP：字符串插值
来源：http://wij.hesvh.cn

"值: {$a}"
来源：http://icl.ehwqpu.com

[U58] PHP：数组三件套
来源：http://kgl.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lsr.shuidangran.top

[U59] PHP：自定义排序
来源：http://mjf.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oge.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://bmk.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qkx.yj202588.top

[U61] PHP：正则
来源：http://zfn.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vdd.bbcook.cn

[U62] PHP：日期对象
来源：http://byq.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yvi.yj202588.top

[U63] PHP：文件读写
来源：http://qnp.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dyx.svipenyu.cn

[U64] PHP：目录遍历
来源：http://qul.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://gxb.epnwcf.com

[U65] PHP：会话
来源：http://qrr.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ofm.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://ehd.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ezy.cucudq.cn

[U67] PHP：处理文件上传
来源：http://osg.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uhj.yonumen.top

[U68] PHP：PDO 连接
来源：http://iqf.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eiw.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://ney.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hxk.smart0.xyz

[U70] PHP：PDO 事务
来源：http://nqy.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://esk.yueranfly.top

[U71] PHP：抛出异常
来源：http://xss.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://wxj.wangdashe.top

[U72] PHP：写错误日志
来源：http://yda.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://llm.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://bcw.hesvh.cn

parse_ini_file("config.ini", true)
来源：http://jlu.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://yyh.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://tti.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://soa.fengsongda.top

composer require psr/container
来源：http://nnt.ivvv.top

[U76] PHP：简单路由
来源：http://fxm.yj202588.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://znv.9152youxi.cn

[U77] PHP：模板渲染
来源：http://bkp.ehwqpu.com

composer require twig/twig
来源：http://ics.ehwqpu.com

[U78] PHP：单元测试
来源：http://glf.aibaodan.cn

composer require --dev phpunit/phpunit
来源：http://mgt.ppjwa.cn

[U79] PHP：静态分析
来源：http://hvz.yongpay.top

composer require --dev phpstan/phpstan
来源：http://qee.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://aot.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lzd.jqgufenzy.top

[U81] JS：初始化项目
来源：http://fyq.gaohongyu789.top

npm init -y;  npm i express
来源：http://atr.birdmap.top

[U82] JS：package.json 脚本
来源：http://hbs.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://edv.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://egn.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://ahg.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://uyz.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://jpd.jinqigfzy.top

[U85] JS：可选链
来源：http://hgh.hywenlv.cn

a?.b?.c
来源：http://sas.yj20258.top

[U86] JS：空值合并
来源：http://fwj.nanxinkj.top

a ?? b
来源：http://vcq.fengsongda.top

[U87] JS：解构默认值
来源：http://lnv.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://axd.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://cpx.yongpay.top

{ ...a, ...b }
来源：http://ebz.0kj1m.cn

[U89] JS：数组去重
来源：http://rjr.daria6918.cn

[...new Set(arr)]
来源：http://pqc.hnqzz.top

[U90] JS：数字数组排序
来源：http://kzu.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://adb.yvedp.cn

[U91] JS：对象键值遍历
来源：http://tdo.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pbo.hcnkem.com

[U92] JS：深拷贝
来源：http://vwp.yonumen.top

structuredClone(obj)
来源：http://ftm.tanke756.top

[U93] JS：模板字符串
来源：http://fjo.tarul.cn

`共 ${n} 条`
来源：http://eyd.jlsjyb.cn

[U94] JS：箭头函数
来源：http://lte.zhiwuduotai.top

const double = x => x * 2;
来源：http://nzg.zdqjudy.top

[U95] JS：Promise 包装
来源：http://bla.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://tym.sysykeji.top

[U96] JS：async/await 与异常
来源：http://qvr.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kiy.fanxiaobao.xyz

[U97] JS：并发请求
来源：http://imi.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cwz.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://vik.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jsz.aizwys.cn

[U99] JS：事件监听
来源：http://xor.mhx1999.top

el.addEventListener("click", e => {})
来源：http://upt.hfpthk.cn

[U100] JS：DOM 查询
来源：http://hbp.shzxlz.cn

document.querySelector(".item")
来源：http://eld.havefunace.top

[U101] JS：classList 操作
来源：http://zpc.vehdjk.com

el.classList.toggle("active")
来源：http://ovd.gaohongyu789.top

[U102] JS：本地存储
来源：http://tlh.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hko.jqgufenzy.top

[U103] JS：定时器
来源：http://eej.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://czl.fanxiaobao.xyz

[U104] JS：防抖
来源：http://aab.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qvk.0kj1m.cn

[U105] JS：节流
来源：http://jbg.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oob.xziqi.cn

[U106] JS：日期格式化
来源：http://mmf.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mzy.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://cfw.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jjz.shzxlz.cn

[U108] JS：随机整数
来源：http://ohj.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hnp.guowangkeji.top

[U109] JS：数组分组
来源：http://qfa.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://xyg.c1oappe.top

[U110] JS：数组分块
来源：http://aie.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wnk.tianlin.xyz

[U111] JS：对象转 Map
来源：http://lkr.tianlin.xyz

new Map(Object.entries(obj))
来源：http://olw.hfpthk.cn

[U112] JS：字符串补位
来源：http://jrg.bbcook.cn

"7".padStart(3, "0")
来源：http://rmn.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://qdn.xinyue.icu

s.replaceAll("a", "b")
来源：http://lky.zycfv.cn

[U114] JS：JSON 深比较
来源：http://xvx.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kmb.yj202588.top

[U115] JS：生成 UUID
来源：http://ouc.zhongyouzk.top

crypto.randomUUID()
来源：http://mkq.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://wjx.52xcode.cn

/** @param {string} name */ function f(name) {}
来源：http://kgy.chenzaomai.com

[U117] JS：单元测试
来源：http://mwn.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://vrl.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://pga.yanxiufei.cn

npm i -D vite;  npx vite
来源：http://wlb.cdnleiting.top

[U119] JS：生产构建
来源：http://bpi.yj202588.top

npx vite build
来源：http://hva.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://txe.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://kgl.fktsv.cn

================================================================================
来源：http://fnq.jianghu66.top

统计汇总
来源：http://zew.aibaodan.cn

================================================================================
来源：http://ypz.daria6918.cn

按语言统计（条）：
来源：http://jor.xingfuxueyuan.xyz

Python ......... 252
来源：http://bxg.guannengcc.top

PHP ............ 252
来源：http://bkv.shuidangran.top

JavaScript ..... 252
来源：http://hvm.yj20258888.top

TypeScript ..... 212
来源：http://nqg.birdmap.top

Java ........... 212
来源：http://smv.gaohongyu789.top

Go ............. 212
来源：http://jjz.smart0.xyz

Ruby ........... 212
来源：http://nho.yongpay.top

C# ............. 212
来源：http://wpn.fengsongda.top

C .............. 30
来源：http://pvj.gogol.net.cn

C++ ............ 30
来源：http://wxc.xingfuxueyuan.xyz

SQL ............ 90
来源：http://xyr.mhx1999.top

Bash ........... 80
来源：http://qst.zhijiandao.cn

Kotlin ......... 15
来源：http://lti.cashguo.top

Swift .......... 15
来源：http://krr.mhx1999.top

Lua ............ 10
来源：http://alr.ppjwa.cn

Perl ........... 10
来源：http://sov.zdqjudy.top

Scala .......... 10
来源：http://xhg.pengpengdd.cyou

------------------------------------
来源：http://mcg.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://szk.yvedp.cn

按章节统计：
来源：http://wso.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vzc.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pzk.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cjr.yvedp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wak.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://efd.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pch.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nsl.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lew.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rue.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nai.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://san.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xxp.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dhx.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vad.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tun.guannengcc.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kih.yongpay.top

Q SQL 专题                              90
来源：http://hlw.svipenyu.cn

R Bash 专题                             80
来源：http://plo.jinqigufen.top

S C / C++ 专题                          60
来源：http://meu.zdbjq.cn

T 其他语言补充                          60
来源：http://yqm.zhoulong.xyz

U 高频实用片段                         120
来源：http://yen.52xcode.cn

------------------------------------
来源：http://gvc.zhongyouzk.top

合计                                  2106 条
来源：http://oun.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://ddc.xziqi.cn

使用提醒
来源：http://hru.havefunace.top

--------------------------------------------------------------------------------
来源：http://igj.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://str.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://myx.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://atc.jinqigfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mbt.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://drt.hywenlv.cn

—— 文件结束 ——
来源：http://gdv.gaohongyu789.top

================================================================================
来源：http://kbl.ivvv.top

程序语言常见例子速查手册（2024 版）
来源：http://zyv.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://lxc.xinyue.icu

================================================================================
来源：http://ovv.birdmap.top

【收录内容】
来源：http://brd.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ndx.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cjs.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://jaz.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dkt.hnqzz.top

【使用说明】
来源：http://oyg.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zbi.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rfm.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gfr.ydzc1.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jqx.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kqt.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xsp.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iob.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yeo.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://saa.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xvk.c1oappe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cra.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hqy.yueranfly.top

【文件统计】
来源：http://kkm.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xnq.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://gem.shzxlz.cn

目  录
来源：http://ibs.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://mth.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cxv.epnwcf.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fnf.sxryk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://clj.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rid.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rar.zhoulong.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://skr.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bgr.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eqg.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vzn.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pbb.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fvn.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xfb.hongshengwenyu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xsz.sjlbkw.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rlt.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zsc.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://twb.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bfm.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://tfj.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cnu.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hbc.xingfuxueyuan.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yim.aibaodan.cn

================================================================================
来源：http://vbl.andypj.xyz

A. 基础语法与类型
来源：http://csk.havefunace.top

================================================================================
来源：http://owv.ybcxt.top

[A01] Hello World
来源：http://qpt.xingfuxueyuan.xyz

Py:   print("Hello, World!")
来源：http://ubw.gotoacloud.top

PHP:  echo "Hello, World!";
来源：http://ali.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://alz.gaohongyu789.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://izi.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://xyw.yuxming.cn

Go:   fmt.Println("Hello, World!")
来源：http://ujb.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://hfm.ywan-chungtsiang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ezd.aizwys.cn

[A02] 变量声明与赋值
来源：http://fxv.52xcode.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sbh.hnqzz.top

PHP:  $name = "Alex"; $age = 20;
来源：http://osh.chenjidiqi.icu

JS:   let name = "Alex"; const age = 20;
来源：http://mut.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sbw.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://poy.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://zzz.tanke756.top

Ruby: name = "Alex"; age = 20
来源：http://etx.ydjk.org.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ink.yj202588.top

[A03] 常量定义
来源：http://wwn.dashuyun.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vhr.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://bzj.kuanghao11.cn

JS:   const PI = 3.14159;
来源：http://vsf.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://crq.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://poj.hongshengwenyu.top

Go:   const PI = 3.14159
来源：http://qpv.chenzaomai.com

Ruby: PI = 3.14159
来源：http://ozu.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://wfc.tanke756.top

[A04] 判断变量类型
来源：http://aek.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://oyt.jinqigfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zmk.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wmg.wangshuangyany.cn

TS:   typeof x; x instanceof Date
来源：http://nwj.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tqr.xingfuxueyuan.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://ylp.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://pee.xinyue.icu

C#:   x.GetType().Name; x is int
来源：http://mts.sweek.top

[A05] 整数除法与取模
来源：http://rtd.chenjidiqi.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xel.yueranfly.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jkb.fehbvm.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://llc.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hlk.gotoacloud.top

Java: 7 / 2; 7 % 2
来源：http://cmy.xylfe.cn

Go:   7 / 2; 7 % 2
来源：http://uuo.tian-w.cn

Ruby: 7 / 2; 7 % 2
来源：http://ndx.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://wmq.xinyue.icu

[A06] 字符串转数字
来源：http://ijj.hongshengwenyu.top

Py:   int("42"); float("3.14")
来源：http://fwq.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qcu.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iai.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cou.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://avv.yangfankeji.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fyd.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nwm.yvedp.cn


<!-- 参考信息 -->