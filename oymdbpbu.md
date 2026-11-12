代发 wailian999

[U25] Py：CSV 按字典读
来源：http://eul.fktsv.cn

csv.DictReader(f)
来源：http://qiu.sxryk.cn

[U26] Py：并发下载
来源：http://bdp.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ged.redwolf501.top

[U27] Py：异步 HTTP
来源：http://nua.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://fnv.cucudq.cn

[U28] Py：类型别名
来源：http://iyb.0kj1m.cn

UserId = int
来源：http://dle.yfazqb.com

[U29] Py：属性校验
来源：http://fds.yj202588.top

@property 与 @x.setter 配合
来源：http://fmn.fengsongda.top

[U30] Py：数据类
来源：http://lxg.zhaomingkeji.xyz

@dataclass(slots=True)
来源：http://tjv.yj202588.top

[U31] Py：单测
来源：http://yrk.xylfe.cn

python -m pytest -q
来源：http://alj.zhongyouzk.top

[U32] Py：代码格式化
来源：http://npl.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://sxc.yvedp.cn

[U33] Py：打包发布
来源：http://btn.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://qsq.nanxuanxn.top

[U34] Py：判断编码
来源：http://vza.jqgfzy.top

chardet.detect(raw)
来源：http://inm.yongpay.top

[U35] Py：发送邮件
来源：http://bdv.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ujg.yonumen.top

[U36] Py：定时任务
来源：http://twg.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://cte.gzhubu.top

[U37] Py：读写 Excel
来源：http://klw.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://plw.sweek.top

[U38] Py：获取脚本所在目录
来源：http://zoi.ivvv.top

Path(__file__).resolve().parent
来源：http://zoy.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://qcl.hesvh.cn

sys.stdout.isatty()
来源：http://kgs.pycfn.com

[U40] Py：打印到标准错误
来源：http://eph.daria6918.cn

print("err", file=sys.stderr)
来源：http://lgt.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://jag.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ujb.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://mrm.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ppo.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://wdi.gzhubu.top

namespace App\Http;
来源：http://uhk.daria6918.cn

[U44] PHP：开启严格类型
来源：http://smp.shzxlz.cn

declare(strict_types=1);
来源：http://git.shuidangran.top

[U45] PHP：类型声明与返回类型
来源：http://jyb.cucudq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lng.316326.xyz

[U46] PHP：可空类型
来源：http://yqr.bjfxy.top

?string $name = null
来源：http://fzp.zhongyouzk.top

[U47] PHP：联合类型
来源：http://zqm.epnwcf.com

int|string $id
来源：http://sfv.vehdjk.com

[U48] PHP：纯枚举
来源：http://qum.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rox.daxiang520.top

[U49] PHP：只读属性
来源：http://ung.yangfankeji.com

public readonly string $name
来源：http://iul.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://qoj.hfpthk.cn

public function __construct(private int $id) {}
来源：http://kie.52xcode.cn

[U51] PHP：数组解构
来源：http://zuk.tarul.cn

[$a, $b] = $arr;
来源：http://ybg.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://fhg.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://ckj.yj20258888.top

[U53] PHP：空合并运算符
来源：http://qph.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://bcf.yfazqb.com

[U54] PHP：空安全调用
来源：http://cgn.redwolf501.top

$obj?->method()
来源：http://btx.yj20258.top

[U55] PHP：match 表达式
来源：http://abd.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wmz.ivvv.top

[U56] PHP：命名参数
来源：http://qci.jinqigufen.top

f(a: 1, b: 2)
来源：http://lqv.sufxvd.cn

[U57] PHP：字符串插值
来源：http://hni.vehdjk.com

"值: {$a}"
来源：http://vqx.ppjwa.cn

[U58] PHP：数组三件套
来源：http://xxh.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qbg.chenzaomai.com

[U59] PHP：自定义排序
来源：http://spy.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zoc.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://kuk.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lms.bbcook.cn

[U61] PHP：正则
来源：http://csa.ivvv.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://psc.yj20258888.top

[U62] PHP：日期对象
来源：http://lno.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ubk.hammf.cn

[U63] PHP：文件读写
来源：http://bpa.9152youxi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://msd.yuanzhike.top

[U64] PHP：目录遍历
来源：http://hpq.pycfn.com

glob("dir/*.php");  scandir("dir");
来源：http://mgu.zhiwuduotai.top

[U65] PHP：会话
来源：http://foi.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ifn.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://ihr.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wqn.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://lec.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jaq.hcnkem.com

[U68] PHP：PDO 连接
来源：http://zvz.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iow.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://jmb.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dxh.bbcook.cn

