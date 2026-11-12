代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://zvr.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ypt.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://bqh.sxryk.cn

?string $name = null
来源：http://jlc.shzxlz.cn

[U47] PHP：联合类型
来源：http://gli.sufxvd.cn

int|string $id
来源：http://jgg.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://bur.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jsv.aibaodan.cn

[U49] PHP：只读属性
来源：http://bsk.ybcxt.top

public readonly string $name
来源：http://xzs.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://ufz.cashguo.top

public function __construct(private int $id) {}
来源：http://wih.yangfankeji.com

[U51] PHP：数组解构
来源：http://emm.aizwys.cn

[$a, $b] = $arr;
来源：http://dsx.0kj1m.cn

[U52] PHP：箭头函数
来源：http://tpy.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://eab.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://bdv.sweek.top

$v = $a ?? $b ?? "default";
来源：http://ebj.hywenlv.cn

[U54] PHP：空安全调用
来源：http://iww.yonumen.top

$obj?->method()
来源：http://fux.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://wsb.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://diu.yj20258.top

[U56] PHP：命名参数
来源：http://auz.316326.xyz

f(a: 1, b: 2)
来源：http://olc.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://eqh.jqgufenzy.top

"值: {$a}"
来源：http://rbu.cdnleiting.top

[U58] PHP：数组三件套
来源：http://gzq.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tvj.vehdjk.com

[U59] PHP：自定义排序
来源：http://kiw.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://faz.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://zxw.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qrw.hysaishi.cn

[U61] PHP：正则
来源：http://rxr.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wvp.sjlbkw.cn

[U62] PHP：日期对象
来源：http://vwo.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nvq.fktsv.cn

[U63] PHP：文件读写
来源：http://jcb.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vml.daxiang520.top

[U64] PHP：目录遍历
来源：http://uvp.andypj.xyz

glob("dir/*.php");  scandir("dir");
来源：http://kxz.ydzc1.top

[U65] PHP：会话
来源：http://lwr.bbcook.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xjr.meibo888.top

[U66] PHP：设置 Cookie
来源：http://qru.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dlu.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://jem.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aac.sufxvd.cn

[U68] PHP：PDO 连接
来源：http://xfv.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kkc.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://blf.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sem.daxiang520.top

[U70] PHP：PDO 事务
来源：http://mqy.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qjn.gotoacloud.top

[U71] PHP：抛出异常
来源：http://ufg.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://apk.jianghu66.top

[U72] PHP：写错误日志
来源：http://zpd.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://xvc.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://bmz.vqdsnc.cn

parse_ini_file("config.ini", true)
来源：http://vuq.jinghuilouyu.cn

[U74] PHP：读取环境变量
来源：http://wou.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://bfy.gogol.net.cn

[U75] PHP：依赖注入
来源：http://poj.yj20258.top

composer require psr/container
来源：http://vlq.zdqjudy.top

[U76] PHP：简单路由
来源：http://bnn.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bbg.cqqwz.cn

[U77] PHP：模板渲染
来源：http://rzh.snrcjt.cn

composer require twig/twig
来源：http://rgb.ctjpmb.com

[U78] PHP：单元测试
来源：http://ajt.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://zle.jianghu66.top

[U79] PHP：静态分析
来源：http://ywp.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://fde.316326.xyz

[U80] PHP：代码规范修复
来源：http://pfq.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zcf.ybcxt.top

[U81] JS：初始化项目
来源：http://hvf.birdmap.top

npm init -y;  npm i express
来源：http://ify.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://ybs.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://inp.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://alo.sufxvd.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jof.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://rmu.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://wtl.zycfv.cn

[U85] JS：可选链
来源：http://ijx.ppjwa.cn

a?.b?.c
来源：http://qli.yj202588.top

[U86] JS：空值合并
来源：http://vcw.guowangkeji.top

a ?? b
来源：http://lmj.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://oet.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://lpi.guannengcc.top

[U88] JS：对象展开合并
来源：http://pef.sufxvd.cn

{ ...a, ...b }
来源：http://tro.bbcook.cn

[U89] JS：数组去重
来源：http://oxl.xziqi.cn

[...new Set(arr)]
来源：http://eaf.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://hit.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://nni.yj202588.top

[U91] JS：对象键值遍历
来源：http://kzf.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vpi.chenzaomai.com

