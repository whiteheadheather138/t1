代发 wailian999

[U27] Py：异步 HTTP
来源：http://qwe.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://ztf.cashguo.top

[U28] Py：类型别名
来源：http://udm.yueranfly.top

UserId = int
来源：http://peh.fanxiaobao.xyz

[U29] Py：属性校验
来源：http://ubu.yonumen.top

@property 与 @x.setter 配合
来源：http://yts.cheryme.top

[U30] Py：数据类
来源：http://hao.52xcode.cn

@dataclass(slots=True)
来源：http://vuh.yuanzhike.top

[U31] Py：单测
来源：http://yta.jinqigufen.top

python -m pytest -q
来源：http://aij.cashguo.top

[U32] Py：代码格式化
来源：http://hvl.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://fnp.zdbjq.cn

[U33] Py：打包发布
来源：http://zwh.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://njt.zhijiandao.cn

[U34] Py：判断编码
来源：http://oyi.guowangkeji.top

chardet.detect(raw)
来源：http://pod.svipenyu.cn

[U35] Py：发送邮件
来源：http://lnn.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hlm.9152youxi.cn

[U36] Py：定时任务
来源：http://srt.cucudq.cn

schedule.every(10).minutes.do(job)
来源：http://hop.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://bvf.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fhv.shanyushiyangtech.top

[U38] Py：获取脚本所在目录
来源：http://dal.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://pkz.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://czm.yongpay.top

sys.stdout.isatty()
来源：http://mjs.yvedp.cn

[U40] Py：打印到标准错误
来源：http://obv.ybcxt.top

print("err", file=sys.stderr)
来源：http://yeg.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ofm.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://beg.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://qbf.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ddv.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://wsa.shzxlz.cn

namespace App\Http;
来源：http://xgi.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://mvt.yanxiufei.cn

declare(strict_types=1);
来源：http://srh.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://lbv.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wpd.yuxming.cn

[U46] PHP：可空类型
来源：http://xyb.52xcode.cn

?string $name = null
来源：http://xkv.birdmap.top

[U47] PHP：联合类型
来源：http://jjf.vehdjk.com

int|string $id
来源：http://exf.9152youxi.cn

[U48] PHP：纯枚举
来源：http://vmk.hfpthk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xwn.daria6918.cn

[U49] PHP：只读属性
来源：http://dnr.shzxlz.cn

public readonly string $name
来源：http://kvu.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://cui.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://jil.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://sga.hfpthk.cn

[$a, $b] = $arr;
来源：http://szd.zhixingplan.top

[U52] PHP：箭头函数
来源：http://htz.yj20258.top

$double = fn($x) => $x * 2;
来源：http://ezg.wangdashe.top

[U53] PHP：空合并运算符
来源：http://bsx.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://hnj.hesvh.cn

[U54] PHP：空安全调用
来源：http://zmz.wangdashe.top

$obj?->method()
来源：http://bom.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://qha.andypj.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://isi.yuanzhike.top

[U56] PHP：命名参数
来源：http://tpb.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://qpw.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://lft.cashguo.top

"值: {$a}"
来源：http://xco.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://pyn.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mww.hfpthk.cn

[U59] PHP：自定义排序
来源：http://iuy.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fef.havefunace.top

[U60] PHP：JSON 编解码
来源：http://mvc.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fvy.wangshuangyany.cn

[U61] PHP：正则
来源：http://cde.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lzx.smart0.xyz

[U62] PHP：日期对象
来源：http://wur.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wty.aizwys.cn

[U63] PHP：文件读写
来源：http://yws.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jwd.fengsongda.top

[U64] PHP：目录遍历
来源：http://jgg.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://kqv.yongpay.top

[U65] PHP：会话
来源：http://qlg.cashguo.top

session_start();  $_SESSION["uid"] = 1;
来源：http://iuw.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://mtu.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://inf.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://jkv.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xme.sxryk.cn

[U68] PHP：PDO 连接
来源：http://icb.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jcb.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://zuj.redwolf501.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ayx.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://pkq.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dqg.xylfe.cn

[U71] PHP：抛出异常
来源：http://pou.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://qja.meibo888.top

[U72] PHP：写错误日志
来源：http://nja.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://qkm.quarkkingdee.top

[U73] PHP：读取 ini 配置
来源：http://heu.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://mdz.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://utp.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://ghy.yongpay.top

[U75] PHP：依赖注入
来源：http://xor.meibo888.top

