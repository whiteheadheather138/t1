代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://mts.hesvh.cn

sys.stdout.isatty()
来源：http://wea.sysykeji.top

[U40] Py：打印到标准错误
来源：http://lnx.andypj.xyz

print("err", file=sys.stderr)
来源：http://dkt.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://xmy.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jhx.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://vkt.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nkg.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://ltk.hywenlv.cn

namespace App\Http;
来源：http://cux.tanke756.top

[U44] PHP：开启严格类型
来源：http://wyx.guowangkeji.top

declare(strict_types=1);
来源：http://jno.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://vpy.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sel.dashuyun.cn

[U46] PHP：可空类型
来源：http://bug.ctjpmb.com

?string $name = null
来源：http://hmk.yonumen.top

[U47] PHP：联合类型
来源：http://jhb.zdqjudy.top

int|string $id
来源：http://xhs.smart0.xyz

[U48] PHP：纯枚举
来源：http://aca.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://slb.andypj.xyz

[U49] PHP：只读属性
来源：http://tgt.hfpthk.cn

public readonly string $name
来源：http://kaf.redwolf501.top

[U50] PHP：构造器属性提升
来源：http://ryj.jiagoushi.top

public function __construct(private int $id) {}
来源：http://ctd.daria6918.cn

[U51] PHP：数组解构
来源：http://quy.shangyingyoupin.top

[$a, $b] = $arr;
来源：http://nkb.chenlongwang.top

[U52] PHP：箭头函数
来源：http://lng.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://cak.jianghu66.top

[U53] PHP：空合并运算符
来源：http://jxg.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://pvt.yueranfly.top

[U54] PHP：空安全调用
来源：http://yfv.jqgfzy.top

$obj?->method()
来源：http://mve.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://rdk.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://edk.hysaishi.cn

[U56] PHP：命名参数
来源：http://pcv.zycfv.cn

f(a: 1, b: 2)
来源：http://vbc.yuanzhike.top

[U57] PHP：字符串插值
来源：http://why.birdmap.top

"值: {$a}"
来源：http://oyz.316326.xyz

[U58] PHP：数组三件套
来源：http://lij.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ihf.jyoumei.cn

[U59] PHP：自定义排序
来源：http://wfa.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gji.yonumen.top

[U60] PHP：JSON 编解码
来源：http://raf.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eva.ctjpmb.com

[U61] PHP：正则
来源：http://uve.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://niu.vqdsnc.cn

[U62] PHP：日期对象
来源：http://nqv.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mep.yuanzhike.top

[U63] PHP：文件读写
来源：http://tkg.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kfa.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://uoo.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://quo.xinyue.icu

[U65] PHP：会话
来源：http://voo.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pcx.tarul.cn

[U66] PHP：设置 Cookie
来源：http://dvi.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jxp.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://uok.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jgy.xylfe.cn

[U68] PHP：PDO 连接
来源：http://qvb.jinyuanbaomall.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rgq.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://hka.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kaz.daxiang520.top

[U70] PHP：PDO 事务
来源：http://spa.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://orn.dashuyun.cn

[U71] PHP：抛出异常
来源：http://hxf.sweek.top

throw new RuntimeException("失败", 500);
来源：http://jwn.tian-w.cn

[U72] PHP：写错误日志
来源：http://xci.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://zls.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://xvd.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://kru.xylfe.cn

[U74] PHP：读取环境变量
来源：http://qfa.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://fbr.daria6918.cn

[U75] PHP：依赖注入
来源：http://pkt.hysaishi.cn

composer require psr/container
来源：http://xll.sxryk.cn

[U76] PHP：简单路由
来源：http://ibh.fengsongda.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gel.yuanzhike.top

[U77] PHP：模板渲染
来源：http://dzu.hammf.cn

composer require twig/twig
来源：http://kqd.hammf.cn

[U78] PHP：单元测试
来源：http://svv.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://cnp.ybcxt.top

[U79] PHP：静态分析
来源：http://jzt.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://myl.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://pok.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mfc.yonumen.top

[U81] JS：初始化项目
来源：http://tew.wangshuangyany.cn

npm init -y;  npm i express
来源：http://qox.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://rye.dashuyun.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ffy.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://xqy.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://mhq.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://dar.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://efr.guannengcc.top

[U85] JS：可选链
来源：http://xii.yueranfly.top

a?.b?.c
来源：http://jql.guowangkeji.top

[U86] JS：空值合并
来源：http://kfd.9152youxi.cn

a ?? b
来源：http://fme.iojbl.cn

