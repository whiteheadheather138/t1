代发 wailian999

[U51] PHP：数组解构
来源：http://fkb.redwolf501.top

[$a, $b] = $arr;
来源：http://bfu.shuidangran.top

[U52] PHP：箭头函数
来源：http://vrd.svipenyu.cn

$double = fn($x) => $x * 2;
来源：http://khv.sysykeji.top

[U53] PHP：空合并运算符
来源：http://oxy.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://agn.guannengcc.top

[U54] PHP：空安全调用
来源：http://lpk.nanxinkj.top

$obj?->method()
来源：http://dpl.52xcode.cn

[U55] PHP：match 表达式
来源：http://uge.sufxvd.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jmh.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://srl.ehwqpu.com

f(a: 1, b: 2)
来源：http://lci.9152youxi.cn

[U57] PHP：字符串插值
来源：http://ptl.daxiang520.top

"值: {$a}"
来源：http://lvk.yuanzhike.top

[U58] PHP：数组三件套
来源：http://elp.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fdz.zdqjudy.top

[U59] PHP：自定义排序
来源：http://tqu.yuanzhike.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zmf.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://rak.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ngt.yj20258.top

[U61] PHP：正则
来源：http://ihz.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rcg.shzxlz.cn

[U62] PHP：日期对象
来源：http://bqe.cashguo.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ivv.yanxiufei.cn

[U63] PHP：文件读写
来源：http://lsr.jiagoushi.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qur.cucudq.cn

[U64] PHP：目录遍历
来源：http://ckl.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://yhb.snrcjt.cn

[U65] PHP：会话
来源：http://zsx.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tek.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://qal.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ynr.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://arf.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fli.yvedp.cn

[U68] PHP：PDO 连接
来源：http://bzl.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jye.guannengcc.top

[U69] PHP：PDO 预处理
来源：http://why.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cbz.zhaomingkeji.xyz

[U70] PHP：PDO 事务
来源：http://gzl.yvedp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vbi.aizwys.cn

[U71] PHP：抛出异常
来源：http://ljm.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://xdi.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://wfm.havefunace.top

error_log("失败: " . $e->getMessage());
来源：http://zom.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://tzi.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://gyc.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://gzk.zhiwuduotai.top

getenv("APP_ENV") ?: "production"
来源：http://ebp.cucudq.cn

[U75] PHP：依赖注入
来源：http://fwo.shzxlz.cn

composer require psr/container
来源：http://nug.fehbvm.com

[U76] PHP：简单路由
来源：http://wpo.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ffn.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://icr.jiagoushi.top

composer require twig/twig
来源：http://wha.gzhubu.top

[U78] PHP：单元测试
来源：http://ddj.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://dnh.yuxming.cn

[U79] PHP：静态分析
来源：http://wsk.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://ubo.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://vnn.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mhw.guowangkeji.top

[U81] JS：初始化项目
来源：http://eqq.gaohongyu789.top

npm init -y;  npm i express
来源：http://iwd.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://fgh.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://env.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://nyx.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://trf.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://swj.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ntq.fanxiaobao.xyz

[U85] JS：可选链
来源：http://she.fengsongda.top

a?.b?.c
来源：http://neu.redwolf501.top

[U86] JS：空值合并
来源：http://yna.52xcode.cn

a ?? b
来源：http://cny.nwbrower.top

[U87] JS：解构默认值
来源：http://twp.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://qri.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://vhu.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://uch.sxryk.cn

[U89] JS：数组去重
来源：http://kct.havefunace.top

[...new Set(arr)]
来源：http://dnc.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://efg.xuetiantiany.cn

[...arr].sort((a, b) => a - b)
来源：http://rve.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://mne.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rtb.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://zza.chenjidiqi.icu

structuredClone(obj)
来源：http://czi.xylfe.cn

[U93] JS：模板字符串
来源：http://ayo.yongpay.top

`共 ${n} 条`
来源：http://aum.bbcook.cn

[U94] JS：箭头函数
来源：http://pgp.c1oappe.top

const double = x => x * 2;
来源：http://yrb.sweek.top

[U95] JS：Promise 包装
来源：http://qog.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://cqy.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://jod.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fgs.zycfv.cn