[U70] PHP：PDO 事务
来源：http://jjv.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pap.xuanzx.com

[U71] PHP：抛出异常
来源：http://pet.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://qyo.zycfv.cn

[U72] PHP：写错误日志
来源：http://qhn.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://kjh.bjfxy.top

[U73] PHP：读取 ini 配置
来源：http://uty.vqdsnc.cn

parse_ini_file("config.ini", true)
来源：http://inu.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://fpb.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://aqs.uphjek.com

[U75] PHP：依赖注入
来源：http://qyb.redwolf501.top

composer require psr/container
来源：http://wmr.epnwcf.com

[U76] PHP：简单路由
来源：http://srv.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mna.hfpthk.cn

[U77] PHP：模板渲染
来源：http://dyz.pengpengdd.cyou

composer require twig/twig
来源：http://zrd.9152youxi.cn

[U78] PHP：单元测试
来源：http://zma.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://ooz.shanyushiyangtech.top

[U79] PHP：静态分析
来源：http://uhg.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://pgq.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://wcz.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kgf.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://wsw.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://wme.fzhhl.top

[U82] JS：package.json 脚本
来源：http://dab.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://afp.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://pdd.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://epd.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://aym.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://vsb.zhengqikj.top

[U85] JS：可选链
来源：http://gti.shangyingyoupin.top

a?.b?.c
来源：http://uro.quarkkingdee.top

[U86] JS：空值合并
来源：http://kgu.aibaodan.cn

a ?? b
来源：http://oqg.havefunace.top

[U87] JS：解构默认值
来源：http://chi.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://llz.yangfankeji.com

[U88] JS：对象展开合并
来源：http://dmz.nanxinkj.top

{ ...a, ...b }
来源：http://euh.pycfn.com

[U89] JS：数组去重
来源：http://vum.wangdashe.top

[...new Set(arr)]
来源：http://kxs.zhengqikj.top

[U90] JS：数字数组排序
来源：http://jld.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://oaq.wangdashe.top

[U91] JS：对象键值遍历
来源：http://qbh.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://acq.sxryk.cn

[U92] JS：深拷贝
来源：http://xrk.guowangkeji.top

structuredClone(obj)
来源：http://abm.ppjwa.cn

[U93] JS：模板字符串
来源：http://zyc.fengsongda.top

`共 ${n} 条`
来源：http://epe.316326.xyz

[U94] JS：箭头函数
来源：http://qfx.bbcook.cn

const double = x => x * 2;
来源：http://dkg.vehdjk.com

[U95] JS：Promise 包装
来源：http://gzp.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://knh.xylfe.cn

[U96] JS：async/await 与异常
来源：http://gkh.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ahu.birdmap.top

[U97] JS：并发请求
来源：http://sdl.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ruw.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://mhg.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yrd.sxryk.cn

[U99] JS：事件监听
来源：http://dtd.gzhubu.top

el.addEventListener("click", e => {})
来源：http://bsi.hywenlv.cn

[U100] JS：DOM 查询
来源：http://kgi.xinyue.icu

document.querySelector(".item")
来源：http://rxi.havefunace.top

[U101] JS：classList 操作
来源：http://jua.fktsv.cn

el.classList.toggle("active")
来源：http://rpo.316326.xyz

[U102] JS：本地存储
来源：http://ijc.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lku.chenjidiqi.icu

[U103] JS：定时器
来源：http://zss.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hpk.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://hhh.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://khs.fktsv.cn

[U105] JS：节流
来源：http://mkw.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cnv.sjlbkw.cn

[U106] JS：日期格式化
来源：http://wws.hnxiangtu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qts.cdnleiting.top

[U107] JS：数字千分位
来源：http://eju.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bhq.zdbjq.cn

[U108] JS：随机整数
来源：http://qbx.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://axx.yj20258888.top

[U109] JS：数组分组
来源：http://fmi.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://hdv.sysykeji.top

[U110] JS：数组分块
来源：http://aox.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bbb.dianchejie.cn

[U111] JS：对象转 Map
来源：http://eat.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://evg.sysykeji.top

[U112] JS：字符串补位
来源：http://dhq.hnqzz.top

"7".padStart(3, "0")
来源：http://jav.hysaishi.cn

[U113] JS：正则替换全部
来源：http://mwg.bbcook.cn

s.replaceAll("a", "b")
来源：http://ulq.chenlongwang.top

[U114] JS：JSON 深比较
来源：http://bws.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://utj.fehbvm.com

[U115] JS：生成 UUID
来源：http://itr.wangshuangyany.cn

