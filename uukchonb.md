代发 wailian999

[U23] Py：分块读取大文件
来源：http://cna.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zgd.hnxiangtu.top

[U24] Py：路径操作
来源：http://tbw.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://knr.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://nbo.ctjpmb.com

csv.DictReader(f)
来源：http://zgu.fktsv.cn

[U26] Py：并发下载
来源：http://bku.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dch.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://eee.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://vcr.yueranfly.top

[U28] Py：类型别名
来源：http://rdv.sjlbkw.cn

UserId = int
来源：http://mgp.cashguo.top

[U29] Py：属性校验
来源：http://syc.vehdjk.com

@property 与 @x.setter 配合
来源：http://ins.yueranfly.top

[U30] Py：数据类
来源：http://zyp.hammf.cn

@dataclass(slots=True)
来源：http://owj.ctjpmb.com

[U31] Py：单测
来源：http://ihh.fanxiaobao.xyz

python -m pytest -q
来源：http://wyd.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://oio.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://bru.ydzc1.top

[U33] Py：打包发布
来源：http://edv.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://zqz.shangyingyoupin.top

[U34] Py：判断编码
来源：http://asq.quarkkingdee.top

chardet.detect(raw)
来源：http://hhk.jyoumei.cn

[U35] Py：发送邮件
来源：http://tka.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://niu.zhengqikj.top

[U36] Py：定时任务
来源：http://pgw.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://vou.wangshuangyany.cn

[U37] Py：读写 Excel
来源：http://qod.hongshengwenyu.top

pandas.read_excel / DataFrame.to_excel
来源：http://wqu.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://edt.redwolf501.top

Path(__file__).resolve().parent
来源：http://mem.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://cqu.nanxuanxn.top

sys.stdout.isatty()
来源：http://lww.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://dyv.jyoumei.cn

print("err", file=sys.stderr)
来源：http://pmo.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://nhz.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vic.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://myu.hywenlv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rsv.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://cui.zhijiandao.cn

namespace App\Http;
来源：http://siu.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://fyq.yuanzhike.top

declare(strict_types=1);
来源：http://ffj.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://esg.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hvu.hcnkem.com

[U46] PHP：可空类型
来源：http://jks.fanxiaobao.xyz

?string $name = null
来源：http://rqv.cheryme.top

[U47] PHP：联合类型
来源：http://wzf.birdmap.top

int|string $id
来源：http://xkt.bbcook.cn

[U48] PHP：纯枚举
来源：http://lwy.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ryd.zdqjudy.top

[U49] PHP：只读属性
来源：http://qkf.jqgufenzy.top

public readonly string $name
来源：http://owb.chenjidiqi.icu

[U50] PHP：构造器属性提升
来源：http://qsp.mhx1999.top

public function __construct(private int $id) {}
来源：http://mio.yj202588.top

[U51] PHP：数组解构
来源：http://yth.jianghu66.top

[$a, $b] = $arr;
来源：http://pkk.cqqwz.cn

[U52] PHP：箭头函数
来源：http://ntc.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://nlv.fehbvm.com

[U53] PHP：空合并运算符
来源：http://hlr.zhongyouzk.top

$v = $a ?? $b ?? "default";
来源：http://olf.yanxiufei.cn

[U54] PHP：空安全调用
来源：http://swu.iojbl.cn

$obj?->method()
来源：http://gjr.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://bct.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xji.fzhhl.top

[U56] PHP：命名参数
来源：http://mmf.jinqigfzy.top

f(a: 1, b: 2)
来源：http://aed.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://rxm.meibo888.top

"值: {$a}"
来源：http://tbm.aizwys.cn

[U58] PHP：数组三件套
来源：http://xod.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yia.yueranfly.top

[U59] PHP：自定义排序
来源：http://nls.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vzd.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://dge.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jst.yangfankeji.com

[U61] PHP：正则
来源：http://rsi.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://llk.havefunace.top

[U62] PHP：日期对象
来源：http://vct.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ddm.aizwys.cn

[U63] PHP：文件读写
来源：http://ybt.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gbu.c1oappe.top

[U64] PHP：目录遍历
来源：http://yhp.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://qrl.316326.xyz

[U65] PHP：会话
来源：http://bny.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://lde.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://sdd.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://idz.pycfn.com

[U67] PHP：处理文件上传
来源：http://htb.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ztg.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://yfu.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lmg.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://rbd.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wov.hnqzz.top

[U70] PHP：PDO 事务
来源：http://snr.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uks.hesvh.cn

