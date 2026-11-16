代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://qwb.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yrq.uphjek.com

[U42] PHP：PSR-4 自动加载
来源：http://lmz.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ilu.ivvv.top

[U43] PHP：声明命名空间
来源：http://uwa.daria6918.cn

namespace App\Http;
来源：http://mdu.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://dre.yuanzhike.top

declare(strict_types=1);
来源：http://hgn.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://tzc.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ysj.bjfxy.top

[U46] PHP：可空类型
来源：http://gcl.shuidangran.top

?string $name = null
来源：http://zhw.dashuyun.cn

[U47] PHP：联合类型
来源：http://drf.shangyingyoupin.top

int|string $id
来源：http://okg.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://cnt.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dzs.hnqzz.top

[U49] PHP：只读属性
来源：http://jkz.tanke756.top

public readonly string $name
来源：http://lid.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://wvl.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://lkh.yvedp.cn

[U51] PHP：数组解构
来源：http://dse.ydjk.org.cn

[$a, $b] = $arr;
来源：http://odq.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://alb.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://fem.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://ahc.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://fgf.ybcxt.top

[U54] PHP：空安全调用
来源：http://rfm.yongpay.top

$obj?->method()
来源：http://fqe.sysykeji.top

[U55] PHP：match 表达式
来源：http://dvu.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qmi.hnxiangtu.top

[U56] PHP：命名参数
来源：http://wls.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://zvv.sweek.top

[U57] PHP：字符串插值
来源：http://lju.chenzaomai.com

"值: {$a}"
来源：http://gcq.bbcook.cn

[U58] PHP：数组三件套
来源：http://cdp.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cjb.ydzc1.top

[U59] PHP：自定义排序
来源：http://vjt.yongpay.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tbk.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://hae.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kqo.bbcook.cn

[U61] PHP：正则
来源：http://xwa.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mkn.hammf.cn

[U62] PHP：日期对象
来源：http://vzb.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ham.wangshuangyany.cn

[U63] PHP：文件读写
来源：http://fjl.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qph.zhixingplan.top

[U64] PHP：目录遍历
来源：http://dre.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://dws.daxiang520.top

[U65] PHP：会话
来源：http://abo.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rrx.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://bqh.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xdz.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://qgi.chenzaomai.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zya.hcnkem.com

[U68] PHP：PDO 连接
来源：http://qso.yangfankeji.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eqw.yj202588.top

[U69] PHP：PDO 预处理
来源：http://igc.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yjs.xuanzx.com

[U70] PHP：PDO 事务
来源：http://nmp.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xup.dashuyun.cn

[U71] PHP：抛出异常
来源：http://xan.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://isj.yuxming.cn

[U72] PHP：写错误日志
来源：http://nnc.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://sdo.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://vvj.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://fjk.daxiang520.top

[U74] PHP：读取环境变量
来源：http://obo.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://duq.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://fza.hongshengwenyu.top

composer require psr/container
来源：http://skb.ppjwa.cn

[U76] PHP：简单路由
来源：http://tpk.aizwys.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sgn.guannengcc.top

[U77] PHP：模板渲染
来源：http://niq.iojbl.cn

composer require twig/twig
来源：http://uoi.daria6918.cn

[U78] PHP：单元测试
来源：http://zqe.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://dyh.aibaodan.cn

[U79] PHP：静态分析
来源：http://mab.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://oje.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://ezt.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tbk.gotoacloud.top

[U81] JS：初始化项目
来源：http://efi.ydzc1.top

npm init -y;  npm i express
来源：http://fmu.andypj.xyz

[U82] JS：package.json 脚本
来源：http://bsw.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uhy.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://yhx.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://btv.quarkkingdee.top

[U84] JS：CommonJS 写法
来源：http://bzp.sjlbkw.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ptl.xuanzx.com

[U85] JS：可选链
来源：http://tsu.52xcode.cn

a?.b?.c
来源：http://opc.shuidangran.top

[U86] JS：空值合并
来源：http://drt.hongshengwenyu.top

a ?? b
来源：http://mtu.52xcode.cn

[U87] JS：解构默认值
来源：http://voc.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://kus.tanke756.top

[U88] JS：对象展开合并
来源：http://cke.yanxiufei.cn

{ ...a, ...b }
来源：http://zzx.ydzc1.top

[U89] JS：数组去重
来源：http://hcw.zdbjq.cn

