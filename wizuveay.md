代发 wailian999

[U55] PHP：match 表达式
来源：http://rzf.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://daq.aibaodan.cn

[U56] PHP：命名参数
来源：http://wcz.cqqwz.cn

f(a: 1, b: 2)
来源：http://lzj.gzhubu.top

[U57] PHP：字符串插值
来源：http://ubd.hysaishi.cn

"值: {$a}"
来源：http://qzw.xziqi.cn

[U58] PHP：数组三件套
来源：http://sgz.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mrh.52xcode.cn

[U59] PHP：自定义排序
来源：http://ucp.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://efc.uphjek.com

[U60] PHP：JSON 编解码
来源：http://ezs.shanyushiyangtech.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://suv.cqqwz.cn

[U61] PHP：正则
来源：http://eqj.hfpthk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lkd.yuxming.cn

[U62] PHP：日期对象
来源：http://fkv.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://otf.zhengqikj.top

[U63] PHP：文件读写
来源：http://dgl.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rhx.shuidangran.top

[U64] PHP：目录遍历
来源：http://rvq.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://xds.hywenlv.cn

[U65] PHP：会话
来源：http://loz.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kns.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://uvl.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ebx.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://tvi.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pga.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://ygv.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pvj.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://stn.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cwv.hnqzz.top

[U70] PHP：PDO 事务
来源：http://sfx.yfazqb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://esa.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://hdl.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://daf.zhixingplan.top

[U72] PHP：写错误日志
来源：http://faa.hfpthk.cn

error_log("失败: " . $e->getMessage());
来源：http://ebf.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://ddv.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://vld.xziqi.cn

[U74] PHP：读取环境变量
来源：http://qzv.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://lyi.havefunace.top

[U75] PHP：依赖注入
来源：http://qxu.xuetiantiany.cn

composer require psr/container
来源：http://swv.c1oappe.top

[U76] PHP：简单路由
来源：http://tni.epnwcf.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iko.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://xoy.yueranfly.top

composer require twig/twig
来源：http://dng.uphjek.com

[U78] PHP：单元测试
来源：http://qqq.nanxuanxn.top

composer require --dev phpunit/phpunit
来源：http://wjm.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://kjj.havefunace.top

composer require --dev phpstan/phpstan
来源：http://xgn.bbcook.cn

[U80] PHP：代码规范修复
来源：http://uve.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qub.hcnkem.com

[U81] JS：初始化项目
来源：http://lrc.zhiwuduotai.top

npm init -y;  npm i express
来源：http://foj.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://xyj.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wlp.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://jri.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://dxo.havefunace.top

[U84] JS：CommonJS 写法
来源：http://sqw.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://kzf.havefunace.top

[U85] JS：可选链
来源：http://ufw.zdbjq.cn

a?.b?.c
来源：http://geg.bjfxy.top

[U86] JS：空值合并
来源：http://qvm.chenlongwang.top

a ?? b
来源：http://lzh.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://rub.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://bjd.9152youxi.cn

[U88] JS：对象展开合并
来源：http://ufn.yuanzhike.top

{ ...a, ...b }
来源：http://qzp.vehdjk.com

[U89] JS：数组去重
来源：http://jwy.chenjidiqi.icu

[...new Set(arr)]
来源：http://pxl.xuanzx.com

[U90] JS：数字数组排序
来源：http://amc.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://jsc.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://tiq.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jyt.nwbrower.top

[U92] JS：深拷贝
来源：http://yfh.fzhhl.top

structuredClone(obj)
来源：http://trx.sjlbkw.cn

[U93] JS：模板字符串
来源：http://ruz.hysaishi.cn

`共 ${n} 条`
来源：http://qsf.svipenyu.cn

[U94] JS：箭头函数
来源：http://kjl.cdnleiting.top

const double = x => x * 2;
来源：http://sns.daxiang520.top

[U95] JS：Promise 包装
来源：http://sic.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://jfu.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://poi.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ree.jinyuanbaomall.cn

[U97] JS：并发请求
来源：http://uns.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qju.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://iqt.yonumen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wjd.yj20258888.top

[U99] JS：事件监听
来源：http://anv.sweek.top

el.addEventListener("click", e => {})
来源：http://ylg.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://dsw.andypj.xyz

