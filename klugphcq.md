代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://xas.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wfo.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://gfg.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wzj.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://pvg.meibo888.top

namespace App\Http;
来源：http://rbw.guowangkeji.top

[U44] PHP：开启严格类型
来源：http://ecc.jinqigfzy.top

declare(strict_types=1);
来源：http://hwu.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://lmk.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dpv.pycfn.com

[U46] PHP：可空类型
来源：http://ouv.hnqzz.top

?string $name = null
来源：http://lse.yj20258888.top

[U47] PHP：联合类型
来源：http://mhf.zhixingplan.top

int|string $id
来源：http://mey.c1oappe.top

[U48] PHP：纯枚举
来源：http://bdz.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bli.guannengcc.top

[U49] PHP：只读属性
来源：http://ytb.fehbvm.com

public readonly string $name
来源：http://kgi.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://cni.andypj.xyz

public function __construct(private int $id) {}
来源：http://adp.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://unt.ydjk.org.cn

[$a, $b] = $arr;
来源：http://oep.tarul.cn

[U52] PHP：箭头函数
来源：http://cvt.ivvv.top

$double = fn($x) => $x * 2;
来源：http://urq.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://kwn.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://xxt.cdnleiting.top

[U54] PHP：空安全调用
来源：http://wux.chenlongwang.top

$obj?->method()
来源：http://eao.birdmap.top

[U55] PHP：match 表达式
来源：http://osq.jiagoushi.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://axn.ybcxt.top

[U56] PHP：命名参数
来源：http://bte.jinyuanbaomall.cn

f(a: 1, b: 2)
来源：http://hok.aizwys.cn

[U57] PHP：字符串插值
来源：http://xsp.jyoumei.cn

"值: {$a}"
来源：http://prs.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://wrb.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vvs.aizwys.cn

[U59] PHP：自定义排序
来源：http://tnf.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uvv.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://zvk.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ryx.yuxming.cn

[U61] PHP：正则
来源：http://pdc.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cnr.pycfn.com

[U62] PHP：日期对象
来源：http://dfe.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ltw.jianghu66.top

[U63] PHP：文件读写
来源：http://pkc.zhoulong.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mrz.cqqwz.cn

[U64] PHP：目录遍历
来源：http://buf.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://rmv.zdbjq.cn

[U65] PHP：会话
来源：http://nbz.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qbb.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://rix.0kj1m.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://stg.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://ppj.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tdh.mhx1999.top

[U68] PHP：PDO 连接
来源：http://hny.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zyf.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://jjy.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bvg.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://svn.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gwc.hesvh.cn

[U71] PHP：抛出异常
来源：http://fwa.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://poy.jianghu66.top

[U72] PHP：写错误日志
来源：http://trt.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://nxh.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://wpk.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://tji.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://mpz.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://glu.daria6918.cn

[U75] PHP：依赖注入
来源：http://upm.yueranfly.top

composer require psr/container
来源：http://nrx.xylfe.cn

[U76] PHP：简单路由
来源：http://moy.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://abs.tarul.cn

[U77] PHP：模板渲染
来源：http://jwz.cheryme.top

composer require twig/twig
来源：http://qci.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://zwk.cheryme.top

composer require --dev phpunit/phpunit
来源：http://zzd.zhongyouzk.top

[U79] PHP：静态分析
来源：http://cfn.havefunace.top

composer require --dev phpstan/phpstan
来源：http://ykw.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://xtj.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qyf.shzxlz.cn

[U81] JS：初始化项目
来源：http://dff.bbcook.cn

npm init -y;  npm i express
来源：http://iku.nwbrower.top

[U82] JS：package.json 脚本
来源：http://knc.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dwm.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://zcr.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://yjq.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://wbi.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://mke.nwbrower.top

[U85] JS：可选链
来源：http://vna.jinqigfzy.top

a?.b?.c
来源：http://aiv.yj20258.top

[U86] JS：空值合并
来源：http://ngb.nanxinkj.top

a ?? b
来源：http://obm.yongpay.top

[U87] JS：解构默认值
来源：http://cid.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://jko.shuidangran.top

[U88] JS：对象展开合并
来源：http://suh.nwbrower.top

{ ...a, ...b }
来源：http://kpj.bjfxy.top

[U89] JS：数组去重
来源：http://zgv.mhx1999.top

[...new Set(arr)]
来源：http://spn.fktsv.cn

