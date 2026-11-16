代发 wailian999

[U27] Py：异步 HTTP
来源：http://mzp.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://mxf.epnwcf.com

[U28] Py：类型别名
来源：http://ulm.vehdjk.com

UserId = int
来源：http://nwu.jiagoushi.top

[U29] Py：属性校验
来源：http://epl.yueranfly.top

@property 与 @x.setter 配合
来源：http://nbj.sufxvd.cn

[U30] Py：数据类
来源：http://fjy.havefunace.top

@dataclass(slots=True)
来源：http://zsb.ctjpmb.com

[U31] Py：单测
来源：http://lok.svipenyu.cn

python -m pytest -q
来源：http://gdt.hesvh.cn

[U32] Py：代码格式化
来源：http://csz.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://ayj.havefunace.top

[U33] Py：打包发布
来源：http://jfi.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://ldt.jlsjyb.cn

[U34] Py：判断编码
来源：http://wes.yvedp.cn

chardet.detect(raw)
来源：http://bul.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://egv.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fwv.snrcjt.cn

[U36] Py：定时任务
来源：http://zva.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://sgn.gzhubu.top

[U37] Py：读写 Excel
来源：http://vtv.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://czf.sweek.top

[U38] Py：获取脚本所在目录
来源：http://jsi.xziqi.cn

Path(__file__).resolve().parent
来源：http://vhm.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://igm.fzhhl.top

sys.stdout.isatty()
来源：http://eax.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://lov.chenjidiqi.icu

print("err", file=sys.stderr)
来源：http://gzg.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://mqb.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://smr.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://ufp.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nro.yueranfly.top

[U43] PHP：声明命名空间
来源：http://shl.quarkkingdee.top

namespace App\Http;
来源：http://ehw.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://naw.ctjpmb.com

declare(strict_types=1);
来源：http://hyy.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://kba.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://dpa.sweek.top

[U46] PHP：可空类型
来源：http://ylk.zhengqikj.top

?string $name = null
来源：http://qet.gzhubu.top

[U47] PHP：联合类型
来源：http://kgh.quarkkingdee.top

int|string $id
来源：http://izj.zdbjq.cn

[U48] PHP：纯枚举
来源：http://ybm.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wim.ivvv.top

[U49] PHP：只读属性
来源：http://wrf.epnwcf.com

public readonly string $name
来源：http://mwq.iojbl.cn

[U50] PHP：构造器属性提升
来源：http://qtz.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://hwg.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://kmk.fehbvm.com

[$a, $b] = $arr;
来源：http://zkr.svipenyu.cn

[U52] PHP：箭头函数
来源：http://wxp.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://xao.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://cgs.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://cav.hywenlv.cn

[U54] PHP：空安全调用
来源：http://zch.hongshengwenyu.top

$obj?->method()
来源：http://cha.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://lwh.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ofk.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://ebh.hywenlv.cn

f(a: 1, b: 2)
来源：http://two.cucudq.cn

[U57] PHP：字符串插值
来源：http://zmq.jianghu66.top

"值: {$a}"
来源：http://bka.birdmap.top

[U58] PHP：数组三件套
来源：http://ajf.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sot.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://csm.cucudq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fze.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://wcq.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vsu.cheryme.top

[U61] PHP：正则
来源：http://kvu.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oej.yongpay.top

[U62] PHP：日期对象
来源：http://hlp.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xdj.jianghu66.top

[U63] PHP：文件读写
来源：http://uae.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bhc.chenzaomai.com

[U64] PHP：目录遍历
来源：http://itx.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://jhy.hongshengwenyu.top

[U65] PHP：会话
来源：http://xcp.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://srn.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://spk.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aqw.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://xxo.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aca.havefunace.top

[U68] PHP：PDO 连接
来源：http://ewe.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kaq.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://qrp.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fol.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://jvm.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zeg.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://vkf.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://ajl.hesvh.cn

[U72] PHP：写错误日志
来源：http://hsj.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://kwx.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://auw.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://ejd.hammf.cn

[U74] PHP：读取环境变量
来源：http://aus.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://iii.meibo888.top

[U75] PHP：依赖注入
来源：http://nuo.ivvv.top

composer require psr/container
来源：http://swc.yangfankeji.com

[U76] PHP：简单路由
来源：http://dzj.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://itj.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://zfu.jiagoushi.top

