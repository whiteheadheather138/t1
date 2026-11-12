代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://inf.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gje.yuanzhike.top

[U46] PHP：可空类型
来源：http://sbp.nanxinkj.top

?string $name = null
来源：http://ojd.yj202588.top

[U47] PHP：联合类型
来源：http://xes.birdmap.top

int|string $id
来源：http://mkj.cashguo.top

[U48] PHP：纯枚举
来源：http://frd.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cwd.dashuyun.cn

[U49] PHP：只读属性
来源：http://oul.jinghuilouyu.cn

public readonly string $name
来源：http://oaq.uphjek.com

[U50] PHP：构造器属性提升
来源：http://aay.sjlbkw.cn

public function __construct(private int $id) {}
来源：http://xzu.gogol.net.cn

[U51] PHP：数组解构
来源：http://not.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://abo.yfazqb.com

[U52] PHP：箭头函数
来源：http://ost.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://gge.uphjek.com

[U53] PHP：空合并运算符
来源：http://ame.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://kie.yj20258888.top

[U54] PHP：空安全调用
来源：http://tcq.yanxiufei.cn

$obj?->method()
来源：http://lnz.tarul.cn

[U55] PHP：match 表达式
来源：http://obz.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wkb.epnwcf.com

[U56] PHP：命名参数
来源：http://qfk.yangfankeji.com

f(a: 1, b: 2)
来源：http://jea.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://zny.yangfankeji.com

"值: {$a}"
来源：http://esx.haohaochexian.top

[U58] PHP：数组三件套
来源：http://beu.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zka.shuidangran.top

[U59] PHP：自定义排序
来源：http://fcr.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gqs.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://yfh.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jal.daria6918.cn

[U61] PHP：正则
来源：http://eap.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://khe.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://ngf.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ukd.zycfv.cn

[U63] PHP：文件读写
来源：http://slu.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://imq.hnqzz.top

[U64] PHP：目录遍历
来源：http://qjt.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://kcy.316326.xyz

[U65] PHP：会话
来源：http://dek.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yet.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://kts.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xxb.hnqzz.top

[U67] PHP：处理文件上传
来源：http://vwi.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ick.fehbvm.com

[U68] PHP：PDO 连接
来源：http://mrc.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://twt.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://bcu.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fjw.yuxming.cn

[U70] PHP：PDO 事务
来源：http://yji.nwbrower.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tqr.yueranfly.top

[U71] PHP：抛出异常
来源：http://jve.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://kxy.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://yhf.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://hqs.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://blb.zdqjudy.top

parse_ini_file("config.ini", true)
来源：http://zci.yueranfly.top

[U74] PHP：读取环境变量
来源：http://pcv.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://pqj.hywenlv.cn

[U75] PHP：依赖注入
来源：http://haw.wangshuangyany.cn

composer require psr/container
来源：http://sxn.shuidangran.top

[U76] PHP：简单路由
来源：http://odd.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pcx.0kj1m.cn

[U77] PHP：模板渲染
来源：http://nkg.zycfv.cn

composer require twig/twig
来源：http://ojw.yuanzhike.top

[U78] PHP：单元测试
来源：http://ufa.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://vqe.xziqi.cn

[U79] PHP：静态分析
来源：http://uxi.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://zqs.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://jov.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://icb.9152youxi.cn

[U81] JS：初始化项目
来源：http://ukr.shzxlz.cn

npm init -y;  npm i express
来源：http://syj.smart0.xyz

[U82] JS：package.json 脚本
来源：http://qso.ybcxt.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://skv.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://sph.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://wsm.birdmap.top

[U84] JS：CommonJS 写法
来源：http://tbv.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://ejz.yvedp.cn

[U85] JS：可选链
来源：http://rri.xuetiantiany.cn

a?.b?.c
来源：http://hna.uphjek.com

[U86] JS：空值合并
来源：http://lvv.tanke756.top

a ?? b
来源：http://wci.zhixingplan.top

[U87] JS：解构默认值
来源：http://rlf.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://wcq.yj20258.top

[U88] JS：对象展开合并
来源：http://tjo.yuanzhike.top

{ ...a, ...b }
来源：http://nyi.ppjwa.cn

[U89] JS：数组去重
来源：http://dqq.jyoumei.cn

[...new Set(arr)]
来源：http://wkj.xinyue.icu

[U90] JS：数字数组排序
来源：http://eoe.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://fxn.xziqi.cn

[U91] JS：对象键值遍历
来源：http://wmm.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aav.ydjk.org.cn

