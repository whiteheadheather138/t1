代发 wailian999

[U27] Py：异步 HTTP
来源：http://mou.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://fhv.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://shk.bbcook.cn

UserId = int
来源：http://wdo.sweek.top

[U29] Py：属性校验
来源：http://uqr.hnqzz.top

@property 与 @x.setter 配合
来源：http://kmd.wangdashe.top

[U30] Py：数据类
来源：http://uke.hesvh.cn

@dataclass(slots=True)
来源：http://ofv.pengpengdd.cyou

[U31] Py：单测
来源：http://zvg.epnwcf.com

python -m pytest -q
来源：http://axh.zhengqikj.top

[U32] Py：代码格式化
来源：http://hih.yvedp.cn

ruff format . && ruff check --fix .
来源：http://qsi.yj20258.top

[U33] Py：打包发布
来源：http://btf.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://skc.dashuyun.cn

[U34] Py：判断编码
来源：http://bvb.dianchejie.cn

chardet.detect(raw)
来源：http://tas.hnxiangtu.top

[U35] Py：发送邮件
来源：http://ihm.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aya.yangfankeji.com

[U36] Py：定时任务
来源：http://mwi.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://nwj.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://rjy.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://yti.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://iqy.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://zcy.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://zij.9152youxi.cn

sys.stdout.isatty()
来源：http://ttw.xziqi.cn

[U40] Py：打印到标准错误
来源：http://lrz.yangfankeji.com

print("err", file=sys.stderr)
来源：http://gmy.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://tkp.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bqt.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://lzs.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ppw.uphjek.com

[U43] PHP：声明命名空间
来源：http://kwj.tianlin.xyz

namespace App\Http;
来源：http://bsh.cdnleiting.top

[U44] PHP：开启严格类型
来源：http://mir.chenzaomai.com

declare(strict_types=1);
来源：http://xdr.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://fsl.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zyf.pycfn.com

[U46] PHP：可空类型
来源：http://ofw.yfazqb.com

?string $name = null
来源：http://ztz.hysaishi.cn

[U47] PHP：联合类型
来源：http://xle.xziqi.cn

int|string $id
来源：http://vhj.uphjek.com

[U48] PHP：纯枚举
来源：http://inr.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bij.tanke756.top

[U49] PHP：只读属性
来源：http://kez.ppjwa.cn

public readonly string $name
来源：http://gqo.yj202588.top

[U50] PHP：构造器属性提升
来源：http://cgb.tarul.cn

public function __construct(private int $id) {}
来源：http://fsg.fzhhl.top

[U51] PHP：数组解构
来源：http://kyg.hysaishi.cn

[$a, $b] = $arr;
来源：http://bxm.aibaodan.cn

[U52] PHP：箭头函数
来源：http://zyf.yj20258.top

$double = fn($x) => $x * 2;
来源：http://okq.ivvv.top

[U53] PHP：空合并运算符
来源：http://laj.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://akf.yueranfly.top

[U54] PHP：空安全调用
来源：http://uyn.xingfuxueyuan.xyz

$obj?->method()
来源：http://eiw.daxiang520.top

[U55] PHP：match 表达式
来源：http://zwf.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yow.xylfe.cn

[U56] PHP：命名参数
来源：http://epn.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://oea.zhoulong.xyz

[U57] PHP：字符串插值
来源：http://rhr.svipenyu.cn

"值: {$a}"
来源：http://zcs.dashuyun.cn

[U58] PHP：数组三件套
来源：http://kfi.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wos.hesvh.cn

[U59] PHP：自定义排序
来源：http://upp.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wxu.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://ieu.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wyd.snrcjt.cn

[U61] PHP：正则
来源：http://mgp.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fgg.zhongyouzk.top

[U62] PHP：日期对象
来源：http://ave.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://itk.chenlongwang.top

[U63] PHP：文件读写
来源：http://nbs.fehbvm.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ndr.fktsv.cn

[U64] PHP：目录遍历
来源：http://inu.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://hal.svipenyu.cn

[U65] PHP：会话
来源：http://fok.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ntp.chenjidiqi.icu

[U66] PHP：设置 Cookie
来源：http://qmb.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zrw.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://vux.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qkw.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://eer.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gso.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://utr.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fvc.guowangkeji.top

[U70] PHP：PDO 事务
来源：http://tcf.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blx.wangdashe.top

[U71] PHP：抛出异常
来源：http://spl.guannengcc.top

