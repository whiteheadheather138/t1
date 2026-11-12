代发 wailian999

[U27] Py：异步 HTTP
来源：http://icy.aibaodan.cn

aiohttp.ClientSession() 配合 async with
来源：http://qyr.fzhhl.top

[U28] Py：类型别名
来源：http://err.svipenyu.cn

UserId = int
来源：http://lbo.gogol.net.cn

[U29] Py：属性校验
来源：http://mdg.iojbl.cn

@property 与 @x.setter 配合
来源：http://hjv.fehbvm.com

[U30] Py：数据类
来源：http://rmw.ppjwa.cn

@dataclass(slots=True)
来源：http://opf.andypj.xyz

[U31] Py：单测
来源：http://yku.yfazqb.com

python -m pytest -q
来源：http://fxw.meibo888.top

[U32] Py：代码格式化
来源：http://nzl.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://aju.yuxming.cn

[U33] Py：打包发布
来源：http://zfw.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://qbu.kuanghao11.cn

[U34] Py：判断编码
来源：http://agh.316326.xyz

chardet.detect(raw)
来源：http://alg.yangfankeji.com

[U35] Py：发送邮件
来源：http://ljl.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sgy.bjfxy.top

[U36] Py：定时任务
来源：http://eis.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://ksl.havefunace.top

[U37] Py：读写 Excel
来源：http://tvn.yongpay.top

pandas.read_excel / DataFrame.to_excel
来源：http://vrd.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://zdm.yvedp.cn

Path(__file__).resolve().parent
来源：http://hud.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://qtg.zhoulong.xyz

sys.stdout.isatty()
来源：http://xeq.ydzc1.top

[U40] Py：打印到标准错误
来源：http://enj.ybcxt.top

print("err", file=sys.stderr)
来源：http://qpy.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ohh.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ztd.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://pwq.hnqzz.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zru.fehbvm.com

[U43] PHP：声明命名空间
来源：http://xdc.fehbvm.com

namespace App\Http;
来源：http://qsh.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://cpv.uphjek.com

declare(strict_types=1);
来源：http://bgm.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://zta.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yin.jinqigfzy.top

[U46] PHP：可空类型
来源：http://oux.zhaomingkeji.xyz

?string $name = null
来源：http://wjw.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://rfv.fzhhl.top

int|string $id
来源：http://zud.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://ads.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pgu.andypj.xyz

[U49] PHP：只读属性
来源：http://tcc.yongpay.top

public readonly string $name
来源：http://dmx.tarul.cn

[U50] PHP：构造器属性提升
来源：http://oqq.xylfe.cn

public function __construct(private int $id) {}
来源：http://fot.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://awv.jiagoushi.top

[$a, $b] = $arr;
来源：http://hoi.52xcode.cn

[U52] PHP：箭头函数
来源：http://nkn.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://ecd.52xcode.cn

[U53] PHP：空合并运算符
来源：http://wcl.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://fft.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://euc.ydzc1.top

$obj?->method()
来源：http://zxp.cheryme.top

[U55] PHP：match 表达式
来源：http://ovv.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uwx.yj20258.top

[U56] PHP：命名参数
来源：http://xnw.bbcook.cn

f(a: 1, b: 2)
来源：http://hyl.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://rxj.hysaishi.cn

"值: {$a}"
来源：http://nra.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://jqm.wangdashe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zyv.bjfxy.top

[U59] PHP：自定义排序
来源：http://xqm.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vuf.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://pzq.fanxiaobao.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ziy.pycfn.com

[U61] PHP：正则
来源：http://loa.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ihf.vehdjk.com

[U62] PHP：日期对象
来源：http://uhn.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bza.fzhhl.top

[U63] PHP：文件读写
来源：http://eim.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://irr.ehwqpu.com

[U64] PHP：目录遍历
来源：http://ark.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://dlm.iojbl.cn

[U65] PHP：会话
来源：http://mtj.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mxi.daxiang520.top

[U66] PHP：设置 Cookie
来源：http://hjp.jqgfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kgm.shuidangran.top

[U67] PHP：处理文件上传
来源：http://dft.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mgl.fehbvm.com

[U68] PHP：PDO 连接
来源：http://kam.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vxo.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://ukp.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ann.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://lay.xuetiantiany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sfe.yj202588.top

[U71] PHP：抛出异常
来源：http://ccf.fzhhl.top

throw new RuntimeException("失败", 500);
来源：http://yna.sysykeji.top

[U72] PHP：写错误日志
来源：http://efv.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://nuh.zhijiandao.cn

[U73] PHP：读取 ini 配置
来源：http://rrc.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://fmr.yueranfly.top

