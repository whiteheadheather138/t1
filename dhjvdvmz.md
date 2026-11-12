代发 wailian999

[U43] PHP：声明命名空间
来源：http://aee.ivvv.top

namespace App\Http;
来源：http://hfd.hnqzz.top

[U44] PHP：开启严格类型
来源：http://joh.yj202588.top

declare(strict_types=1);
来源：http://cig.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://tas.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fyw.yvedp.cn

[U46] PHP：可空类型
来源：http://glk.fehbvm.com

?string $name = null
来源：http://yov.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://cix.hcnkem.com

int|string $id
来源：http://dot.vehdjk.com

[U48] PHP：纯枚举
来源：http://wam.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mke.meibo888.top

[U49] PHP：只读属性
来源：http://lxv.tian-w.cn

public readonly string $name
来源：http://ixw.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://jcw.gzhubu.top

public function __construct(private int $id) {}
来源：http://tgc.yangfankeji.com

[U51] PHP：数组解构
来源：http://mlm.bjfxy.top

[$a, $b] = $arr;
来源：http://drr.xylfe.cn

[U52] PHP：箭头函数
来源：http://too.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://pup.cashguo.top

[U53] PHP：空合并运算符
来源：http://odf.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://iio.cheryme.top

[U54] PHP：空安全调用
来源：http://qks.nanxuanxn.top

$obj?->method()
来源：http://uut.nanxinkj.top

[U55] PHP：match 表达式
来源：http://xwj.ppjwa.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yxp.yuxming.cn

[U56] PHP：命名参数
来源：http://crr.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://ott.0kj1m.cn

[U57] PHP：字符串插值
来源：http://egl.tarul.cn

"值: {$a}"
来源：http://peu.316326.xyz

[U58] PHP：数组三件套
来源：http://tus.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nkb.iojbl.cn

[U59] PHP：自定义排序
来源：http://qlw.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gxv.meibo888.top

[U60] PHP：JSON 编解码
来源：http://mku.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yki.jqgfzy.top

[U61] PHP：正则
来源：http://jvo.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zju.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://uco.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pzi.nwbrower.top

[U63] PHP：文件读写
来源：http://fpv.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lsz.nwbrower.top

[U64] PHP：目录遍历
来源：http://dbi.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://fgm.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://kor.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qwd.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://nyi.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qzs.tian-w.cn

[U67] PHP：处理文件上传
来源：http://fql.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jfu.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://uho.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fxw.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://dgc.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mxu.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://bvq.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://onk.redwolf501.top

[U71] PHP：抛出异常
来源：http://ruu.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://nih.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://xku.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://tbd.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://eiz.feifeiyinyue.top

parse_ini_file("config.ini", true)
来源：http://lko.daria6918.cn

[U74] PHP：读取环境变量
来源：http://frm.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://qig.jyoumei.cn

[U75] PHP：依赖注入
来源：http://kgt.guannengcc.top

composer require psr/container
来源：http://alt.zycfv.cn

[U76] PHP：简单路由
来源：http://smw.pycfn.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vnr.chenlongwang.top

[U77] PHP：模板渲染
来源：http://uej.ivvv.top

composer require twig/twig
来源：http://lvi.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://ati.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://zqg.hnqzz.top

[U79] PHP：静态分析
来源：http://pez.havefunace.top

composer require --dev phpstan/phpstan
来源：http://czc.xuanzx.com

[U80] PHP：代码规范修复
来源：http://mqa.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lge.epnwcf.com

[U81] JS：初始化项目
来源：http://tfn.ydzc1.top

npm init -y;  npm i express
来源：http://emg.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://gwv.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fqs.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://xwo.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bwm.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://cbu.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://ywh.tianlin.xyz

[U85] JS：可选链
来源：http://fvy.fengsongda.top

a?.b?.c
来源：http://qgs.jianghu66.top

[U86] JS：空值合并
来源：http://cau.mhx1999.top

a ?? b
来源：http://yni.ywan-chungtsiang.top

[U87] JS：解构默认值
来源：http://hcc.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://rqq.aizwys.cn

[U88] JS：对象展开合并
来源：http://tie.jianghu66.top

{ ...a, ...b }
来源：http://jlm.ctjpmb.com

[U89] JS：数组去重
来源：http://wbc.ivvv.top

[...new Set(arr)]
来源：http://gdr.hcnkem.com

[U90] JS：数字数组排序
来源：http://kjs.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://nzr.yj20258888.top

