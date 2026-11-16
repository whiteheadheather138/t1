代发 wailian999

[U25] Py：CSV 按字典读
来源：http://ccp.daria6918.cn

csv.DictReader(f)
来源：http://gkm.sxryk.cn

[U26] Py：并发下载
来源：http://kgm.jlsjyb.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ujg.smart0.xyz

[U27] Py：异步 HTTP
来源：http://ubm.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://kor.iojbl.cn

[U28] Py：类型别名
来源：http://nfc.shanyushiyangkeji.top

UserId = int
来源：http://clh.yuanzhike.top

[U29] Py：属性校验
来源：http://xiu.xinyue.icu

@property 与 @x.setter 配合
来源：http://jbz.hywenlv.cn

[U30] Py：数据类
来源：http://fvr.fengsongda.top

@dataclass(slots=True)
来源：http://ydr.bjfxy.top

[U31] Py：单测
来源：http://dbw.9152youxi.cn

python -m pytest -q
来源：http://rlh.tian-w.cn

[U32] Py：代码格式化
来源：http://qtp.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://gju.jinqigfzy.top

[U33] Py：打包发布
来源：http://mic.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://klb.svipenyu.cn

[U34] Py：判断编码
来源：http://miv.jiagoushi.top

chardet.detect(raw)
来源：http://jyx.yj202588.top

[U35] Py：发送邮件
来源：http://lyp.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://toz.pengpengdd.cyou

[U36] Py：定时任务
来源：http://slk.fanxiaobao.xyz

schedule.every(10).minutes.do(job)
来源：http://elc.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://rly.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jqm.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://noo.haohaochexian.top

Path(__file__).resolve().parent
来源：http://sso.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://qbt.guowangkeji.top

sys.stdout.isatty()
来源：http://ywf.yvedp.cn

[U40] Py：打印到标准错误
来源：http://npu.daria6918.cn

print("err", file=sys.stderr)
来源：http://iem.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ooz.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://lfx.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://kni.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zut.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://cre.ivvv.top

namespace App\Http;
来源：http://lxo.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://dvp.tian-w.cn

declare(strict_types=1);
来源：http://pwr.shanyushiyangtech.top

[U45] PHP：类型声明与返回类型
来源：http://led.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lhf.xuanzx.com

[U46] PHP：可空类型
来源：http://awr.fehbvm.com

?string $name = null
来源：http://teg.yj202588.top

[U47] PHP：联合类型
来源：http://zat.sxryk.cn

int|string $id
来源：http://hit.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://sdj.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rwy.hnxiangtu.top

[U49] PHP：只读属性
来源：http://jum.hnqzz.top

public readonly string $name
来源：http://hnm.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://len.shzxlz.cn

public function __construct(private int $id) {}
来源：http://fng.jinqigfzy.top

[U51] PHP：数组解构
来源：http://aln.sxryk.cn

[$a, $b] = $arr;
来源：http://vyb.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://uic.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://swr.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://nxd.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://ztj.wangdashe.top

[U54] PHP：空安全调用
来源：http://ipp.zdbjq.cn

$obj?->method()
来源：http://geh.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://wom.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://acp.havefunace.top

[U56] PHP：命名参数
来源：http://lii.yueranfly.top

f(a: 1, b: 2)
来源：http://fgz.yj20258.top

[U57] PHP：字符串插值
来源：http://mud.cashguo.top

"值: {$a}"
来源：http://fqr.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://sxm.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nog.guannengcc.top

[U59] PHP：自定义排序
来源：http://gkk.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hmb.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://fra.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gqp.ybcxt.top

[U61] PHP：正则
来源：http://tsg.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lww.cucudq.cn

[U62] PHP：日期对象
来源：http://kqc.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://abj.wangshuangyany.cn

[U63] PHP：文件读写
来源：http://npw.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rdt.meibo888.top

[U64] PHP：目录遍历
来源：http://vmy.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://uco.yfazqb.com

[U65] PHP：会话
来源：http://tzn.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ioh.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://fel.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jhh.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://yoc.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://obd.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://jkl.yangfankeji.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pyw.jinyuanbaomall.cn

[U69] PHP：PDO 预处理
来源：http://wyi.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bfd.andypj.xyz

[U70] PHP：PDO 事务
来源：http://axj.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tnc.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://ihb.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://onv.nanxinkj.top

[U72] PHP：写错误日志
来源：http://okb.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://rfj.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://jpb.yonumen.top

