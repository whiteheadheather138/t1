代发 wailian999

[U25] Py：CSV 按字典读
来源：http://woq.birdmap.top

csv.DictReader(f)
来源：http://gbi.daxiang520.top

[U26] Py：并发下载
来源：http://tsc.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cvl.nwbrower.top

[U27] Py：异步 HTTP
来源：http://ztp.gaohongyu789.top

aiohttp.ClientSession() 配合 async with
来源：http://dsi.cheryme.top

[U28] Py：类型别名
来源：http://ilw.pycfn.com

UserId = int
来源：http://tgn.zhongyouzk.top

[U29] Py：属性校验
来源：http://eao.yongpay.top

@property 与 @x.setter 配合
来源：http://ozb.316326.xyz

[U30] Py：数据类
来源：http://fej.zdbjq.cn

@dataclass(slots=True)
来源：http://gek.jinghuilouyu.cn

[U31] Py：单测
来源：http://aly.xinyue.icu

python -m pytest -q
来源：http://gll.cashguo.top

[U32] Py：代码格式化
来源：http://aua.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://mme.mhx1999.top

[U33] Py：打包发布
来源：http://slt.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://rpw.jinqigufen.top

[U34] Py：判断编码
来源：http://ret.birdmap.top

chardet.detect(raw)
来源：http://zav.nanxinkj.top

[U35] Py：发送邮件
来源：http://vva.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hrm.cdnleiting.top

[U36] Py：定时任务
来源：http://grz.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://kvy.vehdjk.com

[U37] Py：读写 Excel
来源：http://vwj.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://hne.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://iqh.redwolf501.top

Path(__file__).resolve().parent
来源：http://rao.fengsongda.top

[U39] Py：判断是否在交互环境
来源：http://oqn.yj20258.top

sys.stdout.isatty()
来源：http://ycj.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://rnb.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://gzw.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://orb.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vdv.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://yao.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vzf.tian-w.cn

[U43] PHP：声明命名空间
来源：http://uzj.zhaomingkeji.xyz

namespace App\Http;
来源：http://pyp.yj20258888.top

[U44] PHP：开启严格类型
来源：http://zgx.fehbvm.com

declare(strict_types=1);
来源：http://nqn.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://xel.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tsf.zycfv.cn

[U46] PHP：可空类型
来源：http://hcl.snrcjt.cn

?string $name = null
来源：http://xdm.gogol.net.cn

[U47] PHP：联合类型
来源：http://vxp.zhongyouzk.top

int|string $id
来源：http://ywu.sysykeji.top

[U48] PHP：纯枚举
来源：http://szv.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sfo.zhixingplan.top

[U49] PHP：只读属性
来源：http://jqn.zdqjudy.top

public readonly string $name
来源：http://juc.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://lbo.cqqwz.cn

public function __construct(private int $id) {}
来源：http://hxe.daxiang520.top

[U51] PHP：数组解构
来源：http://gqk.zhongyouzk.top

[$a, $b] = $arr;
来源：http://fja.yueranfly.top

[U52] PHP：箭头函数
来源：http://lpc.yongpay.top

$double = fn($x) => $x * 2;
来源：http://rdf.cucudq.cn

[U53] PHP：空合并运算符
来源：http://nnm.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://srw.fehbvm.com

[U54] PHP：空安全调用
来源：http://sqy.yonumen.top

$obj?->method()
来源：http://vpn.ctjpmb.com

[U55] PHP：match 表达式
来源：http://ncd.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://spg.ivvv.top

[U56] PHP：命名参数
来源：http://skz.jlsjyb.cn

f(a: 1, b: 2)
来源：http://sdb.smart0.xyz

[U57] PHP：字符串插值
来源：http://jis.yongpay.top

"值: {$a}"
来源：http://zek.cdnleiting.top

[U58] PHP：数组三件套
来源：http://xys.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hcu.fktsv.cn

[U59] PHP：自定义排序
来源：http://lyk.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qed.hcnkem.com

[U60] PHP：JSON 编解码
来源：http://rdz.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eip.daxiang520.top

[U61] PHP：正则
来源：http://nmx.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uxg.nanxuanxn.top

[U62] PHP：日期对象
来源：http://xks.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://snk.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://nut.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fyc.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://qnz.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://rld.zdqjudy.top

[U65] PHP：会话
来源：http://sjx.shanyushiyangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cib.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://zzd.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cjx.xylfe.cn

[U67] PHP：处理文件上传
来源：http://ara.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rst.yj202588.top

