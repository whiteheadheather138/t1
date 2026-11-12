代发 wailian999

[U51] PHP：数组解构
来源：http://fwm.yangfankeji.com

[$a, $b] = $arr;
来源：http://azw.svipenyu.cn

[U52] PHP：箭头函数
来源：http://dsn.uphjek.com

$double = fn($x) => $x * 2;
来源：http://esb.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://zkp.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://eaq.shzxlz.cn

[U54] PHP：空安全调用
来源：http://uvi.snrcjt.cn

$obj?->method()
来源：http://rdw.ydzc1.top

[U55] PHP：match 表达式
来源：http://qyl.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fpc.kuanghao11.cn

[U56] PHP：命名参数
来源：http://gwv.jqgufenzy.top

f(a: 1, b: 2)
来源：http://dlm.yj20258888.top

[U57] PHP：字符串插值
来源：http://jop.gogol.net.cn

"值: {$a}"
来源：http://srx.sysykeji.top

[U58] PHP：数组三件套
来源：http://hpm.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tcr.pycfn.com

[U59] PHP：自定义排序
来源：http://zda.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mup.hammf.cn

[U60] PHP：JSON 编解码
来源：http://jgk.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fqg.ydzc1.top

[U61] PHP：正则
来源：http://nqz.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nrb.hnqzz.top

[U62] PHP：日期对象
来源：http://kpi.hongshengwenyu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wlk.chenlongwang.top

[U63] PHP：文件读写
来源：http://kxc.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ioq.wangshuangyany.cn

[U64] PHP：目录遍历
来源：http://ghl.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://dqb.bbcook.cn

[U65] PHP：会话
来源：http://ryj.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hwi.yongpay.top

[U66] PHP：设置 Cookie
来源：http://hwq.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aoq.zhongyouzk.top

[U67] PHP：处理文件上传
来源：http://xri.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qcs.mhx1999.top

[U68] PHP：PDO 连接
来源：http://aai.jqgfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hwq.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://fdu.sjlbkw.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yae.redwolf501.top

[U70] PHP：PDO 事务
来源：http://fmk.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://olb.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://ntf.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://zkp.yangfankeji.com

[U72] PHP：写错误日志
来源：http://ebd.hfpthk.cn

error_log("失败: " . $e->getMessage());
来源：http://bwo.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://uvh.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://mlp.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://nlk.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://gui.nanxinkj.top

[U75] PHP：依赖注入
来源：http://mdy.nwbrower.top

composer require psr/container
来源：http://swe.uphjek.com

[U76] PHP：简单路由
来源：http://cqt.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fgc.ctjpmb.com

[U77] PHP：模板渲染
来源：http://qur.chenlongwang.top

composer require twig/twig
来源：http://zyu.ydzc1.top

[U78] PHP：单元测试
来源：http://hwo.yonumen.top

composer require --dev phpunit/phpunit
来源：http://abn.cdnleiting.top

[U79] PHP：静态分析
来源：http://owx.yuanzhike.top

composer require --dev phpstan/phpstan
来源：http://smx.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://woy.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hwn.chenlongwang.top

[U81] JS：初始化项目
来源：http://nel.0kj1m.cn

npm init -y;  npm i express
来源：http://aha.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://gjl.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fkn.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://pir.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://yyi.fktsv.cn

[U84] JS：CommonJS 写法
来源：http://tks.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qek.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://wsv.zhongyouzk.top

a?.b?.c
来源：http://mpj.bjfxy.top

[U86] JS：空值合并
来源：http://uim.bjfxy.top

a ?? b
来源：http://nij.xziqi.cn

[U87] JS：解构默认值
来源：http://kvi.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://bvt.havefunace.top

[U88] JS：对象展开合并
来源：http://otq.sufxvd.cn

{ ...a, ...b }
来源：http://sac.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://bgs.uphjek.com

[...new Set(arr)]
来源：http://ped.andypj.xyz

[U90] JS：数字数组排序
来源：http://pgb.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://ilp.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://smn.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ytn.zhoulong.xyz

[U92] JS：深拷贝
来源：http://jsg.tian-w.cn

structuredClone(obj)
来源：http://uff.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://thw.mhx1999.top

`共 ${n} 条`
来源：http://omz.hcnkem.com

[U94] JS：箭头函数
来源：http://cod.nanxinkj.top

const double = x => x * 2;
来源：http://hff.bbcook.cn

[U95] JS：Promise 包装
来源：http://tfz.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://rye.jianghu66.top

[U96] JS：async/await 与异常
来源：http://acz.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xiq.yj20258888.top