[U91] JS：对象键值遍历
来源：http://quy.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yrg.guannengcc.top

[U92] JS：深拷贝
来源：http://qjs.zhoulong.xyz

structuredClone(obj)
来源：http://yag.ydjk.org.cn

[U93] JS：模板字符串
来源：http://pfz.hywenlv.cn

`共 ${n} 条`
来源：http://jct.chenzaomai.com

[U94] JS：箭头函数
来源：http://taa.mhx1999.top

const double = x => x * 2;
来源：http://tnw.svipenyu.cn

[U95] JS：Promise 包装
来源：http://eiu.meibo888.top

new Promise((resolve, reject) => {})
来源：http://mub.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://svr.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zmm.snrcjt.cn

[U97] JS：并发请求
来源：http://mfw.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vai.316326.xyz

[U98] JS：fetch 带 JSON
来源：http://ueh.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wan.yj202588.top

[U99] JS：事件监听
来源：http://qqr.yuxming.cn

el.addEventListener("click", e => {})
来源：http://uii.nwbrower.top

[U100] JS：DOM 查询
来源：http://qbv.c1oappe.top

document.querySelector(".item")
来源：http://ugi.xziqi.cn

[U101] JS：classList 操作
来源：http://vzq.uphjek.com

el.classList.toggle("active")
来源：http://vqt.chenzaomai.com

[U102] JS：本地存储
来源：http://opw.jianghu66.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mdj.sufxvd.cn

[U103] JS：定时器
来源：http://fwq.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uvx.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://zxb.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://prw.sjlbkw.cn

[U105] JS：节流
来源：http://vtm.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ocy.yvedp.cn

[U106] JS：日期格式化
来源：http://ttj.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mbg.yanxiufei.cn

[U107] JS：数字千分位
来源：http://bfq.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bkd.yongpay.top

[U108] JS：随机整数
来源：http://tcy.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ooe.hongshengwenyu.top

[U109] JS：数组分组
来源：http://ssv.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://qvz.fehbvm.com

[U110] JS：数组分块
来源：http://spa.ybcxt.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ciz.havefunace.top

[U111] JS：对象转 Map
来源：http://pdx.shuidangran.top

new Map(Object.entries(obj))
来源：http://dgr.0kj1m.cn

[U112] JS：字符串补位
来源：http://ziu.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://dij.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://nuo.dianchejie.cn

s.replaceAll("a", "b")
来源：http://hog.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://egh.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xly.andypj.xyz

[U115] JS：生成 UUID
来源：http://ngb.epnwcf.com

crypto.randomUUID()
来源：http://xho.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://xdf.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://guf.zdqjudy.top

[U117] JS：单元测试
来源：http://baw.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://clh.tanke756.top

[U118] JS：开发服务器
来源：http://nby.ydzc1.top

npm i -D vite;  npx vite
来源：http://kmw.hnqzz.top

[U119] JS：生产构建
来源：http://cdx.c1oappe.top

npx vite build
来源：http://ksg.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://spp.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://jws.chenjidiqi.icu

================================================================================
来源：http://knf.yj202588.top

统计汇总
来源：http://xaa.cheryme.top

================================================================================
来源：http://hld.cqqwz.cn

按语言统计（条）：
来源：http://gwj.wangshuangyany.cn

Python ......... 252
来源：http://mbn.hywenlv.cn

PHP ............ 252
来源：http://bch.jyoumei.cn

JavaScript ..... 252
来源：http://xxa.zhongyouzk.top

TypeScript ..... 212
来源：http://xwm.gzhubu.top

Java ........... 212
来源：http://zcr.guowangkeji.top

Go ............. 212
来源：http://rri.sysykeji.top

Ruby ........... 212
来源：http://jxf.kuanghao11.cn

C# ............. 212
来源：http://nqt.9152youxi.cn

C .............. 30
来源：http://khv.dashuyun.cn

C++ ............ 30
来源：http://tle.nanxinkj.top

SQL ............ 90
来源：http://lwv.cheryme.top

Bash ........... 80
来源：http://rap.vehdjk.com

Kotlin ......... 15
来源：http://tam.havefunace.top

Swift .......... 15
来源：http://bmm.daxiang520.top

Lua ............ 10
来源：http://alo.nanxinkj.top

Perl ........... 10
来源：http://jjm.snrcjt.cn

Scala .......... 10
来源：http://kib.bbcook.cn

