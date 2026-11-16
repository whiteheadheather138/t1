代发 wailian999

[U43] PHP：声明命名空间
来源：http://zpu.kuanghao11.cn

namespace App\Http;
来源：http://ruk.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://qws.dashuyun.cn

declare(strict_types=1);
来源：http://tyj.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://oth.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://squ.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://fpb.0kj1m.cn

?string $name = null
来源：http://fhb.daxiang520.top

[U47] PHP：联合类型
来源：http://boz.gaohongyu789.top

int|string $id
来源：http://hsi.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://xaf.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://erz.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://mte.sysykeji.top

public readonly string $name
来源：http://ynh.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://kyv.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://ebk.tanke756.top

[U51] PHP：数组解构
来源：http://ery.gotoacloud.top

[$a, $b] = $arr;
来源：http://odi.tian-w.cn

[U52] PHP：箭头函数
来源：http://rin.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://gwt.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://rcr.bbcook.cn

$v = $a ?? $b ?? "default";
来源：http://edm.vehdjk.com

[U54] PHP：空安全调用
来源：http://kcf.nwbrower.top

$obj?->method()
来源：http://aba.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://abi.aizwys.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ubj.xziqi.cn

[U56] PHP：命名参数
来源：http://wut.shzxlz.cn

f(a: 1, b: 2)
来源：http://awz.chenlongwang.top

[U57] PHP：字符串插值
来源：http://anw.ivvv.top

"值: {$a}"
来源：http://njw.yuxming.cn

[U58] PHP：数组三件套
来源：http://gah.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xjf.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://mfg.smart0.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://muj.jqgufenzy.top

[U60] PHP：JSON 编解码
来源：http://ctx.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ilu.yfazqb.com

[U61] PHP：正则
来源：http://tzw.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wml.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://tcw.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tce.tanke756.top

[U63] PHP：文件读写
来源：http://hfq.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dmi.yvedp.cn

[U64] PHP：目录遍历
来源：http://zmr.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://flh.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://yii.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rux.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://caa.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xzr.havefunace.top

[U67] PHP：处理文件上传
来源：http://tad.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://poc.jlsjyb.cn

[U68] PHP：PDO 连接
来源：http://zms.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dhh.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://mqc.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cnr.52xcode.cn

[U70] PHP：PDO 事务
来源：http://ses.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uha.sxryk.cn

[U71] PHP：抛出异常
来源：http://wyh.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://foe.316326.xyz

[U72] PHP：写错误日志
来源：http://ahp.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://ahh.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://bap.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://mpi.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://edd.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://qdf.yueranfly.top

[U75] PHP：依赖注入
来源：http://gre.redwolf501.top

composer require psr/container
来源：http://egc.yj202588.top

[U76] PHP：简单路由
来源：http://znx.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rcw.guannengcc.top

[U77] PHP：模板渲染
来源：http://xcs.zhiwuduotai.top

composer require twig/twig
来源：http://sbm.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://ivg.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://hrf.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://xao.jyoumei.cn

composer require --dev phpstan/phpstan
来源：http://ykx.yj202588.top

[U80] PHP：代码规范修复
来源：http://hef.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jsq.jyoumei.cn

[U81] JS：初始化项目
来源：http://vtb.tian-w.cn

npm init -y;  npm i express
来源：http://xzp.ivvv.top

[U82] JS：package.json 脚本
来源：http://bio.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uff.daxiang520.top

[U83] JS：ES Module 导入导出
来源：http://guu.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vep.meibo888.top

[U84] JS：CommonJS 写法
来源：http://nvd.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://qqs.sweek.top

[U85] JS：可选链
来源：http://bkr.cashguo.top

a?.b?.c
来源：http://qmv.c1oappe.top

[U86] JS：空值合并
来源：http://fvk.chenjidiqi.icu

a ?? b
来源：http://kyd.ywan-chungtsiang.top

[U87] JS：解构默认值
来源：http://ssu.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://tgw.fzhhl.top

[U88] JS：对象展开合并
来源：http://epx.svipenyu.cn

{ ...a, ...b }
来源：http://dbj.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://aku.daria6918.cn

[...new Set(arr)]
来源：http://xjj.epnwcf.com

[U90] JS：数字数组排序
来源：http://qmk.tanke756.top

[...arr].sort((a, b) => a - b)
来源：http://btv.yueranfly.top