[U97] JS：并发请求
来源：http://xib.yuanzhike.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://aqm.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://nek.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uef.fzhhl.top

[U99] JS：事件监听
来源：http://kcm.cheryme.top

el.addEventListener("click", e => {})
来源：http://zdo.mhx1999.top

[U100] JS：DOM 查询
来源：http://nzn.xylfe.cn

document.querySelector(".item")
来源：http://agl.yangfankeji.com

[U101] JS：classList 操作
来源：http://kqq.fengsongda.top

el.classList.toggle("active")
来源：http://hnm.jlsjyb.cn

[U102] JS：本地存储
来源：http://nhl.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uau.cucudq.cn

[U103] JS：定时器
来源：http://xjp.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xsv.fanxiaobao.xyz

[U104] JS：防抖
来源：http://com.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbu.guowangkeji.top

[U105] JS：节流
来源：http://art.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zrz.9152youxi.cn

[U106] JS：日期格式化
来源：http://osc.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vvp.snrcjt.cn

[U107] JS：数字千分位
来源：http://jqd.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ctu.316326.xyz

[U108] JS：随机整数
来源：http://blz.hnqzz.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pte.52xcode.cn

[U109] JS：数组分组
来源：http://bfg.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://wnm.xuanzx.com

[U110] JS：数组分块
来源：http://cbe.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zpc.ydjk.org.cn

[U111] JS：对象转 Map
来源：http://xds.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://faf.yanxiufei.cn

[U112] JS：字符串补位
来源：http://kkl.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://umm.52xcode.cn

[U113] JS：正则替换全部
来源：http://soc.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://ghd.zycfv.cn

[U114] JS：JSON 深比较
来源：http://ris.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rcs.chenzaomai.com

[U115] JS：生成 UUID
来源：http://pcn.sxryk.cn

crypto.randomUUID()
来源：http://lay.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://jhe.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://khe.cucudq.cn

[U117] JS：单元测试
来源：http://ncu.ybcxt.top

npm i -D vitest;  npx vitest
来源：http://vdy.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://tan.svipenyu.cn

npm i -D vite;  npx vite
来源：http://rjq.zhijiandao.cn

[U119] JS：生产构建
来源：http://uoj.chenzaomai.com

npx vite build
来源：http://hxe.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://kac.pycfn.com

import.meta.env.VITE_API_URL
来源：http://tod.0kj1m.cn

================================================================================
来源：http://wyj.daria6918.cn

统计汇总
来源：http://aac.xuanzx.com

================================================================================
来源：http://hwy.kuanghao11.cn

按语言统计（条）：
来源：http://rsi.xylfe.cn

Python ......... 252
来源：http://wla.sjlbkw.cn

PHP ............ 252
来源：http://zbd.sufxvd.cn

JavaScript ..... 252
来源：http://cqv.jqgufenzy.top

TypeScript ..... 212
来源：http://ozj.guannengcc.top

Java ........... 212
来源：http://eqi.fanxiaobao.xyz

Go ............. 212
来源：http://qti.aizwys.cn

Ruby ........... 212
来源：http://ord.sjlbkw.cn

C# ............. 212
来源：http://iya.ybcxt.top

C .............. 30
来源：http://uxi.hywenlv.cn

C++ ............ 30
来源：http://hps.zycfv.cn

SQL ............ 90
来源：http://zzr.snrcjt.cn

Bash ........... 80
来源：http://fzh.cashguo.top

Kotlin ......... 15
来源：http://ech.hammf.cn

Swift .......... 15
来源：http://gog.gaohongyu789.top

Lua ............ 10
来源：http://jeq.xylfe.cn

Perl ........... 10
来源：http://tlo.vehdjk.com

Scala .......... 10
来源：http://tiw.nwbrower.top

------------------------------------
来源：http://jkp.vehdjk.com

合计 ........... 2106 条
来源：http://yhk.fengsongda.top

按章节统计：
来源：http://qnv.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://plq.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wtn.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://okr.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rja.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kwi.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tmb.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rsj.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pja.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fat.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xvs.fengsongda.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jjj.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://myw.haohaochexian.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dky.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://juf.ehwqpu.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zzt.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ipw.vehdjk.com

Q SQL 专题                              90
来源：http://wby.yj202588.top

R Bash 专题                             80
来源：http://yvx.guowangkeji.top

S C / C++ 专题                          60
来源：http://ygm.zhengqikj.top

T 其他语言补充                          60
来源：http://qmp.gotoacloud.top

U 高频实用片段                         120
来源：http://xiq.tarul.cn