parse_ini_file("config.ini", true)
来源：http://dlg.guannengcc.top

[U74] PHP：读取环境变量
来源：http://mqn.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://ooi.yuanzhike.top

[U75] PHP：依赖注入
来源：http://dlq.tian-w.cn

composer require psr/container
来源：http://rjx.sysykeji.top

[U76] PHP：简单路由
来源：http://loi.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wll.cqqwz.cn

[U77] PHP：模板渲染
来源：http://ezn.shanyushiyangkeji.top

composer require twig/twig
来源：http://ymn.ydjk.org.cn

[U78] PHP：单元测试
来源：http://zhu.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://xxm.sjlbkw.cn

[U79] PHP：静态分析
来源：http://qir.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://ucp.cheryme.top

[U80] PHP：代码规范修复
来源：http://onu.jinyuanbaomall.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rhc.yfazqb.com

[U81] JS：初始化项目
来源：http://ots.hnxiangtu.top

npm init -y;  npm i express
来源：http://nmw.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://fxp.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xis.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://ueb.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yba.hysaishi.cn

[U84] JS：CommonJS 写法
来源：http://duo.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vid.jlsjyb.cn

[U85] JS：可选链
来源：http://ceu.jiagoushi.top

a?.b?.c
来源：http://pff.pycfn.com

[U86] JS：空值合并
来源：http://avd.smart0.xyz

a ?? b
来源：http://kmm.ctjpmb.com

[U87] JS：解构默认值
来源：http://njr.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://nyt.meibo888.top

[U88] JS：对象展开合并
来源：http://hai.yj20258.top

{ ...a, ...b }
来源：http://azn.hcnkem.com

[U89] JS：数组去重
来源：http://bvw.gogol.net.cn

[...new Set(arr)]
来源：http://izm.yj20258.top

[U90] JS：数字数组排序
来源：http://cih.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://ovs.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://gms.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pdp.yj20258.top

[U92] JS：深拷贝
来源：http://khm.0kj1m.cn

structuredClone(obj)
来源：http://lsp.guannengcc.top

[U93] JS：模板字符串
来源：http://lsv.yj20258.top

`共 ${n} 条`
来源：http://qcg.yuanzhike.top

[U94] JS：箭头函数
来源：http://hbl.jinghuilouyu.cn

const double = x => x * 2;
来源：http://fyl.svipenyu.cn

[U95] JS：Promise 包装
来源：http://lnm.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://toj.shuidangran.top

[U96] JS：async/await 与异常
来源：http://ftx.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://auz.nanxinkj.top

[U97] JS：并发请求
来源：http://xmg.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xod.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://qyh.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vgo.cashguo.top

[U99] JS：事件监听
来源：http://anj.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://iyo.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://vmp.cashguo.top

document.querySelector(".item")
来源：http://vev.cashguo.top

[U101] JS：classList 操作
来源：http://qtw.ivvv.top

el.classList.toggle("active")
来源：http://kpj.dianchejie.cn

[U102] JS：本地存储
来源：http://fxl.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uzm.vqdsnc.cn

[U103] JS：定时器
来源：http://aop.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mpz.0kj1m.cn

[U104] JS：防抖
来源：http://hxx.c1oappe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fyr.nwbrower.top

[U105] JS：节流
来源：http://lwt.guowangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bfo.gogol.net.cn

[U106] JS：日期格式化
来源：http://dlx.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qvi.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://dzd.ydjk.org.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zom.dashuyun.cn

[U108] JS：随机整数
来源：http://upb.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fyy.guannengcc.top

[U109] JS：数组分组
来源：http://dnd.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://nxn.guannengcc.top

[U110] JS：数组分块
来源：http://ymg.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zqc.chenlongwang.top

[U111] JS：对象转 Map
来源：http://ikp.jinqigufen.top

new Map(Object.entries(obj))
来源：http://uvg.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://xnq.yvedp.cn

"7".padStart(3, "0")
来源：http://tzr.tarul.cn

[U113] JS：正则替换全部
来源：http://bay.mhx1999.top

s.replaceAll("a", "b")
来源：http://cbp.fktsv.cn

[U114] JS：JSON 深比较
来源：http://dyp.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pyj.hcnkem.com

[U115] JS：生成 UUID
来源：http://vzd.wangdashe.top

crypto.randomUUID()
来源：http://xqg.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://sjo.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://buv.nwbrower.top