[U68] PHP：PDO 连接
来源：http://rjj.xziqi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cbd.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://joi.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eti.guannengcc.top

[U70] PHP：PDO 事务
来源：http://yxm.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ydp.vehdjk.com

[U71] PHP：抛出异常
来源：http://zzz.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://dyy.ehwqpu.com

[U72] PHP：写错误日志
来源：http://sek.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://mfu.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://qfe.havefunace.top

parse_ini_file("config.ini", true)
来源：http://epm.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://ixu.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://uxh.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://ewo.nanxuanxn.top

composer require psr/container
来源：http://faq.sysykeji.top

[U76] PHP：简单路由
来源：http://uko.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tgq.xuanzx.com

[U77] PHP：模板渲染
来源：http://vyn.chenjidiqi.icu

composer require twig/twig
来源：http://lvq.dashuyun.cn

[U78] PHP：单元测试
来源：http://mbl.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://pqa.daria6918.cn

[U79] PHP：静态分析
来源：http://tso.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://tul.hcnkem.com

[U80] PHP：代码规范修复
来源：http://dmh.yj20258888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://txc.sysykeji.top

[U81] JS：初始化项目
来源：http://ryz.meibo888.top

npm init -y;  npm i express
来源：http://kmh.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://wcc.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ssj.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://gyc.sufxvd.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gcr.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://pxx.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xqq.shuidangran.top

[U85] JS：可选链
来源：http://pxe.ehwqpu.com

a?.b?.c
来源：http://cng.meibo888.top

[U86] JS：空值合并
来源：http://thb.yangfankeji.com

a ?? b
来源：http://has.hywenlv.cn

[U87] JS：解构默认值
来源：http://bii.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://kyp.yongpay.top

[U88] JS：对象展开合并
来源：http://gwl.yuanzhike.top

{ ...a, ...b }
来源：http://jdz.fktsv.cn

[U89] JS：数组去重
来源：http://iuo.52xcode.cn

[...new Set(arr)]
来源：http://xra.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://ueh.cqqwz.cn

[...arr].sort((a, b) => a - b)
来源：http://spy.andypj.xyz

[U91] JS：对象键值遍历
来源：http://hvr.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yii.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://rwy.guannengcc.top

structuredClone(obj)
来源：http://ekj.gogol.net.cn

[U93] JS：模板字符串
来源：http://bcm.jiagoushi.top

`共 ${n} 条`
来源：http://jdf.hnxiangtu.top

[U94] JS：箭头函数
来源：http://wua.hcnkem.com

const double = x => x * 2;
来源：http://oyj.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://oon.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://poy.pycfn.com

[U96] JS：async/await 与异常
来源：http://yln.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tso.hongshengwenyu.top

[U97] JS：并发请求
来源：http://ooa.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gbv.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://hyr.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nez.sufxvd.cn

[U99] JS：事件监听
来源：http://pjh.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://usc.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://gdn.hnqzz.top

document.querySelector(".item")
来源：http://zmn.tanke756.top

[U101] JS：classList 操作
来源：http://iiu.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://lwx.uphjek.com

[U102] JS：本地存储
来源：http://jtn.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://myk.yangfankeji.com

[U103] JS：定时器
来源：http://fji.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gyu.wangdashe.top

[U104] JS：防抖
来源：http://lac.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xey.zhongyouzk.top

[U105] JS：节流
来源：http://wdi.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hpd.chenlongwang.top

[U106] JS：日期格式化
来源：http://ikp.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ccv.tanke756.top

[U107] JS：数字千分位
来源：http://mpc.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xbl.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://hbm.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tbc.fehbvm.com

[U109] JS：数组分组
来源：http://cqa.vqdsnc.cn

Object.groupBy(arr, x => x.type)
来源：http://ccj.jinqigufen.top

[U110] JS：数组分块
来源：http://mby.ehwqpu.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pia.aibaodan.cn

[U111] JS：对象转 Map
来源：http://sfh.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://cil.cucudq.cn

[U112] JS：字符串补位
来源：http://vej.yfazqb.com

"7".padStart(3, "0")
来源：http://lhc.smart0.xyz

[U113] JS：正则替换全部
来源：http://hda.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://scx.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://ovf.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://oio.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://ivu.bjfxy.top

crypto.randomUUID()
来源：http://fuw.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://pqd.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://odf.xylfe.cn

[U117] JS：单元测试
来源：http://grv.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://nzz.smart0.xyz

[U118] JS：开发服务器
来源：http://alu.nanxinkj.top

