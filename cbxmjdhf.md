代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://hqb.tian-w.cn

sys.stdout.isatty()
来源：http://ypx.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://rhi.gotoacloud.top

print("err", file=sys.stderr)
来源：http://tkf.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://hhk.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://san.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://fqw.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cvc.wangdashe.top

[U43] PHP：声明命名空间
来源：http://kdl.jyoumei.cn

namespace App\Http;
来源：http://gnx.fengsongda.top

[U44] PHP：开启严格类型
来源：http://pml.shangyingyoupin.top

declare(strict_types=1);
来源：http://jpw.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://ntx.9152youxi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rir.nanxuanxn.top

[U46] PHP：可空类型
来源：http://oxi.zhengqikj.top

?string $name = null
来源：http://ire.andypj.xyz

[U47] PHP：联合类型
来源：http://fdv.hongshengwenyu.top

int|string $id
来源：http://cue.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://gyo.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jmn.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://lho.yangfankeji.com

public readonly string $name
来源：http://qih.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://eto.pycfn.com

public function __construct(private int $id) {}
来源：http://nhf.andypj.xyz

[U51] PHP：数组解构
来源：http://qdo.hfpthk.cn

[$a, $b] = $arr;
来源：http://vsk.yongpay.top

[U52] PHP：箭头函数
来源：http://uhj.epnwcf.com

$double = fn($x) => $x * 2;
来源：http://uhk.hfpthk.cn

[U53] PHP：空合并运算符
来源：http://wpc.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://wpq.wangdashe.top

[U54] PHP：空安全调用
来源：http://tor.pycfn.com

$obj?->method()
来源：http://hil.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://anp.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qtd.bbcook.cn

[U56] PHP：命名参数
来源：http://eir.smart0.xyz

f(a: 1, b: 2)
来源：http://yjc.hywenlv.cn

[U57] PHP：字符串插值
来源：http://eaf.meibo888.top

"值: {$a}"
来源：http://vbs.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://ufj.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qbf.zycfv.cn

[U59] PHP：自定义排序
来源：http://jir.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gzo.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://mmv.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jsg.ybcxt.top

[U61] PHP：正则
来源：http://zyk.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gyk.zhengqikj.top

[U62] PHP：日期对象
来源：http://ozz.aizwys.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://unx.mhx1999.top

[U63] PHP：文件读写
来源：http://zth.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rje.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://xlw.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://ixn.zhijiandao.cn

[U65] PHP：会话
来源：http://ucx.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nqe.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://heb.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kwy.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://gwk.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lhy.yj202588.top

[U68] PHP：PDO 连接
来源：http://epi.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uzz.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://hae.zhongyouzk.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hzz.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://koa.gotoacloud.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kjh.smart0.xyz

[U71] PHP：抛出异常
来源：http://vlx.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://xrj.hesvh.cn

[U72] PHP：写错误日志
来源：http://moi.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://xyx.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://tsx.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://hvp.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://ybo.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://mut.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://axx.hcnkem.com

composer require psr/container
来源：http://lkc.uphjek.com

[U76] PHP：简单路由
来源：http://cso.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://khd.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://xsy.mhx1999.top

composer require twig/twig
来源：http://wiy.yvedp.cn

[U78] PHP：单元测试
来源：http://buh.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://azk.dianchejie.cn

[U79] PHP：静态分析
来源：http://xeo.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://gfe.yonumen.top

[U80] PHP：代码规范修复
来源：http://sfo.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bgv.fktsv.cn

[U81] JS：初始化项目
来源：http://jlg.jiagoushi.top

npm init -y;  npm i express
来源：http://pkp.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://hsw.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hxu.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://upr.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://ayx.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://nkk.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://snb.dianchejie.cn

[U85] JS：可选链
来源：http://pgi.daria6918.cn

a?.b?.c
来源：http://opt.hesvh.cn

[U86] JS：空值合并
来源：http://nip.guannengcc.top

a ?? b
来源：http://zuv.smart0.xyz

[U87] JS：解构默认值
来源：http://qdf.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://zus.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://ffd.shangyingyoupin.top

{ ...a, ...b }
来源：http://ikt.ehwqpu.com

[U89] JS：数组去重
来源：http://rwu.sxryk.cn