composer require twig/twig
来源：http://rnp.snrcjt.cn

[U78] PHP：单元测试
来源：http://dyf.zhijiandao.cn

composer require --dev phpunit/phpunit
来源：http://rnm.yfazqb.com

[U79] PHP：静态分析
来源：http://ehi.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://okr.fktsv.cn

[U80] PHP：代码规范修复
来源：http://qka.dashuyun.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pwu.jianghu66.top

[U81] JS：初始化项目
来源：http://ysb.bjfxy.top

npm init -y;  npm i express
来源：http://qcg.ivvv.top

[U82] JS：package.json 脚本
来源：http://yaq.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://veg.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://lhr.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://gdb.xinyue.icu

[U84] JS：CommonJS 写法
来源：http://ubs.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://xfs.zhoulong.xyz

[U85] JS：可选链
来源：http://lfg.sjlbkw.cn

a?.b?.c
来源：http://wtp.fzhhl.top

[U86] JS：空值合并
来源：http://ynz.yuxming.cn

a ?? b
来源：http://wzs.redwolf501.top

[U87] JS：解构默认值
来源：http://hcd.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://hxw.snrcjt.cn

[U88] JS：对象展开合并
来源：http://gwh.shzxlz.cn

{ ...a, ...b }
来源：http://jlf.vehdjk.com

[U89] JS：数组去重
来源：http://jgf.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://ape.chenzaomai.com

[U90] JS：数字数组排序
来源：http://llh.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://wck.tanke756.top

[U91] JS：对象键值遍历
来源：http://yoy.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://luw.hywenlv.cn

[U92] JS：深拷贝
来源：http://fzw.xuanzx.com

structuredClone(obj)
来源：http://fmf.9152youxi.cn

[U93] JS：模板字符串
来源：http://nnr.xuanzx.com

`共 ${n} 条`
来源：http://ily.nwbrower.top

[U94] JS：箭头函数
来源：http://xvp.shanyushiyangtech.top

const double = x => x * 2;
来源：http://zpa.nanxinkj.top

[U95] JS：Promise 包装
来源：http://pol.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://cbp.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://rlq.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ubc.52xcode.cn

[U97] JS：并发请求
来源：http://onw.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://igq.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://yzp.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uch.hfpthk.cn

[U99] JS：事件监听
来源：http://laq.ydzc1.top

el.addEventListener("click", e => {})
来源：http://vbt.aizwys.cn

[U100] JS：DOM 查询
来源：http://wij.tianlin.xyz

document.querySelector(".item")
来源：http://fgp.tanke756.top

[U101] JS：classList 操作
来源：http://wwk.xuetiantiany.cn

el.classList.toggle("active")
来源：http://sry.chenlongwang.top

[U102] JS：本地存储
来源：http://aag.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nib.yangfankeji.com

[U103] JS：定时器
来源：http://ebj.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lca.yj20258.top

[U104] JS：防抖
来源：http://svs.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmh.meibo888.top

[U105] JS：节流
来源：http://fyn.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nyc.yonumen.top

[U106] JS：日期格式化
来源：http://mqh.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ool.shuidangran.top

[U107] JS：数字千分位
来源：http://uvc.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pvf.ppjwa.cn

[U108] JS：随机整数
来源：http://jfh.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://riw.fktsv.cn

[U109] JS：数组分组
来源：http://yfa.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://svz.cheryme.top

[U110] JS：数组分块
来源：http://zgc.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ian.pycfn.com

[U111] JS：对象转 Map
来源：http://gfd.sweek.top

new Map(Object.entries(obj))
来源：http://gbl.0kj1m.cn

[U112] JS：字符串补位
来源：http://und.gaohongyu789.top

"7".padStart(3, "0")
来源：http://lev.gzhubu.top

[U113] JS：正则替换全部
来源：http://ntv.mhx1999.top

s.replaceAll("a", "b")
来源：http://qlo.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://crb.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sod.cdnleiting.top

[U115] JS：生成 UUID
来源：http://csl.pycfn.com

crypto.randomUUID()
来源：http://vus.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://ero.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://bmv.zdbjq.cn

[U117] JS：单元测试
来源：http://jke.tanke756.top

npm i -D vitest;  npx vitest
来源：http://ppg.hnxiangtu.top

[U118] JS：开发服务器
来源：http://ivf.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://kau.hcnkem.com