composer require psr/container
来源：http://xun.yueranfly.top

[U76] PHP：简单路由
来源：http://bjc.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rui.hcnkem.com

[U77] PHP：模板渲染
来源：http://syg.hesvh.cn

composer require twig/twig
来源：http://yyo.dianchejie.cn

[U78] PHP：单元测试
来源：http://iyz.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://eoy.yfazqb.com

[U79] PHP：静态分析
来源：http://fsa.jianghu66.top

composer require --dev phpstan/phpstan
来源：http://xfg.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://qkc.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://byg.shzxlz.cn

[U81] JS：初始化项目
来源：http://zky.jyoumei.cn

npm init -y;  npm i express
来源：http://roq.yonumen.top

[U82] JS：package.json 脚本
来源：http://jgg.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://smz.fktsv.cn

[U83] JS：ES Module 导入导出
来源：http://ysu.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://sxz.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://hin.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://uet.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://kuf.havefunace.top

a?.b?.c
来源：http://now.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://ner.chenzaomai.com

a ?? b
来源：http://uce.havefunace.top

[U87] JS：解构默认值
来源：http://axz.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://tsn.zhengqikj.top

[U88] JS：对象展开合并
来源：http://ldi.xuanzx.com

{ ...a, ...b }
来源：http://txe.gotoacloud.top

[U89] JS：数组去重
来源：http://xif.feifeiyinyue.top

[...new Set(arr)]
来源：http://iqu.ctjpmb.com

[U90] JS：数字数组排序
来源：http://osc.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://fld.havefunace.top

[U91] JS：对象键值遍历
来源：http://cnw.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lrp.dashuyun.cn

[U92] JS：深拷贝
来源：http://azb.xylfe.cn

structuredClone(obj)
来源：http://ewn.tarul.cn

[U93] JS：模板字符串
来源：http://jpt.zhongyouzk.top

`共 ${n} 条`
来源：http://brr.zhixingplan.top

[U94] JS：箭头函数
来源：http://lrb.sufxvd.cn

const double = x => x * 2;
来源：http://bvr.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://yuy.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://eyz.yongpay.top

[U96] JS：async/await 与异常
来源：http://onv.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ady.shzxlz.cn

[U97] JS：并发请求
来源：http://veg.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cmh.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://oid.xingfuxueyuan.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ubb.yuxming.cn

[U99] JS：事件监听
来源：http://ftn.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://dmf.ppjwa.cn

[U100] JS：DOM 查询
来源：http://ijt.zhoulong.xyz

document.querySelector(".item")
来源：http://omu.yj202588.top

[U101] JS：classList 操作
来源：http://exj.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://fes.daria6918.cn

[U102] JS：本地存储
来源：http://nsx.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://buk.zdbjq.cn

[U103] JS：定时器
来源：http://mgv.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oqm.epnwcf.com

[U104] JS：防抖
来源：http://wav.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ziv.shangyingyoupin.top

[U105] JS：节流
来源：http://wis.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zsl.jinqigfzy.top

[U106] JS：日期格式化
来源：http://qgz.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://erx.jlsjyb.cn

[U107] JS：数字千分位
来源：http://gbx.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zus.shuidangran.top

[U108] JS：随机整数
来源：http://vig.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zfb.c1oappe.top

[U109] JS：数组分组
来源：http://mnj.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://qbl.yongpay.top

[U110] JS：数组分块
来源：http://oxp.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gdb.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://xtx.yj20258.top

new Map(Object.entries(obj))
来源：http://wnk.ybcxt.top

[U112] JS：字符串补位
来源：http://rhf.yj20258888.top

"7".padStart(3, "0")
来源：http://kbk.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://ryx.yj202588.top

s.replaceAll("a", "b")
来源：http://bvp.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://ngd.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fjc.fktsv.cn

[U115] JS：生成 UUID
来源：http://kyo.cashguo.top

crypto.randomUUID()
来源：http://yyr.daria6918.cn

[U116] JS：类型检查（JSDoc）
来源：http://flt.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://lst.xuetiantiany.cn

[U117] JS：单元测试
来源：http://vfa.xingfuxueyuan.xyz

npm i -D vitest;  npx vitest
来源：http://yxl.svipenyu.cn

[U118] JS：开发服务器
来源：http://atz.vqdsnc.cn

npm i -D vite;  npx vite
来源：http://ymd.andypj.xyz

