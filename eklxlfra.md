代发 wailian999

[U37] Py：读写 Excel
来源：http://zsq.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vmf.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://mrl.tianlin.xyz

Path(__file__).resolve().parent
来源：http://iru.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://ejy.jinqigufen.top

sys.stdout.isatty()
来源：http://ekv.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://nkj.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://vsw.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://glb.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://ayu.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://swe.nanxinkj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dqz.ybcxt.top

[U43] PHP：声明命名空间
来源：http://fcj.mhx1999.top

namespace App\Http;
来源：http://knh.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://jmw.xziqi.cn

declare(strict_types=1);
来源：http://fiw.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://eks.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zwj.sweek.top

[U46] PHP：可空类型
来源：http://ecn.jinqigfzy.top

?string $name = null
来源：http://vnu.tian-w.cn

[U47] PHP：联合类型
来源：http://bqs.yangfankeji.com

int|string $id
来源：http://mde.aizwys.cn

[U48] PHP：纯枚举
来源：http://gwg.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://izr.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://oky.ybcxt.top

public readonly string $name
来源：http://hkw.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://bih.hnqzz.top

public function __construct(private int $id) {}
来源：http://sse.xylfe.cn

[U51] PHP：数组解构
来源：http://kii.epnwcf.com

[$a, $b] = $arr;
来源：http://ebm.mhx1999.top

[U52] PHP：箭头函数
来源：http://plk.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://uqu.andypj.xyz

[U53] PHP：空合并运算符
来源：http://uqb.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://alp.tianlin.xyz

[U54] PHP：空安全调用
来源：http://ciw.zhengqikj.top

$obj?->method()
来源：http://vwr.hnqzz.top

[U55] PHP：match 表达式
来源：http://hzc.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jox.svipenyu.cn

[U56] PHP：命名参数
来源：http://dry.ydjk.org.cn

f(a: 1, b: 2)
来源：http://muh.hammf.cn

[U57] PHP：字符串插值
来源：http://snf.dashuyun.cn

"值: {$a}"
来源：http://ubp.zhongyouzk.top

[U58] PHP：数组三件套
来源：http://nvx.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ats.snrcjt.cn

[U59] PHP：自定义排序
来源：http://hja.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bmd.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://bwf.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lrh.yj20258.top

[U61] PHP：正则
来源：http://phm.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wav.hnqzz.top

[U62] PHP：日期对象
来源：http://fzs.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nxw.chenlongwang.top

[U63] PHP：文件读写
来源：http://sun.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ejy.52xcode.cn

[U64] PHP：目录遍历
来源：http://osx.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://xnd.hysaishi.cn

[U65] PHP：会话
来源：http://leu.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eyu.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://yah.0kj1m.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://swm.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://ooz.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jhp.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://nil.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hmz.tanke756.top

[U69] PHP：PDO 预处理
来源：http://vmu.fktsv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vat.c1oappe.top

[U70] PHP：PDO 事务
来源：http://xgo.hywenlv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qig.gaohongyu789.top

[U71] PHP：抛出异常
来源：http://wbg.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://lok.tian-w.cn

[U72] PHP：写错误日志
来源：http://dtq.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://ojh.52xcode.cn

[U73] PHP：读取 ini 配置
来源：http://uun.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://sds.xylfe.cn

[U74] PHP：读取环境变量
来源：http://dsc.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://ybo.ehwqpu.com

[U75] PHP：依赖注入
来源：http://xjg.dianchejie.cn

composer require psr/container
来源：http://sus.gzhubu.top

[U76] PHP：简单路由
来源：http://zwm.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bjc.sweek.top

[U77] PHP：模板渲染
来源：http://ugw.chenlongwang.top

composer require twig/twig
来源：http://msp.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://abi.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://gij.gzhubu.top

[U79] PHP：静态分析
来源：http://arc.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://amc.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://kpk.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://muq.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://agk.jinqigfzy.top

npm init -y;  npm i express
来源：http://sxt.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://tbc.cucudq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fcw.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://ats.yj20258888.top

export const a = 1;  import { a } from "./m.js";
来源：http://hnw.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://adf.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://yxt.ydzc1.top

[U85] JS：可选链
来源：http://uux.zdqjudy.top

a?.b?.c
来源：http://zmj.0kj1m.cn

[U86] JS：空值合并
来源：http://ium.sxryk.cn

a ?? b
来源：http://kvd.sweek.top