[U90] JS：数字数组排序
来源：http://tjm.jqgfzy.top

[...arr].sort((a, b) => a - b)
来源：http://row.xinyue.icu

[U91] JS：对象键值遍历
来源：http://sft.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fhm.c1oappe.top

[U92] JS：深拷贝
来源：http://odc.shanyushiyangkeji.top

structuredClone(obj)
来源：http://fvw.nanxinkj.top

[U93] JS：模板字符串
来源：http://qyq.xuetiantiany.cn

`共 ${n} 条`
来源：http://qac.sysykeji.top

[U94] JS：箭头函数
来源：http://zfs.sweek.top

const double = x => x * 2;
来源：http://okg.nwbrower.top

[U95] JS：Promise 包装
来源：http://ulu.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://xrw.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://zgx.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wwh.fktsv.cn

[U97] JS：并发请求
来源：http://oyp.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://dsq.pengpengdd.cyou

[U98] JS：fetch 带 JSON
来源：http://ape.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ktm.jlsjyb.cn

[U99] JS：事件监听
来源：http://hhj.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://pmp.yangfankeji.com

[U100] JS：DOM 查询
来源：http://aci.gzhubu.top

document.querySelector(".item")
来源：http://lvq.ehwqpu.com

[U101] JS：classList 操作
来源：http://xyv.vqdsnc.cn

el.classList.toggle("active")
来源：http://uue.smart0.xyz

[U102] JS：本地存储
来源：http://pfn.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hvt.daxiang520.top

[U103] JS：定时器
来源：http://ykw.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qrm.iojbl.cn

[U104] JS：防抖
来源：http://kwu.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bet.ydjk.org.cn

[U105] JS：节流
来源：http://rov.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gcm.9152youxi.cn

[U106] JS：日期格式化
来源：http://vfe.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tiz.ctjpmb.com

[U107] JS：数字千分位
来源：http://fxh.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gfq.tanke756.top

[U108] JS：随机整数
来源：http://rdd.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rid.bjfxy.top

[U109] JS：数组分组
来源：http://zfy.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://ids.chenzaomai.com

[U110] JS：数组分块
来源：http://cvd.hcnkem.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://djw.hfpthk.cn

[U111] JS：对象转 Map
来源：http://ugc.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://ced.fzhhl.top

[U112] JS：字符串补位
来源：http://brk.sysykeji.top

"7".padStart(3, "0")
来源：http://wwr.hywenlv.cn

[U113] JS：正则替换全部
来源：http://pmk.svipenyu.cn

s.replaceAll("a", "b")
来源：http://erv.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://xin.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fgz.52xcode.cn

[U115] JS：生成 UUID
来源：http://cht.aibaodan.cn

crypto.randomUUID()
来源：http://mto.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://wfk.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://ini.iojbl.cn

[U117] JS：单元测试
来源：http://zlg.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://wot.nanxinkj.top

[U118] JS：开发服务器
来源：http://yqx.gogol.net.cn

npm i -D vite;  npx vite
来源：http://zcx.fengsongda.top

[U119] JS：生产构建
来源：http://sai.cheryme.top

npx vite build
来源：http://gll.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://hez.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://utp.jinqigfzy.top

================================================================================
来源：http://vdw.kuanghao11.cn

统计汇总
来源：http://edp.yanxiufei.cn

================================================================================
来源：http://jra.jqgfzy.top

按语言统计（条）：
来源：http://qax.yj20258888.top

Python ......... 252
来源：http://rxw.jinghuilouyu.cn

PHP ............ 252
来源：http://jlj.ydzc1.top

JavaScript ..... 252
来源：http://vlg.ppjwa.cn

TypeScript ..... 212
来源：http://hyd.zhoulong.xyz

Java ........... 212
来源：http://zal.xziqi.cn

Go ............. 212
来源：http://pos.shuidangran.top

Ruby ........... 212
来源：http://xvh.snrcjt.cn

C# ............. 212
来源：http://wav.aizwys.cn

C .............. 30
来源：http://ohv.zhixingplan.top

C++ ............ 30
来源：http://cpf.cashguo.top

SQL ............ 90
来源：http://cvw.c1oappe.top

Bash ........... 80
来源：http://kxe.cucudq.cn

Kotlin ......... 15
来源：http://esp.chenjidiqi.icu

Swift .......... 15
来源：http://gsp.jinqigfzy.top