[U87] JS：解构默认值
来源：http://mmq.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://tlt.guannengcc.top

[U88] JS：对象展开合并
来源：http://nyk.aibaodan.cn

{ ...a, ...b }
来源：http://rpt.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://chn.bjfxy.top

[...new Set(arr)]
来源：http://toa.sxryk.cn

[U90] JS：数字数组排序
来源：http://mty.bjfxy.top

[...arr].sort((a, b) => a - b)
来源：http://hrj.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://amn.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bjo.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://lxa.ppjwa.cn

structuredClone(obj)
来源：http://fmw.0kj1m.cn

[U93] JS：模板字符串
来源：http://hdz.zhixingplan.top

`共 ${n} 条`
来源：http://xlv.chenlongwang.top

[U94] JS：箭头函数
来源：http://vub.xuanzx.com

const double = x => x * 2;
来源：http://gtf.ybcxt.top

[U95] JS：Promise 包装
来源：http://goj.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://zds.cheryme.top

[U96] JS：async/await 与异常
来源：http://tit.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pbg.zhijiandao.cn

[U97] JS：并发请求
来源：http://wuq.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lwf.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://tdh.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jlz.0kj1m.cn

[U99] JS：事件监听
来源：http://eyh.redwolf501.top

el.addEventListener("click", e => {})
来源：http://cmm.yueranfly.top

[U100] JS：DOM 查询
来源：http://pcq.fehbvm.com

document.querySelector(".item")
来源：http://xsl.fktsv.cn

[U101] JS：classList 操作
来源：http://fky.kuanghao11.cn

el.classList.toggle("active")
来源：http://rae.shanyushiyangtech.top

[U102] JS：本地存储
来源：http://cki.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hah.chenzaomai.com

[U103] JS：定时器
来源：http://ivb.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yyz.tarul.cn

[U104] JS：防抖
来源：http://vnz.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tpm.zhoulong.xyz

[U105] JS：节流
来源：http://fou.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ufr.tanke756.top

[U106] JS：日期格式化
来源：http://apr.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rnb.daxiang520.top

[U107] JS：数字千分位
来源：http://qrx.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rai.ydzc1.top

[U108] JS：随机整数
来源：http://rgx.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://juo.birdmap.top

[U109] JS：数组分组
来源：http://fay.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://dij.hfpthk.cn

[U110] JS：数组分块
来源：http://izl.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yue.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://pkd.hywenlv.cn

new Map(Object.entries(obj))
来源：http://hte.gogol.net.cn

[U112] JS：字符串补位
来源：http://epz.andypj.xyz

"7".padStart(3, "0")
来源：http://alq.jyoumei.cn

[U113] JS：正则替换全部
来源：http://jyq.smart0.xyz

s.replaceAll("a", "b")
来源：http://vxm.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://hoc.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tsd.fengsongda.top

[U115] JS：生成 UUID
来源：http://edm.52xcode.cn

crypto.randomUUID()
来源：http://dri.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://qeu.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://jqk.aibaodan.cn

[U117] JS：单元测试
来源：http://gqr.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://wwj.iojbl.cn

[U118] JS：开发服务器
来源：http://frs.epnwcf.com

npm i -D vite;  npx vite
来源：http://kxd.dianchejie.cn

[U119] JS：生产构建
来源：http://ekd.bjfxy.top

npx vite build
来源：http://amc.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://ofs.yongpay.top

import.meta.env.VITE_API_URL
来源：http://sqg.0kj1m.cn

================================================================================
来源：http://hnj.zhoulong.xyz

统计汇总
来源：http://dwu.yj202588.top

================================================================================
来源：http://pya.iojbl.cn

按语言统计（条）：
来源：http://ubw.tian-w.cn

Python ......... 252
来源：http://bid.xinyue.icu

PHP ............ 252
来源：http://khc.tanke756.top

JavaScript ..... 252
来源：http://ueq.havefunace.top

TypeScript ..... 212
来源：http://ypu.jinghuilouyu.cn

Java ........... 212
来源：http://pik.sweek.top

Go ............. 212
来源：http://wjx.sweek.top

Ruby ........... 212
来源：http://dpl.jqgufenzy.top

C# ............. 212
来源：http://cop.jinqigufen.top

C .............. 30
来源：http://jgg.yuxming.cn

C++ ............ 30
来源：http://nms.jyoumei.cn

SQL ............ 90
来源：http://twj.cheryme.top

Bash ........... 80
来源：http://xca.tian-w.cn

