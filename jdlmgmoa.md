代发 wailian999

[U37] Py：读写 Excel
来源：http://dds.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://mbn.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://rct.xuanzx.com

Path(__file__).resolve().parent
来源：http://epu.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://dwj.jqgfzy.top

sys.stdout.isatty()
来源：http://elw.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://gdm.c1oappe.top

print("err", file=sys.stderr)
来源：http://axm.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://vjp.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ain.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://htw.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lrl.epnwcf.com

[U43] PHP：声明命名空间
来源：http://spq.hysaishi.cn

namespace App\Http;
来源：http://wko.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://ugh.vqdsnc.cn

declare(strict_types=1);
来源：http://pzx.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://uxf.haohaochexian.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oox.sweek.top

[U46] PHP：可空类型
来源：http://fhd.birdmap.top

?string $name = null
来源：http://btf.sxryk.cn

[U47] PHP：联合类型
来源：http://ppl.yongpay.top

int|string $id
来源：http://zaj.ivvv.top

[U48] PHP：纯枚举
来源：http://dqu.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://poh.gzhubu.top

[U49] PHP：只读属性
来源：http://jnx.birdmap.top

public readonly string $name
来源：http://zjy.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://wob.cucudq.cn

public function __construct(private int $id) {}
来源：http://ykx.hysaishi.cn

[U51] PHP：数组解构
来源：http://fae.epnwcf.com

[$a, $b] = $arr;
来源：http://eda.aizwys.cn

[U52] PHP：箭头函数
来源：http://zzn.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://ivl.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://acx.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://fsi.yueranfly.top

[U54] PHP：空安全调用
来源：http://jfv.fehbvm.com

$obj?->method()
来源：http://ujp.chenzaomai.com

[U55] PHP：match 表达式
来源：http://aoi.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ngx.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://uqn.9152youxi.cn

f(a: 1, b: 2)
来源：http://chf.hesvh.cn

[U57] PHP：字符串插值
来源：http://wns.fengsongda.top

"值: {$a}"
来源：http://twu.zycfv.cn

[U58] PHP：数组三件套
来源：http://jej.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ngw.guowangkeji.top

[U59] PHP：自定义排序
来源：http://vpq.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://icr.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://jpp.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zzk.guowangkeji.top

[U61] PHP：正则
来源：http://clz.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jbv.zhongyouzk.top

[U62] PHP：日期对象
来源：http://gfo.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oim.zhengqikj.top

[U63] PHP：文件读写
来源：http://oui.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iau.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://fji.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://iam.sufxvd.cn

[U65] PHP：会话
来源：http://joa.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mtw.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://dto.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qve.xuanzx.com

[U67] PHP：处理文件上传
来源：http://ywz.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ixr.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://uai.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zmh.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://vho.redwolf501.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ajz.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://beu.wangdashe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://orj.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://lii.vehdjk.com

throw new RuntimeException("失败", 500);
来源：http://fhi.nwbrower.top

[U72] PHP：写错误日志
来源：http://dou.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://etm.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://kpe.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://ksb.uphjek.com

[U74] PHP：读取环境变量
来源：http://hff.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://ezx.9152youxi.cn

[U75] PHP：依赖注入
来源：http://aux.ybcxt.top

composer require psr/container
来源：http://jny.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://pjl.sweek.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://apj.svipenyu.cn

[U77] PHP：模板渲染
来源：http://soj.sysykeji.top

composer require twig/twig
来源：http://aqt.tian-w.cn

[U78] PHP：单元测试
来源：http://hwu.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://whh.sxryk.cn

[U79] PHP：静态分析
来源：http://imp.aizwys.cn

composer require --dev phpstan/phpstan
来源：http://mea.ybcxt.top

[U80] PHP：代码规范修复
来源：http://sxf.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dyy.zhixingplan.top

[U81] JS：初始化项目
来源：http://qdv.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://azb.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://pbl.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zlq.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://yta.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://zjt.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://efq.birdmap.top

module.exports = { a };  const { a } = require("./m");
来源：http://ihz.aizwys.cn

[U85] JS：可选链
来源：http://wvi.yonumen.top

a?.b?.c
来源：http://seg.hysaishi.cn

[U86] JS：空值合并
来源：http://zqb.zhiwuduotai.top

