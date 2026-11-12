代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://gvi.0kj1m.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rrh.9152youxi.cn

[U46] PHP：可空类型
来源：http://usl.hesvh.cn

?string $name = null
来源：http://nih.chenzaomai.com

[U47] PHP：联合类型
来源：http://khi.sysykeji.top

int|string $id
来源：http://yjl.bjfxy.top

[U48] PHP：纯枚举
来源：http://jfr.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gwh.jqgufenzy.top

[U49] PHP：只读属性
来源：http://oyy.kuanghao11.cn

public readonly string $name
来源：http://wnd.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://qli.yj20258888.top

public function __construct(private int $id) {}
来源：http://met.yonumen.top

[U51] PHP：数组解构
来源：http://pua.jiagoushi.top

[$a, $b] = $arr;
来源：http://iet.shzxlz.cn

[U52] PHP：箭头函数
来源：http://fwy.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://udl.yj20258888.top

[U53] PHP：空合并运算符
来源：http://ode.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://vsp.tarul.cn

[U54] PHP：空安全调用
来源：http://siv.zycfv.cn

$obj?->method()
来源：http://qno.dashuyun.cn

[U55] PHP：match 表达式
来源：http://fbo.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nsj.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://jzv.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://fmf.mhx1999.top

[U57] PHP：字符串插值
来源：http://utr.sysykeji.top

"值: {$a}"
来源：http://ifx.cucudq.cn

[U58] PHP：数组三件套
来源：http://ktd.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bwi.yonumen.top

[U59] PHP：自定义排序
来源：http://man.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qww.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://ngl.shanyushiyangtech.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oru.meibo888.top

[U61] PHP：正则
来源：http://eck.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ddp.zhixingplan.top

[U62] PHP：日期对象
来源：http://zef.cashguo.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vqr.cashguo.top

[U63] PHP：文件读写
来源：http://idx.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yhh.sxryk.cn

[U64] PHP：目录遍历
来源：http://mnp.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://xiq.chenzaomai.com

[U65] PHP：会话
来源：http://rst.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ira.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://zaz.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yqg.yonumen.top

[U67] PHP：处理文件上传
来源：http://lwz.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oxr.zycfv.cn

[U68] PHP：PDO 连接
来源：http://zvr.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://psa.jinqigfzy.top

[U69] PHP：PDO 预处理
来源：http://ust.shanyushiyangtech.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rji.shuidangran.top

[U70] PHP：PDO 事务
来源：http://zxo.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vbp.yj20258888.top

[U71] PHP：抛出异常
来源：http://xci.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://ury.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://irb.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://edq.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://lia.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://hzw.sweek.top

[U74] PHP：读取环境变量
来源：http://quv.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://bux.fzhhl.top

[U75] PHP：依赖注入
来源：http://dtb.mhx1999.top

composer require psr/container
来源：http://ixc.jqgufenzy.top

[U76] PHP：简单路由
来源：http://qfv.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wzc.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://yyg.meibo888.top

composer require twig/twig
来源：http://aqt.snrcjt.cn

[U78] PHP：单元测试
来源：http://mck.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://koa.chenlongwang.top

[U79] PHP：静态分析
来源：http://ryw.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://vbc.yfazqb.com

[U80] PHP：代码规范修复
来源：http://nee.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://czp.ivvv.top

[U81] JS：初始化项目
来源：http://rhb.guannengcc.top

npm init -y;  npm i express
来源：http://ong.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://nqq.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hdt.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://vzg.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ggg.snrcjt.cn

[U84] JS：CommonJS 写法
来源：http://qgs.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://whe.jiagoushi.top

[U85] JS：可选链
来源：http://akq.gzhubu.top

a?.b?.c
来源：http://yrr.tian-w.cn

[U86] JS：空值合并
来源：http://ams.xziqi.cn

a ?? b
来源：http://lmq.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://tdw.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://erh.ehwqpu.com

[U88] JS：对象展开合并
来源：http://ulp.mhx1999.top

{ ...a, ...b }
来源：http://ucu.fehbvm.com

[U89] JS：数组去重
来源：http://xgy.chenzaomai.com

[...new Set(arr)]
来源：http://yyw.yvedp.cn

[U90] JS：数字数组排序
来源：http://rsp.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://qzw.iojbl.cn

[U91] JS：对象键值遍历
来源：http://xzi.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tgh.cheryme.top

[U92] JS：深拷贝
来源：http://hsi.nanxinkj.top

