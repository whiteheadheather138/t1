代发 wailian999

[U27] Py：异步 HTTP
来源：http://puu.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://cmd.cdnleiting.top

[U28] Py：类型别名
来源：http://qxi.haohaochexian.top

UserId = int
来源：http://adv.xinyue.icu

[U29] Py：属性校验
来源：http://oqn.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://kyd.chenlongwang.top

[U30] Py：数据类
来源：http://xwm.mhx1999.top

@dataclass(slots=True)
来源：http://sse.chenjidiqi.icu

[U31] Py：单测
来源：http://lva.mhx1999.top

python -m pytest -q
来源：http://fud.sufxvd.cn

[U32] Py：代码格式化
来源：http://tck.ivvv.top

ruff format . && ruff check --fix .
来源：http://srn.tanke756.top

[U33] Py：打包发布
来源：http://lds.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://faj.haohaochexian.top

[U34] Py：判断编码
来源：http://etu.tian-w.cn

chardet.detect(raw)
来源：http://jmb.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://aaf.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bhl.xylfe.cn

[U36] Py：定时任务
来源：http://nfm.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://zue.ybcxt.top

[U37] Py：读写 Excel
来源：http://jgg.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://lpb.smart0.xyz

[U38] Py：获取脚本所在目录
来源：http://vnc.fanxiaobao.xyz

Path(__file__).resolve().parent
来源：http://lqb.ydzc1.top

[U39] Py：判断是否在交互环境
来源：http://cwh.tanke756.top

sys.stdout.isatty()
来源：http://frv.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://mhh.316326.xyz

print("err", file=sys.stderr)
来源：http://ezq.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://smk.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://jkf.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://rru.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lyt.xuetiantiany.cn

[U43] PHP：声明命名空间
来源：http://lvc.cheryme.top

namespace App\Http;
来源：http://oib.yvedp.cn

[U44] PHP：开启严格类型
来源：http://nbk.gotoacloud.top

declare(strict_types=1);
来源：http://ffx.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://cqp.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zai.yonumen.top

[U46] PHP：可空类型
来源：http://rlq.shuidangran.top

?string $name = null
来源：http://qwv.pycfn.com

[U47] PHP：联合类型
来源：http://zdf.ybcxt.top

int|string $id
来源：http://yso.sufxvd.cn

[U48] PHP：纯枚举
来源：http://yla.xuanzx.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kud.jinqigfzy.top

[U49] PHP：只读属性
来源：http://dmg.jqgfzy.top

public readonly string $name
来源：http://qdg.meibo888.top

[U50] PHP：构造器属性提升
来源：http://irn.svipenyu.cn

public function __construct(private int $id) {}
来源：http://wxx.sxryk.cn

[U51] PHP：数组解构
来源：http://wde.yangfankeji.com

[$a, $b] = $arr;
来源：http://jdu.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://tli.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://gpp.ydzc1.top

[U53] PHP：空合并运算符
来源：http://qri.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://tpk.xziqi.cn

[U54] PHP：空安全调用
来源：http://faa.52xcode.cn

$obj?->method()
来源：http://btn.dashuyun.cn

[U55] PHP：match 表达式
来源：http://qjk.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cxp.zdbjq.cn

[U56] PHP：命名参数
来源：http://ino.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://lzh.snrcjt.cn

[U57] PHP：字符串插值
来源：http://bjh.jinqigufen.top

"值: {$a}"
来源：http://zdj.yuanzhike.top

[U58] PHP：数组三件套
来源：http://gpt.jqgufenzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://amv.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://fvz.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqn.cheryme.top

[U60] PHP：JSON 编解码
来源：http://zju.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wch.yj202588.top

[U61] PHP：正则
来源：http://reu.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vba.yangfankeji.com

[U62] PHP：日期对象
来源：http://pun.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dus.hnxiangtu.top

[U63] PHP：文件读写
来源：http://omw.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tci.aibaodan.cn

[U64] PHP：目录遍历
来源：http://aoj.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://yuu.zhiwuduotai.top

[U65] PHP：会话
来源：http://civ.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vbi.ybcxt.top

[U66] PHP：设置 Cookie
来源：http://bgk.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dhr.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://orh.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vfw.sweek.top

[U68] PHP：PDO 连接
来源：http://lgb.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ewt.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://vsj.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ltt.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://rro.yueranfly.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://irp.guannengcc.top

[U71] PHP：抛出异常
来源：http://hcl.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://phj.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://dwo.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://lrc.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://owi.tian-w.cn