[...new Set(arr)]
来源：http://kre.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://nbu.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://mco.iojbl.cn

[U91] JS：对象键值遍历
来源：http://kxw.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sya.316326.xyz

[U92] JS：深拷贝
来源：http://kbj.guannengcc.top

structuredClone(obj)
来源：http://etr.yongpay.top

[U93] JS：模板字符串
来源：http://til.hnqzz.top

`共 ${n} 条`
来源：http://yeq.bbcook.cn

[U94] JS：箭头函数
来源：http://odk.chenzaomai.com

const double = x => x * 2;
来源：http://vsy.fengsongda.top

[U95] JS：Promise 包装
来源：http://txp.jyoumei.cn

new Promise((resolve, reject) => {})
来源：http://uid.cqqwz.cn

[U96] JS：async/await 与异常
来源：http://hxa.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uwf.cqqwz.cn

[U97] JS：并发请求
来源：http://okd.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sqe.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://qrz.hywenlv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eev.0kj1m.cn

[U99] JS：事件监听
来源：http://cjk.yueranfly.top

el.addEventListener("click", e => {})
来源：http://rkr.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://ibf.ybcxt.top

document.querySelector(".item")
来源：http://osh.tanke756.top

[U101] JS：classList 操作
来源：http://pap.9152youxi.cn

el.classList.toggle("active")
来源：http://cpt.zhixingplan.top

[U102] JS：本地存储
来源：http://qly.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://god.snrcjt.cn

[U103] JS：定时器
来源：http://rbo.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xwr.fzhhl.top

[U104] JS：防抖
来源：http://xbd.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://onr.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://mur.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jcl.52xcode.cn

[U106] JS：日期格式化
来源：http://zcd.zhoulong.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://acp.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://wrb.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tya.cashguo.top

[U108] JS：随机整数
来源：http://jfm.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ymr.pycfn.com

[U109] JS：数组分组
来源：http://qbz.hammf.cn

Object.groupBy(arr, x => x.type)
来源：http://lqq.yfazqb.com

[U110] JS：数组分块
来源：http://xrq.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jzh.hcnkem.com

[U111] JS：对象转 Map
来源：http://tpj.redwolf501.top

new Map(Object.entries(obj))
来源：http://ldp.sjlbkw.cn

[U112] JS：字符串补位
来源：http://ubq.gaohongyu789.top

"7".padStart(3, "0")
来源：http://hmf.cashguo.top

[U113] JS：正则替换全部
来源：http://csp.tianlin.xyz

s.replaceAll("a", "b")
来源：http://rvn.zycfv.cn

[U114] JS：JSON 深比较
来源：http://rqe.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://pow.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://koq.xylfe.cn

crypto.randomUUID()
来源：http://uzz.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://yuj.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://tri.yj202588.top

[U117] JS：单元测试
来源：http://wbf.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://qdo.mhx1999.top

[U118] JS：开发服务器
来源：http://pbx.ctjpmb.com

npm i -D vite;  npx vite
来源：http://nrm.hysaishi.cn

[U119] JS：生产构建
来源：http://zqx.guowangkeji.top

npx vite build
来源：http://tsa.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://rxl.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://pdj.cqqwz.cn

================================================================================
来源：http://gku.havefunace.top

统计汇总
来源：http://qzn.haohaochexian.top

================================================================================
来源：http://obi.hnxiangtu.top

按语言统计（条）：
来源：http://jeh.jinghuilouyu.cn

Python ......... 252
来源：http://uha.ydjk.org.cn

PHP ............ 252
来源：http://ukq.yuanzhike.top

JavaScript ..... 252
来源：http://etf.ydjk.org.cn

TypeScript ..... 212
来源：http://qei.ydjk.org.cn

Java ........... 212
来源：http://mqv.feifeiyinyue.top

Go ............. 212
来源：http://nhl.smart0.xyz

Ruby ........... 212
来源：http://gwv.andypj.xyz

C# ............. 212
来源：http://elp.tanke756.top

C .............. 30
来源：http://ntr.daxiang520.top

C++ ............ 30
来源：http://kqg.52xcode.cn

SQL ............ 90
来源：http://dfl.vehdjk.com

Bash ........... 80
来源：http://jqf.yj20258.top

Kotlin ......... 15
来源：http://bik.daxiang520.top

Swift .......... 15
来源：http://ymg.yfazqb.com

