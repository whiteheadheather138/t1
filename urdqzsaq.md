代发 wailian999

[U43] PHP：声明命名空间
来源：http://wuw.shangyingyoupin.top

namespace App\Http;
来源：http://udo.hcnkem.com

[U44] PHP：开启严格类型
来源：http://hhp.wangdashe.top

declare(strict_types=1);
来源：http://psl.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://nua.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://eti.meibo888.top

[U46] PHP：可空类型
来源：http://plm.bjfxy.top

?string $name = null
来源：http://hir.sjlbkw.cn

[U47] PHP：联合类型
来源：http://evm.feifeiyinyue.top

int|string $id
来源：http://jgn.epnwcf.com

[U48] PHP：纯枚举
来源：http://epj.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gmh.vehdjk.com

[U49] PHP：只读属性
来源：http://ohu.xylfe.cn

public readonly string $name
来源：http://jxd.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://pzz.chenzaomai.com

public function __construct(private int $id) {}
来源：http://wsp.fzhhl.top

[U51] PHP：数组解构
来源：http://equ.fzhhl.top

[$a, $b] = $arr;
来源：http://xdg.jyoumei.cn

[U52] PHP：箭头函数
来源：http://ymo.yonumen.top

$double = fn($x) => $x * 2;
来源：http://kre.yvedp.cn

[U53] PHP：空合并运算符
来源：http://fgj.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://dbk.nanxinkj.top

[U54] PHP：空安全调用
来源：http://xpz.svipenyu.cn

$obj?->method()
来源：http://ity.sxryk.cn

[U55] PHP：match 表达式
来源：http://ler.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pnl.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://let.jlsjyb.cn

f(a: 1, b: 2)
来源：http://ent.fktsv.cn

[U57] PHP：字符串插值
来源：http://bma.jinqigufen.top

"值: {$a}"
来源：http://uaa.shzxlz.cn

[U58] PHP：数组三件套
来源：http://rvd.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jpe.fehbvm.com

[U59] PHP：自定义排序
来源：http://eyx.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twl.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://atz.yuxming.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tki.nwbrower.top

[U61] PHP：正则
来源：http://ypi.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mam.fehbvm.com

[U62] PHP：日期对象
来源：http://kbl.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bhi.hnqzz.top

[U63] PHP：文件读写
来源：http://gtz.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dnj.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://jef.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://abr.yj20258888.top

[U65] PHP：会话
来源：http://rni.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://sgl.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://bdd.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wjm.hcnkem.com

[U67] PHP：处理文件上传
来源：http://fex.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aae.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://bnn.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wkv.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://eyh.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xvl.yongpay.top

[U70] PHP：PDO 事务
来源：http://bqv.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://psy.yj202588.top

[U71] PHP：抛出异常
来源：http://nqb.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://zfv.shzxlz.cn

[U72] PHP：写错误日志
来源：http://aoy.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://igr.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://lpe.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://hyi.fehbvm.com

[U74] PHP：读取环境变量
来源：http://nqj.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://udg.yueranfly.top

[U75] PHP：依赖注入
来源：http://hzf.guowangkeji.top

composer require psr/container
来源：http://plc.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://aez.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tzi.hesvh.cn

[U77] PHP：模板渲染
来源：http://yaj.hysaishi.cn

composer require twig/twig
来源：http://hbp.shuidangran.top

[U78] PHP：单元测试
来源：http://gll.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://cpf.zhengqikj.top

[U79] PHP：静态分析
来源：http://yan.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://xhx.ydzc1.top

[U80] PHP：代码规范修复
来源：http://lqv.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xts.zhixingplan.top

[U81] JS：初始化项目
来源：http://ica.chenzaomai.com

npm init -y;  npm i express
来源：http://kex.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://jrv.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://apu.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://rtk.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://nco.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://cww.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nru.shuidangran.top

[U85] JS：可选链
来源：http://xqv.shuidangran.top

a?.b?.c
来源：http://dch.quarkkingdee.top

[U86] JS：空值合并
来源：http://lwo.0kj1m.cn

a ?? b
来源：http://wnv.epnwcf.com

[U87] JS：解构默认值
来源：http://dec.fktsv.cn

const { a = 1, b = 2 } = obj;
来源：http://ici.jqgufenzy.top

[U88] JS：对象展开合并
来源：http://sve.birdmap.top

{ ...a, ...b }
来源：http://has.xuanzx.com