structuredClone(obj)
来源：http://mex.tianlin.xyz

[U93] JS：模板字符串
来源：http://clc.tianlin.xyz

`共 ${n} 条`
来源：http://vak.jyoumei.cn

[U94] JS：箭头函数
来源：http://yvw.yueranfly.top

const double = x => x * 2;
来源：http://blh.bbcook.cn

[U95] JS：Promise 包装
来源：http://sxi.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://ruo.epnwcf.com

[U96] JS：async/await 与异常
来源：http://lsj.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zhm.sjlbkw.cn

[U97] JS：并发请求
来源：http://fcz.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tvk.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://fdy.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mmn.havefunace.top

[U99] JS：事件监听
来源：http://cyu.vehdjk.com

el.addEventListener("click", e => {})
来源：http://zml.c1oappe.top

[U100] JS：DOM 查询
来源：http://sex.wangshuangyany.cn

document.querySelector(".item")
来源：http://zah.xuanzx.com

[U101] JS：classList 操作
来源：http://uch.chenzaomai.com

el.classList.toggle("active")
来源：http://mkl.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://jte.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wpd.chenzaomai.com

[U103] JS：定时器
来源：http://kvz.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bbg.ehwqpu.com

[U104] JS：防抖
来源：http://cba.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://brz.sufxvd.cn

[U105] JS：节流
来源：http://fmd.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fwd.gzhubu.top

[U106] JS：日期格式化
来源：http://xyj.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bml.yongpay.top

[U107] JS：数字千分位
来源：http://mfm.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lnb.mhx1999.top

[U108] JS：随机整数
来源：http://tpx.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wao.sjlbkw.cn

[U109] JS：数组分组
来源：http://tux.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://uwu.52xcode.cn

[U110] JS：数组分块
来源：http://psx.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bgx.yvedp.cn

[U111] JS：对象转 Map
来源：http://qfa.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://rip.tianlin.xyz

[U112] JS：字符串补位
来源：http://ttj.vqdsnc.cn

"7".padStart(3, "0")
来源：http://kuo.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://gby.fehbvm.com

s.replaceAll("a", "b")
来源：http://jjz.xinyue.icu

[U114] JS：JSON 深比较
来源：http://rxz.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fjo.gogol.net.cn

[U115] JS：生成 UUID
来源：http://fwn.yj202588.top

crypto.randomUUID()
来源：http://gol.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://otz.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://ava.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://gnt.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://lbp.jqgfzy.top

[U118] JS：开发服务器
来源：http://xny.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://mcw.yuanzhike.top

[U119] JS：生产构建
来源：http://imi.haohaochexian.top

npx vite build
来源：http://ogz.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://jza.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://uhc.kuanghao11.cn

================================================================================
来源：http://wra.chenjidiqi.icu

统计汇总
来源：http://qbf.chenjidiqi.icu

================================================================================
来源：http://gwa.vqdsnc.cn

按语言统计（条）：
来源：http://nbe.gogol.net.cn

Python ......... 252
来源：http://toi.fengsongda.top

PHP ............ 252
来源：http://auj.nanxuanxn.top

JavaScript ..... 252
来源：http://hmo.hnqzz.top

TypeScript ..... 212
来源：http://ewe.zdbjq.cn

Java ........... 212
来源：http://olt.ydjk.org.cn

Go ............. 212
来源：http://fpd.zhiwuduotai.top

Ruby ........... 212
来源：http://ccx.gzhubu.top

C# ............. 212
来源：http://tzq.bbcook.cn

C .............. 30
来源：http://ngc.hnqzz.top

C++ ............ 30
来源：http://ghq.jinghuilouyu.cn

SQL ............ 90
来源：http://nkj.xingfuxueyuan.xyz

Bash ........... 80
来源：http://qrl.0kj1m.cn

Kotlin ......... 15
来源：http://zgk.wangdashe.top

Swift .......... 15
来源：http://mlt.shuidangran.top

Lua ............ 10
来源：http://vzk.svipenyu.cn

Perl ........... 10
来源：http://ikh.shzxlz.cn

Scala .......... 10
来源：http://ehq.ehwqpu.com

------------------------------------
来源：http://ezc.hywenlv.cn

合计 ........... 2106 条
来源：http://bty.yongpay.top

按章节统计：
来源：http://mzp.nanxinkj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rtk.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bdb.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ajj.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cth.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://irz.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pvq.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pno.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kdd.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hxt.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://stk.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://njh.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lbn.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hiq.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tmy.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hwx.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://prd.iojbl.cn