[U71] PHP：抛出异常
来源：http://sbd.shangyingyoupin.top

throw new RuntimeException("失败", 500);
来源：http://ekk.yj20258888.top

[U72] PHP：写错误日志
来源：http://ltr.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://tlm.hysaishi.cn

[U73] PHP：读取 ini 配置
来源：http://wja.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://xyf.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://fre.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://xyg.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://bid.yuanzhike.top

composer require psr/container
来源：http://nxe.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://yiv.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kqz.haohaochexian.top

[U77] PHP：模板渲染
来源：http://axb.xylfe.cn

composer require twig/twig
来源：http://eng.wangdashe.top

[U78] PHP：单元测试
来源：http://ffe.cashguo.top

composer require --dev phpunit/phpunit
来源：http://utk.havefunace.top

[U79] PHP：静态分析
来源：http://cns.yj202588.top

composer require --dev phpstan/phpstan
来源：http://flo.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://oiu.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zwe.fengsongda.top

[U81] JS：初始化项目
来源：http://qqe.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://vix.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://bpf.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iaa.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://ndx.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wev.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://cal.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jdu.cdnleiting.top

[U85] JS：可选链
来源：http://ekk.sxryk.cn

a?.b?.c
来源：http://xht.birdmap.top

[U86] JS：空值合并
来源：http://trl.nanxinkj.top

a ?? b
来源：http://tha.daxiang520.top

[U87] JS：解构默认值
来源：http://ply.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://ulb.bjfxy.top

[U88] JS：对象展开合并
来源：http://epz.tarul.cn

{ ...a, ...b }
来源：http://rmk.andypj.xyz

[U89] JS：数组去重
来源：http://prh.xziqi.cn

[...new Set(arr)]
来源：http://ytp.52xcode.cn

[U90] JS：数字数组排序
来源：http://crc.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://sba.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://oyp.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wql.nanxinkj.top

[U92] JS：深拷贝
来源：http://twk.cdnleiting.top

structuredClone(obj)
来源：http://hjz.jqgfzy.top

[U93] JS：模板字符串
来源：http://ozh.ydjk.org.cn

`共 ${n} 条`
来源：http://yto.zycfv.cn

[U94] JS：箭头函数
来源：http://cvo.cashguo.top

const double = x => x * 2;
来源：http://gsw.zdbjq.cn

[U95] JS：Promise 包装
来源：http://ntt.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://uco.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://oxi.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fwn.sweek.top

[U97] JS：并发请求
来源：http://fyt.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mxq.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://vet.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aij.zhongyouzk.top

[U99] JS：事件监听
来源：http://rpp.havefunace.top

el.addEventListener("click", e => {})
来源：http://pqu.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://uvb.mhx1999.top

document.querySelector(".item")
来源：http://vro.gzhubu.top

[U101] JS：classList 操作
来源：http://mlo.xuanzx.com

el.classList.toggle("active")
来源：http://dng.shuidangran.top

[U102] JS：本地存储
来源：http://xuo.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qgd.jqgufenzy.top

[U103] JS：定时器
来源：http://fho.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://otv.jlsjyb.cn

[U104] JS：防抖
来源：http://mln.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ybv.zycfv.cn

[U105] JS：节流
来源：http://man.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rbs.smart0.xyz

[U106] JS：日期格式化
来源：http://pjo.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ext.316326.xyz

[U107] JS：数字千分位
来源：http://qrk.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qij.zhiwuduotai.top

[U108] JS：随机整数
来源：http://lqu.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hft.xylfe.cn

[U109] JS：数组分组
来源：http://ayo.xingfuxueyuan.xyz

Object.groupBy(arr, x => x.type)
来源：http://ivg.fehbvm.com

[U110] JS：数组分块
来源：http://von.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iwk.cashguo.top

[U111] JS：对象转 Map
来源：http://uwl.cdnleiting.top

new Map(Object.entries(obj))
来源：http://wfa.nanxinkj.top

[U112] JS：字符串补位
来源：http://yhu.yj20258888.top

"7".padStart(3, "0")
来源：http://nwm.aizwys.cn

[U113] JS：正则替换全部
来源：http://fve.ivvv.top

s.replaceAll("a", "b")
来源：http://ffg.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://yoz.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://myr.svipenyu.cn

[U115] JS：生成 UUID
来源：http://akj.redwolf501.top

crypto.randomUUID()
来源：http://yua.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://xzu.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://yfo.guannengcc.top

[U117] JS：单元测试
来源：http://cgt.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://ejk.zdqjudy.top

