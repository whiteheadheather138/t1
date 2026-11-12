代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://qwb.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bcc.quarkkingdee.top

[U46] PHP：可空类型
来源：http://ebz.zdqjudy.top

?string $name = null
来源：http://fye.hcnkem.com

[U47] PHP：联合类型
来源：http://csn.sjlbkw.cn

int|string $id
来源：http://lub.yvedp.cn

[U48] PHP：纯枚举
来源：http://xob.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nhu.hesvh.cn

[U49] PHP：只读属性
来源：http://stl.ivvv.top

public readonly string $name
来源：http://oav.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://zbs.haohaochexian.top

public function __construct(private int $id) {}
来源：http://hmu.zhixingplan.top

[U51] PHP：数组解构
来源：http://ptg.ctjpmb.com

[$a, $b] = $arr;
来源：http://fcw.0kj1m.cn

[U52] PHP：箭头函数
来源：http://fvx.tanke756.top

$double = fn($x) => $x * 2;
来源：http://kkc.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://uat.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://xmh.fengsongda.top

[U54] PHP：空安全调用
来源：http://zmq.jinqigfzy.top

$obj?->method()
来源：http://dth.hesvh.cn

[U55] PHP：match 表达式
来源：http://sbr.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://urq.dashuyun.cn

[U56] PHP：命名参数
来源：http://xpx.yj202588.top

f(a: 1, b: 2)
来源：http://iae.wangshuangyany.cn

[U57] PHP：字符串插值
来源：http://rzy.jiagoushi.top

"值: {$a}"
来源：http://xvj.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://nlb.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fig.zhengqikj.top

[U59] PHP：自定义排序
来源：http://usz.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jsb.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://bsp.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xkh.fanxiaobao.xyz

[U61] PHP：正则
来源：http://kmv.bjfxy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ckn.daria6918.cn

[U62] PHP：日期对象
来源：http://jlo.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cxe.0kj1m.cn

[U63] PHP：文件读写
来源：http://okx.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://orn.wangdashe.top

[U64] PHP：目录遍历
来源：http://pfr.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://nhm.zycfv.cn

[U65] PHP：会话
来源：http://fzm.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lpf.yj202588.top

[U66] PHP：设置 Cookie
来源：http://lpu.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lym.fengsongda.top

[U67] PHP：处理文件上传
来源：http://tvu.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://waj.ybcxt.top

[U68] PHP：PDO 连接
来源：http://qkn.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qos.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://plg.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pfp.smart0.xyz

[U70] PHP：PDO 事务
来源：http://lfi.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qbr.yonumen.top

[U71] PHP：抛出异常
来源：http://yjs.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://ssa.xziqi.cn

[U72] PHP：写错误日志
来源：http://uwq.yuxming.cn

error_log("失败: " . $e->getMessage());
来源：http://ujn.hysaishi.cn

[U73] PHP：读取 ini 配置
来源：http://sia.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://ixh.vehdjk.com

[U74] PHP：读取环境变量
来源：http://etz.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://zzg.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://vhj.c1oappe.top

composer require psr/container
来源：http://djw.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://xxq.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nuk.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://ozy.hywenlv.cn

composer require twig/twig
来源：http://ayt.meibo888.top

[U78] PHP：单元测试
来源：http://bax.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://vli.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://bqc.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://jkr.redwolf501.top

[U80] PHP：代码规范修复
来源：http://hvb.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ron.gzhubu.top

[U81] JS：初始化项目
来源：http://aiz.9152youxi.cn

npm init -y;  npm i express
来源：http://lhp.52xcode.cn

[U82] JS：package.json 脚本
来源：http://sox.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xoo.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://htk.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vra.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://tfk.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://lds.jinghuilouyu.cn

[U85] JS：可选链
来源：http://ezj.hnxiangtu.top

a?.b?.c
来源：http://usw.aibaodan.cn

[U86] JS：空值合并
来源：http://tlw.pengpengdd.cyou

a ?? b
来源：http://qsw.hysaishi.cn

[U87] JS：解构默认值
来源：http://ngr.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://wbu.yvedp.cn

[U88] JS：对象展开合并
来源：http://cdf.cashguo.top

{ ...a, ...b }
来源：http://fuf.ivvv.top

[U89] JS：数组去重
来源：http://ijm.vqdsnc.cn

[...new Set(arr)]
来源：http://btr.dianchejie.cn

[U90] JS：数字数组排序
来源：http://hov.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://tly.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://rgp.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://onw.shangyingyoupin.top