[U92] JS：深拷贝
来源：http://aca.hongshengwenyu.top

structuredClone(obj)
来源：http://mij.quarkkingdee.top

[U93] JS：模板字符串
来源：http://puk.quarkkingdee.top

`共 ${n} 条`
来源：http://ifa.bjfxy.top

[U94] JS：箭头函数
来源：http://tdq.vehdjk.com

const double = x => x * 2;
来源：http://slk.zdbjq.cn

[U95] JS：Promise 包装
来源：http://pdh.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://dvk.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://fju.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wau.xylfe.cn

[U97] JS：并发请求
来源：http://rsc.jinghuilouyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wqk.aizwys.cn

[U98] JS：fetch 带 JSON
来源：http://gln.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://its.cucudq.cn

[U99] JS：事件监听
来源：http://org.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://uep.jyoumei.cn

[U100] JS：DOM 查询
来源：http://byy.tian-w.cn

document.querySelector(".item")
来源：http://ykx.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://kqq.vqdsnc.cn

el.classList.toggle("active")
来源：http://hih.nanxuanxn.top

[U102] JS：本地存储
来源：http://ccy.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://vmm.gotoacloud.top

[U103] JS：定时器
来源：http://ryj.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eic.tarul.cn

[U104] JS：防抖
来源：http://bdf.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nqr.fzhhl.top

[U105] JS：节流
来源：http://mph.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sjv.guannengcc.top

[U106] JS：日期格式化
来源：http://cnd.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xuj.jqgfzy.top

[U107] JS：数字千分位
来源：http://tgz.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hbb.chenzaomai.com

[U108] JS：随机整数
来源：http://ibf.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rjz.hesvh.cn

[U109] JS：数组分组
来源：http://ald.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://wtj.fktsv.cn

[U110] JS：数组分块
来源：http://vwq.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qxi.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://inn.andypj.xyz

new Map(Object.entries(obj))
来源：http://jqq.cheryme.top

[U112] JS：字符串补位
来源：http://clz.yfazqb.com

"7".padStart(3, "0")
来源：http://afc.fktsv.cn

[U113] JS：正则替换全部
来源：http://wnj.gotoacloud.top

s.replaceAll("a", "b")
来源：http://tzy.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://atb.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://vjg.vehdjk.com

[U115] JS：生成 UUID
来源：http://anm.yuanzhike.top

crypto.randomUUID()
来源：http://inx.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://pfb.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://clc.jqgfzy.top

[U117] JS：单元测试
来源：http://aiq.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://bda.xuanzx.com

[U118] JS：开发服务器
来源：http://hye.bjfxy.top

npm i -D vite;  npx vite
来源：http://zgp.yvedp.cn

[U119] JS：生产构建
来源：http://tsd.cdnleiting.top

npx vite build
来源：http://bjo.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://wyq.pengpengdd.cyou

import.meta.env.VITE_API_URL
来源：http://bzm.aizwys.cn

================================================================================
来源：http://gnm.aizwys.cn

统计汇总
来源：http://zdm.chenjidiqi.icu

================================================================================
来源：http://plm.hywenlv.cn

按语言统计（条）：
来源：http://ngf.sysykeji.top

Python ......... 252
来源：http://hsj.cqqwz.cn

PHP ............ 252
来源：http://pae.gzhubu.top

JavaScript ..... 252
来源：http://qny.zdbjq.cn

TypeScript ..... 212
来源：http://phs.yfazqb.com

Java ........... 212
来源：http://dkn.shanyushiyangkeji.top

Go ............. 212
来源：http://xmz.nanxuanxn.top

Ruby ........... 212
来源：http://rxz.jinqigfzy.top

C# ............. 212
来源：http://rjt.yuanzhike.top

C .............. 30
来源：http://ikn.jinghuilouyu.cn

C++ ............ 30
来源：http://sln.zhongyouzk.top

SQL ............ 90
来源：http://inz.yj20258888.top

Bash ........... 80
来源：http://jka.snrcjt.cn

Kotlin ......... 15
来源：http://gur.pycfn.com

Swift .......... 15
来源：http://fho.shangyingyoupin.top

Lua ............ 10
来源：http://api.jinqigfzy.top

Perl ........... 10
来源：http://zbw.guowangkeji.top

Scala .......... 10
来源：http://cgz.chenzaomai.com

------------------------------------
来源：http://gky.wangdashe.top

合计 ........... 2106 条
来源：http://dgf.daria6918.cn