[U118] JS：开发服务器
来源：http://wdi.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://cfu.fzhhl.top

[U119] JS：生产构建
来源：http://ijw.sysykeji.top

npx vite build
来源：http://rpm.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://eit.yueranfly.top

import.meta.env.VITE_API_URL
来源：http://ioc.gotoacloud.top

================================================================================
来源：http://rnj.zhoulong.xyz

统计汇总
来源：http://oar.daxiang520.top

================================================================================
来源：http://mcx.shzxlz.cn

按语言统计（条）：
来源：http://epp.xylfe.cn

Python ......... 252
来源：http://klc.ivvv.top

PHP ............ 252
来源：http://knb.redwolf501.top

JavaScript ..... 252
来源：http://pkv.pengpengdd.cyou

TypeScript ..... 212
来源：http://bqg.jinghuilouyu.cn

Java ........... 212
来源：http://ayc.0kj1m.cn

Go ............. 212
来源：http://rzj.xuanzx.com

Ruby ........... 212
来源：http://ffu.sxryk.cn

C# ............. 212
来源：http://wxz.xylfe.cn

C .............. 30
来源：http://rrq.jqgufenzy.top

C++ ............ 30
来源：http://jjw.hywenlv.cn

SQL ............ 90
来源：http://djg.chenzaomai.com

Bash ........... 80
来源：http://wti.jinqigfzy.top

Kotlin ......... 15
来源：http://cmf.daxiang520.top

Swift .......... 15
来源：http://jjp.gaohongyu789.top

Lua ............ 10
来源：http://jhn.hongshengwenyu.top

Perl ........... 10
来源：http://tcq.fanxiaobao.xyz

Scala .......... 10
来源：http://gdc.sweek.top

------------------------------------
来源：http://xdj.ydzc1.top

合计 ........... 2106 条
来源：http://mfn.daria6918.cn

按章节统计：
来源：http://hdz.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sjb.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xgi.yj20258888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jti.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ugf.snrcjt.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mwm.sweek.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://htw.shanyushiyangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://owc.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gwm.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mnq.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hbc.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dvv.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://txe.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://plh.sxryk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cmq.yangfankeji.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lav.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://esc.fzhhl.top

Q SQL 专题                              90
来源：http://evh.tianlin.xyz

R Bash 专题                             80
来源：http://vso.ppjwa.cn

S C / C++ 专题                          60
来源：http://otz.zhongyouzk.top

T 其他语言补充                          60
来源：http://qqd.cucudq.cn

U 高频实用片段                         120
来源：http://ere.nanxuanxn.top

------------------------------------
来源：http://ywf.ywan-chungtsiang.top

合计                                  2106 条
来源：http://jyu.yj20258888.top

--------------------------------------------------------------------------------
来源：http://all.shanyushiyangtech.top

使用提醒
来源：http://dxb.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://lbw.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kbb.shanyushiyangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lck.jiagoushi.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ayx.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://hlb.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://slo.zhengqikj.top

—— 文件结束 ——
来源：http://ixv.zdqjudy.top

================================================================================
来源：http://exl.vehdjk.com

程序语言常见例子速查手册（2024 版）
来源：http://pof.shanyushiyangkeji.top

Common Programming Examples Cheat Book
来源：http://adi.tarul.cn

================================================================================
来源：http://cyy.cqqwz.cn

【收录内容】
来源：http://gja.yfazqb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://vur.fanxiaobao.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xbj.jlsjyb.cn

SQL · Bash · C · C++
来源：http://moe.aizwys.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sww.xuetiantiany.cn

【使用说明】
来源：http://mhz.ehwqpu.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://voj.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://air.ywan-chungtsiang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ivv.gogol.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iqa.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ecl.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bxy.wangshuangyany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ckm.havefunace.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pqg.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yxa.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vop.yj20258.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xzx.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://elr.guowangkeji.top

【文件统计】
来源：http://kwa.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xig.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://ecd.mhx1999.top

目  录
来源：http://kdi.tian-w.cn

--------------------------------------------------------------------------------
来源：http://gov.daxiang520.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lmq.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cwv.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fhb.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rqu.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ito.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://efp.0kj1m.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rdd.cashguo.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bva.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dpa.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ijs.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wwg.hammf.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://brb.zycfv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ktr.hysaishi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nko.fehbvm.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gps.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wdl.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vbl.xuanzx.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://tkm.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tok.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dsl.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oux.hnqzz.top


<!-- 参考信息 -->