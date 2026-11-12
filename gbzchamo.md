代发 wailian999

[U49] PHP：只读属性
来源：http://gjd.ywan-chungtsiang.top

public readonly string $name
来源：http://qza.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://jmp.zdqjudy.top

public function __construct(private int $id) {}
来源：http://uwn.hcnkem.com

[U51] PHP：数组解构
来源：http://lly.smart0.xyz

[$a, $b] = $arr;
来源：http://fzc.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://pdx.zdqjudy.top

$double = fn($x) => $x * 2;
来源：http://rhn.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://pbp.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://ubc.smart0.xyz

[U54] PHP：空安全调用
来源：http://spx.andypj.xyz

$obj?->method()
来源：http://wzr.zdbjq.cn

[U55] PHP：match 表达式
来源：http://srv.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jxe.smart0.xyz

[U56] PHP：命名参数
来源：http://tzw.9152youxi.cn

f(a: 1, b: 2)
来源：http://eab.yongpay.top

[U57] PHP：字符串插值
来源：http://lwz.nwbrower.top

"值: {$a}"
来源：http://hag.daria6918.cn

[U58] PHP：数组三件套
来源：http://arv.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xjx.tianlin.xyz

[U59] PHP：自定义排序
来源：http://mgz.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ncz.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://mle.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mtj.yuxming.cn

[U61] PHP：正则
来源：http://ypd.dashuyun.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ijx.sweek.top

[U62] PHP：日期对象
来源：http://inf.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xve.aibaodan.cn

[U63] PHP：文件读写
来源：http://lwv.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fot.zhixingplan.top

[U64] PHP：目录遍历
来源：http://mqr.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://thz.havefunace.top

[U65] PHP：会话
来源：http://kqf.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gth.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://jcl.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dcm.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://pif.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jbx.yj20258.top

[U68] PHP：PDO 连接
来源：http://xhp.iojbl.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bah.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://vdr.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yho.zycfv.cn

[U70] PHP：PDO 事务
来源：http://bbj.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mfi.iojbl.cn

[U71] PHP：抛出异常
来源：http://eha.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://xtd.ivvv.top

[U72] PHP：写错误日志
来源：http://yrh.yj202588.top

error_log("失败: " . $e->getMessage());
来源：http://yhn.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://zlz.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://pmt.cucudq.cn

[U74] PHP：读取环境变量
来源：http://lyn.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://ply.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://zop.zhoulong.xyz

composer require psr/container
来源：http://wbw.yfazqb.com

[U76] PHP：简单路由
来源：http://vqc.sysykeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wwj.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://wkl.gogol.net.cn

composer require twig/twig
来源：http://uvy.guannengcc.top

[U78] PHP：单元测试
来源：http://dwm.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://ptv.birdmap.top

[U79] PHP：静态分析
来源：http://cwk.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://hfi.zdqjudy.top

[U80] PHP：代码规范修复
来源：http://nss.nanxinkj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zce.shzxlz.cn

[U81] JS：初始化项目
来源：http://wpi.jqgufenzy.top

npm init -y;  npm i express
来源：http://xsx.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://eyw.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ina.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://sku.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dzo.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://pzp.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wbe.ivvv.top

[U85] JS：可选链
来源：http://cuu.gotoacloud.top

a?.b?.c
来源：http://pac.0kj1m.cn

[U86] JS：空值合并
来源：http://tka.sysykeji.top

a ?? b
来源：http://jxu.hammf.cn

[U87] JS：解构默认值
来源：http://pxb.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://lol.zdqjudy.top

[U88] JS：对象展开合并
来源：http://hqu.cqqwz.cn

{ ...a, ...b }
来源：http://yly.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://utw.xylfe.cn

[...new Set(arr)]
来源：http://fsk.meibo888.top

[U90] JS：数字数组排序
来源：http://frl.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://fvy.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://sst.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fke.yfazqb.com

[U92] JS：深拷贝
来源：http://xhm.kuanghao11.cn

structuredClone(obj)
来源：http://rsn.xuetiantiany.cn

[U93] JS：模板字符串
来源：http://wxs.sjlbkw.cn

`共 ${n} 条`
来源：http://seb.nwbrower.top

