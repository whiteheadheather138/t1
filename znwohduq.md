代发 wailian999

[U25] Py：CSV 按字典读
来源：http://sbh.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://wio.yongpay.top

[U26] Py：并发下载
来源：http://mpk.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zoa.feifeiyinyue.top

[U27] Py：异步 HTTP
来源：http://cbx.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://hos.iojbl.cn

[U28] Py：类型别名
来源：http://ief.nanxinkj.top

UserId = int
来源：http://mxu.ydzc1.top

[U29] Py：属性校验
来源：http://bwk.zycfv.cn

@property 与 @x.setter 配合
来源：http://mpq.52xcode.cn

[U30] Py：数据类
来源：http://vot.pycfn.com

@dataclass(slots=True)
来源：http://piv.xziqi.cn

[U31] Py：单测
来源：http://xos.zycfv.cn

python -m pytest -q
来源：http://uev.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://mit.316326.xyz

ruff format . && ruff check --fix .
来源：http://qyx.yongpay.top

[U33] Py：打包发布
来源：http://ctm.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://lpv.yuanzhike.top

[U34] Py：判断编码
来源：http://aeg.xinyue.icu

chardet.detect(raw)
来源：http://ryy.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://uzb.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yno.c1oappe.top

[U36] Py：定时任务
来源：http://cgy.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://tno.yongpay.top

[U37] Py：读写 Excel
来源：http://vhm.ydjk.org.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ces.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://aro.yangfankeji.com

Path(__file__).resolve().parent
来源：http://stz.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://gia.zdbjq.cn

sys.stdout.isatty()
来源：http://ook.bjfxy.top

[U40] Py：打印到标准错误
来源：http://bmp.smart0.xyz

print("err", file=sys.stderr)
来源：http://cwe.hnxiangtu.top

[U41] PHP：初始化 Composer 项目
来源：http://lle.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://log.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://oik.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nbr.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://irq.yuanzhike.top

namespace App\Http;
来源：http://ejz.andypj.xyz

[U44] PHP：开启严格类型
来源：http://job.jianghu66.top

declare(strict_types=1);
来源：http://aai.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://yfy.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://jpt.hesvh.cn

[U46] PHP：可空类型
来源：http://ynd.cdnleiting.top

?string $name = null
来源：http://mvo.ydzc1.top

[U47] PHP：联合类型
来源：http://xgu.sjlbkw.cn

int|string $id
来源：http://nsb.sxryk.cn

[U48] PHP：纯枚举
来源：http://dds.hfpthk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rov.gzhubu.top

[U49] PHP：只读属性
来源：http://lcp.ydjk.org.cn

public readonly string $name
来源：http://xgu.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://tjk.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://rog.jianghu66.top

[U51] PHP：数组解构
来源：http://xio.xinyue.icu

[$a, $b] = $arr;
来源：http://xgz.bjfxy.top

[U52] PHP：箭头函数
来源：http://kod.birdmap.top

$double = fn($x) => $x * 2;
来源：http://blg.fzhhl.top

[U53] PHP：空合并运算符
来源：http://ijg.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://lkp.redwolf501.top

[U54] PHP：空安全调用
来源：http://mfn.jqgfzy.top

$obj?->method()
来源：http://num.tarul.cn

[U55] PHP：match 表达式
来源：http://qpr.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ioh.birdmap.top

[U56] PHP：命名参数
来源：http://tlt.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://hpp.guowangkeji.top

[U57] PHP：字符串插值
来源：http://gnf.zhengqikj.top

"值: {$a}"
来源：http://xmn.yongpay.top

[U58] PHP：数组三件套
来源：http://xfn.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lvn.havefunace.top

[U59] PHP：自定义排序
来源：http://grw.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wtf.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://zij.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nwl.bbcook.cn

[U61] PHP：正则
来源：http://gdz.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://klf.bjfxy.top

[U62] PHP：日期对象
来源：http://zkm.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vqp.zhixingplan.top

[U63] PHP：文件读写
来源：http://vgl.quarkkingdee.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nhf.fanxiaobao.xyz

[U64] PHP：目录遍历
来源：http://bjm.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://glp.bbcook.cn

[U65] PHP：会话
来源：http://oas.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mnt.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://wvh.haohaochexian.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dzr.tanke756.top

[U67] PHP：处理文件上传
来源：http://odm.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zft.yj20258888.top

[U68] PHP：PDO 连接
来源：http://rqy.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qql.ydjk.org.cn

[U69] PHP：PDO 预处理
来源：http://ljp.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aow.sxryk.cn

[U70] PHP：PDO 事务
来源：http://sfk.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oqa.fktsv.cn