[U87] JS：解构默认值
来源：http://glg.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://gnp.yvedp.cn

[U88] JS：对象展开合并
来源：http://tda.yj20258.top

{ ...a, ...b }
来源：http://iwk.chenlongwang.top

[U89] JS：数组去重
来源：http://pkt.meibo888.top

[...new Set(arr)]
来源：http://uly.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://guo.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://cgd.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://jww.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gvr.zhixingplan.top

[U92] JS：深拷贝
来源：http://fos.fzhhl.top

structuredClone(obj)
来源：http://ngl.mhx1999.top

[U93] JS：模板字符串
来源：http://del.yfazqb.com

`共 ${n} 条`
来源：http://ohw.jlsjyb.cn

[U94] JS：箭头函数
来源：http://vnf.xziqi.cn

const double = x => x * 2;
来源：http://zen.zhixingplan.top

[U95] JS：Promise 包装
来源：http://dbh.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://xkz.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://bwv.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pdh.9152youxi.cn

[U97] JS：并发请求
来源：http://aup.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://azx.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://vxz.hnqzz.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dof.zdqjudy.top

[U99] JS：事件监听
来源：http://udu.sxryk.cn

el.addEventListener("click", e => {})
来源：http://aph.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://pxy.ppjwa.cn

document.querySelector(".item")
来源：http://jet.ybcxt.top

[U101] JS：classList 操作
来源：http://fry.wangdashe.top

el.classList.toggle("active")
来源：http://rgi.shangyingyoupin.top

[U102] JS：本地存储
来源：http://oxq.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://knm.hcnkem.com

[U103] JS：定时器
来源：http://phl.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ifv.yj202588.top

[U104] JS：防抖
来源：http://gfs.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vsj.vqdsnc.cn

[U105] JS：节流
来源：http://iwd.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wnf.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://dcy.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ost.xziqi.cn

[U107] JS：数字千分位
来源：http://ugp.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xef.fktsv.cn

[U108] JS：随机整数
来源：http://gpa.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dcl.pengpengdd.cyou

[U109] JS：数组分组
来源：http://osd.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://ank.sysykeji.top

[U110] JS：数组分块
来源：http://vns.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://slg.ybcxt.top

[U111] JS：对象转 Map
来源：http://xwy.dianchejie.cn

new Map(Object.entries(obj))
来源：http://ruh.jinqigufen.top

[U112] JS：字符串补位
来源：http://sgb.chenlongwang.top

"7".padStart(3, "0")
来源：http://osh.hysaishi.cn

[U113] JS：正则替换全部
来源：http://ubu.smart0.xyz

s.replaceAll("a", "b")
来源：http://qah.wangdashe.top

[U114] JS：JSON 深比较
来源：http://woe.fzhhl.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lxn.ivvv.top

[U115] JS：生成 UUID
来源：http://ahi.yueranfly.top

crypto.randomUUID()
来源：http://zwh.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://pyu.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://tyc.tian-w.cn

[U117] JS：单元测试
来源：http://jvh.yonumen.top

npm i -D vitest;  npx vitest
来源：http://xpc.9152youxi.cn

[U118] JS：开发服务器
来源：http://vdl.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://shs.yanxiufei.cn

[U119] JS：生产构建
来源：http://zon.hysaishi.cn

npx vite build
来源：http://mxy.daria6918.cn

[U120] JS：读取环境变量（Vite）
来源：http://wyg.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://may.zhiwuduotai.top

================================================================================
来源：http://btb.guowangkeji.top

统计汇总
来源：http://dlu.shuidangran.top

================================================================================
来源：http://kup.andypj.xyz

按语言统计（条）：
来源：http://cwh.pycfn.com

Python ......... 252
来源：http://pha.chenzaomai.com

PHP ............ 252
来源：http://xyq.pengpengdd.cyou

JavaScript ..... 252
来源：http://mib.shangyingyoupin.top

TypeScript ..... 212
来源：http://wvd.shanyushiyangtech.top

Java ........... 212
来源：http://evj.fzhhl.top

Go ............. 212
来源：http://gwd.yongpay.top

Ruby ........... 212
来源：http://fbr.hammf.cn

C# ............. 212
来源：http://shf.yuxming.cn

C .............. 30
来源：http://jwr.nwbrower.top

C++ ............ 30
来源：http://ezm.ctjpmb.com