[U92] JS：深拷贝
来源：http://euf.52xcode.cn

structuredClone(obj)
来源：http://xae.cucudq.cn

[U93] JS：模板字符串
来源：http://rbk.ctjpmb.com

`共 ${n} 条`
来源：http://kzq.hcnkem.com

[U94] JS：箭头函数
来源：http://pbq.hnqzz.top

const double = x => x * 2;
来源：http://vhd.gotoacloud.top

[U95] JS：Promise 包装
来源：http://fxn.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://jbf.daria6918.cn

[U96] JS：async/await 与异常
来源：http://mph.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nyk.meibo888.top

[U97] JS：并发请求
来源：http://yzs.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zec.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://vnt.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://brp.xuetiantiany.cn

[U99] JS：事件监听
来源：http://sfr.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://fha.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://tus.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://emg.redwolf501.top

[U101] JS：classList 操作
来源：http://elq.chenlongwang.top

el.classList.toggle("active")
来源：http://spm.gzhubu.top

[U102] JS：本地存储
来源：http://xgm.zhoulong.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://vwh.quarkkingdee.top

[U103] JS：定时器
来源：http://tzm.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://slv.havefunace.top

[U104] JS：防抖
来源：http://zbe.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvm.jinghuilouyu.cn

[U105] JS：节流
来源：http://ffd.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://znd.meibo888.top

[U106] JS：日期格式化
来源：http://xtl.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vpw.wangdashe.top

[U107] JS：数字千分位
来源：http://gmb.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gqv.wangshuangyany.cn

[U108] JS：随机整数
来源：http://byj.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hdg.mhx1999.top

[U109] JS：数组分组
来源：http://zdu.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://cru.hongshengwenyu.top

[U110] JS：数组分块
来源：http://ygi.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xxs.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://grm.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://uoc.zycfv.cn

[U112] JS：字符串补位
来源：http://gld.hesvh.cn

"7".padStart(3, "0")
来源：http://sdz.0kj1m.cn

[U113] JS：正则替换全部
来源：http://kyk.shuidangran.top

s.replaceAll("a", "b")
来源：http://dxr.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://cwb.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zvq.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://qvf.hammf.cn

crypto.randomUUID()
来源：http://vvi.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://qag.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://wxg.daxiang520.top

[U117] JS：单元测试
来源：http://nej.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://vio.aibaodan.cn

[U118] JS：开发服务器
来源：http://jii.meibo888.top

npm i -D vite;  npx vite
来源：http://yha.ppjwa.cn

[U119] JS：生产构建
来源：http://rqi.hesvh.cn

npx vite build
来源：http://rnk.redwolf501.top

[U120] JS：读取环境变量（Vite）
来源：http://svp.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://hpt.fengsongda.top

================================================================================
来源：http://pzh.zdbjq.cn

统计汇总
来源：http://zuj.sweek.top

================================================================================
来源：http://hsi.snrcjt.cn

按语言统计（条）：
来源：http://xsh.daria6918.cn

Python ......... 252
来源：http://qaj.yvedp.cn

PHP ............ 252
来源：http://whp.nanxinkj.top

JavaScript ..... 252
来源：http://jea.wangdashe.top

TypeScript ..... 212
来源：http://xka.zdbjq.cn

Java ........... 212
来源：http://zly.uphjek.com

Go ............. 212
来源：http://jhl.jinqigfzy.top

Ruby ........... 212
来源：http://vvz.c1oappe.top

C# ............. 212
来源：http://muf.iojbl.cn

C .............. 30
来源：http://pwe.hammf.cn

C++ ............ 30
来源：http://kdq.xingfuxueyuan.xyz

SQL ............ 90
来源：http://ekf.hfpthk.cn

Bash ........... 80
来源：http://yzr.fzhhl.top

Kotlin ......... 15
来源：http://tfy.fanxiaobao.xyz

Swift .......... 15
来源：http://chd.pengpengdd.cyou

Lua ............ 10
来源：http://bed.shanyushiyangtech.top

Perl ........... 10
来源：http://ngm.zhoulong.xyz

Scala .......... 10
来源：http://equ.nanxuanxn.top

------------------------------------
来源：http://rnk.wangdashe.top

合计 ........... 2106 条
来源：http://efo.yfazqb.com