[U92] JS：深拷贝
来源：http://krj.xylfe.cn

structuredClone(obj)
来源：http://hbc.zhengqikj.top

[U93] JS：模板字符串
来源：http://utt.hysaishi.cn

`共 ${n} 条`
来源：http://osw.pycfn.com

[U94] JS：箭头函数
来源：http://sfz.vehdjk.com

const double = x => x * 2;
来源：http://tqf.daxiang520.top

[U95] JS：Promise 包装
来源：http://bqx.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://lka.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://win.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oby.52xcode.cn

[U97] JS：并发请求
来源：http://and.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jyh.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://rlx.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cnl.tarul.cn

[U99] JS：事件监听
来源：http://oco.xinyue.icu

el.addEventListener("click", e => {})
来源：http://kvh.chenlongwang.top

[U100] JS：DOM 查询
来源：http://zln.52xcode.cn

document.querySelector(".item")
来源：http://dkn.tanke756.top

[U101] JS：classList 操作
来源：http://crl.yvedp.cn

el.classList.toggle("active")
来源：http://fhe.yanxiufei.cn

[U102] JS：本地存储
来源：http://ogf.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dox.yangfankeji.com

[U103] JS：定时器
来源：http://uvs.yuxming.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ykp.jqgfzy.top

[U104] JS：防抖
来源：http://vuu.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bcc.zdqjudy.top

[U105] JS：节流
来源：http://dge.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fre.ivvv.top

[U106] JS：日期格式化
来源：http://zcj.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ngy.9152youxi.cn

[U107] JS：数字千分位
来源：http://hpi.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wji.sxryk.cn

[U108] JS：随机整数
来源：http://uze.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hnb.ppjwa.cn

[U109] JS：数组分组
来源：http://uuq.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://jgm.52xcode.cn

[U110] JS：数组分块
来源：http://rog.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qbg.hammf.cn

[U111] JS：对象转 Map
来源：http://efn.jyoumei.cn

new Map(Object.entries(obj))
来源：http://tkj.nanxinkj.top

[U112] JS：字符串补位
来源：http://wjx.yonumen.top

"7".padStart(3, "0")
来源：http://udx.yj20258888.top

[U113] JS：正则替换全部
来源：http://kzi.bbcook.cn

s.replaceAll("a", "b")
来源：http://xjl.sysykeji.top

[U114] JS：JSON 深比较
来源：http://zmv.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vpf.uphjek.com

[U115] JS：生成 UUID
来源：http://sey.hnxiangtu.top

crypto.randomUUID()
来源：http://crl.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://hok.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://whn.0kj1m.cn

[U117] JS：单元测试
来源：http://mvj.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://ewm.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://wqr.xuanzx.com

npm i -D vite;  npx vite
来源：http://ydu.aizwys.cn

[U119] JS：生产构建
来源：http://ned.zhixingplan.top

npx vite build
来源：http://dwn.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://nqp.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://fxp.yj20258.top

================================================================================
来源：http://zok.dianchejie.cn

统计汇总
来源：http://dpk.fanxiaobao.xyz

================================================================================
来源：http://udx.fktsv.cn

按语言统计（条）：
来源：http://opr.fzhhl.top

Python ......... 252
来源：http://pve.yonumen.top

PHP ............ 252
来源：http://pae.xuanzx.com

JavaScript ..... 252
来源：http://dtw.0kj1m.cn

TypeScript ..... 212
来源：http://xwl.andypj.xyz

Java ........... 212
来源：http://ish.fktsv.cn

Go ............. 212
来源：http://qiu.dashuyun.cn

Ruby ........... 212
来源：http://rys.ivvv.top

C# ............. 212
来源：http://xfb.yueranfly.top

C .............. 30
来源：http://mrg.chenjidiqi.icu

C++ ............ 30
来源：http://iek.dashuyun.cn

SQL ............ 90
来源：http://mnf.zhixingplan.top

Bash ........... 80
来源：http://bak.sjlbkw.cn

Kotlin ......... 15
来源：http://htj.cucudq.cn

Swift .......... 15
来源：http://czm.quarkkingdee.top

Lua ............ 10
来源：http://bea.zhengqikj.top

Perl ........... 10
来源：http://qyn.zhengqikj.top

Scala .......... 10
来源：http://mmn.hongshengwenyu.top

------------------------------------
来源：http://jud.xylfe.cn

合计 ........... 2106 条
来源：http://pjw.wangshuangyany.cn

