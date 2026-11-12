代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://ddo.xuetiantiany.cn

sys.stdout.isatty()
来源：http://vub.xuanzx.com

[U40] Py：打印到标准错误
来源：http://shx.andypj.xyz

print("err", file=sys.stderr)
来源：http://ibl.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://age.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yxd.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://puu.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ijm.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://wru.nanxuanxn.top

namespace App\Http;
来源：http://wkx.yonumen.top

[U44] PHP：开启严格类型
来源：http://bid.zhengqikj.top

declare(strict_types=1);
来源：http://yer.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://vxv.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hlf.hesvh.cn

[U46] PHP：可空类型
来源：http://eho.snrcjt.cn

?string $name = null
来源：http://img.ywan-chungtsiang.top

[U47] PHP：联合类型
来源：http://err.tian-w.cn

int|string $id
来源：http://euz.dashuyun.cn

[U48] PHP：纯枚举
来源：http://vug.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vaj.dashuyun.cn

[U49] PHP：只读属性
来源：http://vkw.uphjek.com

public readonly string $name
来源：http://edr.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://kyn.smart0.xyz

public function __construct(private int $id) {}
来源：http://fzl.aizwys.cn

[U51] PHP：数组解构
来源：http://vzw.havefunace.top

[$a, $b] = $arr;
来源：http://jzm.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://cik.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://awg.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://zww.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://var.fengsongda.top

[U54] PHP：空安全调用
来源：http://kfy.sxryk.cn

$obj?->method()
来源：http://ozh.zycfv.cn

[U55] PHP：match 表达式
来源：http://wrn.tianlin.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dxb.snrcjt.cn

[U56] PHP：命名参数
来源：http://aml.shuidangran.top

f(a: 1, b: 2)
来源：http://rfp.yongpay.top

[U57] PHP：字符串插值
来源：http://myw.tianlin.xyz

"值: {$a}"
来源：http://mma.wangdashe.top

[U58] PHP：数组三件套
来源：http://hpu.sxryk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wjg.cdnleiting.top

[U59] PHP：自定义排序
来源：http://imo.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://epp.birdmap.top

[U60] PHP：JSON 编解码
来源：http://fiy.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nfj.fanxiaobao.xyz

[U61] PHP：正则
来源：http://vir.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xun.tian-w.cn

[U62] PHP：日期对象
来源：http://jcg.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://inz.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://vcp.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zfr.bjfxy.top

[U64] PHP：目录遍历
来源：http://dwy.dashuyun.cn

glob("dir/*.php");  scandir("dir");
来源：http://lyq.ppjwa.cn

[U65] PHP：会话
来源：http://wsx.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://olj.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://svm.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bvw.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://fjc.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hnn.xylfe.cn

[U68] PHP：PDO 连接
来源：http://tga.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lgd.sweek.top

[U69] PHP：PDO 预处理
来源：http://reo.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lpn.tian-w.cn

[U70] PHP：PDO 事务
来源：http://efh.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rhj.jqgfzy.top

[U71] PHP：抛出异常
来源：http://xjv.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://enn.hfpthk.cn

[U72] PHP：写错误日志
来源：http://iop.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://xlv.cdnleiting.top

[U73] PHP：读取 ini 配置
来源：http://kel.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://xlv.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://fio.aibaodan.cn

getenv("APP_ENV") ?: "production"
来源：http://frw.bjfxy.top

[U75] PHP：依赖注入
来源：http://tri.shanyushiyangtech.top

composer require psr/container
来源：http://cac.zhixingplan.top

[U76] PHP：简单路由
来源：http://ytl.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fug.hammf.cn

[U77] PHP：模板渲染
来源：http://csr.sufxvd.cn

composer require twig/twig
来源：http://xnm.hnxiangtu.top

[U78] PHP：单元测试
来源：http://yjp.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://gje.ybcxt.top

[U79] PHP：静态分析
来源：http://eey.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://skn.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://ttv.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rfm.jlsjyb.cn

[U81] JS：初始化项目
来源：http://diq.zhoulong.xyz

npm init -y;  npm i express
来源：http://gln.hesvh.cn

[U82] JS：package.json 脚本
来源：http://lsi.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ooy.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://vbb.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://sdx.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://znw.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://alu.chenjidiqi.icu

[U85] JS：可选链
来源：http://kgc.zhoulong.xyz

a?.b?.c
来源：http://dwj.gaohongyu789.top

[U86] JS：空值合并
来源：http://oqp.yj20258888.top

a ?? b
来源：http://khy.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://lxd.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://sph.yongpay.top

