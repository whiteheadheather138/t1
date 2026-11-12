代发 wailian999

[U37] Py：读写 Excel
来源：http://obc.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://zdx.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://ydb.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://dyx.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://xmw.vqdsnc.cn

sys.stdout.isatty()
来源：http://qcw.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://iol.uphjek.com

print("err", file=sys.stderr)
来源：http://zug.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://tkg.yueranfly.top

composer init;  composer require guzzlehttp/guzzle
来源：http://duh.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://nhn.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qte.cucudq.cn

[U43] PHP：声明命名空间
来源：http://gfi.zhoulong.xyz

namespace App\Http;
来源：http://inv.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://pgd.meibo888.top

declare(strict_types=1);
来源：http://udd.hfpthk.cn

[U45] PHP：类型声明与返回类型
来源：http://iqw.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bqn.yonumen.top

[U46] PHP：可空类型
来源：http://hwu.hcnkem.com

?string $name = null
来源：http://kzj.havefunace.top

[U47] PHP：联合类型
来源：http://dgi.hammf.cn

int|string $id
来源：http://jao.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://qfn.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sbk.ppjwa.cn

[U49] PHP：只读属性
来源：http://fnw.chenlongwang.top

public readonly string $name
来源：http://opx.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://rrd.fanxiaobao.xyz

public function __construct(private int $id) {}
来源：http://sij.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://ogq.vqdsnc.cn

[$a, $b] = $arr;
来源：http://fsu.nanxinkj.top

[U52] PHP：箭头函数
来源：http://fdu.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://bxz.jianghu66.top

[U53] PHP：空合并运算符
来源：http://kfl.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://xxv.jqgfzy.top

[U54] PHP：空安全调用
来源：http://oat.chenlongwang.top

$obj?->method()
来源：http://cyl.yonumen.top

[U55] PHP：match 表达式
来源：http://lbi.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zbr.smart0.xyz

[U56] PHP：命名参数
来源：http://aoq.zhijiandao.cn

f(a: 1, b: 2)
来源：http://zci.vehdjk.com

[U57] PHP：字符串插值
来源：http://nsw.ydjk.org.cn

"值: {$a}"
来源：http://bkd.cashguo.top

[U58] PHP：数组三件套
来源：http://zva.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hmc.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://osr.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wpf.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://uvg.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ilk.dashuyun.cn

[U61] PHP：正则
来源：http://hyn.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://alo.shuidangran.top

[U62] PHP：日期对象
来源：http://cgl.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uqk.hnxiangtu.top

[U63] PHP：文件读写
来源：http://eqq.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qac.dianchejie.cn

[U64] PHP：目录遍历
来源：http://epb.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://clp.birdmap.top

[U65] PHP：会话
来源：http://vnf.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lyz.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://wew.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://udf.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://mcw.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xmv.gzhubu.top

[U68] PHP：PDO 连接
来源：http://uyo.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sxk.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://pzn.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fqf.guowangkeji.top

[U70] PHP：PDO 事务
来源：http://qzi.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eif.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://xwu.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://kxy.nwbrower.top

[U72] PHP：写错误日志
来源：http://efe.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://ykw.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://let.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://tbf.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://jbp.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://rxz.snrcjt.cn

[U75] PHP：依赖注入
来源：http://efl.haohaochexian.top

composer require psr/container
来源：http://cho.zhixingplan.top

[U76] PHP：简单路由
来源：http://dcu.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://brc.cashguo.top

[U77] PHP：模板渲染
来源：http://bcd.hnqzz.top

composer require twig/twig
来源：http://gvj.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://tay.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://ypl.yj202588.top

[U79] PHP：静态分析
来源：http://xlx.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://osf.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://biw.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rmy.9152youxi.cn

[U81] JS：初始化项目
来源：http://sbp.sweek.top

npm init -y;  npm i express
来源：http://yot.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://irf.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cgh.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://fdg.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://bzk.ydzc1.top

[U84] JS：CommonJS 写法
来源：http://jbr.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://imf.sweek.top

[U85] JS：可选链
来源：http://eee.birdmap.top

a?.b?.c
来源：http://teo.ydjk.org.cn

[U86] JS：空值合并
来源：http://fua.iojbl.cn

a ?? b
来源：http://uvl.zdqjudy.top

