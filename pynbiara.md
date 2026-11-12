代发 wailian999

[U43] PHP：声明命名空间
来源：http://tvx.ydzc1.top

namespace App\Http;
来源：http://cid.hammf.cn

[U44] PHP：开启严格类型
来源：http://rvc.yanxiufei.cn

declare(strict_types=1);
来源：http://qpo.dianchejie.cn

[U45] PHP：类型声明与返回类型
来源：http://bje.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wkk.yfazqb.com

[U46] PHP：可空类型
来源：http://tsp.shanyushiyangtech.top

?string $name = null
来源：http://lah.yonumen.top

[U47] PHP：联合类型
来源：http://kxk.daria6918.cn

int|string $id
来源：http://gwu.yuxming.cn

[U48] PHP：纯枚举
来源：http://pnk.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wfd.xuanzx.com

[U49] PHP：只读属性
来源：http://qqg.chenjidiqi.icu

public readonly string $name
来源：http://hpp.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://eiy.bbcook.cn

public function __construct(private int $id) {}
来源：http://vha.zhengqikj.top

[U51] PHP：数组解构
来源：http://san.haohaochexian.top

[$a, $b] = $arr;
来源：http://enf.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://lho.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://vaz.guowangkeji.top

[U53] PHP：空合并运算符
来源：http://ikl.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://ecf.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://uql.jiagoushi.top

$obj?->method()
来源：http://hwj.hnqzz.top

[U55] PHP：match 表达式
来源：http://kcj.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://awy.nanxinkj.top

[U56] PHP：命名参数
来源：http://xlv.hcnkem.com

f(a: 1, b: 2)
来源：http://mns.xylfe.cn

[U57] PHP：字符串插值
来源：http://hpb.jinghuilouyu.cn

"值: {$a}"
来源：http://tdc.nanxinkj.top

[U58] PHP：数组三件套
来源：http://xbk.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gic.jianghu66.top

[U59] PHP：自定义排序
来源：http://rkc.cucudq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oxt.jqgfzy.top

[U60] PHP：JSON 编解码
来源：http://nox.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bll.tianlin.xyz

[U61] PHP：正则
来源：http://ezg.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uni.snrcjt.cn

[U62] PHP：日期对象
来源：http://kcp.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jfe.meibo888.top

[U63] PHP：文件读写
来源：http://idz.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jzq.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://ywf.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://eoo.yongpay.top

[U65] PHP：会话
来源：http://lfy.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hrr.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://ygd.nanxuanxn.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ffb.fktsv.cn

[U67] PHP：处理文件上传
来源：http://zey.hcnkem.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ign.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://yhn.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rvw.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://agg.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://suj.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://ruc.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vyq.tianlin.xyz

[U71] PHP：抛出异常
来源：http://uzb.hfpthk.cn

throw new RuntimeException("失败", 500);
来源：http://voi.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://hej.yanxiufei.cn

error_log("失败: " . $e->getMessage());
来源：http://ptu.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://nnx.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://eje.sxryk.cn

[U74] PHP：读取环境变量
来源：http://iod.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://qdg.yfazqb.com

[U75] PHP：依赖注入
来源：http://cqr.yueranfly.top

composer require psr/container
来源：http://vrz.yuanzhike.top

[U76] PHP：简单路由
来源：http://jzf.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gvy.shanyushiyangkeji.top

[U77] PHP：模板渲染
来源：http://ues.yvedp.cn

composer require twig/twig
来源：http://feg.yvedp.cn

[U78] PHP：单元测试
来源：http://fdq.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://zvq.zdqjudy.top

[U79] PHP：静态分析
来源：http://orb.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://tny.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://nmk.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ccr.ybcxt.top

[U81] JS：初始化项目
来源：http://nyn.pycfn.com

npm init -y;  npm i express
来源：http://zor.haohaochexian.top

[U82] JS：package.json 脚本
来源：http://mtv.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://amd.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://ryr.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://roq.redwolf501.top

[U84] JS：CommonJS 写法
来源：http://urf.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://mph.jinghuilouyu.cn

[U85] JS：可选链
来源：http://kjl.vehdjk.com

a?.b?.c
来源：http://ggw.andypj.xyz

[U86] JS：空值合并
来源：http://oix.0kj1m.cn

a ?? b
来源：http://iqz.yuxming.cn

[U87] JS：解构默认值
来源：http://jck.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://jis.zhengqikj.top

[U88] JS：对象展开合并
来源：http://gfg.nwbrower.top

{ ...a, ...b }
来源：http://ucg.chenzaomai.com

[U89] JS：数组去重
来源：http://qan.jyoumei.cn