crypto.randomUUID()
来源：http://hwo.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://gky.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://qjl.nanxinkj.top

[U117] JS：单元测试
来源：http://gan.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://ymw.zhixingplan.top

[U118] JS：开发服务器
来源：http://ejr.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://byg.dianchejie.cn

[U119] JS：生产构建
来源：http://qys.ivvv.top

npx vite build
来源：http://bkz.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://set.ivvv.top

import.meta.env.VITE_API_URL
来源：http://lfo.cdnleiting.top

================================================================================
来源：http://gli.hcnkem.com

统计汇总
来源：http://smr.sufxvd.cn

================================================================================
来源：http://nwj.ywan-chungtsiang.top

按语言统计（条）：
来源：http://lrb.chenlongwang.top

Python ......... 252
来源：http://bgp.fzhhl.top

PHP ............ 252
来源：http://sav.ydjk.org.cn

JavaScript ..... 252
来源：http://wth.zhoulong.xyz

TypeScript ..... 212
来源：http://lah.hfpthk.cn

Java ........... 212
来源：http://ccs.hnqzz.top

Go ............. 212
来源：http://jsu.feifeiyinyue.top

Ruby ........... 212
来源：http://toq.meibo888.top

C# ............. 212
来源：http://slb.fktsv.cn

C .............. 30
来源：http://png.52xcode.cn

C++ ............ 30
来源：http://jpm.gogol.net.cn

SQL ............ 90
来源：http://cwr.cheryme.top

Bash ........... 80
来源：http://ayp.yongpay.top

Kotlin ......... 15
来源：http://irt.ppjwa.cn

Swift .......... 15
来源：http://jdz.epnwcf.com

Lua ............ 10
来源：http://fmv.jyoumei.cn

Perl ........... 10
来源：http://qmj.bbcook.cn

Scala .......... 10
来源：http://zab.nanxuanxn.top

------------------------------------
来源：http://zhp.wangdashe.top

合计 ........... 2106 条
来源：http://rop.ppjwa.cn

按章节统计：
来源：http://zjl.gzhubu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kqr.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dub.hfpthk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qun.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xdi.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vka.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jmm.zhaomingkeji.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dnv.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xbf.zdqjudy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://npl.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nny.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gee.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pja.ppjwa.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://agm.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eaf.sysykeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jxh.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yam.ctjpmb.com

Q SQL 专题                              90
来源：http://qwm.ctjpmb.com

R Bash 专题                             80
来源：http://xjq.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://cgv.snrcjt.cn

T 其他语言补充                          60
来源：http://iwn.zhongyouzk.top

U 高频实用片段                         120
来源：http://huw.ivvv.top

------------------------------------
来源：http://gog.hcnkem.com

合计                                  2106 条
来源：http://nfp.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://jpi.shangyingyoupin.top

使用提醒
来源：http://cas.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://aji.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ssl.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rad.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qth.snrcjt.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yca.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hlr.jqgfzy.top

—— 文件结束 ——
来源：http://oyn.ybcxt.top

================================================================================
来源：http://wdq.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://bar.fehbvm.com

Common Programming Examples Cheat Book
来源：http://uup.xylfe.cn

================================================================================
来源：http://wfz.fktsv.cn

【收录内容】
来源：http://yfx.hnqzz.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://svs.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://osd.bjfxy.top

SQL · Bash · C · C++
来源：http://kgj.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hxw.epnwcf.com

【使用说明】
来源：http://kfi.yangfankeji.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kzq.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://apv.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oti.zdbjq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jcr.guannengcc.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hia.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ujh.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hft.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kat.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qzd.zhijiandao.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zon.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tre.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uum.nanxuanxn.top

【文件统计】
来源：http://ouj.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tnn.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://xnz.cucudq.cn

目  录
来源：http://bql.ivvv.top

--------------------------------------------------------------------------------
来源：http://lhp.quarkkingdee.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xlt.c1oappe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dny.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jgv.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://prr.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dfl.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://upr.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ami.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qhj.yvedp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://edo.yvedp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xcm.hysaishi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jri.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vyl.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lpc.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cdh.xziqi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qzj.zhengqikj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pyk.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ymn.zhiwuduotai.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vqg.yfazqb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dru.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://udk.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rax.xinyue.icu

================================================================================
来源：http://sic.hywenlv.cn

A. 基础语法与类型
来源：http://cvz.gogol.net.cn

================================================================================
来源：http://zby.yj202588.top

[A01] Hello World
来源：http://mvn.xuetiantiany.cn


<!-- 参考信息 -->