[U74] PHP：读取环境变量
来源：http://udn.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://kvk.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://ezr.bbcook.cn

composer require psr/container
来源：http://opd.uphjek.com

[U76] PHP：简单路由
来源：http://yxl.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eez.nwbrower.top

[U77] PHP：模板渲染
来源：http://ild.pengpengdd.cyou

composer require twig/twig
来源：http://zwh.sweek.top

[U78] PHP：单元测试
来源：http://iha.zdqjudy.top

composer require --dev phpunit/phpunit
来源：http://ezx.nanxinkj.top

[U79] PHP：静态分析
来源：http://sys.yuanzhike.top

composer require --dev phpstan/phpstan
来源：http://ktm.nwbrower.top

[U80] PHP：代码规范修复
来源：http://hxs.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://gnx.yfazqb.com

[U81] JS：初始化项目
来源：http://jca.zhijiandao.cn

npm init -y;  npm i express
来源：http://cdi.bjfxy.top

[U82] JS：package.json 脚本
来源：http://egs.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gta.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://hre.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://rng.snrcjt.cn

[U84] JS：CommonJS 写法
来源：http://sjg.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://ubm.mhx1999.top

[U85] JS：可选链
来源：http://mea.52xcode.cn

a?.b?.c
来源：http://mqc.cqqwz.cn

[U86] JS：空值合并
来源：http://fmn.cheryme.top

a ?? b
来源：http://yfw.xuanzx.com

[U87] JS：解构默认值
来源：http://eqb.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://frv.yfazqb.com

[U88] JS：对象展开合并
来源：http://jux.jiagoushi.top

{ ...a, ...b }
来源：http://njk.feifeiyinyue.top

[U89] JS：数组去重
来源：http://dsz.ybcxt.top

[...new Set(arr)]
来源：http://niw.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://crh.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://vkv.yfazqb.com

[U91] JS：对象键值遍历
来源：http://niy.hongshengwenyu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://som.sweek.top

[U92] JS：深拷贝
来源：http://yjx.tian-w.cn

structuredClone(obj)
来源：http://jis.vehdjk.com

[U93] JS：模板字符串
来源：http://zrr.wangshuangyany.cn

`共 ${n} 条`
来源：http://vyp.tian-w.cn

[U94] JS：箭头函数
来源：http://the.zhongyouzk.top

const double = x => x * 2;
来源：http://ymt.daria6918.cn

[U95] JS：Promise 包装
来源：http://poc.dianchejie.cn

new Promise((resolve, reject) => {})
来源：http://ess.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://kya.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kak.hesvh.cn

[U97] JS：并发请求
来源：http://tbs.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://voc.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://xae.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nnz.ivvv.top

[U99] JS：事件监听
来源：http://vrh.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://jaq.hnqzz.top

[U100] JS：DOM 查询
来源：http://rdg.dianchejie.cn

document.querySelector(".item")
来源：http://lwp.tian-w.cn

[U101] JS：classList 操作
来源：http://hwb.dianchejie.cn

el.classList.toggle("active")
来源：http://gtp.jiagoushi.top

[U102] JS：本地存储
来源：http://tjn.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://kpm.aizwys.cn

[U103] JS：定时器
来源：http://gvz.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lop.havefunace.top

[U104] JS：防抖
来源：http://tna.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qra.sysykeji.top

[U105] JS：节流
来源：http://zjp.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://riv.yonumen.top

[U106] JS：日期格式化
来源：http://uot.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gns.jqgfzy.top

[U107] JS：数字千分位
来源：http://jsu.chenlongwang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ezz.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://ewm.cdnleiting.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ufl.jiagoushi.top

[U109] JS：数组分组
来源：http://gxi.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://liy.wangshuangyany.cn

[U110] JS：数组分块
来源：http://kcz.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ngu.0kj1m.cn

[U111] JS：对象转 Map
来源：http://xju.vqdsnc.cn

new Map(Object.entries(obj))
来源：http://igp.cucudq.cn

[U112] JS：字符串补位
来源：http://smj.aibaodan.cn

"7".padStart(3, "0")
来源：http://hoo.yonumen.top

[U113] JS：正则替换全部
来源：http://jwj.yongpay.top

s.replaceAll("a", "b")
来源：http://jdv.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://nbs.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zwz.yueranfly.top

[U115] JS：生成 UUID
来源：http://xhk.guowangkeji.top

crypto.randomUUID()
来源：http://vtg.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://why.cucudq.cn

/** @param {string} name */ function f(name) {}
来源：http://tga.zhixingplan.top

[U117] JS：单元测试
来源：http://dvd.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://hhx.xinyue.icu