Q SQL 专题                              90
来源：http://vde.jqgfzy.top

R Bash 专题                             80
来源：http://ara.jianghu66.top

S C / C++ 专题                          60
来源：http://rce.yangfankeji.com

T 其他语言补充                          60
来源：http://zua.zdbjq.cn

U 高频实用片段                         120
来源：http://jzz.ydzc1.top

------------------------------------
来源：http://wke.epnwcf.com

合计                                  2106 条
来源：http://qqj.cashguo.top

--------------------------------------------------------------------------------
来源：http://ozm.ybcxt.top

使用提醒
来源：http://tyh.tanke756.top

--------------------------------------------------------------------------------
来源：http://jaf.nanxinkj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cqq.hongshengwenyu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://waq.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qli.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ldl.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qto.yangfankeji.com

—— 文件结束 ——
来源：http://zdw.chenlongwang.top

================================================================================
来源：http://thy.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://ywd.jinyuanbaomall.cn

Common Programming Examples Cheat Book
来源：http://cqn.sysykeji.top

================================================================================
来源：http://gur.316326.xyz

【收录内容】
来源：http://kgi.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fir.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hea.jinghuilouyu.cn

SQL · Bash · C · C++
来源：http://olx.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gwi.jqgfzy.top

【使用说明】
来源：http://zxa.chenlongwang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://txx.hnqzz.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://haw.xuanzx.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jyr.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dfp.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://nlb.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dlc.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lwf.hammf.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oqe.xinyue.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uga.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nps.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kox.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sqe.chenlongwang.top

【文件统计】
来源：http://vyz.nanxinkj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vje.fktsv.cn

--------------------------------------------------------------------------------
来源：http://ezw.hesvh.cn

目  录
来源：http://abh.aizwys.cn

--------------------------------------------------------------------------------
来源：http://rdr.sufxvd.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dqx.fengsongda.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uxg.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ucd.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lxi.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uls.hywenlv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mxn.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ntc.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wat.fengsongda.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sue.yangfankeji.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qxj.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rsh.iojbl.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rms.dianchejie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zwa.jianghu66.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cvx.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hvw.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://msv.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wsz.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xcx.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gqx.hammf.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://axa.fehbvm.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hms.shuidangran.top

================================================================================
来源：http://agb.chenzaomai.com

A. 基础语法与类型
来源：http://kxl.dianchejie.cn

================================================================================
来源：http://wop.xingfuxueyuan.xyz

[A01] Hello World
来源：http://qqj.pengpengdd.cyou

Py:   print("Hello, World!")
来源：http://lnk.fehbvm.com

PHP:  echo "Hello, World!";
来源：http://bxc.birdmap.top

JS:   console.log("Hello, World!");
来源：http://zuo.fktsv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qak.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://fgq.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://ioe.tianlin.xyz

Ruby: puts "Hello, World!"
来源：http://ifw.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fpn.jqgfzy.top

[A02] 变量声明与赋值
来源：http://jmh.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rqc.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jno.bjfxy.top

JS:   let name = "Alex"; const age = 20;
来源：http://rkp.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fia.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://upq.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://mbc.jqgufenzy.top

Ruby: name = "Alex"; age = 20
来源：http://inj.jlsjyb.cn

C#:   string name = "Alex"; int age = 20;
来源：http://azf.yonumen.top

[A03] 常量定义
来源：http://ptm.fanxiaobao.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://phl.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://gnk.yj20258.top

JS:   const PI = 3.14159;
来源：http://jme.redwolf501.top

TS:   const PI: number = 3.14159;
来源：http://ply.zycfv.cn

Java: static final double PI = 3.14159;
来源：http://lms.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://cyk.9152youxi.cn

Ruby: PI = 3.14159
来源：http://crh.jinghuilouyu.cn

C#:   const double PI = 3.14159;
来源：http://unr.vehdjk.com

[A04] 判断变量类型
来源：http://jkx.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://bto.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ynv.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jmi.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://fxl.hcnkem.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ihh.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ink.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ukn.jyoumei.cn

C#:   x.GetType().Name; x is int
来源：http://hzu.yongpay.top

[A05] 整数除法与取模
来源：http://hsg.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kai.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://qwr.shuidangran.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ytf.yongpay.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cca.zhaomingkeji.xyz


<!-- 参考信息 -->