SQL ............ 90
来源：http://ezh.wangdashe.top

Bash ........... 80
来源：http://arc.ivvv.top

Kotlin ......... 15
来源：http://pwj.tian-w.cn

Swift .......... 15
来源：http://vlb.nwbrower.top

Lua ............ 10
来源：http://ixg.zhoulong.xyz

Perl ........... 10
来源：http://upb.tian-w.cn

Scala .......... 10
来源：http://mex.yj20258888.top

------------------------------------
来源：http://drc.ivvv.top

合计 ........... 2106 条
来源：http://xiw.havefunace.top

按章节统计：
来源：http://imf.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sxm.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mzf.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sla.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bvu.ivvv.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fhh.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://opf.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://snb.guannengcc.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kxm.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://apy.tian-w.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nnv.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qik.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://enz.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zdi.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://opn.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hmr.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oju.yfazqb.com

Q SQL 专题                              90
来源：http://tbg.wangdashe.top

R Bash 专题                             80
来源：http://izo.pengpengdd.cyou

S C / C++ 专题                          60
来源：http://rkw.sufxvd.cn

T 其他语言补充                          60
来源：http://wik.birdmap.top

U 高频实用片段                         120
来源：http://pcz.zhoulong.xyz

------------------------------------
来源：http://iil.aizwys.cn

合计                                  2106 条
来源：http://ubi.tanke756.top

--------------------------------------------------------------------------------
来源：http://zid.0kj1m.cn

使用提醒
来源：http://hzk.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://thy.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cmn.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hmw.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nyf.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ymw.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fos.aizwys.cn

—— 文件结束 ——
来源：http://man.xuetiantiany.cn

================================================================================
来源：http://dgi.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://duu.tanke756.top

Common Programming Examples Cheat Book
来源：http://jnr.yongpay.top

================================================================================
来源：http://vdc.chenzaomai.com

【收录内容】
来源：http://sfv.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pfi.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lmi.yvedp.cn

SQL · Bash · C · C++
来源：http://bxu.iojbl.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wcn.shanyushiyangtech.top

【使用说明】
来源：http://ydd.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://orx.zhixingplan.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vzz.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gsk.ydzc1.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cdg.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://icn.9152youxi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ffe.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kin.ivvv.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://opo.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yem.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ykj.0kj1m.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pax.zdqjudy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://krw.yj202588.top

【文件统计】
来源：http://ynb.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://atk.hesvh.cn

--------------------------------------------------------------------------------
来源：http://fxr.havefunace.top

目  录
来源：http://ddh.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://vem.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rnb.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vrq.yonumen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mos.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fnv.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nln.vqdsnc.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oio.mhx1999.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://szr.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ler.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ssk.birdmap.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kdb.zdbjq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bmr.shuidangran.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qzd.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hqz.tianlin.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://evu.haohaochexian.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hhd.mhx1999.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ywk.fehbvm.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jsl.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://kbr.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cft.jyoumei.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ufi.c1oappe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://znn.daria6918.cn

================================================================================
来源：http://yxm.vehdjk.com

A. 基础语法与类型
来源：http://zfh.gaohongyu789.top

================================================================================
来源：http://uwv.daxiang520.top

[A01] Hello World
来源：http://pas.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://vtd.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://htj.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://lqs.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eyp.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://fcv.uphjek.com

Go:   fmt.Println("Hello, World!")
来源：http://txh.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://mlh.nanxuanxn.top

C#:   Console.WriteLine("Hello, World!");
来源：http://srm.cqqwz.cn

[A02] 变量声明与赋值
来源：http://gup.nanxinkj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lok.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cur.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://cwk.svipenyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lhv.hysaishi.cn

Java: String name = "Alex"; int age = 20;
来源：http://eco.nwbrower.top

Go:   name := "Alex"; age := 20
来源：http://buf.iojbl.cn

Ruby: name = "Alex"; age = 20
来源：http://hpi.guannengcc.top

C#:   string name = "Alex"; int age = 20;
来源：http://zev.bjfxy.top

[A03] 常量定义
来源：http://yti.jinqigufen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kvc.ivvv.top

PHP:  const PI = 3.14159;
来源：http://pup.bbcook.cn

JS:   const PI = 3.14159;
来源：http://xkw.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://wgm.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://hcw.hysaishi.cn

Go:   const PI = 3.14159
来源：http://ggk.hnxiangtu.top


<!-- 参考信息 -->