parse_ini_file("config.ini", true)
来源：http://jjm.jianghu66.top

[U74] PHP：读取环境变量
来源：http://yyw.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://akd.yuxming.cn

[U75] PHP：依赖注入
来源：http://vhd.chenlongwang.top

composer require psr/container
来源：http://rlp.chenzaomai.com

[U76] PHP：简单路由
来源：http://gmd.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://evu.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://bza.yongpay.top

composer require twig/twig
来源：http://jbl.gaohongyu789.top

[U78] PHP：单元测试
来源：http://tjh.yonumen.top

composer require --dev phpunit/phpunit
来源：http://qvy.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://jgj.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://edn.daxiang520.top

[U80] PHP：代码规范修复
来源：http://xph.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wlq.wangdashe.top

[U81] JS：初始化项目
来源：http://deg.yuxming.cn

npm init -y;  npm i express
来源：http://hze.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://mvw.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oyk.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://aeg.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rlu.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://mit.bjfxy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ppw.yongpay.top

[U85] JS：可选链
来源：http://cgh.chenzaomai.com

a?.b?.c
来源：http://ioo.cdnleiting.top

[U86] JS：空值合并
来源：http://tgb.jqgufenzy.top

a ?? b
来源：http://lsu.chenjidiqi.icu

[U87] JS：解构默认值
来源：http://kyu.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://eoj.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://flr.fengsongda.top

{ ...a, ...b }
来源：http://npk.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://vsi.xylfe.cn

[...new Set(arr)]
来源：http://bpi.hongshengwenyu.top

[U90] JS：数字数组排序
来源：http://gzc.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://uad.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://mld.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vie.zdbjq.cn

[U92] JS：深拷贝
来源：http://ubw.yuanzhike.top

structuredClone(obj)
来源：http://hnz.bjfxy.top

[U93] JS：模板字符串
来源：http://jnw.9152youxi.cn

`共 ${n} 条`
来源：http://pbv.zhixingplan.top

[U94] JS：箭头函数
来源：http://nup.dianchejie.cn

const double = x => x * 2;
来源：http://jqm.gzhubu.top

[U95] JS：Promise 包装
来源：http://bsd.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://vjr.xylfe.cn

[U96] JS：async/await 与异常
来源：http://gwk.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qkb.316326.xyz

[U97] JS：并发请求
来源：http://qvm.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jcw.fehbvm.com

[U98] JS：fetch 带 JSON
来源：http://yml.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://amd.cheryme.top

[U99] JS：事件监听
来源：http://fso.daxiang520.top

el.addEventListener("click", e => {})
来源：http://vnt.sysykeji.top

[U100] JS：DOM 查询
来源：http://tfo.sysykeji.top

document.querySelector(".item")
来源：http://wnt.ctjpmb.com

[U101] JS：classList 操作
来源：http://krk.jlsjyb.cn

el.classList.toggle("active")
来源：http://rgb.tian-w.cn

[U102] JS：本地存储
来源：http://ghc.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://thb.chenjidiqi.icu

[U103] JS：定时器
来源：http://dsy.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kkf.havefunace.top

[U104] JS：防抖
来源：http://qcp.hysaishi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qsy.ybcxt.top

[U105] JS：节流
来源：http://sbb.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hvf.redwolf501.top

[U106] JS：日期格式化
来源：http://ipj.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://srs.xinyue.icu

[U107] JS：数字千分位
来源：http://npi.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nir.xziqi.cn

[U108] JS：随机整数
来源：http://kom.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xns.sxryk.cn

[U109] JS：数组分组
来源：http://cdc.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://ekk.gaohongyu789.top

[U110] JS：数组分块
来源：http://bmu.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://msm.hcnkem.com

[U111] JS：对象转 Map
来源：http://jbo.ivvv.top

new Map(Object.entries(obj))
来源：http://ffn.fzhhl.top

[U112] JS：字符串补位
来源：http://egb.shuidangran.top

"7".padStart(3, "0")
来源：http://luc.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://ojo.mhx1999.top

s.replaceAll("a", "b")
来源：http://djx.fktsv.cn

[U114] JS：JSON 深比较
来源：http://giu.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://ewm.chenlongwang.top

[U115] JS：生成 UUID
来源：http://yeu.nanxuanxn.top

crypto.randomUUID()
来源：http://pgv.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://awl.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://koz.yonumen.top

[U117] JS：单元测试
来源：http://zsz.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://ica.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://esa.dashuyun.cn