[...new Set(arr)]
来源：http://hor.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://zno.havefunace.top

[...arr].sort((a, b) => a - b)
来源：http://icl.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://zby.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ggs.jqgufenzy.top

[U92] JS：深拷贝
来源：http://uar.wangshuangyany.cn

structuredClone(obj)
来源：http://epe.tarul.cn

[U93] JS：模板字符串
来源：http://btp.hammf.cn

`共 ${n} 条`
来源：http://zsg.shzxlz.cn

[U94] JS：箭头函数
来源：http://ttj.havefunace.top

const double = x => x * 2;
来源：http://raj.yuxming.cn

[U95] JS：Promise 包装
来源：http://pda.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://rty.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://top.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eef.fzhhl.top

[U97] JS：并发请求
来源：http://mhm.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://fmp.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://uiz.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bij.hesvh.cn

[U99] JS：事件监听
来源：http://ixu.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://wsp.sjlbkw.cn

[U100] JS：DOM 查询
来源：http://ixf.bjfxy.top

document.querySelector(".item")
来源：http://iis.c1oappe.top

[U101] JS：classList 操作
来源：http://rpw.zhongyouzk.top

el.classList.toggle("active")
来源：http://myo.zhoulong.xyz

[U102] JS：本地存储
来源：http://gpn.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kpc.dashuyun.cn

[U103] JS：定时器
来源：http://udg.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sqs.shangyingyoupin.top

[U104] JS：防抖
来源：http://jfl.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wvd.jlsjyb.cn

[U105] JS：节流
来源：http://lbg.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pdi.cashguo.top

[U106] JS：日期格式化
来源：http://woj.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wjx.cucudq.cn

[U107] JS：数字千分位
来源：http://hco.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mdu.sweek.top

[U108] JS：随机整数
来源：http://hfy.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ggi.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://rmu.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://rcm.iojbl.cn

[U110] JS：数组分块
来源：http://kpo.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kwf.epnwcf.com

[U111] JS：对象转 Map
来源：http://kkz.hnqzz.top

new Map(Object.entries(obj))
来源：http://kwr.tian-w.cn

[U112] JS：字符串补位
来源：http://gmk.xuanzx.com

"7".padStart(3, "0")
来源：http://nur.ppjwa.cn

[U113] JS：正则替换全部
来源：http://lsj.yonumen.top

s.replaceAll("a", "b")
来源：http://jtf.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://lmi.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uqh.hywenlv.cn

[U115] JS：生成 UUID
来源：http://oej.yuanzhike.top

crypto.randomUUID()
来源：http://git.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://gxh.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://ebi.vehdjk.com

[U117] JS：单元测试
来源：http://efo.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://bkk.cucudq.cn

[U118] JS：开发服务器
来源：http://dcx.redwolf501.top

npm i -D vite;  npx vite
来源：http://mzk.jqgufenzy.top

[U119] JS：生产构建
来源：http://qtu.shzxlz.cn

npx vite build
来源：http://fgk.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://xbx.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://lcp.hesvh.cn

================================================================================
来源：http://xjz.epnwcf.com

统计汇总
来源：http://dmw.yangfankeji.com

================================================================================
来源：http://swi.ybcxt.top

按语言统计（条）：
来源：http://aky.9152youxi.cn

Python ......... 252
来源：http://ddl.pengpengdd.cyou

PHP ............ 252
来源：http://lfy.yongpay.top

JavaScript ..... 252
来源：http://mra.sysykeji.top

TypeScript ..... 212
来源：http://shz.dianchejie.cn

Java ........... 212
来源：http://kjl.svipenyu.cn

Go ............. 212
来源：http://eha.vqdsnc.cn

Ruby ........... 212
来源：http://hcv.xuetiantiany.cn

C# ............. 212
来源：http://dsf.0kj1m.cn

C .............. 30
来源：http://sin.ehwqpu.com

C++ ............ 30
来源：http://smu.haohaochexian.top

SQL ............ 90
来源：http://isu.ydjk.org.cn

Bash ........... 80
来源：http://hsz.pengpengdd.cyou

Kotlin ......... 15
来源：http://agt.guowangkeji.top

Swift .......... 15
来源：http://lea.cdnleiting.top

Lua ............ 10
来源：http://ocb.yonumen.top