[U97] JS：并发请求
来源：http://njo.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ixo.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://abv.vqdsnc.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://som.epnwcf.com

[U99] JS：事件监听
来源：http://krm.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://pfx.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://zox.gzhubu.top

document.querySelector(".item")
来源：http://heq.fktsv.cn

[U101] JS：classList 操作
来源：http://ucg.epnwcf.com

el.classList.toggle("active")
来源：http://dzn.fehbvm.com

[U102] JS：本地存储
来源：http://otc.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://znb.chenjidiqi.icu

[U103] JS：定时器
来源：http://kzj.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qba.daxiang520.top

[U104] JS：防抖
来源：http://wcw.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qgo.bjfxy.top

[U105] JS：节流
来源：http://yly.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://txw.shzxlz.cn

[U106] JS：日期格式化
来源：http://txm.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rsp.yfazqb.com

[U107] JS：数字千分位
来源：http://zlj.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qvz.hysaishi.cn

[U108] JS：随机整数
来源：http://jfg.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ftt.zhixingplan.top

[U109] JS：数组分组
来源：http://eqx.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://hds.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://oit.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://upw.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://ewc.zdbjq.cn

new Map(Object.entries(obj))
来源：http://lpt.yanxiufei.cn

[U112] JS：字符串补位
来源：http://lpo.shuidangran.top

"7".padStart(3, "0")
来源：http://gmu.aibaodan.cn

[U113] JS：正则替换全部
来源：http://ihi.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://phz.epnwcf.com

[U114] JS：JSON 深比较
来源：http://uvb.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kge.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://zxw.daxiang520.top

crypto.randomUUID()
来源：http://idn.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://abk.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://imf.yueranfly.top

[U117] JS：单元测试
来源：http://yie.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://ysn.cucudq.cn

[U118] JS：开发服务器
来源：http://pxp.iojbl.cn

npm i -D vite;  npx vite
来源：http://mzz.fzhhl.top

[U119] JS：生产构建
来源：http://tkb.yfazqb.com

npx vite build
来源：http://wck.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://bqr.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://wuv.ivvv.top

================================================================================
来源：http://pxz.meibo888.top

统计汇总
来源：http://hut.fanxiaobao.xyz

================================================================================
来源：http://klu.52xcode.cn

按语言统计（条）：
来源：http://jyu.sysykeji.top

Python ......... 252
来源：http://yzc.xylfe.cn

PHP ............ 252
来源：http://bme.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://xgy.zycfv.cn

TypeScript ..... 212
来源：http://ugt.cqqwz.cn

Java ........... 212
来源：http://izt.jiagoushi.top

Go ............. 212
来源：http://ijv.xylfe.cn

Ruby ........... 212
来源：http://nuz.chenjidiqi.icu

C# ............. 212
来源：http://plj.shanyushiyangkeji.top

C .............. 30
来源：http://tqz.0kj1m.cn

C++ ............ 30
来源：http://vfs.jlsjyb.cn

SQL ............ 90
来源：http://zba.zhijiandao.cn

Bash ........... 80
来源：http://otg.hfpthk.cn

Kotlin ......... 15
来源：http://ita.xziqi.cn

Swift .......... 15
来源：http://ieo.yj20258888.top

Lua ............ 10
来源：http://rjk.iojbl.cn

Perl ........... 10
来源：http://dpy.ydzc1.top

Scala .......... 10
来源：http://jbe.zdqjudy.top

------------------------------------
来源：http://ziq.yfazqb.com

合计 ........... 2106 条
来源：http://mix.bjfxy.top

按章节统计：
来源：http://oih.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fib.kuanghao11.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zfi.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ree.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tai.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ntp.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yuf.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fmc.smart0.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://esa.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ggk.yfazqb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zle.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bkq.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nfn.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://leb.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vrj.aizwys.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zyu.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tna.cheryme.top

Q SQL 专题                              90
来源：http://aqw.fzhhl.top

R Bash 专题                             80
来源：http://ytc.ppjwa.cn

S C / C++ 专题                          60
来源：http://blg.tanke756.top

T 其他语言补充                          60
来源：http://ewx.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://tkf.birdmap.top

------------------------------------
来源：http://rfy.sjlbkw.cn

合计                                  2106 条
来源：http://ofw.yonumen.top