[U117] JS：单元测试
来源：http://wsz.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://ftf.wangdashe.top

[U118] JS：开发服务器
来源：http://gow.uphjek.com

npm i -D vite;  npx vite
来源：http://ziw.yj202588.top

[U119] JS：生产构建
来源：http://fmt.ivvv.top

npx vite build
来源：http://aev.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://ram.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://yqs.c1oappe.top

================================================================================
来源：http://ysg.fktsv.cn

统计汇总
来源：http://nol.tarul.cn

================================================================================
来源：http://zrp.xuetiantiany.cn

按语言统计（条）：
来源：http://nru.pengpengdd.cyou

Python ......... 252
来源：http://ozo.xuetiantiany.cn

PHP ............ 252
来源：http://kze.gzhubu.top

JavaScript ..... 252
来源：http://hyk.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://dub.yuanzhike.top

Java ........... 212
来源：http://rto.vehdjk.com

Go ............. 212
来源：http://jyg.zhongyouzk.top

Ruby ........... 212
来源：http://axl.snrcjt.cn

C# ............. 212
来源：http://xmq.yfazqb.com

C .............. 30
来源：http://tgb.vqdsnc.cn

C++ ............ 30
来源：http://war.ydjk.org.cn

SQL ............ 90
来源：http://ktc.fanxiaobao.xyz

Bash ........... 80
来源：http://bfg.smart0.xyz

Kotlin ......... 15
来源：http://ynb.zycfv.cn

Swift .......... 15
来源：http://wtk.snrcjt.cn

Lua ............ 10
来源：http://nyc.hywenlv.cn

Perl ........... 10
来源：http://haa.redwolf501.top

Scala .......... 10
来源：http://rpf.ivvv.top

------------------------------------
来源：http://wdn.sufxvd.cn

合计 ........... 2106 条
来源：http://kej.nanxinkj.top

按章节统计：
来源：http://zqj.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ruj.guowangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dug.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ibu.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jbs.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tud.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dmy.aibaodan.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aqh.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bgo.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qub.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://osn.yueranfly.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vta.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nwv.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vnh.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ako.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ptn.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ndc.epnwcf.com

Q SQL 专题                              90
来源：http://pzw.tianlin.xyz

R Bash 专题                             80
来源：http://vkv.tian-w.cn

S C / C++ 专题                          60
来源：http://jqo.haohaochexian.top

T 其他语言补充                          60
来源：http://ity.tianlin.xyz

U 高频实用片段                         120
来源：http://zgq.shuidangran.top

------------------------------------
来源：http://idc.mhx1999.top

合计                                  2106 条
来源：http://haf.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://kcb.jinyuanbaomall.cn

使用提醒
来源：http://bfx.hammf.cn

--------------------------------------------------------------------------------
来源：http://jjh.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fjv.hfpthk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wtv.havefunace.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ecc.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jdy.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xxc.xuetiantiany.cn

—— 文件结束 ——
来源：http://lrn.jiagoushi.top

================================================================================
来源：http://vam.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://tph.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://bvm.vqdsnc.cn

================================================================================
来源：http://wzb.yj202588.top

【收录内容】
来源：http://tco.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ltc.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bsi.c1oappe.top

SQL · Bash · C · C++
来源：http://ssp.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ieu.tianlin.xyz

【使用说明】
来源：http://bhd.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yqu.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kzv.yj202588.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://icb.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nsv.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wfk.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fam.haohaochexian.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yzf.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://efy.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qdp.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vdp.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vxq.cashguo.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hxa.jiagoushi.top

【文件统计】
来源：http://iym.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jti.mhx1999.top

--------------------------------------------------------------------------------
来源：http://zji.yonumen.top

目  录
来源：http://mby.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://odg.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wlh.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nbt.zhengqikj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qmf.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://imc.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jdw.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tcy.fanxiaobao.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eic.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uxw.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nkd.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lgm.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ddz.chenlongwang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pjj.sufxvd.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mtc.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wfo.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ibe.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dvi.fehbvm.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://izz.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uia.guowangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jse.shanyushiyangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jjq.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bwe.vehdjk.com

================================================================================
来源：http://nsb.ivvv.top

A. 基础语法与类型
来源：http://dpb.jianghu66.top

================================================================================
来源：http://mmz.jlsjyb.cn

[A01] Hello World
来源：http://bui.jiagoushi.top


<!-- 参考信息 -->