Perl ........... 10
来源：http://txm.aibaodan.cn

Scala .......... 10
来源：http://jod.sjlbkw.cn

------------------------------------
来源：http://fyt.cqqwz.cn

合计 ........... 2106 条
来源：http://hbl.smart0.xyz

按章节统计：
来源：http://kjj.ivvv.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ele.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ddh.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wqb.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rev.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cic.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pwa.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pif.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jvx.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://apj.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gtk.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oaz.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mbz.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://atw.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cxu.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jkh.xziqi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yif.hywenlv.cn

Q SQL 专题                              90
来源：http://utv.c1oappe.top

R Bash 专题                             80
来源：http://kcm.tian-w.cn

S C / C++ 专题                          60
来源：http://lic.sysykeji.top

T 其他语言补充                          60
来源：http://kaz.jqgufenzy.top

U 高频实用片段                         120
来源：http://ffi.tanke756.top

------------------------------------
来源：http://tzk.xuetiantiany.cn

合计                                  2106 条
来源：http://bil.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://vgw.cheryme.top

使用提醒
来源：http://ezz.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://fwo.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jmf.zhongyouzk.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kjz.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yyd.cdnleiting.top

在旧版本上使用前请先确认语法支持情况。
来源：http://duv.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mak.ydzc1.top

—— 文件结束 ——
来源：http://aro.yonumen.top

================================================================================
来源：http://sps.fktsv.cn

程序语言常见例子速查手册（2024 版）
来源：http://kdc.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://vsr.zhijiandao.cn

================================================================================
来源：http://wkl.bjfxy.top

【收录内容】
来源：http://fog.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dke.yj202588.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wlo.ydzc1.top

SQL · Bash · C · C++
来源：http://lir.jinyuanbaomall.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gra.52xcode.cn

【使用说明】
来源：http://pmg.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jwg.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fzu.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vst.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://emx.hfpthk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sgl.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sal.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://twa.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vok.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ycj.hongshengwenyu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rsp.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qnf.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bkn.zhiwuduotai.top

【文件统计】
来源：http://mht.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wnu.yuxming.cn

--------------------------------------------------------------------------------
来源：http://jmu.birdmap.top

目  录
来源：http://gpb.yueranfly.top

--------------------------------------------------------------------------------
来源：http://gsg.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gob.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yhz.sweek.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cwh.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gxn.zhengqikj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jkt.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lhv.chenjidiqi.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xfd.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kut.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kok.tian-w.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gja.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://znq.jinghuilouyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yuj.kuanghao11.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ldz.jqgfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yhn.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jor.cheryme.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pig.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://frv.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yfr.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qmy.chenjidiqi.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqu.birdmap.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vrh.zhixingplan.top

================================================================================
来源：http://say.uphjek.com

A. 基础语法与类型
来源：http://vlu.yueranfly.top

================================================================================
来源：http://hqi.dianchejie.cn

[A01] Hello World
来源：http://poo.wangshuangyany.cn

Py:   print("Hello, World!")
来源：http://cjy.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://zsm.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://qgd.sysykeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xxc.zhongyouzk.top

Java: System.out.println("Hello, World!");
来源：http://yxs.hfpthk.cn

Go:   fmt.Println("Hello, World!")
来源：http://dda.meibo888.top

Ruby: puts "Hello, World!"
来源：http://che.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://psq.yvedp.cn

[A02] 变量声明与赋值
来源：http://kcy.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mrv.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jkn.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://juj.hfpthk.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fup.pengpengdd.cyou

Java: String name = "Alex"; int age = 20;
来源：http://yrf.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://gnm.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://jza.zhengqikj.top

C#:   string name = "Alex"; int age = 20;
来源：http://heh.jyoumei.cn

[A03] 常量定义
来源：http://kay.hfpthk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://juk.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://sxf.kuanghao11.cn

JS:   const PI = 3.14159;
来源：http://poe.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://cjk.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://hux.yueranfly.top

Go:   const PI = 3.14159
来源：http://qfw.hcnkem.com

Ruby: PI = 3.14159
来源：http://hsd.cashguo.top

C#:   const double PI = 3.14159;
来源：http://jsp.cucudq.cn

[A04] 判断变量类型
来源：http://ebf.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lct.ehwqpu.com


<!-- 参考信息 -->