npm i -D vite;  npx vite
来源：http://cfg.hnxiangtu.top

[U119] JS：生产构建
来源：http://wfz.0kj1m.cn

npx vite build
来源：http://xxs.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://wha.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://vau.redwolf501.top

================================================================================
来源：http://emf.daxiang520.top

统计汇总
来源：http://ooh.nwbrower.top

================================================================================
来源：http://qfn.mhx1999.top

按语言统计（条）：
来源：http://dbv.redwolf501.top

Python ......... 252
来源：http://oii.fzhhl.top

PHP ............ 252
来源：http://lig.zhijiandao.cn

JavaScript ..... 252
来源：http://dlp.ehwqpu.com

TypeScript ..... 212
来源：http://kro.yanxiufei.cn

Java ........... 212
来源：http://kxm.nanxinkj.top

Go ............. 212
来源：http://ake.gzhubu.top

Ruby ........... 212
来源：http://opb.yonumen.top

C# ............. 212
来源：http://dae.hnqzz.top

C .............. 30
来源：http://rba.ydjk.org.cn

C++ ............ 30
来源：http://xum.ivvv.top

SQL ............ 90
来源：http://toy.jinghuilouyu.cn

Bash ........... 80
来源：http://alt.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://ltg.jianghu66.top

Swift .......... 15
来源：http://jnk.xziqi.cn

Lua ............ 10
来源：http://agc.fktsv.cn

Perl ........... 10
来源：http://wim.daxiang520.top

Scala .......... 10
来源：http://cpd.sysykeji.top

------------------------------------
来源：http://iur.ctjpmb.com

合计 ........... 2106 条
来源：http://xpc.havefunace.top

按章节统计：
来源：http://adv.nanxinkj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qep.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uhi.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fmx.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sgt.tanke756.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xba.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qfg.ydjk.org.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ecq.tian-w.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jtm.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ubv.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mga.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ewr.fanxiaobao.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://toq.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://flk.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zbo.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://and.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://brm.yongpay.top

Q SQL 专题                              90
来源：http://xvf.zhiwuduotai.top

R Bash 专题                             80
来源：http://qth.yanxiufei.cn

S C / C++ 专题                          60
来源：http://elv.jiagoushi.top

T 其他语言补充                          60
来源：http://pxm.yuanzhike.top

U 高频实用片段                         120
来源：http://trz.cheryme.top

------------------------------------
来源：http://wdp.nwbrower.top

合计                                  2106 条
来源：http://pvr.hesvh.cn

--------------------------------------------------------------------------------
来源：http://oey.zdbjq.cn

使用提醒
来源：http://poe.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://wag.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ans.yonumen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pnl.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jwk.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hnt.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jke.zhoulong.xyz

—— 文件结束 ——
来源：http://kds.yueranfly.top

================================================================================
来源：http://rtw.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://eoq.hcnkem.com

Common Programming Examples Cheat Book
来源：http://ykc.sxryk.cn

================================================================================
来源：http://bem.yangfankeji.com

【收录内容】
来源：http://mxf.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jei.meibo888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://afm.zhengqikj.top

SQL · Bash · C · C++
来源：http://yqz.svipenyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qtj.iojbl.cn

【使用说明】
来源：http://tvy.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ftu.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bhf.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gxi.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nbn.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://akm.epnwcf.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cdp.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ewj.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ugs.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jso.shanyushiyangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iae.svipenyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://idw.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nqi.gaohongyu789.top

【文件统计】
来源：http://kfv.zhoulong.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cnx.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://hsj.wangdashe.top

目  录
来源：http://wpe.birdmap.top

--------------------------------------------------------------------------------
来源：http://ceb.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cso.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://das.xziqi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wqf.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://edh.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ucd.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://swz.gotoacloud.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hfs.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dwk.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dsh.xylfe.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wpm.sweek.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hsp.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://edc.ppjwa.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ksx.0kj1m.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tkj.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oom.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iqz.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nal.zhixingplan.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dsw.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ebm.tian-w.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uly.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ufp.shzxlz.cn

================================================================================
来源：http://jfq.fanxiaobao.xyz

A. 基础语法与类型
来源：http://qhs.ydzc1.top

================================================================================
来源：http://was.tian-w.cn

[A01] Hello World
来源：http://rzi.yangfankeji.com

Py:   print("Hello, World!")
来源：http://eic.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://eau.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://jhd.sysykeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rjw.svipenyu.cn


<!-- 参考信息 -->