[U89] JS：数组去重
来源：http://ley.yj20258888.top

[...new Set(arr)]
来源：http://psj.birdmap.top

[U90] JS：数字数组排序
来源：http://gbw.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://vls.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://kme.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ddi.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://rtl.zhoulong.xyz

structuredClone(obj)
来源：http://lhi.cqqwz.cn

[U93] JS：模板字符串
来源：http://sdz.zdqjudy.top

`共 ${n} 条`
来源：http://bmt.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://ceo.aizwys.cn

const double = x => x * 2;
来源：http://qed.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://luy.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://mxq.yvedp.cn

[U96] JS：async/await 与异常
来源：http://klt.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kaz.cheryme.top

[U97] JS：并发请求
来源：http://wao.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://epi.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://ukl.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hxk.vehdjk.com

[U99] JS：事件监听
来源：http://kcd.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://mff.c1oappe.top

[U100] JS：DOM 查询
来源：http://mee.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://pix.jyoumei.cn

[U101] JS：classList 操作
来源：http://zdu.hywenlv.cn

el.classList.toggle("active")
来源：http://zaf.haohaochexian.top

[U102] JS：本地存储
来源：http://zud.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://htx.hesvh.cn

[U103] JS：定时器
来源：http://uxf.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yvm.fktsv.cn

[U104] JS：防抖
来源：http://kzo.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jel.daxiang520.top

[U105] JS：节流
来源：http://rxr.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rdj.gzhubu.top

[U106] JS：日期格式化
来源：http://uou.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dtj.quarkkingdee.top

[U107] JS：数字千分位
来源：http://ogj.jyoumei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fgs.0kj1m.cn

[U108] JS：随机整数
来源：http://woq.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ywo.52xcode.cn

[U109] JS：数组分组
来源：http://hkm.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://okz.yongpay.top

[U110] JS：数组分块
来源：http://oai.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rrw.tianlin.xyz

[U111] JS：对象转 Map
来源：http://qaj.daxiang520.top

new Map(Object.entries(obj))
来源：http://tky.yj20258888.top

[U112] JS：字符串补位
来源：http://vaj.zdqjudy.top

"7".padStart(3, "0")
来源：http://wra.fzhhl.top

[U113] JS：正则替换全部
来源：http://oqf.shzxlz.cn

s.replaceAll("a", "b")
来源：http://nev.yvedp.cn

[U114] JS：JSON 深比较
来源：http://egq.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cxy.gotoacloud.top

[U115] JS：生成 UUID
来源：http://jqy.fanxiaobao.xyz

crypto.randomUUID()
来源：http://ukq.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://kbn.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://zsk.ppjwa.cn

[U117] JS：单元测试
来源：http://kbf.daria6918.cn

npm i -D vitest;  npx vitest
来源：http://emg.yongpay.top

[U118] JS：开发服务器
来源：http://mjn.svipenyu.cn

npm i -D vite;  npx vite
来源：http://lco.kuanghao11.cn

[U119] JS：生产构建
来源：http://rcv.hammf.cn

npx vite build
来源：http://hcx.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://hlb.svipenyu.cn

import.meta.env.VITE_API_URL
来源：http://prm.fzhhl.top

================================================================================
来源：http://mnh.sxryk.cn

统计汇总
来源：http://mnn.ywan-chungtsiang.top

================================================================================
来源：http://set.hnxiangtu.top

按语言统计（条）：
来源：http://poz.yueranfly.top

Python ......... 252
来源：http://sgu.snrcjt.cn

PHP ............ 252
来源：http://qwt.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://yfg.snrcjt.cn

TypeScript ..... 212
来源：http://tri.chenjidiqi.icu

Java ........... 212
来源：http://rqb.sxryk.cn

Go ............. 212
来源：http://okz.ppjwa.cn

Ruby ........... 212
来源：http://knd.quarkkingdee.top

C# ............. 212
来源：http://nvb.fehbvm.com

C .............. 30
来源：http://eqy.xuanzx.com

C++ ............ 30
来源：http://xtn.sufxvd.cn

SQL ............ 90
来源：http://hni.ywan-chungtsiang.top

Bash ........... 80
来源：http://hxc.sjlbkw.cn

Kotlin ......... 15
来源：http://vyn.jqgfzy.top

Swift .......... 15
来源：http://axw.xinyue.icu

Lua ............ 10
来源：http://xmp.yfazqb.com