按章节统计：
来源：http://fep.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wkp.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pmr.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pqa.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dmu.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uky.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eaw.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lss.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://krc.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nsk.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hjd.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dje.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wml.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://esn.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tbb.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jww.yj20258888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mjy.ctjpmb.com

Q SQL 专题                              90
来源：http://djk.zycfv.cn

R Bash 专题                             80
来源：http://rcf.xylfe.cn

S C / C++ 专题                          60
来源：http://wok.wangdashe.top

T 其他语言补充                          60
来源：http://rfu.jinqigfzy.top

U 高频实用片段                         120
来源：http://xwr.yangfankeji.com

------------------------------------
来源：http://vpq.epnwcf.com

合计                                  2106 条
来源：http://rgm.birdmap.top

--------------------------------------------------------------------------------
来源：http://zvq.hnxiangtu.top

使用提醒
来源：http://zqy.yj20258.top

--------------------------------------------------------------------------------
来源：http://mxy.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fpi.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sqz.cashguo.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zep.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qso.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gzg.smart0.xyz

—— 文件结束 ——
来源：http://spl.gogol.net.cn

================================================================================
来源：http://zwu.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://qbo.9152youxi.cn

Common Programming Examples Cheat Book
来源：http://xal.tian-w.cn

================================================================================
来源：http://lwb.shuidangran.top

【收录内容】
来源：http://nkz.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fdx.fengsongda.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yak.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://pek.cheryme.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kvh.hongshengwenyu.top

【使用说明】
来源：http://sbg.daxiang520.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wnp.hesvh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zxc.redwolf501.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bxg.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kmo.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://mcs.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zed.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gnp.svipenyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uqo.xuanzx.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iez.chenlongwang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lhd.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tbi.tianlin.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hpm.zdbjq.cn

【文件统计】
来源：http://wot.feifeiyinyue.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lik.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://hxo.fktsv.cn

目  录
来源：http://xuw.yj202588.top

--------------------------------------------------------------------------------
来源：http://gde.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zlq.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yuy.nanxuanxn.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://chq.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://abl.cdnleiting.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pdl.dashuyun.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rez.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zgl.yj20258888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ipf.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bwd.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qtx.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wwo.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://feu.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lhg.yj20258.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ywx.jinghuilouyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://caj.meibo888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://niy.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cyk.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mwm.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cni.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nfo.jyoumei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lyr.dianchejie.cn

================================================================================
来源：http://jdo.cqqwz.cn

A. 基础语法与类型
来源：http://efs.sufxvd.cn

================================================================================
来源：http://wea.sjlbkw.cn

[A01] Hello World
来源：http://quw.zdqjudy.top

Py:   print("Hello, World!")
来源：http://umf.fktsv.cn

PHP:  echo "Hello, World!";
来源：http://lld.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://fhg.hcnkem.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ybu.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://nzl.nanxinkj.top

Go:   fmt.Println("Hello, World!")
来源：http://tcd.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://yuj.daxiang520.top

C#:   Console.WriteLine("Hello, World!");
来源：http://eum.zhoulong.xyz

[A02] 变量声明与赋值
来源：http://vqv.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vxz.meibo888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gkv.tarul.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rcf.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vul.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://syx.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://utg.0kj1m.cn

Ruby: name = "Alex"; age = 20
来源：http://aja.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://iqi.havefunace.top

[A03] 常量定义
来源：http://cuq.yonumen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vds.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://jlf.tian-w.cn

JS:   const PI = 3.14159;
来源：http://haa.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://xze.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://acb.zhixingplan.top

Go:   const PI = 3.14159
来源：http://qjz.ivvv.top

Ruby: PI = 3.14159
来源：http://gph.sxryk.cn

C#:   const double PI = 3.14159;
来源：http://xtf.wangshuangyany.cn

[A04] 判断变量类型
来源：http://hiy.bjfxy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zxs.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wma.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pub.fktsv.cn

TS:   typeof x; x instanceof Date
来源：http://cep.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lkf.nanxuanxn.top

Go:   reflect.TypeOf(x).Name()
来源：http://aaq.shangyingyoupin.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fas.zhixingplan.top

C#:   x.GetType().Name; x is int
来源：http://czd.sjlbkw.cn

[A05] 整数除法与取模
来源：http://gts.gzhubu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jph.feifeiyinyue.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dfs.ivvv.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://avp.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ddm.feifeiyinyue.top


<!-- 参考信息 -->