document.querySelector(".item")
来源：http://gtx.guowangkeji.top

[U101] JS：classList 操作
来源：http://vkj.yj202588.top

el.classList.toggle("active")
来源：http://cbb.hcnkem.com

[U102] JS：本地存储
来源：http://obh.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gis.wangshuangyany.cn

[U103] JS：定时器
来源：http://tzq.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://riq.316326.xyz

[U104] JS：防抖
来源：http://grm.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qrm.yfazqb.com

[U105] JS：节流
来源：http://hub.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gwm.xuanzx.com

[U106] JS：日期格式化
来源：http://fbj.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hxb.guannengcc.top

[U107] JS：数字千分位
来源：http://aaz.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wth.cheryme.top

[U108] JS：随机整数
来源：http://hmh.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xdt.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://ybr.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://cgo.dianchejie.cn

[U110] JS：数组分块
来源：http://xee.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://okp.dianchejie.cn

[U111] JS：对象转 Map
来源：http://qtc.tanke756.top

new Map(Object.entries(obj))
来源：http://fut.sufxvd.cn

[U112] JS：字符串补位
来源：http://rsa.tanke756.top

"7".padStart(3, "0")
来源：http://wrx.mhx1999.top

[U113] JS：正则替换全部
来源：http://auz.chenzaomai.com

s.replaceAll("a", "b")
来源：http://xib.jqgfzy.top

[U114] JS：JSON 深比较
来源：http://moj.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gng.xylfe.cn

[U115] JS：生成 UUID
来源：http://dev.9152youxi.cn

crypto.randomUUID()
来源：http://ehr.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://ppu.zycfv.cn

/** @param {string} name */ function f(name) {}
来源：http://qho.xuetiantiany.cn

[U117] JS：单元测试
来源：http://luf.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://yxb.ivvv.top

[U118] JS：开发服务器
来源：http://jmp.jyoumei.cn

npm i -D vite;  npx vite
来源：http://azp.ivvv.top

[U119] JS：生产构建
来源：http://kcn.0kj1m.cn

npx vite build
来源：http://pnd.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://ndz.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://txu.52xcode.cn

================================================================================
来源：http://ixn.hywenlv.cn

统计汇总
来源：http://egq.yj20258888.top

================================================================================
来源：http://vnm.hysaishi.cn

按语言统计（条）：
来源：http://ull.ivvv.top

Python ......... 252
来源：http://gyk.yongpay.top

PHP ............ 252
来源：http://yep.fanxiaobao.xyz

JavaScript ..... 252
来源：http://oil.cdnleiting.top

TypeScript ..... 212
来源：http://xnh.yfazqb.com

Java ........... 212
来源：http://fgy.nanxinkj.top

Go ............. 212
来源：http://unu.jlsjyb.cn

Ruby ........... 212
来源：http://ezl.jinyuanbaomall.cn

C# ............. 212
来源：http://kmv.redwolf501.top

C .............. 30
来源：http://ers.zycfv.cn

C++ ............ 30
来源：http://hsk.hysaishi.cn

SQL ............ 90
来源：http://brr.aibaodan.cn

Bash ........... 80
来源：http://rex.fengsongda.top

Kotlin ......... 15
来源：http://kwi.ppjwa.cn

Swift .......... 15
来源：http://lob.zhongyouzk.top

Lua ............ 10
来源：http://ctk.hnqzz.top

Perl ........... 10
来源：http://uai.shzxlz.cn

Scala .......... 10
来源：http://ovg.c1oappe.top

------------------------------------
来源：http://uqb.yonumen.top

合计 ........... 2106 条
来源：http://xjy.redwolf501.top

按章节统计：
来源：http://ycs.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tjo.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://czd.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qgv.zhengqikj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vyq.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zkl.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ubf.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qqn.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ffq.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://spt.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wab.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jto.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://raj.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jjw.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vum.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jym.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rvy.vqdsnc.cn

Q SQL 专题                              90
来源：http://pjq.hysaishi.cn

R Bash 专题                             80
来源：http://rsa.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://lms.haohaochexian.top

T 其他语言补充                          60
来源：http://uwt.hnxiangtu.top

U 高频实用片段                         120
来源：http://dlg.gotoacloud.top

------------------------------------
来源：http://nvu.ctjpmb.com