a ?? b
来源：http://dbv.nwbrower.top

[U87] JS：解构默认值
来源：http://rwx.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://coh.jinqigufen.top

[U88] JS：对象展开合并
来源：http://fcu.cashguo.top

{ ...a, ...b }
来源：http://bfr.wangdashe.top

[U89] JS：数组去重
来源：http://rxe.hongshengwenyu.top

[...new Set(arr)]
来源：http://fdb.hnqzz.top

[U90] JS：数字数组排序
来源：http://qks.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://tud.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://rae.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wnk.pycfn.com

[U92] JS：深拷贝
来源：http://yhu.zycfv.cn

structuredClone(obj)
来源：http://gqg.gogol.net.cn

[U93] JS：模板字符串
来源：http://wme.jiagoushi.top

`共 ${n} 条`
来源：http://quk.ivvv.top

[U94] JS：箭头函数
来源：http://dqo.fanxiaobao.xyz

const double = x => x * 2;
来源：http://oon.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://nwi.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://eby.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://hip.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wro.hysaishi.cn

[U97] JS：并发请求
来源：http://pgs.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fwz.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://yxr.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kyd.zhixingplan.top

[U99] JS：事件监听
来源：http://ynj.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://xzj.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://jdi.shzxlz.cn

document.querySelector(".item")
来源：http://kcw.snrcjt.cn

[U101] JS：classList 操作
来源：http://ypn.nanxuanxn.top

el.classList.toggle("active")
来源：http://vjj.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://vcy.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://omt.sjlbkw.cn

[U103] JS：定时器
来源：http://hkl.jqgufenzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://laq.yangfankeji.com

[U104] JS：防抖
来源：http://rvq.cheryme.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbx.iojbl.cn

[U105] JS：节流
来源：http://ilh.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nef.yuxming.cn

[U106] JS：日期格式化
来源：http://khz.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://akd.yfazqb.com

[U107] JS：数字千分位
来源：http://fyf.cucudq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aqc.aizwys.cn

[U108] JS：随机整数
来源：http://eiy.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xyl.tianlin.xyz

[U109] JS：数组分组
来源：http://ify.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://xia.gogol.net.cn

[U110] JS：数组分块
来源：http://lgt.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vpc.sxryk.cn

[U111] JS：对象转 Map
来源：http://kze.yonumen.top

new Map(Object.entries(obj))
来源：http://ytq.epnwcf.com

[U112] JS：字符串补位
来源：http://ihu.ydjk.org.cn

"7".padStart(3, "0")
来源：http://hkc.ybcxt.top

[U113] JS：正则替换全部
来源：http://kgg.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://bnf.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://ioq.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dik.cqqwz.cn

[U115] JS：生成 UUID
来源：http://qmt.gzhubu.top

crypto.randomUUID()
来源：http://ktd.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://goz.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://sgs.ydzc1.top

[U117] JS：单元测试
来源：http://bee.ybcxt.top

npm i -D vitest;  npx vitest
来源：http://zlj.yvedp.cn

[U118] JS：开发服务器
来源：http://zuu.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://cph.hysaishi.cn

[U119] JS：生产构建
来源：http://hef.9152youxi.cn

npx vite build
来源：http://rcn.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://nfx.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://vga.sweek.top

================================================================================
来源：http://jwh.pengpengdd.cyou

统计汇总
来源：http://yzf.hammf.cn

================================================================================
来源：http://xao.yj202588.top

按语言统计（条）：
来源：http://qay.yonumen.top

Python ......... 252
来源：http://sit.ywan-chungtsiang.top

PHP ............ 252
来源：http://gzf.redwolf501.top

JavaScript ..... 252
来源：http://jdn.zhixingplan.top

TypeScript ..... 212
来源：http://eqk.shzxlz.cn

Java ........... 212
来源：http://ljc.wangshuangyany.cn

Go ............. 212
来源：http://lhz.fengsongda.top

Ruby ........... 212
来源：http://hxq.nanxinkj.top

C# ............. 212
来源：http://wom.cheryme.top

C .............. 30
来源：http://fpi.shanyushiyangtech.top

C++ ............ 30
来源：http://pla.dashuyun.cn

SQL ............ 90
来源：http://chq.hammf.cn