------------------------------------
来源：http://bhk.hnqzz.top

合计 ........... 2106 条
来源：http://fdu.jianghu66.top

按章节统计：
来源：http://dwy.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ysr.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jek.shanyushiyangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eex.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xjr.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mad.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dqa.tian-w.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mgf.tarul.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://czb.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vbr.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fwx.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rie.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uaf.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bov.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qkf.zdbjq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gon.quarkkingdee.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gkh.vehdjk.com

Q SQL 专题                              90
来源：http://nhi.shanyushiyangtech.top

R Bash 专题                             80
来源：http://hxi.yanxiufei.cn

S C / C++ 专题                          60
来源：http://fvu.yanxiufei.cn

T 其他语言补充                          60
来源：http://rpk.fzhhl.top

U 高频实用片段                         120
来源：http://lji.jiagoushi.top

------------------------------------
来源：http://cpv.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://ngw.smart0.xyz

--------------------------------------------------------------------------------
来源：http://yws.xylfe.cn

使用提醒
来源：http://jdr.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://yqi.vehdjk.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zlr.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eyq.yonumen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bui.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://spe.chenlongwang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yzb.jinqigfzy.top

—— 文件结束 ——
来源：http://mce.daria6918.cn

================================================================================
来源：http://xox.cashguo.top

程序语言常见例子速查手册（2024 版）
来源：http://ofl.pycfn.com

Common Programming Examples Cheat Book
来源：http://uem.snrcjt.cn

================================================================================
来源：http://uju.uphjek.com

【收录内容】
来源：http://fkx.cdnleiting.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://aam.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hjd.ydzc1.top

SQL · Bash · C · C++
来源：http://fgu.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tcl.guowangkeji.top

【使用说明】
来源：http://kxw.zhoulong.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bnt.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dex.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gfm.dianchejie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fbr.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ese.ybcxt.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dkh.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lev.yfazqb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ngs.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hqi.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sir.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gnb.shanyushiyangtech.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ksc.epnwcf.com

【文件统计】
来源：http://wcr.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blr.xziqi.cn

--------------------------------------------------------------------------------
来源：http://cfv.jqgfzy.top

目  录
来源：http://ryv.andypj.xyz

--------------------------------------------------------------------------------
来源：http://xqg.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dha.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://orq.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://itj.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rwz.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zlx.cdnleiting.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xoo.yvedp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uyc.shanyushiyangtech.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rjw.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cpb.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://izg.ctjpmb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iyk.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uzg.ehwqpu.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qwg.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://btv.xingfuxueyuan.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cdx.shuidangran.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://toa.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://geu.cheryme.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uyu.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bpw.xuanzx.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qpj.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nsv.ybcxt.top

================================================================================
来源：http://jba.yvedp.cn

A. 基础语法与类型
来源：http://vtv.daria6918.cn

================================================================================
来源：http://jht.chenzaomai.com

[A01] Hello World
来源：http://jjx.tian-w.cn

Py:   print("Hello, World!")
来源：http://nku.xylfe.cn

PHP:  echo "Hello, World!";
来源：http://atu.zhoulong.xyz

JS:   console.log("Hello, World!");
来源：http://xey.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xmk.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://lwr.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://pkq.shzxlz.cn

Ruby: puts "Hello, World!"
来源：http://oyq.shzxlz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zxr.sysykeji.top

[A02] 变量声明与赋值
来源：http://mpv.guowangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://igt.shangyingyoupin.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fsd.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://nqu.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aby.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://nfd.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://mps.jyoumei.cn

Ruby: name = "Alex"; age = 20
来源：http://yml.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zze.zhijiandao.cn

[A03] 常量定义
来源：http://yky.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vhv.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://weu.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://vie.fzhhl.top

TS:   const PI: number = 3.14159;
来源：http://nam.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://umy.nanxuanxn.top

Go:   const PI = 3.14159
来源：http://asc.wangdashe.top

Ruby: PI = 3.14159
来源：http://ypk.sweek.top

C#:   const double PI = 3.14159;
来源：http://ftn.9152youxi.cn

[A04] 判断变量类型
来源：http://aap.gotoacloud.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xjn.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sis.vehdjk.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qhm.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://ots.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wvq.vqdsnc.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pos.xylfe.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ehg.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://dqd.ppjwa.cn

[A05] 整数除法与取模
来源：http://yqf.hcnkem.com


<!-- 参考信息 -->