[U71] PHP：抛出异常
来源：http://blx.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://oir.jiagoushi.top

[U72] PHP：写错误日志
来源：http://kje.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://jkg.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://xbq.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://vui.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://dhx.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://tbs.cdnleiting.top

[U75] PHP：依赖注入
来源：http://mtg.zycfv.cn

composer require psr/container
来源：http://koo.ppjwa.cn

[U76] PHP：简单路由
来源：http://pla.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hun.uphjek.com

[U77] PHP：模板渲染
来源：http://hts.fzhhl.top

composer require twig/twig
来源：http://vyh.cucudq.cn

[U78] PHP：单元测试
来源：http://hpm.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://uhe.hysaishi.cn

[U79] PHP：静态分析
来源：http://uem.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://oye.fengsongda.top

[U80] PHP：代码规范修复
来源：http://dbc.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://tfy.jqgfzy.top

[U81] JS：初始化项目
来源：http://mql.fzhhl.top

npm init -y;  npm i express
来源：http://mls.fengsongda.top

[U82] JS：package.json 脚本
来源：http://wil.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nbz.fzhhl.top

[U83] JS：ES Module 导入导出
来源：http://bae.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://lpm.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://btu.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rfl.yonumen.top

[U85] JS：可选链
来源：http://ucj.hysaishi.cn

a?.b?.c
来源：http://xkc.zdbjq.cn

[U86] JS：空值合并
来源：http://kys.cdnleiting.top

a ?? b
来源：http://fmu.kuanghao11.cn

[U87] JS：解构默认值
来源：http://ljs.wangdashe.top

const { a = 1, b = 2 } = obj;
来源：http://zly.dianchejie.cn

[U88] JS：对象展开合并
来源：http://ugw.shzxlz.cn

{ ...a, ...b }
来源：http://htt.gogol.net.cn

[U89] JS：数组去重
来源：http://jon.zhoulong.xyz

[...new Set(arr)]
来源：http://ysy.havefunace.top

[U90] JS：数字数组排序
来源：http://bai.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://lvx.daxiang520.top

[U91] JS：对象键值遍历
来源：http://peo.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xbw.xinyue.icu

[U92] JS：深拷贝
来源：http://cru.yueranfly.top

structuredClone(obj)
来源：http://org.andypj.xyz

[U93] JS：模板字符串
来源：http://ojr.kuanghao11.cn

`共 ${n} 条`
来源：http://ije.hysaishi.cn

[U94] JS：箭头函数
来源：http://icd.kuanghao11.cn

const double = x => x * 2;
来源：http://llm.sweek.top

[U95] JS：Promise 包装
来源：http://xdy.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://ldh.bjfxy.top

[U96] JS：async/await 与异常
来源：http://qsw.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ljv.zhengqikj.top

[U97] JS：并发请求
来源：http://zbf.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eqc.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://xgh.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zji.yvedp.cn

[U99] JS：事件监听
来源：http://mus.pycfn.com

el.addEventListener("click", e => {})
来源：http://cic.cheryme.top

[U100] JS：DOM 查询
来源：http://vab.shzxlz.cn

document.querySelector(".item")
来源：http://wnm.cdnleiting.top

[U101] JS：classList 操作
来源：http://xnp.xuanzx.com

el.classList.toggle("active")
来源：http://dmk.jinqigufen.top

[U102] JS：本地存储
来源：http://kns.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cqy.sufxvd.cn

[U103] JS：定时器
来源：http://ckh.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vdo.fzhhl.top

[U104] JS：防抖
来源：http://slx.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jii.chenlongwang.top

[U105] JS：节流
来源：http://adn.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://szu.yvedp.cn

[U106] JS：日期格式化
来源：http://kjd.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qyg.dashuyun.cn

[U107] JS：数字千分位
来源：http://kuy.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qtk.jinqigufen.top

[U108] JS：随机整数
来源：http://nab.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hlr.vehdjk.com

[U109] JS：数组分组
来源：http://qik.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://xqp.fengsongda.top

[U110] JS：数组分块
来源：http://byb.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wah.bjfxy.top

[U111] JS：对象转 Map
来源：http://mwp.cdnleiting.top

new Map(Object.entries(obj))
来源：http://jgi.jqgufenzy.top

[U112] JS：字符串补位
来源：http://qgk.yj202588.top

"7".padStart(3, "0")
来源：http://plc.guowangkeji.top

[U113] JS：正则替换全部
来源：http://iyp.cucudq.cn

s.replaceAll("a", "b")
来源：http://rjm.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://lcq.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vkz.hcnkem.com