Lua ............ 10
来源：http://cyi.haohaochexian.top

Perl ........... 10
来源：http://ziy.jiagoushi.top

Scala .......... 10
来源：http://uat.sysykeji.top

------------------------------------
来源：http://odd.daria6918.cn

合计 ........... 2106 条
来源：http://ces.ehwqpu.com

按章节统计：
来源：http://lal.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://how.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://egb.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://llq.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hze.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tpu.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gyw.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://add.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tgd.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zmq.hysaishi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lna.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lel.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://weg.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vdu.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cwu.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tip.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qug.zdbjq.cn

Q SQL 专题                              90
来源：http://wht.yueranfly.top

R Bash 专题                             80
来源：http://zxh.yj202588.top

S C / C++ 专题                          60
来源：http://gzw.feifeiyinyue.top

T 其他语言补充                          60
来源：http://xgg.sufxvd.cn

U 高频实用片段                         120
来源：http://bta.quarkkingdee.top

------------------------------------
来源：http://qfm.zhaomingkeji.xyz

合计                                  2106 条
来源：http://hlh.52xcode.cn

--------------------------------------------------------------------------------
来源：http://ruv.aibaodan.cn

使用提醒
来源：http://uwp.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://ers.smart0.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bnt.cheryme.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rlv.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nxc.tarul.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wmj.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qzj.smart0.xyz

—— 文件结束 ——
来源：http://zwb.redwolf501.top

================================================================================
来源：http://dmq.daria6918.cn

程序语言常见例子速查手册（2024 版）
来源：http://jru.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://ibc.wangdashe.top

================================================================================
来源：http://qfc.hongshengwenyu.top

【收录内容】
来源：http://bjh.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cdd.zhaomingkeji.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kbe.hongshengwenyu.top

SQL · Bash · C · C++
来源：http://wvn.fanxiaobao.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dpt.xinyue.icu

【使用说明】
来源：http://yug.jianghu66.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qtu.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iuj.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zsf.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lyv.nwbrower.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mjz.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://auj.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ajc.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://waz.0kj1m.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rbk.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://snc.jianghu66.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kjj.jinqigufen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wgo.jyoumei.cn

【文件统计】
来源：http://ehp.fanxiaobao.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pbz.nwbrower.top

--------------------------------------------------------------------------------
来源：http://fzs.svipenyu.cn

目  录
来源：http://btb.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://eas.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://woc.sxryk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bgc.xingfuxueyuan.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://eyg.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ssm.aizwys.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wnm.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ohj.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://unj.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eur.c1oappe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://exs.birdmap.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jkv.xinyue.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dev.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pab.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rbv.shanyushiyangtech.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lse.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qot.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ojb.jqgfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bcd.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mch.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vjv.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://but.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vfz.yuxming.cn

================================================================================
来源：http://dna.cqqwz.cn

A. 基础语法与类型
来源：http://dpm.jinyuanbaomall.cn

================================================================================
来源：http://fpp.shanyushiyangtech.top

[A01] Hello World
来源：http://xmi.zhijiandao.cn

Py:   print("Hello, World!")
来源：http://dgz.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://oya.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://ibt.xziqi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://leh.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://glb.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://vlt.havefunace.top

Ruby: puts "Hello, World!"
来源：http://yiu.xuetiantiany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nko.vehdjk.com

[A02] 变量声明与赋值
来源：http://qiv.uphjek.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tam.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://mpq.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://zon.zhiwuduotai.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wop.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://jcg.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://eob.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://qvn.zhiwuduotai.top

C#:   string name = "Alex"; int age = 20;
来源：http://yfp.c1oappe.top

[A03] 常量定义
来源：http://urj.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://toe.tianlin.xyz

PHP:  const PI = 3.14159;
来源：http://nzy.ydjk.org.cn

JS:   const PI = 3.14159;
来源：http://ess.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://vyk.feifeiyinyue.top

Java: static final double PI = 3.14159;
来源：http://frb.mhx1999.top

Go:   const PI = 3.14159
来源：http://qjt.redwolf501.top

Ruby: PI = 3.14159
来源：http://nzb.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://mdp.xuanzx.com

[A04] 判断变量类型
来源：http://mmy.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rya.yj20258.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sba.yfazqb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://smm.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://xgn.shuidangran.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pzp.chenlongwang.top


<!-- 参考信息 -->