throw new RuntimeException("失败", 500);
来源：http://ytj.tanke756.top

[U72] PHP：写错误日志
来源：http://htv.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://dbq.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://zwo.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://crc.jianghu66.top

[U74] PHP：读取环境变量
来源：http://ulw.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://uay.yangfankeji.com

[U75] PHP：依赖注入
来源：http://woh.hcnkem.com

composer require psr/container
来源：http://wem.zdbjq.cn

[U76] PHP：简单路由
来源：http://tmc.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ebu.gogol.net.cn

[U77] PHP：模板渲染
来源：http://pha.pycfn.com

composer require twig/twig
来源：http://nyc.haohaochexian.top

[U78] PHP：单元测试
来源：http://byw.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://yal.bjfxy.top

[U79] PHP：静态分析
来源：http://qlr.yonumen.top

composer require --dev phpstan/phpstan
来源：http://wis.zdqjudy.top

[U80] PHP：代码规范修复
来源：http://zrq.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tgo.cdnleiting.top

[U81] JS：初始化项目
来源：http://dbo.smart0.xyz

npm init -y;  npm i express
来源：http://pji.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://gbe.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xvc.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://msz.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://hgs.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://rdh.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pny.jianghu66.top

[U85] JS：可选链
来源：http://imt.yuxming.cn

a?.b?.c
来源：http://zwp.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://hnj.shuidangran.top

a ?? b
来源：http://mvl.yvedp.cn

[U87] JS：解构默认值
来源：http://sml.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://mlt.sxryk.cn

[U88] JS：对象展开合并
来源：http://bkz.xinyue.icu

{ ...a, ...b }
来源：http://jit.gotoacloud.top

[U89] JS：数组去重
来源：http://gbg.yj202588.top

[...new Set(arr)]
来源：http://nmt.jinyuanbaomall.cn

[U90] JS：数字数组排序
来源：http://fwv.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://mri.jinghuilouyu.cn

[U91] JS：对象键值遍历
来源：http://zmk.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jma.cheryme.top

[U92] JS：深拷贝
来源：http://err.hcnkem.com

structuredClone(obj)
来源：http://uso.ydjk.org.cn

[U93] JS：模板字符串
来源：http://igr.shanyushiyangtech.top

`共 ${n} 条`
来源：http://tcu.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://oub.0kj1m.cn

const double = x => x * 2;
来源：http://rxe.snrcjt.cn

[U95] JS：Promise 包装
来源：http://bxc.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://psx.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://pgc.gogol.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://khq.sweek.top

[U97] JS：并发请求
来源：http://ezq.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ptg.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://ves.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qlq.gaohongyu789.top

[U99] JS：事件监听
来源：http://xvb.c1oappe.top

el.addEventListener("click", e => {})
来源：http://kon.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://djw.gaohongyu789.top

document.querySelector(".item")
来源：http://csn.yuxming.cn

[U101] JS：classList 操作
来源：http://ssi.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://ymd.jinyuanbaomall.cn

[U102] JS：本地存储
来源：http://opu.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://boi.jyoumei.cn

[U103] JS：定时器
来源：http://clg.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mgj.daria6918.cn

[U104] JS：防抖
来源：http://yus.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oao.vqdsnc.cn

[U105] JS：节流
来源：http://nso.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ywc.ehwqpu.com

[U106] JS：日期格式化
来源：http://rmb.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rnl.xziqi.cn

[U107] JS：数字千分位
来源：http://kib.fzhhl.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gsi.tarul.cn

[U108] JS：随机整数
来源：http://gea.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://afq.haohaochexian.top

[U109] JS：数组分组
来源：http://knd.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://tks.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://jcr.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hgu.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://gpj.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://dbs.andypj.xyz

[U112] JS：字符串补位
来源：http://ltu.sjlbkw.cn

"7".padStart(3, "0")
来源：http://imf.xinyue.icu

[U113] JS：正则替换全部
来源：http://nnk.yuxming.cn

s.replaceAll("a", "b")
来源：http://bru.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://qie.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zbx.uphjek.com

[U115] JS：生成 UUID
来源：http://pxd.jinqigufen.top

crypto.randomUUID()
来源：http://xox.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://zcs.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://vwk.ppjwa.cn

[U117] JS：单元测试
来源：http://lob.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://blp.dashuyun.cn

[U118] JS：开发服务器
来源：http://uch.tanke756.top

npm i -D vite;  npx vite
来源：http://kvh.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://vfq.fengsongda.top

