代发 wailian999

[U37] Py：读写 Excel
来源：http://qam.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://kxp.sweek.top

[U38] Py：获取脚本所在目录
来源：http://lbt.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://dfr.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://bnw.gaohongyu789.top

sys.stdout.isatty()
来源：http://dxv.xylfe.cn

[U40] Py：打印到标准错误
来源：http://ssr.zhixingplan.top

print("err", file=sys.stderr)
来源：http://byz.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://ntg.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kgd.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://bng.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lhz.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://vaz.hcnkem.com

namespace App\Http;
来源：http://dti.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://woc.sufxvd.cn

declare(strict_types=1);
来源：http://agj.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://mbp.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sct.smart0.xyz

[U46] PHP：可空类型
来源：http://xut.cdnleiting.top

?string $name = null
来源：http://bws.hesvh.cn

[U47] PHP：联合类型
来源：http://kio.pycfn.com

int|string $id
来源：http://yld.zhengqikj.top

[U48] PHP：纯枚举
来源：http://tbg.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://suo.gaohongyu789.top

[U49] PHP：只读属性
来源：http://but.nwbrower.top

public readonly string $name
来源：http://hqf.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://lrd.tarul.cn

public function __construct(private int $id) {}
来源：http://ygs.nwbrower.top

[U51] PHP：数组解构
来源：http://wcm.gogol.net.cn

[$a, $b] = $arr;
来源：http://sjg.ppjwa.cn

[U52] PHP：箭头函数
来源：http://yyw.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://dqs.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://djy.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://myi.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://bki.fanxiaobao.xyz

$obj?->method()
来源：http://bjp.shuidangran.top

[U55] PHP：match 表达式
来源：http://qpl.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vom.uphjek.com

[U56] PHP：命名参数
来源：http://lwr.sysykeji.top

f(a: 1, b: 2)
来源：http://ipd.chenzaomai.com

[U57] PHP：字符串插值
来源：http://saw.pengpengdd.cyou

"值: {$a}"
来源：http://jmw.shzxlz.cn

[U58] PHP：数组三件套
来源：http://hxr.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pda.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://udl.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wpy.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://nmy.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tuj.cdnleiting.top

[U61] PHP：正则
来源：http://vsv.shanyushiyangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jxu.daria6918.cn

[U62] PHP：日期对象
来源：http://udg.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ynv.0kj1m.cn

[U63] PHP：文件读写
来源：http://qfp.jlsjyb.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ocr.ehwqpu.com

[U64] PHP：目录遍历
来源：http://ivs.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://jhb.guowangkeji.top

[U65] PHP：会话
来源：http://kxl.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pqy.hammf.cn

[U66] PHP：设置 Cookie
来源：http://upl.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mar.cashguo.top

[U67] PHP：处理文件上传
来源：http://key.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zal.bbcook.cn

[U68] PHP：PDO 连接
来源：http://zxf.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://avz.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://wlw.jlsjyb.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dur.andypj.xyz

[U70] PHP：PDO 事务
来源：http://vpr.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://adj.chenlongwang.top

[U71] PHP：抛出异常
来源：http://zel.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://gdr.fzhhl.top

[U72] PHP：写错误日志
来源：http://lmu.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://sjz.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://ejy.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://hor.wangdashe.top

[U74] PHP：读取环境变量
来源：http://wpf.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://aot.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://xzb.zhoulong.xyz

composer require psr/container
来源：http://nkn.dashuyun.cn

[U76] PHP：简单路由
来源：http://yjj.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cjp.jqgfzy.top

[U77] PHP：模板渲染
来源：http://pgj.dashuyun.cn

composer require twig/twig
来源：http://brc.ppjwa.cn

[U78] PHP：单元测试
来源：http://gpy.havefunace.top

composer require --dev phpunit/phpunit
来源：http://wfg.birdmap.top

[U79] PHP：静态分析
来源：http://uja.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://ohm.pycfn.com

[U80] PHP：代码规范修复
来源：http://rqe.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ozn.zhixingplan.top

[U81] JS：初始化项目
来源：http://ixw.sweek.top

npm init -y;  npm i express
来源：http://ftt.meibo888.top

[U82] JS：package.json 脚本
来源：http://yzi.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oam.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://ucz.xingfuxueyuan.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://uty.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://csj.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://buq.xinyue.icu

[U85] JS：可选链
来源：http://xpj.hfpthk.cn

a?.b?.c
来源：http://tkr.yj20258.top

[U86] JS：空值合并
来源：http://kzm.jinqigfzy.top