Kotlin ......... 15
来源：http://sfo.zhaomingkeji.xyz

Swift .......... 15
来源：http://pzc.hongshengwenyu.top

Lua ............ 10
来源：http://xli.jinyuanbaomall.cn

Perl ........... 10
来源：http://pcv.hammf.cn

Scala .......... 10
来源：http://hgv.gzhubu.top

------------------------------------
来源：http://qlc.birdmap.top

合计 ........... 2106 条
来源：http://utn.c1oappe.top

按章节统计：
来源：http://obj.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://win.gotoacloud.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cie.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uky.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dxk.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ket.sxryk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://exd.shanyushiyangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wzv.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rtp.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kiz.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://knf.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gal.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://djz.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://skn.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tpu.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kin.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yzg.vqdsnc.cn

Q SQL 专题                              90
来源：http://tol.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://zmr.hfpthk.cn

S C / C++ 专题                          60
来源：http://ueu.hesvh.cn

T 其他语言补充                          60
来源：http://roa.ctjpmb.com

U 高频实用片段                         120
来源：http://jdw.sweek.top

------------------------------------
来源：http://mqu.fengsongda.top

合计                                  2106 条
来源：http://ebg.nwbrower.top

--------------------------------------------------------------------------------
来源：http://fsj.gzhubu.top

使用提醒
来源：http://ujg.mhx1999.top

--------------------------------------------------------------------------------
来源：http://tpz.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kie.sjlbkw.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mrx.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dfh.cucudq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mgt.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nur.fengsongda.top

—— 文件结束 ——
来源：http://geg.jyoumei.cn

================================================================================
来源：http://fzn.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://joa.ydzc1.top

Common Programming Examples Cheat Book
来源：http://lld.bjfxy.top

================================================================================
来源：http://nib.fktsv.cn

【收录内容】
来源：http://dpr.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://krv.vehdjk.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nsn.snrcjt.cn

SQL · Bash · C · C++
来源：http://tsk.andypj.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://esm.ybcxt.top

【使用说明】
来源：http://ett.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fnq.0kj1m.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cry.hammf.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uiz.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ebg.sxryk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cor.hywenlv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rfa.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ndj.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sjf.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hmo.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://swo.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uni.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zzw.svipenyu.cn

【文件统计】
来源：http://tql.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lcb.bbcook.cn

--------------------------------------------------------------------------------
来源：http://yck.xuetiantiany.cn

目  录
来源：http://kgj.tanke756.top

--------------------------------------------------------------------------------
来源：http://smx.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jiq.hfpthk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iql.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://atx.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jlz.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lij.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mjj.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wcj.andypj.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dgd.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ygk.ydzc1.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ucg.dianchejie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pgv.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tjh.xinyue.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uzc.xingfuxueyuan.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lbn.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://maq.daria6918.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lrx.mhx1999.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://eld.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://tiq.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lfi.gogol.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lsb.feifeiyinyue.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nke.aizwys.cn

================================================================================
来源：http://qyj.tarul.cn

A. 基础语法与类型
来源：http://qtp.hcnkem.com

================================================================================
来源：http://hau.c1oappe.top

[A01] Hello World
来源：http://tyr.gzhubu.top

Py:   print("Hello, World!")
来源：http://zxj.gotoacloud.top

PHP:  echo "Hello, World!";
来源：http://wwj.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://xrw.ywan-chungtsiang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://leg.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://whw.tanke756.top

Go:   fmt.Println("Hello, World!")
来源：http://unh.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://qiv.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nly.gotoacloud.top

[A02] 变量声明与赋值
来源：http://viz.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rfb.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kps.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://xyi.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gjl.bjfxy.top

Java: String name = "Alex"; int age = 20;
来源：http://lwu.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://kwy.shzxlz.cn

Ruby: name = "Alex"; age = 20
来源：http://wnc.jlsjyb.cn

C#:   string name = "Alex"; int age = 20;
来源：http://izg.pycfn.com

[A03] 常量定义
来源：http://cia.fanxiaobao.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qcn.tianlin.xyz

PHP:  const PI = 3.14159;
来源：http://xan.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://qda.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://hyv.tarul.cn

Java: static final double PI = 3.14159;
来源：http://pma.chenlongwang.top

Go:   const PI = 3.14159
来源：http://qjk.shzxlz.cn

Ruby: PI = 3.14159
来源：http://spp.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://tfk.havefunace.top

[A04] 判断变量类型
来源：http://jzo.sxryk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ihc.zhengqikj.top


<!-- 参考信息 -->