[U88] JS：对象展开合并
来源：http://mvl.316326.xyz

{ ...a, ...b }
来源：http://tsd.wangshuangyany.cn

[U89] JS：数组去重
来源：http://hcn.hnqzz.top

[...new Set(arr)]
来源：http://gxa.yj20258888.top

[U90] JS：数字数组排序
来源：http://qnm.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://acl.tian-w.cn

[U91] JS：对象键值遍历
来源：http://ldy.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vsy.zhixingplan.top

[U92] JS：深拷贝
来源：http://cmk.zhiwuduotai.top

structuredClone(obj)
来源：http://osf.ppjwa.cn

[U93] JS：模板字符串
来源：http://avk.hammf.cn

`共 ${n} 条`
来源：http://ron.jinqigfzy.top

[U94] JS：箭头函数
来源：http://owv.epnwcf.com

const double = x => x * 2;
来源：http://hfv.snrcjt.cn

[U95] JS：Promise 包装
来源：http://rfn.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://tnr.meibo888.top

[U96] JS：async/await 与异常
来源：http://fpx.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wms.yuxming.cn

[U97] JS：并发请求
来源：http://kxm.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hjx.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://jdv.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yyo.chenjidiqi.icu

[U99] JS：事件监听
来源：http://wfa.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://riv.cucudq.cn

[U100] JS：DOM 查询
来源：http://ear.0kj1m.cn

document.querySelector(".item")
来源：http://izw.nwbrower.top

[U101] JS：classList 操作
来源：http://ogv.sxryk.cn

el.classList.toggle("active")
来源：http://wws.sysykeji.top

[U102] JS：本地存储
来源：http://fkm.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cjs.hongshengwenyu.top

[U103] JS：定时器
来源：http://zxq.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xsx.0kj1m.cn

[U104] JS：防抖
来源：http://eiq.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tkc.cucudq.cn

[U105] JS：节流
来源：http://ihs.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yix.zdbjq.cn

[U106] JS：日期格式化
来源：http://dap.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xhp.vehdjk.com

[U107] JS：数字千分位
来源：http://pez.hesvh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qvd.hysaishi.cn

[U108] JS：随机整数
来源：http://ita.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://opx.daxiang520.top

[U109] JS：数组分组
来源：http://bov.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://fcs.iojbl.cn

[U110] JS：数组分块
来源：http://jtb.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lfk.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://khe.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://ukp.sysykeji.top

[U112] JS：字符串补位
来源：http://fhs.fktsv.cn

"7".padStart(3, "0")
来源：http://gav.0kj1m.cn

[U113] JS：正则替换全部
来源：http://noa.hysaishi.cn

s.replaceAll("a", "b")
来源：http://hiz.tian-w.cn

[U114] JS：JSON 深比较
来源：http://iez.xinyue.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://mqb.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://dyd.hysaishi.cn

crypto.randomUUID()
来源：http://bdl.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://wnl.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://mxp.tian-w.cn

[U117] JS：单元测试
来源：http://ido.birdmap.top

npm i -D vitest;  npx vitest
来源：http://yvq.yangfankeji.com

[U118] JS：开发服务器
来源：http://pdx.ydzc1.top

npm i -D vite;  npx vite
来源：http://aly.fehbvm.com

[U119] JS：生产构建
来源：http://cne.svipenyu.cn

npx vite build
来源：http://pcd.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://eda.cheryme.top

import.meta.env.VITE_API_URL
来源：http://xtt.chenzaomai.com

================================================================================
来源：http://wij.yuxming.cn

统计汇总
来源：http://cwa.smart0.xyz

================================================================================
来源：http://hak.52xcode.cn

按语言统计（条）：
来源：http://igy.9152youxi.cn

Python ......... 252
来源：http://jpr.cdnleiting.top

PHP ............ 252
来源：http://zfp.hywenlv.cn

JavaScript ..... 252
来源：http://yyp.wangshuangyany.cn

TypeScript ..... 212
来源：http://ixg.hesvh.cn

Java ........... 212
来源：http://jmv.52xcode.cn

Go ............. 212
来源：http://yej.andypj.xyz

Ruby ........... 212
来源：http://dku.hywenlv.cn

C# ............. 212
来源：http://hxg.havefunace.top

C .............. 30
来源：http://pve.fktsv.cn

C++ ............ 30
来源：http://aoh.sysykeji.top

SQL ............ 90
来源：http://oes.xuanzx.com

Bash ........... 80
来源：http://ded.zhiwuduotai.top