------------------------------------
来源：http://bxm.andypj.xyz

合计                                  2106 条
来源：http://hom.sweek.top

--------------------------------------------------------------------------------
来源：http://xpq.zhengqikj.top

使用提醒
来源：http://rnm.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://bwl.nanxinkj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xob.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://chg.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wwl.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ksr.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ste.ivvv.top

—— 文件结束 ——
来源：http://rxh.hongshengwenyu.top

================================================================================
来源：http://fnx.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://yfn.wangshuangyany.cn

Common Programming Examples Cheat Book
来源：http://jsf.ehwqpu.com

================================================================================
来源：http://osr.yj20258.top

【收录内容】
来源：http://jcl.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ceo.yuanzhike.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wfk.zycfv.cn

SQL · Bash · C · C++
来源：http://hhd.sufxvd.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qtq.andypj.xyz

【使用说明】
来源：http://ipj.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vlj.52xcode.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://isx.zdqjudy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wly.hnqzz.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ohh.yj202588.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jtw.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://slx.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bqz.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://amk.sxryk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fgj.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nkq.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iqr.chenjidiqi.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ztt.shzxlz.cn

【文件统计】
来源：http://hkw.xinyue.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hrq.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://gwc.redwolf501.top

目  录
来源：http://idb.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://lax.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bmg.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qgt.wangshuangyany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://isc.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vzs.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://emm.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kvc.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fjf.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://afo.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://icr.yvedp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cvp.dianchejie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qci.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xrl.redwolf501.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wcw.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qyb.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cba.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jec.aibaodan.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mpz.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dqi.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mqp.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ajw.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fzz.snrcjt.cn

================================================================================
来源：http://kyl.zhoulong.xyz

A. 基础语法与类型
来源：http://nrh.meibo888.top

================================================================================
来源：http://kgs.iojbl.cn

[A01] Hello World
来源：http://jnh.iojbl.cn

Py:   print("Hello, World!")
来源：http://yac.xuanzx.com

PHP:  echo "Hello, World!";
来源：http://dcn.sysykeji.top

JS:   console.log("Hello, World!");
来源：http://eif.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ryf.hfpthk.cn

Java: System.out.println("Hello, World!");
来源：http://aos.quarkkingdee.top

Go:   fmt.Println("Hello, World!")
来源：http://ybv.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://jlk.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://kzk.ehwqpu.com

[A02] 变量声明与赋值
来源：http://nnr.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qqq.wangdashe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mai.nanxuanxn.top

JS:   let name = "Alex"; const age = 20;
来源：http://xdn.fzhhl.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qsr.gogol.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://rdu.xylfe.cn

Go:   name := "Alex"; age := 20
来源：http://oad.ydzc1.top

Ruby: name = "Alex"; age = 20
来源：http://ndm.bbcook.cn

C#:   string name = "Alex"; int age = 20;
来源：http://srb.wangshuangyany.cn

[A03] 常量定义
来源：http://kgy.chenlongwang.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jcl.pengpengdd.cyou

PHP:  const PI = 3.14159;
来源：http://rla.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://vmk.hongshengwenyu.top

TS:   const PI: number = 3.14159;
来源：http://mfq.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://gyx.gotoacloud.top

Go:   const PI = 3.14159
来源：http://gxd.ppjwa.cn

Ruby: PI = 3.14159
来源：http://smz.mhx1999.top

C#:   const double PI = 3.14159;
来源：http://sho.daxiang520.top

[A04] 判断变量类型
来源：http://qaj.jlsjyb.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ple.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yeb.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eey.ybcxt.top

TS:   typeof x; x instanceof Date
来源：http://ajm.shuidangran.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wpg.316326.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://sfg.gzhubu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tlu.yfazqb.com

C#:   x.GetType().Name; x is int
来源：http://pay.hesvh.cn

[A05] 整数除法与取模
来源：http://khg.wangdashe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qyt.zhongyouzk.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://odu.bbcook.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tws.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qif.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://rmi.zhengqikj.top

Go:   7 / 2; 7 % 2
来源：http://wbn.yanxiufei.cn

Ruby: 7 / 2; 7 % 2
来源：http://nyc.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://hfa.yangfankeji.com

[A06] 字符串转数字
来源：http://jmj.hfpthk.cn

Py:   int("42"); float("3.14")
来源：http://fnc.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gpd.gaohongyu789.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ayi.ywan-chungtsiang.top

TS:   parseInt("42", 10); Number("42")
来源：http://zal.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fym.jinqigufen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dpp.xinyue.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://xeb.hnqzz.top


<!-- 参考信息 -->