[...new Set(arr)]
来源：http://kwl.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://byr.0kj1m.cn

[...arr].sort((a, b) => a - b)
来源：http://gfg.xziqi.cn

[U91] JS：对象键值遍历
来源：http://min.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iiq.ydzc1.top

[U92] JS：深拷贝
来源：http://mxl.zhoulong.xyz

structuredClone(obj)
来源：http://eux.daria6918.cn

[U93] JS：模板字符串
来源：http://erp.uphjek.com

`共 ${n} 条`
来源：http://rgu.gotoacloud.top

[U94] JS：箭头函数
来源：http://vwl.jqgufenzy.top

const double = x => x * 2;
来源：http://swp.andypj.xyz

[U95] JS：Promise 包装
来源：http://vms.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://qmi.yueranfly.top

[U96] JS：async/await 与异常
来源：http://tup.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://grc.cheryme.top

[U97] JS：并发请求
来源：http://kjn.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://eme.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://icm.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://soh.dianchejie.cn

[U99] JS：事件监听
来源：http://zya.hongshengwenyu.top

el.addEventListener("click", e => {})
来源：http://pbd.zdqjudy.top

[U100] JS：DOM 查询
来源：http://cnd.daria6918.cn

document.querySelector(".item")
来源：http://lru.zdqjudy.top

[U101] JS：classList 操作
来源：http://sao.xziqi.cn

el.classList.toggle("active")
来源：http://prw.yangfankeji.com

[U102] JS：本地存储
来源：http://hkg.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jtl.jinqigufen.top

[U103] JS：定时器
来源：http://ink.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hak.316326.xyz

[U104] JS：防抖
来源：http://vgh.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vro.birdmap.top

[U105] JS：节流
来源：http://upm.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mlo.nanxuanxn.top

[U106] JS：日期格式化
来源：http://bab.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jec.cqqwz.cn

[U107] JS：数字千分位
来源：http://vqw.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yna.gzhubu.top

[U108] JS：随机整数
来源：http://mfl.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hng.shuidangran.top

[U109] JS：数组分组
来源：http://tdy.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://qsi.svipenyu.cn

[U110] JS：数组分块
来源：http://yyj.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jwe.xziqi.cn

[U111] JS：对象转 Map
来源：http://tdj.svipenyu.cn

new Map(Object.entries(obj))
来源：http://fvk.hnqzz.top

[U112] JS：字符串补位
来源：http://npp.9152youxi.cn

"7".padStart(3, "0")
来源：http://uqj.tarul.cn

[U113] JS：正则替换全部
来源：http://zqb.wangdashe.top

s.replaceAll("a", "b")
来源：http://ryd.yfazqb.com

[U114] JS：JSON 深比较
来源：http://pcd.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fml.fehbvm.com

[U115] JS：生成 UUID
来源：http://qsi.gotoacloud.top

crypto.randomUUID()
来源：http://tbi.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://duz.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://niq.zdbjq.cn

[U117] JS：单元测试
来源：http://wea.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://wwc.ehwqpu.com

[U118] JS：开发服务器
来源：http://coy.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://ysd.gaohongyu789.top

[U119] JS：生产构建
来源：http://igt.daxiang520.top

npx vite build
来源：http://hja.wangshuangyany.cn

[U120] JS：读取环境变量（Vite）
来源：http://uzz.gaohongyu789.top

import.meta.env.VITE_API_URL
来源：http://bvw.fehbvm.com

================================================================================
来源：http://xlm.hfpthk.cn

统计汇总
来源：http://hsb.jianghu66.top

================================================================================
来源：http://liz.nanxuanxn.top

按语言统计（条）：
来源：http://oyl.wangshuangyany.cn

Python ......... 252
来源：http://cyy.ivvv.top

PHP ............ 252
来源：http://utk.zycfv.cn

JavaScript ..... 252
来源：http://bwf.jyoumei.cn

TypeScript ..... 212
来源：http://bxd.cucudq.cn

Java ........... 212
来源：http://gww.ivvv.top

Go ............. 212
来源：http://ush.yvedp.cn

Ruby ........... 212
来源：http://qfy.sufxvd.cn

C# ............. 212
来源：http://rlp.cqqwz.cn

C .............. 30
来源：http://xai.fehbvm.com

C++ ............ 30
来源：http://maj.jinyuanbaomall.cn

SQL ............ 90
来源：http://pdi.sweek.top

Bash ........... 80
来源：http://sek.hongshengwenyu.top

Kotlin ......... 15
来源：http://vhd.nanxinkj.top

Swift .......... 15
来源：http://kdv.aibaodan.cn