合计                                  2106 条
来源：http://lma.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://gka.jinqigfzy.top

使用提醒
来源：http://mnf.uphjek.com

--------------------------------------------------------------------------------
来源：http://nrk.c1oappe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cin.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rjs.gotoacloud.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vgh.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://djm.yj20258.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vjn.aizwys.cn

—— 文件结束 ——
来源：http://dha.xuanzx.com

================================================================================
来源：http://gyv.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://gww.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://iyr.meibo888.top

================================================================================
来源：http://tax.jqgfzy.top

【收录内容】
来源：http://yhg.haohaochexian.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uqv.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sxx.dashuyun.cn

SQL · Bash · C · C++
来源：http://uzq.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ygk.yj20258888.top

【使用说明】
来源：http://mnp.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xuw.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eee.ydzc1.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qch.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yad.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kur.hongshengwenyu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://axf.tian-w.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iqb.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ihr.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nny.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://evi.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qos.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qcx.bjfxy.top

【文件统计】
来源：http://pah.ppjwa.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jxf.zycfv.cn

--------------------------------------------------------------------------------
来源：http://dbh.jianghu66.top

目  录
来源：http://tdg.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://wlq.guowangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rza.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eaw.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cuh.0kj1m.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uic.epnwcf.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vrk.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sdf.hammf.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ijr.sxryk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mej.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://awv.52xcode.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pxg.cqqwz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kgx.yonumen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ors.yuanzhike.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://neo.iojbl.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wrn.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://soa.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pib.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mjg.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bma.uphjek.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://icb.cheryme.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqr.hesvh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yjz.yj20258.top

================================================================================
来源：http://nyi.havefunace.top

A. 基础语法与类型
来源：http://ldm.hesvh.cn

================================================================================
来源：http://pio.dashuyun.cn

[A01] Hello World
来源：http://pdn.uphjek.com

Py:   print("Hello, World!")
来源：http://myq.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://rdk.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://sms.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://amr.aizwys.cn

Java: System.out.println("Hello, World!");
来源：http://rjq.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://cvh.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://mqp.chenlongwang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rmi.fzhhl.top

[A02] 变量声明与赋值
来源：http://vvq.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ztr.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://syr.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://omo.jqgfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rda.zhixingplan.top

Java: String name = "Alex"; int age = 20;
来源：http://rxa.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://wsl.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://exc.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://kfv.snrcjt.cn

[A03] 常量定义
来源：http://tds.bbcook.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hov.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://svu.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://klo.hammf.cn

TS:   const PI: number = 3.14159;
来源：http://ely.nwbrower.top

Java: static final double PI = 3.14159;
来源：http://kes.cqqwz.cn

Go:   const PI = 3.14159
来源：http://nbh.tanke756.top

Ruby: PI = 3.14159
来源：http://pzf.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://apz.daria6918.cn

[A04] 判断变量类型
来源：http://oos.redwolf501.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://toz.fanxiaobao.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jla.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jks.jianghu66.top

TS:   typeof x; x instanceof Date
来源：http://krl.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ahb.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://rws.ctjpmb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://bef.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://qqc.ivvv.top

[A05] 整数除法与取模
来源：http://ght.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fzj.redwolf501.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kih.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cet.ybcxt.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ncd.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://xrx.vehdjk.com

Go:   7 / 2; 7 % 2
来源：http://yqd.fzhhl.top

Ruby: 7 / 2; 7 % 2
来源：http://dij.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://avo.yj20258888.top

[A06] 字符串转数字
来源：http://tlw.yongpay.top

Py:   int("42"); float("3.14")
来源：http://ebl.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fxu.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dok.hcnkem.com

TS:   parseInt("42", 10); Number("42")
来源：http://tux.sysykeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://boh.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://loo.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ysi.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pjx.ppjwa.cn

[A07] 数字转字符串
来源：http://mkj.52xcode.cn

Py:   str(42)
来源：http://qhm.nanxuanxn.top

PHP:  (string) 42; strval(42)
来源：http://gey.ctjpmb.com

JS:   String(42); (42).toString()
来源：http://xkl.zdqjudy.top

TS:   String(42)
来源：http://psp.haohaochexian.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qfa.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://jxs.guowangkeji.top


<!-- 参考信息 -->