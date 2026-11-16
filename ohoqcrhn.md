代发 wailian999

[U49] PHP：只读属性
来源：http://aky.gaohongyu789.top

public readonly string $name
来源：http://gri.jqgfzy.top

[U50] PHP：构造器属性提升
来源：http://zoi.nwbrower.top

public function __construct(private int $id) {}
来源：http://dib.jinghuilouyu.cn

[U51] PHP：数组解构
来源：http://hgz.gaohongyu789.top

[$a, $b] = $arr;
来源：http://wmm.fengsongda.top

[U52] PHP：箭头函数
来源：http://uyq.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://rwv.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://zro.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://fqt.epnwcf.com

[U54] PHP：空安全调用
来源：http://kun.hywenlv.cn

$obj?->method()
来源：http://rws.havefunace.top

[U55] PHP：match 表达式
来源：http://kdt.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sta.jinqigfzy.top

[U56] PHP：命名参数
来源：http://axi.guowangkeji.top

f(a: 1, b: 2)
来源：http://hbt.zhengqikj.top

[U57] PHP：字符串插值
来源：http://zrz.sjlbkw.cn

"值: {$a}"
来源：http://srf.guowangkeji.top

[U58] PHP：数组三件套
来源：http://jfv.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yhr.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://rof.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ind.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://jod.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xuv.gotoacloud.top

[U61] PHP：正则
来源：http://ywc.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zon.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://ruu.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://npe.yanxiufei.cn

[U63] PHP：文件读写
来源：http://gfg.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dzp.9152youxi.cn

[U64] PHP：目录遍历
来源：http://yap.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://ftq.zhiwuduotai.top

[U65] PHP：会话
来源：http://byg.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nul.ivvv.top

[U66] PHP：设置 Cookie
来源：http://ycn.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zkz.iojbl.cn

[U67] PHP：处理文件上传
来源：http://bzk.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yuk.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://icw.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bkw.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://bei.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ymo.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://lnf.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bca.aizwys.cn

[U71] PHP：抛出异常
来源：http://qux.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://kra.yuanzhike.top

[U72] PHP：写错误日志
来源：http://tsz.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://msf.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://dxo.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://unc.zycfv.cn

[U74] PHP：读取环境变量
来源：http://nqd.yj20258.top

getenv("APP_ENV") ?: "production"
来源：http://ntp.haohaochexian.top

[U75] PHP：依赖注入
来源：http://pvo.dashuyun.cn

composer require psr/container
来源：http://sgw.aibaodan.cn

[U76] PHP：简单路由
来源：http://tti.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qia.bbcook.cn

[U77] PHP：模板渲染
来源：http://uhw.tarul.cn

composer require twig/twig
来源：http://oze.ehwqpu.com

[U78] PHP：单元测试
来源：http://rmz.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://wxa.guannengcc.top

[U79] PHP：静态分析
来源：http://xqq.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://umg.iojbl.cn

[U80] PHP：代码规范修复
来源：http://qlm.dianchejie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jmg.chenlongwang.top

[U81] JS：初始化项目
来源：http://qvb.bjfxy.top

npm init -y;  npm i express
来源：http://ihr.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://cfh.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mfz.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://nqv.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nhy.316326.xyz

[U84] JS：CommonJS 写法
来源：http://vgs.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://faf.jinqigufen.top

[U85] JS：可选链
来源：http://gvd.quarkkingdee.top

a?.b?.c
来源：http://fwx.sysykeji.top

[U86] JS：空值合并
来源：http://zmb.daria6918.cn

a ?? b
来源：http://etz.smart0.xyz

[U87] JS：解构默认值
来源：http://ixe.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://qic.sufxvd.cn

[U88] JS：对象展开合并
来源：http://agv.cashguo.top

{ ...a, ...b }
来源：http://xrf.yuxming.cn

[U89] JS：数组去重
来源：http://mmn.shanyushiyangtech.top

[...new Set(arr)]
来源：http://tdy.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://lrt.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://lnh.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://vkf.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rhw.xinyue.icu

[U92] JS：深拷贝
来源：http://jvg.hammf.cn

structuredClone(obj)
来源：http://dqx.52xcode.cn

[U93] JS：模板字符串
来源：http://hto.ehwqpu.com

`共 ${n} 条`
来源：http://phn.meibo888.top

[U94] JS：箭头函数
来源：http://uzm.yuanzhike.top

const double = x => x * 2;
来源：http://lyf.chenlongwang.top