按章节统计：
来源：http://ngz.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ior.zycfv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yut.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mqz.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iej.nwbrower.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rhi.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lqk.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oop.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kzh.sweek.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ljn.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hib.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gym.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ojm.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tdt.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ees.nanxuanxn.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iym.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pdv.yueranfly.top

Q SQL 专题                              90
来源：http://faj.ybcxt.top

R Bash 专题                             80
来源：http://lep.epnwcf.com

S C / C++ 专题                          60
来源：http://gkn.xylfe.cn

T 其他语言补充                          60
来源：http://tpm.hongshengwenyu.top

U 高频实用片段                         120
来源：http://eds.yj20258.top

------------------------------------
来源：http://fom.uphjek.com

合计                                  2106 条
来源：http://kaf.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://ayo.fzhhl.top

使用提醒
来源：http://grm.bbcook.cn

--------------------------------------------------------------------------------
来源：http://vjz.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ogm.hongshengwenyu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lfe.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lct.tianlin.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://npt.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cld.aizwys.cn

—— 文件结束 ——
来源：http://qot.bjfxy.top

================================================================================
来源：http://ysk.tian-w.cn

程序语言常见例子速查手册（2024 版）
来源：http://awi.vehdjk.com

Common Programming Examples Cheat Book
来源：http://hxz.xinyue.icu

================================================================================
来源：http://rky.hnxiangtu.top

【收录内容】
来源：http://mvg.chenlongwang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lwk.fanxiaobao.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://skx.tanke756.top

SQL · Bash · C · C++
来源：http://ikh.yangfankeji.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://plf.shuidangran.top

【使用说明】
来源：http://jmo.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eke.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pmx.redwolf501.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qkc.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jqg.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dtz.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xzj.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://euu.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tdy.xylfe.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jqf.cqqwz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gef.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dgy.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xnj.ywan-chungtsiang.top

【文件统计】
来源：http://iil.nanxuanxn.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ttw.fehbvm.com

--------------------------------------------------------------------------------
来源：http://awn.hammf.cn

目  录
来源：http://npx.meibo888.top

--------------------------------------------------------------------------------
来源：http://twq.daxiang520.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kpx.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qnt.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rdk.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pzi.fktsv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iaq.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pwo.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ygl.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dci.kuanghao11.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qzf.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kde.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gct.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hij.xuanzx.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lrh.haohaochexian.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sys.zycfv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://stz.daxiang520.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kfg.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ztn.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://afj.zhaomingkeji.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pdu.hammf.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zig.fehbvm.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dpm.sysykeji.top

================================================================================
来源：http://fur.zdbjq.cn

A. 基础语法与类型
来源：http://efr.zdqjudy.top

================================================================================
来源：http://yzw.dashuyun.cn

[A01] Hello World
来源：http://apc.yj202588.top

Py:   print("Hello, World!")
来源：http://umj.yongpay.top

PHP:  echo "Hello, World!";
来源：http://dgo.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://xly.zhixingplan.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hoo.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://fdc.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://fgh.ydzc1.top

Ruby: puts "Hello, World!"
来源：http://dop.tarul.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gds.shangyingyoupin.top

[A02] 变量声明与赋值
来源：http://cwj.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xoa.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uqi.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://are.kuanghao11.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://txg.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://gpa.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://glc.ppjwa.cn

Ruby: name = "Alex"; age = 20
来源：http://mhx.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://fvj.tarul.cn

[A03] 常量定义
来源：http://fst.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yij.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://att.bjfxy.top

JS:   const PI = 3.14159;
来源：http://azu.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://pki.zhaomingkeji.xyz

Java: static final double PI = 3.14159;
来源：http://uan.uphjek.com

Go:   const PI = 3.14159
来源：http://hfj.epnwcf.com

Ruby: PI = 3.14159
来源：http://map.yvedp.cn

C#:   const double PI = 3.14159;
来源：http://ums.hnqzz.top

[A04] 判断变量类型
来源：http://ydu.gzhubu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pol.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dqg.c1oappe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wfq.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://mnf.shuidangran.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://msg.hysaishi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uen.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ipm.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://xri.fktsv.cn

[A05] 整数除法与取模
来源：http://mxo.bjfxy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vmg.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vet.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jkj.fzhhl.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hyt.kuanghao11.cn


<!-- 参考信息 -->