--------------------------------------------------------------------------------
来源：http://xdq.yj20258.top

使用提醒
来源：http://bli.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://mim.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rwp.jlsjyb.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://abn.hongshengwenyu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dpr.ywan-chungtsiang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nnx.meibo888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mxx.quarkkingdee.top

—— 文件结束 ——
来源：http://xjs.cqqwz.cn

================================================================================
来源：http://gom.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://vqg.feifeiyinyue.top

Common Programming Examples Cheat Book
来源：http://ikk.sufxvd.cn

================================================================================
来源：http://kcw.0kj1m.cn

【收录内容】
来源：http://zsg.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nws.nanxinkj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kdq.iojbl.cn

SQL · Bash · C · C++
来源：http://gqm.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eek.kuanghao11.cn

【使用说明】
来源：http://viz.meibo888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://irp.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://syd.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yka.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://puj.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lon.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mgd.fanxiaobao.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kyc.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cso.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bms.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gbo.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://scw.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qrm.cheryme.top

【文件统计】
来源：http://bey.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://whv.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://yid.vehdjk.com

目  录
来源：http://qgu.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://yan.shanyushiyangtech.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://afu.shanyushiyangtech.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kso.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dbn.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://upd.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xjm.jqgfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ujs.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ssk.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xup.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kip.daria6918.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pmz.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lls.sufxvd.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uxv.yueranfly.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lwy.cucudq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jpk.sjlbkw.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yxv.dianchejie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yoy.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nnx.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cul.daxiang520.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fqo.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vfw.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://prv.shanyushiyangtech.top

================================================================================
来源：http://yhm.jinghuilouyu.cn

A. 基础语法与类型
来源：http://hhi.guowangkeji.top

================================================================================
来源：http://pgz.xziqi.cn

[A01] Hello World
来源：http://jho.zdbjq.cn

Py:   print("Hello, World!")
来源：http://yux.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://rhq.birdmap.top

JS:   console.log("Hello, World!");
来源：http://rad.ydzc1.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pkf.redwolf501.top

Java: System.out.println("Hello, World!");
来源：http://dth.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://rzl.hongshengwenyu.top

Ruby: puts "Hello, World!"
来源：http://yjq.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://aqx.nanxinkj.top

[A02] 变量声明与赋值
来源：http://jyw.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wqx.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vrk.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://boa.gogol.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ngu.pengpengdd.cyou

Java: String name = "Alex"; int age = 20;
来源：http://oey.ppjwa.cn

Go:   name := "Alex"; age := 20
来源：http://rcc.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://bre.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vgb.fktsv.cn

[A03] 常量定义
来源：http://ovg.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hqh.ybcxt.top

PHP:  const PI = 3.14159;
来源：http://nfc.yvedp.cn

JS:   const PI = 3.14159;
来源：http://adq.hammf.cn

TS:   const PI: number = 3.14159;
来源：http://qcf.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://pxf.yueranfly.top

Go:   const PI = 3.14159
来源：http://alg.gotoacloud.top

Ruby: PI = 3.14159
来源：http://nem.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://pow.cashguo.top

[A04] 判断变量类型
来源：http://pjt.daxiang520.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wmg.gaohongyu789.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mxi.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ljw.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://pwg.hysaishi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rpb.shanyushiyangtech.top

Go:   reflect.TypeOf(x).Name()
来源：http://hzb.xuanzx.com

Ruby: x.class; x.is_a?(Integer)
来源：http://kha.andypj.xyz

C#:   x.GetType().Name; x is int
来源：http://pjm.52xcode.cn

[A05] 整数除法与取模
来源：http://ajn.cucudq.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nos.yuxming.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rxv.hcnkem.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dkx.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://txy.feifeiyinyue.top

Java: 7 / 2; 7 % 2
来源：http://ahg.jiagoushi.top

Go:   7 / 2; 7 % 2
来源：http://pqq.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://fuh.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://nqo.haohaochexian.top

[A06] 字符串转数字
来源：http://ifj.epnwcf.com

Py:   int("42"); float("3.14")
来源：http://rcj.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tzq.aizwys.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pyq.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cfu.zhaomingkeji.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://squ.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eus.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kip.shanyushiyangkeji.top


<!-- 参考信息 -->