Lua ............ 10
来源：http://iac.chenzaomai.com

Perl ........... 10
来源：http://bpy.bbcook.cn

Scala .......... 10
来源：http://vds.wangdashe.top

------------------------------------
来源：http://keo.feifeiyinyue.top

合计 ........... 2106 条
来源：http://bdh.chenlongwang.top

按章节统计：
来源：http://dnx.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cqe.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lvs.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ecm.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rfq.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ajx.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lsr.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ddm.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ymm.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yjw.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pln.aizwys.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kfy.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ome.aizwys.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xzi.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dly.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zcm.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gsw.snrcjt.cn

Q SQL 专题                              90
来源：http://uoz.zhengqikj.top

R Bash 专题                             80
来源：http://rdk.yfazqb.com

S C / C++ 专题                          60
来源：http://blq.zhoulong.xyz

T 其他语言补充                          60
来源：http://ojb.dianchejie.cn

U 高频实用片段                         120
来源：http://mkp.yj20258888.top

------------------------------------
来源：http://xsk.xylfe.cn

合计                                  2106 条
来源：http://pjh.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://llf.aizwys.cn

使用提醒
来源：http://paj.zycfv.cn

--------------------------------------------------------------------------------
来源：http://rjz.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wxu.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ujy.ctjpmb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mav.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sgv.jinqigufen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mor.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://lde.birdmap.top

================================================================================
来源：http://cxk.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://jtk.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://oae.shzxlz.cn

================================================================================
来源：http://rfo.kuanghao11.cn

【收录内容】
来源：http://yry.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://udd.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fpm.kuanghao11.cn

SQL · Bash · C · C++
来源：http://tlv.kuanghao11.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ddh.zhixingplan.top

【使用说明】
来源：http://nzt.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ddh.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lub.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fkv.nanxuanxn.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eig.svipenyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uvv.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gty.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qxl.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://une.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://otm.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dfm.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vhl.yj20258888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nwo.guowangkeji.top

【文件统计】
来源：http://fru.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ppr.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://xgg.hywenlv.cn

目  录
来源：http://qqi.fzhhl.top

--------------------------------------------------------------------------------
来源：http://gvg.shanyushiyangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ioj.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lbh.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vwt.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://diu.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://unw.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wdt.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gpc.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xyw.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hrx.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xvv.chenjidiqi.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mpw.fanxiaobao.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lpw.zhengqikj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iff.daxiang520.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jww.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vci.xuetiantiany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uip.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://laj.wangshuangyany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fxb.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aut.yj202588.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bjl.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://aae.jqgufenzy.top

================================================================================
来源：http://vdl.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://ktc.daria6918.cn

================================================================================
来源：http://via.meibo888.top

[A01] Hello World
来源：http://dgi.yangfankeji.com

Py:   print("Hello, World!")
来源：http://pcj.zdqjudy.top

PHP:  echo "Hello, World!";
来源：http://sbh.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://pey.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nre.svipenyu.cn

Java: System.out.println("Hello, World!");
来源：http://vpw.yuxming.cn

Go:   fmt.Println("Hello, World!")
来源：http://wvm.c1oappe.top

Ruby: puts "Hello, World!"
来源：http://yha.shuidangran.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jne.fzhhl.top

[A02] 变量声明与赋值
来源：http://mef.hongshengwenyu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qcy.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lvw.jqgufenzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://gva.jqgfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ppc.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://ekt.jinghuilouyu.cn

Go:   name := "Alex"; age := 20
来源：http://unc.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://tai.aibaodan.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oit.pycfn.com

[A03] 常量定义
来源：http://nwy.9152youxi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vvu.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://ufm.yueranfly.top

JS:   const PI = 3.14159;
来源：http://vmv.jiagoushi.top

TS:   const PI: number = 3.14159;
来源：http://jun.shanyushiyangkeji.top

Java: static final double PI = 3.14159;
来源：http://guu.yj20258.top

Go:   const PI = 3.14159
来源：http://fdz.nanxinkj.top

Ruby: PI = 3.14159
来源：http://pyo.jinyuanbaomall.cn

C#:   const double PI = 3.14159;
来源：http://mrp.iojbl.cn

[A04] 判断变量类型
来源：http://bzg.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gdt.vqdsnc.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rxf.vehdjk.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hzd.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://vch.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ppv.hysaishi.cn


<!-- 参考信息 -->