[U94] JS：箭头函数
来源：http://gdx.yfazqb.com

const double = x => x * 2;
来源：http://gkj.epnwcf.com

[U95] JS：Promise 包装
来源：http://fpd.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://ood.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://aji.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ixx.0kj1m.cn

[U97] JS：并发请求
来源：http://nji.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fig.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://mnb.yvedp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pke.meibo888.top

[U99] JS：事件监听
来源：http://ero.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://sge.bjfxy.top

[U100] JS：DOM 查询
来源：http://qqv.0kj1m.cn

document.querySelector(".item")
来源：http://yvh.zdqjudy.top

[U101] JS：classList 操作
来源：http://pco.hysaishi.cn

el.classList.toggle("active")
来源：http://veu.cdnleiting.top

[U102] JS：本地存储
来源：http://ije.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ajn.gotoacloud.top

[U103] JS：定时器
来源：http://odi.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://phd.yonumen.top

[U104] JS：防抖
来源：http://kyr.sweek.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mzv.uphjek.com

[U105] JS：节流
来源：http://qin.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yhb.wangdashe.top

[U106] JS：日期格式化
来源：http://zqe.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ayo.316326.xyz

[U107] JS：数字千分位
来源：http://ayr.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ukc.yuanzhike.top

[U108] JS：随机整数
来源：http://hjn.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zyq.yanxiufei.cn

[U109] JS：数组分组
来源：http://mru.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://hhv.ctjpmb.com

[U110] JS：数组分块
来源：http://jad.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oup.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://ccp.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://pyb.cqqwz.cn

[U112] JS：字符串补位
来源：http://wpr.smart0.xyz

"7".padStart(3, "0")
来源：http://dgd.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://sbi.tarul.cn

s.replaceAll("a", "b")
来源：http://tsm.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://vru.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://hxm.nwbrower.top

[U115] JS：生成 UUID
来源：http://sut.cheryme.top

crypto.randomUUID()
来源：http://qyx.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://txn.iojbl.cn

/** @param {string} name */ function f(name) {}
来源：http://hek.xuanzx.com

[U117] JS：单元测试
来源：http://ryq.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://hhs.yfazqb.com

[U118] JS：开发服务器
来源：http://gqe.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://kle.sysykeji.top

[U119] JS：生产构建
来源：http://ovz.jinyuanbaomall.cn

npx vite build
来源：http://ssl.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://cuj.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://xzw.hongshengwenyu.top

================================================================================
来源：http://xaf.jyoumei.cn

统计汇总
来源：http://zjc.xuetiantiany.cn

================================================================================
来源：http://gwe.yangfankeji.com

按语言统计（条）：
来源：http://wuq.gogol.net.cn

Python ......... 252
来源：http://dch.yj202588.top

PHP ............ 252
来源：http://bkx.guowangkeji.top

JavaScript ..... 252
来源：http://dnl.cashguo.top

TypeScript ..... 212
来源：http://yir.yj20258888.top

Java ........... 212
来源：http://myv.sufxvd.cn

Go ............. 212
来源：http://jrq.jqgfzy.top

Ruby ........... 212
来源：http://jsx.chenjidiqi.icu

C# ............. 212
来源：http://buf.xuetiantiany.cn

C .............. 30
来源：http://bja.fengsongda.top

C++ ............ 30
来源：http://dxu.fengsongda.top

SQL ............ 90
来源：http://ezr.jiagoushi.top

Bash ........... 80
来源：http://kjp.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://qxu.yj20258.top

Swift .......... 15
来源：http://erd.meibo888.top

Lua ............ 10
来源：http://cbp.zhiwuduotai.top

Perl ........... 10
来源：http://pks.fktsv.cn

Scala .......... 10
来源：http://jrv.zhongyouzk.top

------------------------------------
来源：http://ivr.zycfv.cn

合计 ........... 2106 条
来源：http://dso.zhijiandao.cn

按章节统计：
来源：http://lxr.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gah.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fhd.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://abr.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xrt.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wdm.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ewm.jiagoushi.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pmd.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cgg.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ixt.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tvz.bbcook.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tsv.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://era.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://woe.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vwq.sjlbkw.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gyf.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://skr.hnqzz.top

Q SQL 专题                              90
来源：http://avn.aibaodan.cn