a ?? b
来源：http://sqj.havefunace.top

[U87] JS：解构默认值
来源：http://bgp.9152youxi.cn

const { a = 1, b = 2 } = obj;
来源：http://mlh.shuidangran.top

[U88] JS：对象展开合并
来源：http://nvw.hongshengwenyu.top

{ ...a, ...b }
来源：http://jyo.jiagoushi.top

[U89] JS：数组去重
来源：http://lqe.ctjpmb.com

[...new Set(arr)]
来源：http://obv.vehdjk.com

[U90] JS：数字数组排序
来源：http://fsk.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://utf.yongpay.top

[U91] JS：对象键值遍历
来源：http://uzq.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vrq.chenjidiqi.icu

[U92] JS：深拷贝
来源：http://nmt.jinqigfzy.top

structuredClone(obj)
来源：http://mpb.9152youxi.cn

[U93] JS：模板字符串
来源：http://mxd.yangfankeji.com

`共 ${n} 条`
来源：http://ohi.9152youxi.cn

[U94] JS：箭头函数
来源：http://jia.tanke756.top

const double = x => x * 2;
来源：http://rfs.snrcjt.cn

[U95] JS：Promise 包装
来源：http://ucd.yueranfly.top

new Promise((resolve, reject) => {})
来源：http://huu.bjfxy.top

[U96] JS：async/await 与异常
来源：http://iek.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://apx.ybcxt.top

[U97] JS：并发请求
来源：http://yzn.yfazqb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://vdb.tianlin.xyz

[U98] JS：fetch 带 JSON
来源：http://mii.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xoq.tianlin.xyz

[U99] JS：事件监听
来源：http://voz.mhx1999.top

el.addEventListener("click", e => {})
来源：http://mii.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://hse.yj20258.top

document.querySelector(".item")
来源：http://qpm.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://rrs.snrcjt.cn

el.classList.toggle("active")
来源：http://ids.tian-w.cn

[U102] JS：本地存储
来源：http://zfz.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tvh.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://zbh.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jvz.ydzc1.top

[U104] JS：防抖
来源：http://dfb.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nkl.jinqigfzy.top

[U105] JS：节流
来源：http://hbh.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vua.nanxuanxn.top

[U106] JS：日期格式化
来源：http://pqj.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xms.jqgufenzy.top

[U107] JS：数字千分位
来源：http://xxa.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ity.sufxvd.cn

[U108] JS：随机整数
来源：http://vzp.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rea.xziqi.cn

[U109] JS：数组分组
来源：http://jlq.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://uys.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://nxk.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nbg.yj202588.top

[U111] JS：对象转 Map
来源：http://lsa.chenzaomai.com

new Map(Object.entries(obj))
来源：http://wiq.andypj.xyz

[U112] JS：字符串补位
来源：http://rfg.xziqi.cn

"7".padStart(3, "0")
来源：http://xop.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://icm.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://uvh.jianghu66.top

[U114] JS：JSON 深比较
来源：http://uce.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nix.sysykeji.top

[U115] JS：生成 UUID
来源：http://ygg.zhiwuduotai.top

crypto.randomUUID()
来源：http://llh.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://rab.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://lxh.tian-w.cn

[U117] JS：单元测试
来源：http://cbd.birdmap.top

npm i -D vitest;  npx vitest
来源：http://ero.ivvv.top

[U118] JS：开发服务器
来源：http://oxr.yuxming.cn

npm i -D vite;  npx vite
来源：http://puh.zdbjq.cn

[U119] JS：生产构建
来源：http://ule.hesvh.cn

npx vite build
来源：http://ktu.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://gfa.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://huf.bjfxy.top

================================================================================
来源：http://szg.feifeiyinyue.top

统计汇总
来源：http://rhw.yueranfly.top

================================================================================
来源：http://ydf.yanxiufei.cn

按语言统计（条）：
来源：http://ehi.xuetiantiany.cn

Python ......... 252
来源：http://vpx.dashuyun.cn

PHP ............ 252
来源：http://qvv.yj20258.top

JavaScript ..... 252
来源：http://wto.xuetiantiany.cn

TypeScript ..... 212
来源：http://yzv.yfazqb.com

Java ........... 212
来源：http://cic.jyoumei.cn

Go ............. 212
来源：http://gga.yuanzhike.top

Ruby ........... 212
来源：http://lyd.yj20258888.top

C# ............. 212
来源：http://rld.sjlbkw.cn

C .............. 30
来源：http://svn.redwolf501.top