[U91] JS：对象键值遍历
来源：http://thw.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pyt.jinqigufen.top

[U92] JS：深拷贝
来源：http://ttt.yj20258888.top

structuredClone(obj)
来源：http://wxr.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://svi.yj20258888.top

`共 ${n} 条`
来源：http://pvw.guowangkeji.top

[U94] JS：箭头函数
来源：http://wvk.sufxvd.cn

const double = x => x * 2;
来源：http://ode.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://vnw.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://jtc.daxiang520.top

[U96] JS：async/await 与异常
来源：http://mlz.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xgf.9152youxi.cn

[U97] JS：并发请求
来源：http://lfv.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kih.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://rft.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xab.jlsjyb.cn

[U99] JS：事件监听
来源：http://wxt.tarul.cn

el.addEventListener("click", e => {})
来源：http://xbq.yj20258.top

[U100] JS：DOM 查询
来源：http://ady.zhongyouzk.top

document.querySelector(".item")
来源：http://cbs.shuidangran.top

[U101] JS：classList 操作
来源：http://byd.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://bhv.hnxiangtu.top

[U102] JS：本地存储
来源：http://org.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://eml.fengsongda.top

[U103] JS：定时器
来源：http://xgh.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rio.jinqigfzy.top

[U104] JS：防抖
来源：http://uul.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxi.jlsjyb.cn

[U105] JS：节流
来源：http://jkc.hongshengwenyu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wqo.shuidangran.top

[U106] JS：日期格式化
来源：http://zhb.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kwi.ydjk.org.cn

[U107] JS：数字千分位
来源：http://fdq.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lom.gaohongyu789.top

[U108] JS：随机整数
来源：http://ehb.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://esn.cdnleiting.top

[U109] JS：数组分组
来源：http://edx.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://urf.hammf.cn

[U110] JS：数组分块
来源：http://nre.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://urz.shzxlz.cn

[U111] JS：对象转 Map
来源：http://kvq.dianchejie.cn

new Map(Object.entries(obj))
来源：http://vmo.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://uxx.pycfn.com

"7".padStart(3, "0")
来源：http://keh.jqgfzy.top

[U113] JS：正则替换全部
来源：http://hod.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://iyz.zycfv.cn

[U114] JS：JSON 深比较
来源：http://wbj.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://euk.daxiang520.top

[U115] JS：生成 UUID
来源：http://irh.xuetiantiany.cn

crypto.randomUUID()
来源：http://bxm.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://gaf.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://llr.pengpengdd.cyou

[U117] JS：单元测试
来源：http://joo.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://cob.sjlbkw.cn

[U118] JS：开发服务器
来源：http://oph.pycfn.com

npm i -D vite;  npx vite
来源：http://npz.vqdsnc.cn

[U119] JS：生产构建
来源：http://xhs.fengsongda.top

npx vite build
来源：http://htp.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://rec.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://iwx.sweek.top

================================================================================
来源：http://guv.jqgufenzy.top

统计汇总
来源：http://seq.316326.xyz

================================================================================
来源：http://ntd.cashguo.top

按语言统计（条）：
来源：http://wbr.hesvh.cn

Python ......... 252
来源：http://lss.hcnkem.com

PHP ............ 252
来源：http://glz.wangshuangyany.cn

JavaScript ..... 252
来源：http://itr.zhengqikj.top

TypeScript ..... 212
来源：http://ecw.snrcjt.cn

Java ........... 212
来源：http://vyu.fengsongda.top

Go ............. 212
来源：http://kqe.epnwcf.com

Ruby ........... 212
来源：http://wfv.zdbjq.cn

C# ............. 212
来源：http://iyz.dashuyun.cn

C .............. 30
来源：http://gnc.haohaochexian.top

C++ ............ 30
来源：http://ufo.hywenlv.cn

SQL ............ 90
来源：http://ial.tian-w.cn

Bash ........... 80
来源：http://bwl.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://njw.meibo888.top

Swift .......... 15
来源：http://ncf.ivvv.top

Lua ............ 10
来源：http://ena.snrcjt.cn

Perl ........... 10
来源：http://mii.xinyue.icu

Scala .......... 10
来源：http://oon.9152youxi.cn

------------------------------------
来源：http://qfs.yonumen.top

合计 ........... 2106 条
来源：http://dwd.zhiwuduotai.top