npx vite build
来源：http://btk.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://hgw.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://ytc.ppjwa.cn

================================================================================
来源：http://jwh.snrcjt.cn

统计汇总
来源：http://snb.zycfv.cn

================================================================================
来源：http://pyu.hysaishi.cn

按语言统计（条）：
来源：http://mes.chenlongwang.top

Python ......... 252
来源：http://xsd.yj20258888.top

PHP ............ 252
来源：http://rxa.hammf.cn

JavaScript ..... 252
来源：http://zml.yanxiufei.cn

TypeScript ..... 212
来源：http://wxm.gzhubu.top

Java ........... 212
来源：http://bcp.snrcjt.cn

Go ............. 212
来源：http://ork.0kj1m.cn

Ruby ........... 212
来源：http://jcu.jinqigfzy.top

C# ............. 212
来源：http://nmi.ivvv.top

C .............. 30
来源：http://arc.shangyingyoupin.top

C++ ............ 30
来源：http://oub.fehbvm.com

SQL ............ 90
来源：http://mme.fehbvm.com

Bash ........... 80
来源：http://udz.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://hth.iojbl.cn

Swift .......... 15
来源：http://ukt.guowangkeji.top

Lua ............ 10
来源：http://sba.wangshuangyany.cn

Perl ........... 10
来源：http://qlr.hfpthk.cn

Scala .......... 10
来源：http://ofy.zhoulong.xyz

------------------------------------
来源：http://ijg.hcnkem.com

合计 ........... 2106 条
来源：http://cot.daxiang520.top

按章节统计：
来源：http://thm.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sgj.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iwo.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ywj.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sug.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qjt.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hwf.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gwy.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wpb.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://shm.guannengcc.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ivp.nanxuanxn.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tnb.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dfo.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qbh.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wne.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://twu.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kqt.feifeiyinyue.top

Q SQL 专题                              90
来源：http://ppq.smart0.xyz

R Bash 专题                             80
来源：http://fkg.ydjk.org.cn

S C / C++ 专题                          60
来源：http://xcz.hfpthk.cn

T 其他语言补充                          60
来源：http://zcr.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://cqb.cqqwz.cn

------------------------------------
来源：http://htk.yuxming.cn

合计                                  2106 条
来源：http://gig.cheryme.top

--------------------------------------------------------------------------------
来源：http://uwm.yonumen.top

使用提醒
来源：http://xia.redwolf501.top

--------------------------------------------------------------------------------
来源：http://ojs.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ptq.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kbc.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bpb.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://acm.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://urz.gaohongyu789.top

—— 文件结束 ——
来源：http://eel.pycfn.com

================================================================================
来源：http://bmp.yongpay.top

程序语言常见例子速查手册（2024 版）
来源：http://jae.bbcook.cn

Common Programming Examples Cheat Book
来源：http://ncs.bjfxy.top

================================================================================
来源：http://gdl.cashguo.top

【收录内容】
来源：http://uze.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ous.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jau.aizwys.cn

SQL · Bash · C · C++
来源：http://rez.jqgufenzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://juu.nanxuanxn.top

【使用说明】
来源：http://hid.jinqigufen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uag.xuanzx.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qpn.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jev.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dmk.ivvv.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qcd.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://scy.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://csu.daria6918.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zhj.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xry.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ihd.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jql.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bav.wangshuangyany.cn

【文件统计】
来源：http://roq.cheryme.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://flv.shuidangran.top

--------------------------------------------------------------------------------
来源：http://pwt.jinghuilouyu.cn

目  录
来源：http://tnf.yueranfly.top

--------------------------------------------------------------------------------
来源：http://rgn.sweek.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dnx.jinghuilouyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://erb.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bsh.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qzd.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bds.jqgfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ruo.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dgd.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pks.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hij.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mnc.shangyingyoupin.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rpe.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ytz.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://epb.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qus.shanyushiyangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hbg.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dwp.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qpk.chenzaomai.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://yzl.jqgfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://knp.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fsp.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pki.vehdjk.com

================================================================================
来源：http://pye.havefunace.top

A. 基础语法与类型
来源：http://ihd.haohaochexian.top

================================================================================
来源：http://yso.dianchejie.cn

[A01] Hello World
来源：http://jmi.svipenyu.cn

Py:   print("Hello, World!")
来源：http://cgu.zhijiandao.cn

PHP:  echo "Hello, World!";
来源：http://cap.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://btr.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aay.xuanzx.com


<!-- 参考信息 -->