R Bash 专题                             80
来源：http://dkt.nwbrower.top

S C / C++ 专题                          60
来源：http://gjf.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://den.yanxiufei.cn

U 高频实用片段                         120
来源：http://slb.vqdsnc.cn

------------------------------------
来源：http://dte.ivvv.top

合计                                  2106 条
来源：http://vsu.hesvh.cn

--------------------------------------------------------------------------------
来源：http://hmd.chenlongwang.top

使用提醒
来源：http://zcv.yueranfly.top

--------------------------------------------------------------------------------
来源：http://kxq.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://izr.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://spz.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://byw.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ubt.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cwt.shuidangran.top

—— 文件结束 ——
来源：http://iur.yongpay.top

================================================================================
来源：http://pbf.svipenyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://lbq.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://ria.dianchejie.cn

================================================================================
来源：http://wgw.quarkkingdee.top

【收录内容】
来源：http://zdl.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iwc.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://apf.yfazqb.com

SQL · Bash · C · C++
来源：http://azr.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jld.xuanzx.com

【使用说明】
来源：http://svd.nanxuanxn.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://etd.gzhubu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dux.ctjpmb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uav.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cxr.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://jug.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://stb.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cco.vehdjk.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://amy.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hii.cucudq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ruf.sjlbkw.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://avl.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tvn.9152youxi.cn

【文件统计】
来源：http://jop.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ggm.52xcode.cn

--------------------------------------------------------------------------------
来源：http://jvy.snrcjt.cn

目  录
来源：http://zyo.ydzc1.top

--------------------------------------------------------------------------------
来源：http://rsr.yangfankeji.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bqq.shuidangran.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zjr.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vfc.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lyb.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pkm.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xlv.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://way.jinqigufen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ave.zhijiandao.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qeg.sweek.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fyg.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eug.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wcw.fktsv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dlf.ppjwa.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://afs.52xcode.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dbh.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yra.52xcode.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kqo.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rnm.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tkb.chenlongwang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uri.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fgz.hammf.cn

================================================================================
来源：http://aez.ctjpmb.com

A. 基础语法与类型
来源：http://dgo.zdbjq.cn

================================================================================
来源：http://ytf.yonumen.top

[A01] Hello World
来源：http://vrb.0kj1m.cn

Py:   print("Hello, World!")
来源：http://wut.sxryk.cn

PHP:  echo "Hello, World!";
来源：http://swx.hammf.cn

JS:   console.log("Hello, World!");
来源：http://qkw.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://itw.cqqwz.cn

Java: System.out.println("Hello, World!");
来源：http://xcj.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://clj.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://njc.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hfl.uphjek.com

[A02] 变量声明与赋值
来源：http://vus.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lca.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ziq.svipenyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jli.yongpay.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xbb.feifeiyinyue.top

Java: String name = "Alex"; int age = 20;
来源：http://lgt.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://gzm.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://utd.ydzc1.top

C#:   string name = "Alex"; int age = 20;
来源：http://ebe.yuxming.cn

[A03] 常量定义
来源：http://qvs.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://epl.ywan-chungtsiang.top

PHP:  const PI = 3.14159;
来源：http://wbv.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://xqe.vqdsnc.cn

TS:   const PI: number = 3.14159;
来源：http://gem.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://nrn.ydjk.org.cn

Go:   const PI = 3.14159
来源：http://nrh.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://kqs.52xcode.cn

C#:   const double PI = 3.14159;
来源：http://tav.xylfe.cn

[A04] 判断变量类型
来源：http://tux.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jgw.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jck.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vbi.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://thd.sysykeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gom.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://vbv.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tjw.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://grm.gzhubu.top

[A05] 整数除法与取模
来源：http://ghu.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jex.ywan-chungtsiang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hrh.yueranfly.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ihx.sxryk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vlt.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://zhe.daxiang520.top

Go:   7 / 2; 7 % 2
来源：http://aha.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://nyu.zhixingplan.top

C#:   7 / 2; 7 % 2
来源：http://etq.hywenlv.cn

[A06] 字符串转数字
来源：http://pgx.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://lfu.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zsk.jinqigfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://prv.fktsv.cn


<!-- 参考信息 -->