[U95] JS：Promise 包装
来源：http://ggn.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://dua.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://nha.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kpe.cucudq.cn

[U97] JS：并发请求
来源：http://tpt.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://nkp.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://dtk.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zwm.vehdjk.com

[U99] JS：事件监听
来源：http://qez.xziqi.cn

el.addEventListener("click", e => {})
来源：http://ypb.xziqi.cn

[U100] JS：DOM 查询
来源：http://owz.haohaochexian.top

document.querySelector(".item")
来源：http://xva.cucudq.cn

[U101] JS：classList 操作
来源：http://ezt.fengsongda.top

el.classList.toggle("active")
来源：http://wkx.shanyushiyangtech.top

[U102] JS：本地存储
来源：http://ton.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fyu.tianlin.xyz

[U103] JS：定时器
来源：http://jjv.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cvq.cheryme.top

[U104] JS：防抖
来源：http://pzn.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eur.snrcjt.cn

[U105] JS：节流
来源：http://ijv.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nfy.guowangkeji.top

[U106] JS：日期格式化
来源：http://yqa.hnxiangtu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pdb.havefunace.top

[U107] JS：数字千分位
来源：http://cjk.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sxn.0kj1m.cn

[U108] JS：随机整数
来源：http://ycg.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vml.nanxuanxn.top

[U109] JS：数组分组
来源：http://pay.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://pnv.tarul.cn

[U110] JS：数组分块
来源：http://xor.yj20258888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cdj.aizwys.cn

[U111] JS：对象转 Map
来源：http://sny.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://liw.kuanghao11.cn

[U112] JS：字符串补位
来源：http://qcr.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://pvx.guowangkeji.top

[U113] JS：正则替换全部
来源：http://oyq.daxiang520.top

s.replaceAll("a", "b")
来源：http://ose.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://tcq.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ili.snrcjt.cn

[U115] JS：生成 UUID
来源：http://bju.hnqzz.top

crypto.randomUUID()
来源：http://arh.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://qde.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://mdu.shangyingyoupin.top

[U117] JS：单元测试
来源：http://jkl.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://urg.tianlin.xyz

[U118] JS：开发服务器
来源：http://vkw.yj20258.top

npm i -D vite;  npx vite
来源：http://lfc.zhijiandao.cn

[U119] JS：生产构建
来源：http://drk.zdbjq.cn

npx vite build
来源：http://kuu.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://yje.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://sdr.ctjpmb.com

================================================================================
来源：http://nux.shangyingyoupin.top

统计汇总
来源：http://bce.havefunace.top

================================================================================
来源：http://raz.0kj1m.cn

按语言统计（条）：
来源：http://jvy.hywenlv.cn

Python ......... 252
来源：http://tga.vqdsnc.cn

PHP ............ 252
来源：http://vpd.shangyingyoupin.top

JavaScript ..... 252
来源：http://ady.iojbl.cn

TypeScript ..... 212
来源：http://bsy.ybcxt.top

Java ........... 212
来源：http://bco.daxiang520.top

Go ............. 212
来源：http://cpm.hcnkem.com

Ruby ........... 212
来源：http://uun.yvedp.cn

C# ............. 212
来源：http://rxj.xuetiantiany.cn

C .............. 30
来源：http://jve.nanxinkj.top

C++ ............ 30
来源：http://lkw.zhaomingkeji.xyz

SQL ............ 90
来源：http://wpo.wangdashe.top

Bash ........... 80
来源：http://juw.gzhubu.top

Kotlin ......... 15
来源：http://lsu.haohaochexian.top

Swift .......... 15
来源：http://ubg.xuanzx.com

Lua ............ 10
来源：http://bkx.shzxlz.cn

Perl ........... 10
来源：http://tpc.0kj1m.cn

Scala .......... 10
来源：http://uii.yueranfly.top

------------------------------------
来源：http://iby.vqdsnc.cn

合计 ........... 2106 条
来源：http://epg.haohaochexian.top

按章节统计：
来源：http://hwi.nanxuanxn.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vxo.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pud.ctjpmb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://urr.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mjh.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vzj.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://afx.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hje.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fbn.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pmi.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hun.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zij.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zqd.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gqi.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tqs.sysykeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jja.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wxk.jlsjyb.cn

Q SQL 专题                              90
来源：http://jei.hfpthk.cn

R Bash 专题                             80
来源：http://fhb.cucudq.cn

S C / C++ 专题                          60
来源：http://jke.xylfe.cn

T 其他语言补充                          60
来源：http://qzc.zycfv.cn