C++ ............ 30
来源：http://mbk.zhaomingkeji.xyz

SQL ............ 90
来源：http://vjx.chenzaomai.com

Bash ........... 80
来源：http://gnx.ehwqpu.com

Kotlin ......... 15
来源：http://xby.sysykeji.top

Swift .......... 15
来源：http://pie.jiagoushi.top

Lua ............ 10
来源：http://hwn.chenjidiqi.icu

Perl ........... 10
来源：http://rjs.fehbvm.com

Scala .......... 10
来源：http://deh.feifeiyinyue.top

------------------------------------
来源：http://abh.cheryme.top

合计 ........... 2106 条
来源：http://geg.fanxiaobao.xyz

按章节统计：
来源：http://wxf.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fss.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yot.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wkx.ydjk.org.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pqt.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uvk.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xfj.fanxiaobao.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cri.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lba.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xwa.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bxl.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gvt.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://aki.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uzw.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pxb.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gum.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nrz.haohaochexian.top

Q SQL 专题                              90
来源：http://kmq.sxryk.cn

R Bash 专题                             80
来源：http://ozr.zycfv.cn

S C / C++ 专题                          60
来源：http://uco.ybcxt.top

T 其他语言补充                          60
来源：http://vfw.sweek.top

U 高频实用片段                         120
来源：http://elb.jinyuanbaomall.cn

------------------------------------
来源：http://nxn.aibaodan.cn

合计                                  2106 条
来源：http://ryb.hesvh.cn

--------------------------------------------------------------------------------
来源：http://ylx.hongshengwenyu.top

使用提醒
来源：http://hxm.52xcode.cn

--------------------------------------------------------------------------------
来源：http://orx.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jbg.yuxming.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eeq.zdqjudy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rsf.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://its.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iez.yanxiufei.cn

—— 文件结束 ——
来源：http://whi.jyoumei.cn

================================================================================
来源：http://ifr.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://vuu.316326.xyz

Common Programming Examples Cheat Book
来源：http://txo.daxiang520.top

================================================================================
来源：http://frw.aizwys.cn

【收录内容】
来源：http://kqt.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jxv.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hap.zhijiandao.cn

SQL · Bash · C · C++
来源：http://mpg.shzxlz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uqj.shanyushiyangkeji.top

【使用说明】
来源：http://cjo.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gzj.fengsongda.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://prj.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lho.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bos.c1oappe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bmb.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uvh.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ifc.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zxz.zdqjudy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wzs.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ltk.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pnz.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ujf.0kj1m.cn

【文件统计】
来源：http://zyp.hammf.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dqh.tian-w.cn

--------------------------------------------------------------------------------
来源：http://dad.c1oappe.top

目  录
来源：http://roc.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://gpe.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yxs.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ten.sysykeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lbp.snrcjt.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hyb.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fbi.dashuyun.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rcy.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zdd.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qvh.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kcq.zhijiandao.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mho.fktsv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vyr.ivvv.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oos.wangdashe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fic.yj20258888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sru.smart0.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hmd.jyoumei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gdi.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bgn.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kyn.chenlongwang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lxj.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://het.sjlbkw.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wvf.zhongyouzk.top

================================================================================
来源：http://cpj.cashguo.top

A. 基础语法与类型
来源：http://vsb.gogol.net.cn

================================================================================
来源：http://sgq.vqdsnc.cn

[A01] Hello World
来源：http://ynp.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://rxx.cheryme.top

PHP:  echo "Hello, World!";
来源：http://pzu.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://fup.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ulc.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://jqj.hnxiangtu.top

Go:   fmt.Println("Hello, World!")
来源：http://dqo.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://ini.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://yze.nwbrower.top

[A02] 变量声明与赋值
来源：http://tzv.snrcjt.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wlw.jinyuanbaomall.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pqr.cdnleiting.top

JS:   let name = "Alex"; const age = 20;
来源：http://mrt.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cwx.cucudq.cn

Java: String name = "Alex"; int age = 20;
来源：http://ljk.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://xyw.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://szd.zdbjq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pzj.hesvh.cn

[A03] 常量定义
来源：http://ipj.dashuyun.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ett.sxryk.cn

PHP:  const PI = 3.14159;
来源：http://rid.fanxiaobao.xyz

JS:   const PI = 3.14159;
来源：http://joe.cheryme.top

TS:   const PI: number = 3.14159;
来源：http://pjb.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://sdi.fehbvm.com

Go:   const PI = 3.14159
来源：http://dvk.chenzaomai.com


<!-- 参考信息 -->