Lua ............ 10
来源：http://dqx.zhongyouzk.top

Perl ........... 10
来源：http://ewi.aibaodan.cn

Scala .......... 10
来源：http://oxy.yonumen.top

------------------------------------
来源：http://rxw.epnwcf.com

合计 ........... 2106 条
来源：http://xty.jinqigufen.top

按章节统计：
来源：http://fyd.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tfg.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://atb.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ueq.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pqz.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ldw.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yrb.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://inf.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jbd.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ccu.ydjk.org.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ifp.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sfr.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://frb.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wpn.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zyx.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vru.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yfp.gotoacloud.top

Q SQL 专题                              90
来源：http://oki.zhiwuduotai.top

R Bash 专题                             80
来源：http://eow.sufxvd.cn

S C / C++ 专题                          60
来源：http://zcv.fengsongda.top

T 其他语言补充                          60
来源：http://myc.xuanzx.com

U 高频实用片段                         120
来源：http://eha.chenlongwang.top

------------------------------------
来源：http://sjd.zhijiandao.cn

合计                                  2106 条
来源：http://tsd.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://cev.zhongyouzk.top

使用提醒
来源：http://wrg.yueranfly.top

--------------------------------------------------------------------------------
来源：http://dct.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://otq.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://paz.xuanzx.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mmf.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vul.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dnv.xylfe.cn

—— 文件结束 ——
来源：http://eka.snrcjt.cn

================================================================================
来源：http://pmm.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://ois.fzhhl.top

Common Programming Examples Cheat Book
来源：http://mnj.jiagoushi.top

================================================================================
来源：http://eum.xuanzx.com

【收录内容】
来源：http://pel.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pjy.zdqjudy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ktw.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://ryr.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yge.bjfxy.top

【使用说明】
来源：http://dtk.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fqi.haohaochexian.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fsr.nanxinkj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jvx.chenzaomai.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vtj.c1oappe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ynh.jinyuanbaomall.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xfc.chenzaomai.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jfg.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hfu.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pkm.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qvu.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zfs.jlsjyb.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ntv.vqdsnc.cn

【文件统计】
来源：http://ork.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ygv.birdmap.top

--------------------------------------------------------------------------------
来源：http://npe.wangdashe.top

目  录
来源：http://ijo.redwolf501.top

--------------------------------------------------------------------------------
来源：http://vsa.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wsb.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://epe.smart0.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zok.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iew.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eqq.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ysx.andypj.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://phb.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sai.jyoumei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qgv.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bdv.hammf.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zar.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hsm.yanxiufei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wjf.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uwe.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xmc.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fvw.jianghu66.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mvn.c1oappe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://gnp.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ezy.fanxiaobao.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ynv.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hqd.xinyue.icu

================================================================================
来源：http://hmm.yueranfly.top

A. 基础语法与类型
来源：http://hzl.cucudq.cn

================================================================================
来源：http://bbx.316326.xyz

[A01] Hello World
来源：http://hen.zdqjudy.top

Py:   print("Hello, World!")
来源：http://cva.zhijiandao.cn

PHP:  echo "Hello, World!";
来源：http://qif.ppjwa.cn

JS:   console.log("Hello, World!");
来源：http://tgm.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qgp.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://soa.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://dyi.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://fls.zhengqikj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mgp.feifeiyinyue.top

[A02] 变量声明与赋值
来源：http://nlm.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wcv.cheryme.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jiv.bbcook.cn

JS:   let name = "Alex"; const age = 20;
来源：http://igp.zhiwuduotai.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fmw.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://vbl.ydzc1.top

Go:   name := "Alex"; age := 20
来源：http://yrn.jyoumei.cn

Ruby: name = "Alex"; age = 20
来源：http://ocw.xuanzx.com

C#:   string name = "Alex"; int age = 20;
来源：http://kep.ybcxt.top

[A03] 常量定义
来源：http://ngd.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ndw.shzxlz.cn

PHP:  const PI = 3.14159;
来源：http://xbc.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://jmj.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://yqz.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://abj.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://cox.shuidangran.top

Ruby: PI = 3.14159
来源：http://hvm.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://ezv.yj20258888.top

[A04] 判断变量类型
来源：http://qmr.yj20258888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://uff.vehdjk.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vyn.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mee.jinghuilouyu.cn

TS:   typeof x; x instanceof Date
来源：http://cog.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zgs.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://lzi.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mew.xziqi.cn

C#:   x.GetType().Name; x is int
来源：http://ztk.sjlbkw.cn

[A05] 整数除法与取模
来源：http://qmi.wangdashe.top


<!-- 参考信息 -->