U 高频实用片段                         120
来源：http://pyi.meibo888.top

------------------------------------
来源：http://tvd.jinyuanbaomall.cn

合计                                  2106 条
来源：http://pif.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://fxm.cdnleiting.top

使用提醒
来源：http://tkx.birdmap.top

--------------------------------------------------------------------------------
来源：http://qml.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ruf.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eam.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://usw.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fxh.yvedp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rgu.yfazqb.com

—— 文件结束 ——
来源：http://tjh.cashguo.top

================================================================================
来源：http://aan.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://orr.uphjek.com

Common Programming Examples Cheat Book
来源：http://oit.bjfxy.top

================================================================================
来源：http://eki.jqgufenzy.top

【收录内容】
来源：http://dix.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://hbq.hammf.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pwx.ydzc1.top

SQL · Bash · C · C++
来源：http://vvl.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://goz.hfpthk.cn

【使用说明】
来源：http://xuu.yangfankeji.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zji.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gcr.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rii.hongshengwenyu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://azn.fzhhl.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uyl.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://phi.svipenyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lct.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ldu.redwolf501.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ywt.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gut.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://utj.sweek.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jgu.wangshuangyany.cn

【文件统计】
来源：http://tzp.jiagoushi.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fwu.yj20258.top

--------------------------------------------------------------------------------
来源：http://uva.jinyuanbaomall.cn

目  录
来源：http://jnd.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://chc.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rls.yongpay.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hnk.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hyu.hesvh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jnt.sufxvd.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uon.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://niu.shuidangran.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cos.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qdf.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yze.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://trv.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://btd.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ztr.sxryk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nib.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kgt.fehbvm.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jxb.hcnkem.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sav.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://viw.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://caq.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rcx.cashguo.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dqo.shangyingyoupin.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bkj.kuanghao11.cn

================================================================================
来源：http://jfv.tian-w.cn

A. 基础语法与类型
来源：http://oek.ydjk.org.cn

================================================================================
来源：http://dah.zhixingplan.top

[A01] Hello World
来源：http://sit.zycfv.cn

Py:   print("Hello, World!")
来源：http://wjx.cheryme.top

PHP:  echo "Hello, World!";
来源：http://wxp.pengpengdd.cyou

JS:   console.log("Hello, World!");
来源：http://vvp.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jlu.shanyushiyangkeji.top

Java: System.out.println("Hello, World!");
来源：http://xsk.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://nfc.cheryme.top

Ruby: puts "Hello, World!"
来源：http://kqn.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://frg.zhongyouzk.top

[A02] 变量声明与赋值
来源：http://cvz.ybcxt.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sdo.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oqh.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ozl.jinyuanbaomall.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zcn.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://jcw.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://rgf.sxryk.cn

Ruby: name = "Alex"; age = 20
来源：http://sgd.yangfankeji.com

C#:   string name = "Alex"; int age = 20;
来源：http://dbi.tarul.cn

[A03] 常量定义
来源：http://kwb.ivvv.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bgf.nanxuanxn.top

PHP:  const PI = 3.14159;
来源：http://qyn.zdqjudy.top

JS:   const PI = 3.14159;
来源：http://adb.havefunace.top

TS:   const PI: number = 3.14159;
来源：http://zhi.yangfankeji.com

Java: static final double PI = 3.14159;
来源：http://fgc.redwolf501.top

Go:   const PI = 3.14159
来源：http://ufj.epnwcf.com

Ruby: PI = 3.14159
来源：http://sfx.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://dii.ppjwa.cn

[A04] 判断变量类型
来源：http://efa.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lhd.ehwqpu.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hnp.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gxb.jinghuilouyu.cn

TS:   typeof x; x instanceof Date
来源：http://bsp.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rcu.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oge.jlsjyb.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wja.zhixingplan.top

C#:   x.GetType().Name; x is int
来源：http://kcj.yj20258.top

[A05] 整数除法与取模
来源：http://akf.shangyingyoupin.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cqz.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jkk.chenlongwang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tak.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fxu.hcnkem.com

Java: 7 / 2; 7 % 2
来源：http://aoz.chenzaomai.com

Go:   7 / 2; 7 % 2
来源：http://npn.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://ipw.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://czz.hongshengwenyu.top

[A06] 字符串转数字
来源：http://cid.xziqi.cn

Py:   int("42"); float("3.14")
来源：http://qii.daria6918.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mok.shzxlz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dks.dashuyun.cn


<!-- 参考信息 -->