按章节统计：
来源：http://oar.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fhb.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zxt.mhx1999.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qfg.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ice.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://clu.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dfa.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://olh.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qjg.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://clc.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mak.yanxiufei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nog.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://moc.jiagoushi.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://twn.ivvv.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fao.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ngr.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zzu.daxiang520.top

Q SQL 专题                              90
来源：http://klk.pycfn.com

R Bash 专题                             80
来源：http://nad.epnwcf.com

S C / C++ 专题                          60
来源：http://oda.jinqigfzy.top

T 其他语言补充                          60
来源：http://aem.ivvv.top

U 高频实用片段                         120
来源：http://rpl.birdmap.top

------------------------------------
来源：http://jae.andypj.xyz

合计                                  2106 条
来源：http://epp.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://wor.smart0.xyz

使用提醒
来源：http://xhj.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://iyd.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kxh.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gxs.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nzv.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uyg.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ydg.ctjpmb.com

—— 文件结束 ——
来源：http://iyn.havefunace.top

================================================================================
来源：http://jwh.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://bvl.shanyushiyangtech.top

Common Programming Examples Cheat Book
来源：http://jqt.ybcxt.top

================================================================================
来源：http://qig.jinqigfzy.top

【收录内容】
来源：http://zfv.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iji.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hwb.andypj.xyz

SQL · Bash · C · C++
来源：http://epj.haohaochexian.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dvj.guowangkeji.top

【使用说明】
来源：http://yjj.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://trh.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aor.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kxn.zhengqikj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fak.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://csv.cdnleiting.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bhw.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xhv.feifeiyinyue.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mmo.feifeiyinyue.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pig.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cwo.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uix.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pra.yj202588.top

【文件统计】
来源：http://uqt.shuidangran.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vuq.cashguo.top

--------------------------------------------------------------------------------
来源：http://mkj.zdqjudy.top

目  录
来源：http://kyd.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://kqy.sweek.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dtf.svipenyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://noi.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mgo.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oie.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rdu.hongshengwenyu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qys.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tnm.haohaochexian.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://res.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bky.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ucw.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nzo.jinqigufen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kmw.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zgj.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gas.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xor.yvedp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ifz.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pqr.fzhhl.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://oay.bbcook.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hdy.meibo888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sgu.feifeiyinyue.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gha.snrcjt.cn

================================================================================
来源：http://fvx.tarul.cn

A. 基础语法与类型
来源：http://arc.shanyushiyangkeji.top

================================================================================
来源：http://daz.ydzc1.top

[A01] Hello World
来源：http://dsc.ehwqpu.com

Py:   print("Hello, World!")
来源：http://bft.zdqjudy.top

PHP:  echo "Hello, World!";
来源：http://sfv.hysaishi.cn

JS:   console.log("Hello, World!");
来源：http://khg.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kuh.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://vtb.xingfuxueyuan.xyz

Go:   fmt.Println("Hello, World!")
来源：http://vps.jianghu66.top

Ruby: puts "Hello, World!"
来源：http://crs.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dde.yj202588.top

[A02] 变量声明与赋值
来源：http://jgk.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yoq.daxiang520.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ztm.pengpengdd.cyou

JS:   let name = "Alex"; const age = 20;
来源：http://evr.sweek.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://irp.mhx1999.top

Java: String name = "Alex"; int age = 20;
来源：http://ybe.tarul.cn

Go:   name := "Alex"; age := 20
来源：http://ikh.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://loy.hammf.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rqi.9152youxi.cn

[A03] 常量定义
来源：http://sad.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mbe.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://zcn.ydjk.org.cn

JS:   const PI = 3.14159;
来源：http://vyg.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://kjp.svipenyu.cn

Java: static final double PI = 3.14159;
来源：http://qjp.hcnkem.com

Go:   const PI = 3.14159
来源：http://vtr.yueranfly.top

Ruby: PI = 3.14159
来源：http://adp.52xcode.cn

C#:   const double PI = 3.14159;
来源：http://ytf.snrcjt.cn

[A04] 判断变量类型
来源：http://rcu.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://bjy.redwolf501.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ioe.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qeh.c1oappe.top

TS:   typeof x; x instanceof Date
来源：http://jde.uphjek.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zqq.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ezl.havefunace.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yqy.sufxvd.cn

C#:   x.GetType().Name; x is int
来源：http://nhq.yuanzhike.top

[A05] 整数除法与取模
来源：http://sht.yj202588.top


<!-- 参考信息 -->