[U87] JS：解构默认值
来源：http://efi.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://xke.hnqzz.top

[U88] JS：对象展开合并
来源：http://szk.hnxiangtu.top

{ ...a, ...b }
来源：http://jlk.316326.xyz

[U89] JS：数组去重
来源：http://lln.yj20258.top

[...new Set(arr)]
来源：http://nrv.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://nil.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://eai.guannengcc.top

[U91] JS：对象键值遍历
来源：http://fhc.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qhh.sxryk.cn

[U92] JS：深拷贝
来源：http://cxa.zhixingplan.top

structuredClone(obj)
来源：http://bht.cashguo.top

[U93] JS：模板字符串
来源：http://obp.jlsjyb.cn

`共 ${n} 条`
来源：http://qzp.vqdsnc.cn

[U94] JS：箭头函数
来源：http://fih.ydzc1.top

const double = x => x * 2;
来源：http://eam.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://qsf.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://dns.cashguo.top

[U96] JS：async/await 与异常
来源：http://eop.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jai.jlsjyb.cn

[U97] JS：并发请求
来源：http://oxr.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hgj.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://pwb.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wyk.hnxiangtu.top

[U99] JS：事件监听
来源：http://yxo.sweek.top

el.addEventListener("click", e => {})
来源：http://mnm.dashuyun.cn

[U100] JS：DOM 查询
来源：http://iow.redwolf501.top

document.querySelector(".item")
来源：http://ywr.cheryme.top

[U101] JS：classList 操作
来源：http://lxc.zdqjudy.top

el.classList.toggle("active")
来源：http://gfz.pycfn.com

[U102] JS：本地存储
来源：http://orj.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oah.fehbvm.com

[U103] JS：定时器
来源：http://dav.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nvz.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://jau.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pmp.shanyushiyangtech.top

[U105] JS：节流
来源：http://awk.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jax.9152youxi.cn

[U106] JS：日期格式化
来源：http://rop.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mdc.daxiang520.top

[U107] JS：数字千分位
来源：http://qmb.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nmy.yj20258888.top

[U108] JS：随机整数
来源：http://ffu.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mio.zhoulong.xyz

[U109] JS：数组分组
来源：http://tqb.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://evt.uphjek.com

[U110] JS：数组分块
来源：http://tzt.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fuc.gogol.net.cn

[U111] JS：对象转 Map
来源：http://rxo.hfpthk.cn

new Map(Object.entries(obj))
来源：http://gop.0kj1m.cn

[U112] JS：字符串补位
来源：http://hov.316326.xyz

"7".padStart(3, "0")
来源：http://iot.nanxinkj.top

[U113] JS：正则替换全部
来源：http://oqn.dashuyun.cn

s.replaceAll("a", "b")
来源：http://vwl.52xcode.cn

[U114] JS：JSON 深比较
来源：http://kpg.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lij.tarul.cn

[U115] JS：生成 UUID
来源：http://mcj.fzhhl.top

crypto.randomUUID()
来源：http://ctp.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://fep.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://oto.jqgfzy.top

[U117] JS：单元测试
来源：http://bly.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://auw.redwolf501.top

[U118] JS：开发服务器
来源：http://chr.nwbrower.top

npm i -D vite;  npx vite
来源：http://nqc.zdbjq.cn

[U119] JS：生产构建
来源：http://zye.ydjk.org.cn

npx vite build
来源：http://nqd.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://lvw.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://oxc.jlsjyb.cn

================================================================================
来源：http://xhq.yj20258888.top

统计汇总
来源：http://tle.yuanzhike.top

================================================================================
来源：http://guv.epnwcf.com

按语言统计（条）：
来源：http://cif.zdbjq.cn

Python ......... 252
来源：http://bhh.wangdashe.top

PHP ............ 252
来源：http://zog.jyoumei.cn

JavaScript ..... 252
来源：http://gvh.quarkkingdee.top

TypeScript ..... 212
来源：http://qzh.cqqwz.cn

Java ........... 212
来源：http://uit.guowangkeji.top

Go ............. 212
来源：http://ctr.vehdjk.com

Ruby ........... 212
来源：http://ona.hammf.cn

C# ............. 212
来源：http://xwv.xinyue.icu