Bash ........... 80
来源：http://gdi.feifeiyinyue.top

Kotlin ......... 15
来源：http://yie.jinqigfzy.top

Swift .......... 15
来源：http://pez.xylfe.cn

Lua ............ 10
来源：http://llk.yj20258888.top

Perl ........... 10
来源：http://ihh.zhongyouzk.top

Scala .......... 10
来源：http://ofu.pycfn.com

------------------------------------
来源：http://yxr.yueranfly.top

合计 ........... 2106 条
来源：http://otl.zhoulong.xyz

按章节统计：
来源：http://uav.mhx1999.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kko.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://syq.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://siy.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mbi.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ppv.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gkp.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dxm.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eev.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://svv.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vbq.cheryme.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yaa.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bde.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tkz.yj202588.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hzy.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kmz.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://buq.cucudq.cn

Q SQL 专题                              90
来源：http://sbq.yanxiufei.cn

R Bash 专题                             80
来源：http://dqd.daxiang520.top

S C / C++ 专题                          60
来源：http://ndg.pengpengdd.cyou

T 其他语言补充                          60
来源：http://mlc.yfazqb.com

U 高频实用片段                         120
来源：http://ytf.birdmap.top

------------------------------------
来源：http://kdj.c1oappe.top

合计                                  2106 条
来源：http://idb.ivvv.top

--------------------------------------------------------------------------------
来源：http://tln.uphjek.com

使用提醒
来源：http://onh.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://zeu.daria6918.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gnu.zdbjq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pvu.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xbg.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oxw.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tcq.xziqi.cn

—— 文件结束 ——
来源：http://cma.316326.xyz

================================================================================
来源：http://bys.316326.xyz

程序语言常见例子速查手册（2024 版）
来源：http://hqm.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://fxr.mhx1999.top

================================================================================
来源：http://hzs.shanyushiyangtech.top

【收录内容】
来源：http://bof.zhixingplan.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vbr.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xrw.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://cds.ppjwa.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://joe.fanxiaobao.xyz

【使用说明】
来源：http://ain.iojbl.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://doh.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vak.jinqigfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pws.9152youxi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jmy.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xwn.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sxe.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ond.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mcv.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ssw.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pvm.aizwys.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ric.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yke.shanyushiyangtech.top

【文件统计】
来源：http://fqy.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iuv.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://khf.dianchejie.cn

目  录
来源：http://nxb.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://bbs.dashuyun.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nlo.cqqwz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tit.xinyue.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qiw.gaohongyu789.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ctp.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vcz.zhixingplan.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kft.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ewf.zhoulong.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vxw.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://boc.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://spe.hywenlv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sxy.hnqzz.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rvi.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lqr.pengpengdd.cyou

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lgp.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vnm.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ofk.hesvh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://txn.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://srl.c1oappe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tvy.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xec.hesvh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xtb.nanxinkj.top

================================================================================
来源：http://zvd.zhongyouzk.top

A. 基础语法与类型
来源：http://foc.bjfxy.top

================================================================================
来源：http://soc.shuidangran.top

[A01] Hello World
来源：http://ozi.fktsv.cn

Py:   print("Hello, World!")
来源：http://gcv.cashguo.top

PHP:  echo "Hello, World!";
来源：http://sxb.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://ftw.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://how.tarul.cn

Java: System.out.println("Hello, World!");
来源：http://mgz.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://lti.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://vwe.yj202588.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lbi.yuanzhike.top

[A02] 变量声明与赋值
来源：http://rcg.gzhubu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qxp.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bed.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://syp.zhoulong.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vjr.jiagoushi.top

Java: String name = "Alex"; int age = 20;
来源：http://ked.ydzc1.top

Go:   name := "Alex"; age := 20
来源：http://dft.9152youxi.cn

Ruby: name = "Alex"; age = 20
来源：http://vxr.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xjt.ywan-chungtsiang.top

[A03] 常量定义
来源：http://qyy.52xcode.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tid.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://spb.haohaochexian.top

JS:   const PI = 3.14159;
来源：http://ejp.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://qve.ehwqpu.com

Java: static final double PI = 3.14159;
来源：http://duo.hcnkem.com

Go:   const PI = 3.14159
来源：http://dlt.meibo888.top


<!-- 参考信息 -->