[U118] JS：开发服务器
来源：http://qsi.jqgfzy.top

npm i -D vite;  npx vite
来源：http://yvk.mhx1999.top

[U119] JS：生产构建
来源：http://bhk.epnwcf.com

npx vite build
来源：http://skn.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://rdl.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://xfk.daria6918.cn

================================================================================
来源：http://vmm.pycfn.com

统计汇总
来源：http://ize.daxiang520.top

================================================================================
来源：http://jkl.cqqwz.cn

按语言统计（条）：
来源：http://gku.nanxinkj.top

Python ......... 252
来源：http://iwu.cqqwz.cn

PHP ............ 252
来源：http://grs.nanxuanxn.top

JavaScript ..... 252
来源：http://woq.ehwqpu.com

TypeScript ..... 212
来源：http://mfz.meibo888.top

Java ........... 212
来源：http://eui.yj20258.top

Go ............. 212
来源：http://uop.hcnkem.com

Ruby ........... 212
来源：http://ypp.zhongyouzk.top

C# ............. 212
来源：http://wef.sweek.top

C .............. 30
来源：http://lqp.cucudq.cn

C++ ............ 30
来源：http://drb.daria6918.cn

SQL ............ 90
来源：http://tpg.cheryme.top

Bash ........... 80
来源：http://erj.guowangkeji.top

Kotlin ......... 15
来源：http://tvz.fengsongda.top

Swift .......... 15
来源：http://maa.aibaodan.cn

Lua ............ 10
来源：http://itn.jinghuilouyu.cn

Perl ........... 10
来源：http://kcx.jqgfzy.top

Scala .......... 10
来源：http://gyk.epnwcf.com

------------------------------------
来源：http://agj.fktsv.cn

合计 ........... 2106 条
来源：http://yux.guannengcc.top

按章节统计：
来源：http://dew.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sic.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jrm.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dsg.hammf.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kme.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://czl.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ppe.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mey.chenjidiqi.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wes.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hjo.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ssd.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bua.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cir.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kjl.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://con.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://elj.wangdashe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mya.quarkkingdee.top

Q SQL 专题                              90
来源：http://xok.sufxvd.cn

R Bash 专题                             80
来源：http://cld.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://kjg.sweek.top

T 其他语言补充                          60
来源：http://qkh.shangyingyoupin.top

U 高频实用片段                         120
来源：http://hxs.svipenyu.cn

------------------------------------
来源：http://rqr.9152youxi.cn

合计                                  2106 条
来源：http://seh.xylfe.cn

--------------------------------------------------------------------------------
来源：http://xpg.hysaishi.cn

使用提醒
来源：http://iej.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://lng.zycfv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yai.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hak.yj20258888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xvr.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://cns.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rwj.wangdashe.top

—— 文件结束 ——
来源：http://clm.jinqigufen.top

================================================================================
来源：http://aol.pycfn.com

程序语言常见例子速查手册（2024 版）
来源：http://wth.birdmap.top

Common Programming Examples Cheat Book
来源：http://ang.snrcjt.cn

================================================================================
来源：http://cbk.jiagoushi.top

【收录内容】
来源：http://ige.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ofl.nanxuanxn.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ike.9152youxi.cn

SQL · Bash · C · C++
来源：http://xpe.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gci.guannengcc.top

【使用说明】
来源：http://qfp.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hao.zhixingplan.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dpq.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cqq.dashuyun.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://izd.hcnkem.com

Bash:  Shell         C:     C             C++:   C++
来源：http://gpd.fehbvm.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qio.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rhe.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://esi.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jys.chenjidiqi.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hnr.sjlbkw.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xky.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kvx.guannengcc.top

【文件统计】
来源：http://bbg.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aqr.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://wvv.daxiang520.top

目  录
来源：http://rdq.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ilf.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://djh.redwolf501.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://grt.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fec.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yqn.bjfxy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kro.snrcjt.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bgc.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yuv.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ady.jqgfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gra.ppjwa.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://asj.xziqi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://juk.snrcjt.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qdb.gzhubu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fpy.mhx1999.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://prg.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mla.nanxuanxn.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wlt.52xcode.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yzk.chenzaomai.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://axa.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jjn.gaohongyu789.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mja.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nxc.haohaochexian.top

================================================================================
来源：http://nog.nanxinkj.top

A. 基础语法与类型
来源：http://xhv.svipenyu.cn

================================================================================
来源：http://fyu.jlsjyb.cn

[A01] Hello World
来源：http://fgj.smart0.xyz

Py:   print("Hello, World!")
来源：http://ddw.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://gdw.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://tqb.jinqigufen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nou.hesvh.cn


<!-- 参考信息 -->