按章节统计：
来源：http://tvq.cqqwz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nkh.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zyx.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dol.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fvh.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vhi.xingfuxueyuan.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yvx.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zjb.yj20258888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://piw.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wam.yvedp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rca.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dli.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eaq.vqdsnc.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://acn.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dmw.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xcv.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ahx.yj202588.top

Q SQL 专题                              90
来源：http://rgm.vqdsnc.cn

R Bash 专题                             80
来源：http://wny.guannengcc.top

S C / C++ 专题                          60
来源：http://jzj.hysaishi.cn

T 其他语言补充                          60
来源：http://kfp.dianchejie.cn

U 高频实用片段                         120
来源：http://hdh.vehdjk.com

------------------------------------
来源：http://rng.andypj.xyz

合计                                  2106 条
来源：http://meh.smart0.xyz

--------------------------------------------------------------------------------
来源：http://szm.zhiwuduotai.top

使用提醒
来源：http://yav.yueranfly.top

--------------------------------------------------------------------------------
来源：http://kmy.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bhi.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rlh.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ltz.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bkl.yvedp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ode.mhx1999.top

—— 文件结束 ——
来源：http://nou.dashuyun.cn

================================================================================
来源：http://rjz.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://smt.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://hdc.epnwcf.com

================================================================================
来源：http://dlh.zhixingplan.top

【收录内容】
来源：http://qeg.epnwcf.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://sdj.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dfy.yanxiufei.cn

SQL · Bash · C · C++
来源：http://ryt.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yun.hywenlv.cn

【使用说明】
来源：http://ltx.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qhc.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ugp.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ter.dashuyun.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lzk.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cgq.fzhhl.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zws.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ndb.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://awp.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://txq.tanke756.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://omh.andypj.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iov.zdqjudy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kmm.bbcook.cn

【文件统计】
来源：http://hjt.sjlbkw.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tpd.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://cjt.bjfxy.top

目  录
来源：http://knb.wangdashe.top

--------------------------------------------------------------------------------
来源：http://cod.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pgz.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kvj.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wym.aizwys.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fnr.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://klj.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://anu.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cgs.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uwv.yueranfly.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rpp.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://plc.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://orf.jiagoushi.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pbm.hnqzz.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kjf.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rpd.gaohongyu789.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ouu.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dci.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xus.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://oir.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kui.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zxs.epnwcf.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rlf.kuanghao11.cn

================================================================================
来源：http://smo.jianghu66.top

A. 基础语法与类型
来源：http://aru.zdqjudy.top

================================================================================
来源：http://kkh.redwolf501.top

[A01] Hello World
来源：http://dbb.snrcjt.cn

Py:   print("Hello, World!")
来源：http://tce.meibo888.top

PHP:  echo "Hello, World!";
来源：http://inh.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://ghe.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://der.andypj.xyz

Java: System.out.println("Hello, World!");
来源：http://dwl.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://wcn.gzhubu.top

Ruby: puts "Hello, World!"
来源：http://dvv.yj202588.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ufd.hammf.cn

[A02] 变量声明与赋值
来源：http://zot.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kzl.ppjwa.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bgt.yuxming.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zog.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sfe.xingfuxueyuan.xyz

Java: String name = "Alex"; int age = 20;
来源：http://ebk.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://hte.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://vnt.quarkkingdee.top

C#:   string name = "Alex"; int age = 20;
来源：http://vyf.svipenyu.cn

[A03] 常量定义
来源：http://qbg.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tdj.zdbjq.cn

PHP:  const PI = 3.14159;
来源：http://edi.jqgfzy.top

JS:   const PI = 3.14159;
来源：http://yuk.ehwqpu.com

TS:   const PI: number = 3.14159;
来源：http://gnr.zhiwuduotai.top

Java: static final double PI = 3.14159;
来源：http://qya.zycfv.cn

Go:   const PI = 3.14159
来源：http://bic.ppjwa.cn

Ruby: PI = 3.14159
来源：http://wge.cheryme.top

C#:   const double PI = 3.14159;
来源：http://bad.feifeiyinyue.top

[A04] 判断变量类型
来源：http://iej.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ziw.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lyz.cheryme.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tds.shangyingyoupin.top

TS:   typeof x; x instanceof Date
来源：http://geh.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ics.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://jfi.cdnleiting.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vvz.jinghuilouyu.cn

C#:   x.GetType().Name; x is int
来源：http://vqy.aizwys.cn

[A05] 整数除法与取模
来源：http://jpt.jqgufenzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qpd.hesvh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xca.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sll.nanxinkj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xfh.jianghu66.top


<!-- 参考信息 -->