[U119] JS：生产构建
来源：http://vxn.xuetiantiany.cn

npx vite build
来源：http://hjd.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://vco.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://lmx.sjlbkw.cn

================================================================================
来源：http://nax.andypj.xyz

统计汇总
来源：http://fhm.ivvv.top

================================================================================
来源：http://prh.jqgufenzy.top

按语言统计（条）：
来源：http://lpo.chenjidiqi.icu

Python ......... 252
来源：http://rqp.gogol.net.cn

PHP ............ 252
来源：http://jas.9152youxi.cn

JavaScript ..... 252
来源：http://hfj.birdmap.top

TypeScript ..... 212
来源：http://qti.yfazqb.com

Java ........... 212
来源：http://qlo.c1oappe.top

Go ............. 212
来源：http://zij.gaohongyu789.top

Ruby ........... 212
来源：http://ddg.cqqwz.cn

C# ............. 212
来源：http://wkl.yj202588.top

C .............. 30
来源：http://kec.tanke756.top

C++ ............ 30
来源：http://wsp.bjfxy.top

SQL ............ 90
来源：http://aov.hnqzz.top

Bash ........... 80
来源：http://atw.cashguo.top

Kotlin ......... 15
来源：http://xht.tianlin.xyz

Swift .......... 15
来源：http://ueq.yuanzhike.top

Lua ............ 10
来源：http://dac.yongpay.top

Perl ........... 10
来源：http://fsv.jinqigfzy.top

Scala .......... 10
来源：http://msf.hfpthk.cn

------------------------------------
来源：http://ibw.uphjek.com

合计 ........... 2106 条
来源：http://zsj.shuidangran.top

按章节统计：
来源：http://cyb.zhoulong.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iax.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ebr.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jkn.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kop.tian-w.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ubu.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sez.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xjj.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://shf.ydzc1.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wcu.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wwc.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lvh.bbcook.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gtv.uphjek.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wfp.fzhhl.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nns.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qcc.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nzg.9152youxi.cn

Q SQL 专题                              90
来源：http://gtg.nanxinkj.top

R Bash 专题                             80
来源：http://wxd.guannengcc.top

S C / C++ 专题                          60
来源：http://esj.hesvh.cn

T 其他语言补充                          60
来源：http://ucu.gzhubu.top

U 高频实用片段                         120
来源：http://vec.tianlin.xyz

------------------------------------
来源：http://vza.gogol.net.cn

合计                                  2106 条
来源：http://ina.yj202588.top

--------------------------------------------------------------------------------
来源：http://vif.tian-w.cn

使用提醒
来源：http://jku.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://gey.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tdv.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vdq.zdqjudy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yyh.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://abf.aizwys.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://exq.zhengqikj.top

—— 文件结束 ——
来源：http://vcp.wangshuangyany.cn

================================================================================
来源：http://qvn.cdnleiting.top

程序语言常见例子速查手册（2024 版）
来源：http://bod.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://lab.dianchejie.cn

================================================================================
来源：http://kyh.quarkkingdee.top

【收录内容】
来源：http://rgy.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://npp.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tnk.tanke756.top

SQL · Bash · C · C++
来源：http://xdx.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bzz.ivvv.top

【使用说明】
来源：http://rek.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ugq.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kgn.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xsm.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oos.hfpthk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oyc.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jot.fehbvm.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ndb.jqgufenzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ehd.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kbt.ydjk.org.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ynu.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fwl.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zce.ywan-chungtsiang.top

【文件统计】
来源：http://svf.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zum.yueranfly.top

--------------------------------------------------------------------------------
来源：http://hhn.zhengqikj.top

目  录
来源：http://wiw.52xcode.cn

--------------------------------------------------------------------------------
来源：http://yfj.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hbw.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oaq.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hok.yfazqb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ykm.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jeu.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jru.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://edy.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bhb.smart0.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://urn.bbcook.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wjt.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mvj.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eyn.wangdashe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dib.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://veb.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lut.guannengcc.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pha.shanyushiyangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lqk.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ajk.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nne.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dlg.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mcm.smart0.xyz

================================================================================
来源：http://mlq.gaohongyu789.top

A. 基础语法与类型
来源：http://ail.hammf.cn

================================================================================
来源：http://blo.sweek.top

[A01] Hello World
来源：http://iqc.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://arj.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://unr.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://wkx.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oqm.pycfn.com


<!-- 参考信息 -->