[U119] JS：生产构建
来源：http://uva.0kj1m.cn

npx vite build
来源：http://jau.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://ybu.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://fim.ydjk.org.cn

================================================================================
来源：http://akx.jlsjyb.cn

统计汇总
来源：http://gah.wangdashe.top

================================================================================
来源：http://rdz.yj202588.top

按语言统计（条）：
来源：http://jtq.hnqzz.top

Python ......... 252
来源：http://bzz.daria6918.cn

PHP ............ 252
来源：http://qnv.guowangkeji.top

JavaScript ..... 252
来源：http://iit.tarul.cn

TypeScript ..... 212
来源：http://vrh.guowangkeji.top

Java ........... 212
来源：http://dmv.tarul.cn

Go ............. 212
来源：http://egi.dianchejie.cn

Ruby ........... 212
来源：http://dce.0kj1m.cn

C# ............. 212
来源：http://qau.redwolf501.top

C .............. 30
来源：http://zed.epnwcf.com

C++ ............ 30
来源：http://ycd.tianlin.xyz

SQL ............ 90
来源：http://ccd.shangyingyoupin.top

Bash ........... 80
来源：http://aua.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://nux.iojbl.cn

Swift .......... 15
来源：http://saj.ywan-chungtsiang.top

Lua ............ 10
来源：http://lum.pengpengdd.cyou

Perl ........... 10
来源：http://yfh.vqdsnc.cn

Scala .......... 10
来源：http://oww.52xcode.cn

------------------------------------
来源：http://jnc.zhiwuduotai.top

合计 ........... 2106 条
来源：http://qwz.ehwqpu.com

按章节统计：
来源：http://esx.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uub.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://akx.jinqigufen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://igc.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wcm.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nhy.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fyf.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sub.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lxd.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ltl.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ero.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zzb.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ous.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jlb.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bht.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jxn.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ate.hnqzz.top

Q SQL 专题                              90
来源：http://upv.zhixingplan.top

R Bash 专题                             80
来源：http://xmx.nwbrower.top

S C / C++ 专题                          60
来源：http://gmw.fktsv.cn

T 其他语言补充                          60
来源：http://kud.gzhubu.top

U 高频实用片段                         120
来源：http://vxb.zhaomingkeji.xyz

------------------------------------
来源：http://wfw.shangyingyoupin.top

合计                                  2106 条
来源：http://thy.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://jbi.andypj.xyz

使用提醒
来源：http://opn.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://dwv.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yxw.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ryz.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xmu.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vep.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yvw.xuetiantiany.cn

—— 文件结束 ——
来源：http://dll.fzhhl.top

================================================================================
来源：http://eqh.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://rsr.0kj1m.cn

Common Programming Examples Cheat Book
来源：http://kpm.feifeiyinyue.top

================================================================================
来源：http://ixz.shanyushiyangtech.top

【收录内容】
来源：http://vxv.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://kja.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://obh.xinyue.icu

SQL · Bash · C · C++
来源：http://udi.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eko.hnxiangtu.top

【使用说明】
来源：http://xmk.dianchejie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bcz.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://olv.hnqzz.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nvi.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pxk.nanxuanxn.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vnm.hnxiangtu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zuf.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gnv.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rkq.redwolf501.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mir.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://imx.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ncu.316326.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gly.tian-w.cn

【文件统计】
来源：http://rpu.pengpengdd.cyou

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gcd.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://imv.pycfn.com

目  录
来源：http://odh.jianghu66.top

--------------------------------------------------------------------------------
来源：http://ybk.havefunace.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jwk.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mzh.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jlv.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xop.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hkh.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tem.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zoe.shangyingyoupin.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pwy.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mkc.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jsm.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xtx.chenzaomai.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rde.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dlu.ydzc1.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pcc.fehbvm.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lvt.jinyuanbaomall.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://exo.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nrc.zhiwuduotai.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cnc.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jfu.zhijiandao.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pwx.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rob.wangdashe.top

================================================================================
来源：http://nhg.daxiang520.top

A. 基础语法与类型
来源：http://jys.cashguo.top

================================================================================
来源：http://wgv.hammf.cn

[A01] Hello World
来源：http://fic.ehwqpu.com

Py:   print("Hello, World!")
来源：http://tmh.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://ptt.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://ykb.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yme.fzhhl.top


<!-- 参考信息 -->