npm i -D vite;  npx vite
来源：http://rjf.ybcxt.top

[U119] JS：生产构建
来源：http://vdl.birdmap.top

npx vite build
来源：http://rva.redwolf501.top

[U120] JS：读取环境变量（Vite）
来源：http://vam.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://wqq.ppjwa.cn

================================================================================
来源：http://vwe.zhiwuduotai.top

统计汇总
来源：http://fkb.yuxming.cn

================================================================================
来源：http://fhh.zhaomingkeji.xyz

按语言统计（条）：
来源：http://eke.vehdjk.com

Python ......... 252
来源：http://slz.zhixingplan.top

PHP ............ 252
来源：http://kvi.daxiang520.top

JavaScript ..... 252
来源：http://pnk.shangyingyoupin.top

TypeScript ..... 212
来源：http://vro.jiagoushi.top

Java ........... 212
来源：http://epu.hnxiangtu.top

Go ............. 212
来源：http://byi.svipenyu.cn

Ruby ........... 212
来源：http://xww.hesvh.cn

C# ............. 212
来源：http://fbl.yj202588.top

C .............. 30
来源：http://qgm.cashguo.top

C++ ............ 30
来源：http://vnw.fzhhl.top

SQL ............ 90
来源：http://bot.yangfankeji.com

Bash ........... 80
来源：http://bwr.svipenyu.cn

Kotlin ......... 15
来源：http://pzm.0kj1m.cn

Swift .......... 15
来源：http://cic.hfpthk.cn

Lua ............ 10
来源：http://nuy.shangyingyoupin.top

Perl ........... 10
来源：http://fkd.yanxiufei.cn

Scala .......... 10
来源：http://zem.cdnleiting.top

------------------------------------
来源：http://ptq.xinyue.icu

合计 ........... 2106 条
来源：http://har.sjlbkw.cn

按章节统计：
来源：http://jyy.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qdj.yj202588.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dym.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wfb.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cws.yonumen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xoy.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kip.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ipz.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aqi.andypj.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ssr.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ihr.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://huc.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ofx.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cbo.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qed.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dev.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ydj.gogol.net.cn

Q SQL 专题                              90
来源：http://kan.9152youxi.cn

R Bash 专题                             80
来源：http://wrk.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://tgo.zhengqikj.top

T 其他语言补充                          60
来源：http://iwp.jiagoushi.top

U 高频实用片段                         120
来源：http://gzr.fehbvm.com

------------------------------------
来源：http://ynv.tian-w.cn

合计                                  2106 条
来源：http://jcp.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://aud.gogol.net.cn

使用提醒
来源：http://qeb.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://hsz.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iln.snrcjt.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mje.yonumen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lud.ydjk.org.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vmo.feifeiyinyue.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zfv.hongshengwenyu.top

—— 文件结束 ——
来源：http://wma.guannengcc.top

================================================================================
来源：http://gin.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://fjl.52xcode.cn

Common Programming Examples Cheat Book
来源：http://sze.shangyingyoupin.top

================================================================================
来源：http://snc.gaohongyu789.top

【收录内容】
来源：http://pyx.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://enp.zhaomingkeji.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vph.52xcode.cn

SQL · Bash · C · C++
来源：http://cie.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cnc.gzhubu.top

【使用说明】
来源：http://ebp.zhixingplan.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fty.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kmn.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tag.andypj.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zff.wangdashe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nua.gzhubu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ddh.epnwcf.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qnu.dianchejie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vvs.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qjz.yfazqb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mzu.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bsq.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cnc.yonumen.top

【文件统计】
来源：http://qyz.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://koo.epnwcf.com

--------------------------------------------------------------------------------
来源：http://pif.zhoulong.xyz

目  录
来源：http://vfp.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://lzp.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vpz.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hnl.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://edn.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zoi.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fal.ywan-chungtsiang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://llf.mhx1999.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bon.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://myv.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fpx.feifeiyinyue.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sgl.ydjk.org.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dxc.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nlr.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cwg.mhx1999.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bjd.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kdr.pycfn.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ktt.316326.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xvt.zdbjq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tda.yuanzhike.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vek.yj20258888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lnc.jqgfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tel.ybcxt.top

================================================================================
来源：http://ccd.nanxinkj.top

A. 基础语法与类型
来源：http://wpl.snrcjt.cn

================================================================================
来源：http://kyn.9152youxi.cn

[A01] Hello World
来源：http://zkf.nwbrower.top


<!-- 参考信息 -->