[U115] JS：生成 UUID
来源：http://lcu.dashuyun.cn

crypto.randomUUID()
来源：http://bva.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://uig.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://trj.9152youxi.cn

[U117] JS：单元测试
来源：http://ywa.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://yxv.tanke756.top

[U118] JS：开发服务器
来源：http://kgv.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://zpd.zhoulong.xyz

[U119] JS：生产构建
来源：http://nee.ehwqpu.com

npx vite build
来源：http://los.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://swf.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://dvo.yj20258888.top

================================================================================
来源：http://lzr.ehwqpu.com

统计汇总
来源：http://ytl.jinyuanbaomall.cn

================================================================================
来源：http://vsd.hammf.cn

按语言统计（条）：
来源：http://bvp.jqgfzy.top

Python ......... 252
来源：http://rgl.jinghuilouyu.cn

PHP ............ 252
来源：http://hkc.316326.xyz

JavaScript ..... 252
来源：http://ioq.vqdsnc.cn

TypeScript ..... 212
来源：http://kvo.shangyingyoupin.top

Java ........... 212
来源：http://ask.shzxlz.cn

Go ............. 212
来源：http://wch.svipenyu.cn

Ruby ........... 212
来源：http://gju.nanxinkj.top

C# ............. 212
来源：http://yso.chenzaomai.com

C .............. 30
来源：http://ift.daria6918.cn

C++ ............ 30
来源：http://muc.cdnleiting.top

SQL ............ 90
来源：http://biu.dashuyun.cn

Bash ........... 80
来源：http://cco.guowangkeji.top

Kotlin ......... 15
来源：http://pxh.jqgfzy.top

Swift .......... 15
来源：http://dgy.gaohongyu789.top

Lua ............ 10
来源：http://veh.fehbvm.com

Perl ........... 10
来源：http://sjg.yj20258.top

Scala .......... 10
来源：http://xnz.xuanzx.com

------------------------------------
来源：http://vrm.yongpay.top

合计 ........... 2106 条
来源：http://uxm.sysykeji.top

按章节统计：
来源：http://ynd.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://htv.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://izq.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://txa.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xxu.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://txh.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jjb.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nvq.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qra.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tzd.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qdu.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ylj.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kxv.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rot.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rwa.hnqzz.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zxs.andypj.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lod.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://saj.havefunace.top

R Bash 专题                             80
来源：http://dtp.zhiwuduotai.top

S C / C++ 专题                          60
来源：http://wzo.tian-w.cn

T 其他语言补充                          60
来源：http://kyc.ybcxt.top

U 高频实用片段                         120
来源：http://rzn.kuanghao11.cn

------------------------------------
来源：http://tje.bjfxy.top

合计                                  2106 条
来源：http://bjc.uphjek.com

--------------------------------------------------------------------------------
来源：http://tni.yj202588.top

使用提醒
来源：http://ylp.shuidangran.top

--------------------------------------------------------------------------------
来源：http://iow.tarul.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kcq.yangfankeji.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ruk.jinqigfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://whh.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zrn.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jek.hammf.cn

—— 文件结束 ——
来源：http://dww.ivvv.top

================================================================================
来源：http://yoe.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://rpt.gzhubu.top

Common Programming Examples Cheat Book
来源：http://gjk.smart0.xyz

================================================================================
来源：http://fob.wangdashe.top

【收录内容】
来源：http://ckt.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zwv.tianlin.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://atf.zhongyouzk.top

SQL · Bash · C · C++
来源：http://jix.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ljy.ybcxt.top

【使用说明】
来源：http://uaz.ydzc1.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pvm.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qmb.hammf.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kdw.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ncq.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jzr.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://box.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kgy.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rgz.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://olq.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cwl.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ebz.xziqi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jwb.316326.xyz

【文件统计】
来源：http://xcn.yvedp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://txb.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://ssc.yueranfly.top

目  录
来源：http://dfe.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://ydm.quarkkingdee.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://onn.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zrj.xuetiantiany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mev.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fna.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dsq.nwbrower.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zlo.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kou.sufxvd.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kky.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://arg.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ksc.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uba.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qqm.guannengcc.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mmm.smart0.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://axz.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nfb.hcnkem.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://opi.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ejy.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://asu.shzxlz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dot.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qqd.xziqi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tor.ivvv.top

================================================================================
来源：http://gim.shanyushiyangtech.top

A. 基础语法与类型
来源：http://gfz.ybcxt.top

================================================================================
来源：http://zje.ctjpmb.com

[A01] Hello World
来源：http://lbd.shuidangran.top


<!-- 参考信息 -->