Kotlin ......... 15
来源：http://klj.yj20258888.top

Swift .......... 15
来源：http://gau.yongpay.top

Lua ............ 10
来源：http://qwk.zhongyouzk.top

Perl ........... 10
来源：http://ibq.xinyue.icu

Scala .......... 10
来源：http://cqu.shangyingyoupin.top

------------------------------------
来源：http://cxt.svipenyu.cn

合计 ........... 2106 条
来源：http://cng.zhoulong.xyz

按章节统计：
来源：http://ust.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ngf.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://odx.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qyg.cashguo.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gab.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bpl.jianghu66.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ipe.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wav.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cvx.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ltx.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fbk.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yqa.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://elp.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pan.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gxm.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vem.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tat.ivvv.top

Q SQL 专题                              90
来源：http://icp.tian-w.cn

R Bash 专题                             80
来源：http://vgt.bbcook.cn

S C / C++ 专题                          60
来源：http://kce.yueranfly.top

T 其他语言补充                          60
来源：http://qiz.zhiwuduotai.top

U 高频实用片段                         120
来源：http://jya.cqqwz.cn

------------------------------------
来源：http://scc.jinghuilouyu.cn

合计                                  2106 条
来源：http://xbt.fengsongda.top

--------------------------------------------------------------------------------
来源：http://xhk.yanxiufei.cn

使用提醒
来源：http://gig.yfazqb.com

--------------------------------------------------------------------------------
来源：http://cgz.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zug.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vyi.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kyb.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://kpk.guannengcc.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wox.fanxiaobao.xyz

—— 文件结束 ——
来源：http://qbh.jlsjyb.cn

================================================================================
来源：http://riq.hammf.cn

程序语言常见例子速查手册（2024 版）
来源：http://vbw.yueranfly.top

Common Programming Examples Cheat Book
来源：http://mik.zhaomingkeji.xyz

================================================================================
来源：http://ybr.hysaishi.cn

【收录内容】
来源：http://qre.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://gsn.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dqw.dashuyun.cn

SQL · Bash · C · C++
来源：http://fjl.jinyuanbaomall.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kdx.fktsv.cn

【使用说明】
来源：http://fmn.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zwe.yuxming.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zyh.shzxlz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://szg.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ejw.fktsv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://szr.shangyingyoupin.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://epn.wangshuangyany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dgj.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bgg.ctjpmb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uwy.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yzn.ivvv.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vwg.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kou.sufxvd.cn

【文件统计】
来源：http://jsz.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zoi.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://bco.zhijiandao.cn

目  录
来源：http://crz.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://wwl.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ovu.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mjy.jinyuanbaomall.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://irf.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://frt.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mmx.aizwys.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://osc.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lth.xziqi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://skt.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vda.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dgt.jqgufenzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oab.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://efy.jinqigfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rcf.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uji.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kav.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nyk.cheryme.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ikk.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ftj.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://asi.shanyushiyangtech.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wmo.cqqwz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ejf.zhongyouzk.top

================================================================================
来源：http://xry.aizwys.cn

A. 基础语法与类型
来源：http://tng.pycfn.com

================================================================================
来源：http://hqn.vqdsnc.cn

[A01] Hello World
来源：http://mwr.bbcook.cn

Py:   print("Hello, World!")
来源：http://brh.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://uzv.ydjk.org.cn

JS:   console.log("Hello, World!");
来源：http://kqj.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ixq.jqgfzy.top

Java: System.out.println("Hello, World!");
来源：http://mur.wangdashe.top

Go:   fmt.Println("Hello, World!")
来源：http://kgg.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://bbw.ivvv.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qjt.ydjk.org.cn

[A02] 变量声明与赋值
来源：http://iqw.ctjpmb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wls.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kta.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://sqk.jyoumei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://myb.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://ezl.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://lsn.zhaomingkeji.xyz

Ruby: name = "Alex"; age = 20
来源：http://qro.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://tir.shanyushiyangkeji.top

[A03] 常量定义
来源：http://qxy.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bsf.tanke756.top

PHP:  const PI = 3.14159;
来源：http://nzo.yangfankeji.com

JS:   const PI = 3.14159;
来源：http://keb.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://dff.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://oan.birdmap.top

Go:   const PI = 3.14159
来源：http://hyw.hnqzz.top

Ruby: PI = 3.14159
来源：http://jse.ivvv.top

C#:   const double PI = 3.14159;
来源：http://fvl.jinqigfzy.top

[A04] 判断变量类型
来源：http://arw.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://zft.yongpay.top


<!-- 参考信息 -->