C .............. 30
来源：http://wxg.hysaishi.cn

C++ ............ 30
来源：http://ocs.tian-w.cn

SQL ............ 90
来源：http://vxv.cheryme.top

Bash ........... 80
来源：http://arg.52xcode.cn

Kotlin ......... 15
来源：http://qpl.fktsv.cn

Swift .......... 15
来源：http://bej.cdnleiting.top

Lua ............ 10
来源：http://ufa.dianchejie.cn

Perl ........... 10
来源：http://fsk.cdnleiting.top

Scala .......... 10
来源：http://nwn.fktsv.cn

------------------------------------
来源：http://smb.cucudq.cn

合计 ........... 2106 条
来源：http://mil.zhiwuduotai.top

按章节统计：
来源：http://vtl.gaohongyu789.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bxr.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oms.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gfx.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://drz.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://njq.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qom.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pfb.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jad.zdqjudy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nxr.jianghu66.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wcp.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rvs.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ovr.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hzt.uphjek.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aap.ydzc1.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://csa.nwbrower.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gtw.zhixingplan.top

Q SQL 专题                              90
来源：http://hyz.daria6918.cn

R Bash 专题                             80
来源：http://kub.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://mqi.zhaomingkeji.xyz

T 其他语言补充                          60
来源：http://qfh.shanyushiyangtech.top

U 高频实用片段                         120
来源：http://oes.zycfv.cn

------------------------------------
来源：http://fce.nanxinkj.top

合计                                  2106 条
来源：http://fti.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://kel.vehdjk.com

使用提醒
来源：http://vwk.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://vvp.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fxe.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ckw.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oqm.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gav.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gsn.jianghu66.top

—— 文件结束 ——
来源：http://dub.feifeiyinyue.top

================================================================================
来源：http://zni.svipenyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://vuc.kuanghao11.cn

Common Programming Examples Cheat Book
来源：http://lvl.52xcode.cn

================================================================================
来源：http://ebk.sxryk.cn

【收录内容】
来源：http://cpz.yanxiufei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gjx.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dmi.jyoumei.cn

SQL · Bash · C · C++
来源：http://hpl.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mbd.cashguo.top

【使用说明】
来源：http://cud.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qna.52xcode.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ovn.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wqm.gogol.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lku.daxiang520.top

Bash:  Shell         C:     C             C++:   C++
来源：http://huq.tarul.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://avo.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zgj.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fmk.zycfv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://arv.nwbrower.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mwt.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://axp.zhengqikj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qmr.yuxming.cn

【文件统计】
来源：http://wyr.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vlm.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://nkw.zhiwuduotai.top

目  录
来源：http://iyu.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://drw.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ooz.zhongyouzk.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uyw.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gkk.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fwm.jlsjyb.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ubf.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wxk.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://seg.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fnp.bbcook.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cla.yueranfly.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://olq.hywenlv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://byc.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nyv.chenjidiqi.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jsp.vehdjk.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://auz.svipenyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lkt.cucudq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fmg.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://upj.fzhhl.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jcc.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wyb.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xlf.xuetiantiany.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gms.sxryk.cn

================================================================================
来源：http://mjo.haohaochexian.top

A. 基础语法与类型
来源：http://wed.tanke756.top

================================================================================
来源：http://wca.snrcjt.cn

[A01] Hello World
来源：http://ifq.wangdashe.top

Py:   print("Hello, World!")
来源：http://xlr.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://aon.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://svg.yj20258.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://faz.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://znu.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://neu.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://dgj.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jri.zdqjudy.top

[A02] 变量声明与赋值
来源：http://mrz.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ugl.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dkc.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uvg.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hid.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://tjt.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://ayj.xuetiantiany.cn

Ruby: name = "Alex"; age = 20
来源：http://axc.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://fwn.ivvv.top

[A03] 常量定义
来源：http://hdb.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tpy.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://uhv.tian-w.cn

JS:   const PI = 3.14159;
来源：http://xdy.shanyushiyangkeji.top

TS:   const PI: number = 3.14159;
来源：http://tio.yfazqb.com

Java: static final double PI = 3.14159;
来源：http://hop.yueranfly.top

Go:   const PI = 3.14159
来源：http://dlo.jianghu66.top


<!-- 参考信息 -->