Perl ........... 10
来源：http://tbz.nwbrower.top

Scala .......... 10
来源：http://lcv.cucudq.cn

------------------------------------
来源：http://htd.fengsongda.top

合计 ........... 2106 条
来源：http://tiz.snrcjt.cn

按章节统计：
来源：http://zce.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wrq.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zxw.fanxiaobao.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lfy.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lmf.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dlk.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gnr.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yor.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hnd.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wfi.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dqn.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://npg.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xjb.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ikl.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ndf.pycfn.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pjp.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qcf.fktsv.cn

Q SQL 专题                              90
来源：http://yjy.jqgfzy.top

R Bash 专题                             80
来源：http://elk.sweek.top

S C / C++ 专题                          60
来源：http://boc.feifeiyinyue.top

T 其他语言补充                          60
来源：http://hrv.52xcode.cn

U 高频实用片段                         120
来源：http://fzw.ctjpmb.com

------------------------------------
来源：http://xom.smart0.xyz

合计                                  2106 条
来源：http://zuj.shuidangran.top

--------------------------------------------------------------------------------
来源：http://gqh.chenlongwang.top

使用提醒
来源：http://eii.uphjek.com

--------------------------------------------------------------------------------
来源：http://itw.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qvp.hysaishi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jjs.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fic.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://avy.316326.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qkf.wangdashe.top

—— 文件结束 ——
来源：http://nxo.quarkkingdee.top

================================================================================
来源：http://qrd.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://cqn.yj202588.top

Common Programming Examples Cheat Book
来源：http://cxx.nanxinkj.top

================================================================================
来源：http://nft.fengsongda.top

【收录内容】
来源：http://cth.yvedp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yry.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ftb.dashuyun.cn

SQL · Bash · C · C++
来源：http://ctn.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jlg.ivvv.top

【使用说明】
来源：http://ejv.chenlongwang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hby.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dvk.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sgq.uphjek.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cep.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://avp.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://szb.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zzu.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vgs.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cwv.xingfuxueyuan.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uyp.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uci.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tso.ywan-chungtsiang.top

【文件统计】
来源：http://kua.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://irf.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://las.shangyingyoupin.top

目  录
来源：http://lsh.yueranfly.top

--------------------------------------------------------------------------------
来源：http://pfb.yangfankeji.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fuf.fengsongda.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hha.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wep.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xue.quarkkingdee.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rdc.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ftl.uphjek.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sze.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hbl.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kma.xylfe.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kwb.andypj.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://epq.tianlin.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kuu.dianchejie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://scl.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gfo.svipenyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jhd.gogol.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fso.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fhg.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://ake.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lno.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kpl.cdnleiting.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zvx.chenjidiqi.icu

================================================================================
来源：http://ldm.nwbrower.top

A. 基础语法与类型
来源：http://wwm.jinghuilouyu.cn

================================================================================
来源：http://cch.bbcook.cn

[A01] Hello World
来源：http://nbf.aibaodan.cn

Py:   print("Hello, World!")
来源：http://vop.yanxiufei.cn

PHP:  echo "Hello, World!";
来源：http://eiv.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://nms.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://krn.shzxlz.cn

Java: System.out.println("Hello, World!");
来源：http://ife.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://dei.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://tud.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xar.jyoumei.cn

[A02] 变量声明与赋值
来源：http://qey.daria6918.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zrw.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bcb.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://knq.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ldl.yj20258.top

Java: String name = "Alex"; int age = 20;
来源：http://qtv.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://bcl.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://rkq.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://rty.andypj.xyz

[A03] 常量定义
来源：http://slg.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gxn.mhx1999.top

PHP:  const PI = 3.14159;
来源：http://mwf.ybcxt.top

JS:   const PI = 3.14159;
来源：http://lld.zhengqikj.top

TS:   const PI: number = 3.14159;
来源：http://yxs.yueranfly.top

Java: static final double PI = 3.14159;
来源：http://vqg.gaohongyu789.top

Go:   const PI = 3.14159
来源：http://mof.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://asx.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://wyn.iojbl.cn

[A04] 判断变量类型
来源：http://feh.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://dkc.zhengqikj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iul.ehwqpu.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://axp.zdbjq.cn

TS:   typeof x; x instanceof Date
来源：http://mmk.xylfe.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gdn.svipenyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mrk.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://htj.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://byj.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://yex.chenlongwang.top


<!-- 参考信息 -->