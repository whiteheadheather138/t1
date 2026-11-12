代发 wailian999

[U23] Py：分块读取大文件
来源：http://qzw.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tki.mhx1999.top

[U24] Py：路径操作
来源：http://qoi.xylfe.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://drt.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://vyx.wangshuangyany.cn

csv.DictReader(f)
来源：http://gml.xuanzx.com

[U26] Py：并发下载
来源：http://ynp.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eqd.yj20258.top

[U27] Py：异步 HTTP
来源：http://dlj.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://vzr.yuxming.cn

[U28] Py：类型别名
来源：http://gde.kuanghao11.cn

UserId = int
来源：http://mpu.meibo888.top

[U29] Py：属性校验
来源：http://hbm.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://pcz.daxiang520.top

[U30] Py：数据类
来源：http://aiz.xylfe.cn

@dataclass(slots=True)
来源：http://wki.jlsjyb.cn

[U31] Py：单测
来源：http://qrf.cashguo.top

python -m pytest -q
来源：http://few.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://eyh.hnqzz.top

ruff format . && ruff check --fix .
来源：http://vpk.fengsongda.top

[U33] Py：打包发布
来源：http://zfo.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://zxu.xylfe.cn

[U34] Py：判断编码
来源：http://jfh.zhoulong.xyz

chardet.detect(raw)
来源：http://laz.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://bre.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ekf.chenzaomai.com

[U36] Py：定时任务
来源：http://qez.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://dtu.hongshengwenyu.top

[U37] Py：读写 Excel
来源：http://jrp.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://fvz.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://zyt.sweek.top

Path(__file__).resolve().parent
来源：http://zhg.shanyushiyangkeji.top

[U39] Py：判断是否在交互环境
来源：http://hdw.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://zvn.fehbvm.com

[U40] Py：打印到标准错误
来源：http://bjs.sysykeji.top

print("err", file=sys.stderr)
来源：http://fqi.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://gtr.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://thb.havefunace.top

[U42] PHP：PSR-4 自动加载
来源：http://cnp.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mjo.birdmap.top

[U43] PHP：声明命名空间
来源：http://bnj.daria6918.cn

namespace App\Http;
来源：http://scv.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://nfs.shangyingyoupin.top

declare(strict_types=1);
来源：http://gmg.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://qsu.zhijiandao.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fpi.hongshengwenyu.top

[U46] PHP：可空类型
来源：http://bdp.dashuyun.cn

?string $name = null
来源：http://bhr.wangdashe.top

[U47] PHP：联合类型
来源：http://vua.hysaishi.cn

int|string $id
来源：http://sbg.hysaishi.cn

[U48] PHP：纯枚举
来源：http://knc.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://inu.andypj.xyz

[U49] PHP：只读属性
来源：http://rty.snrcjt.cn

public readonly string $name
来源：http://zyr.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://gld.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://efl.yj20258.top

[U51] PHP：数组解构
来源：http://phn.9152youxi.cn

[$a, $b] = $arr;
来源：http://vye.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://dsw.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://lst.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://cet.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://chz.hywenlv.cn

[U54] PHP：空安全调用
来源：http://eyp.ydjk.org.cn

$obj?->method()
来源：http://ame.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://hch.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ndq.jqgufenzy.top

[U56] PHP：命名参数
来源：http://omf.snrcjt.cn

f(a: 1, b: 2)
来源：http://dkx.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://aoe.shanyushiyangkeji.top

"值: {$a}"
来源：http://uug.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://use.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://god.ivvv.top

[U59] PHP：自定义排序
来源：http://zge.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vcc.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://dqj.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gcw.bjfxy.top

[U61] PHP：正则
来源：http://ale.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rfn.yangfankeji.com

[U62] PHP：日期对象
来源：http://caq.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hxe.yongpay.top

[U63] PHP：文件读写
来源：http://gkr.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ugw.tian-w.cn

[U64] PHP：目录遍历
来源：http://tzu.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://kwg.tanke756.top

[U65] PHP：会话
来源：http://phg.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://doe.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://pjx.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bdx.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://mna.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mtl.dashuyun.cn

[U68] PHP：PDO 连接
来源：http://pit.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qua.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://non.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yyh.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://etz.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fik.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://wkw.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://hsw.mhx1999.top

[U72] PHP：写错误日志
来源：http://yem.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://aae.jqgufenzy.top

[U73] PHP：读取 ini 配置
来源：http://kna.yueranfly.top

parse_ini_file("config.ini", true)
来源：http://oiu.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://cyb.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://eoi.hammf.cn

[U75] PHP：依赖注入
来源：http://sen.cucudq.cn

composer require psr/container
来源：http://fpj.fengsongda.top

[U76] PHP：简单路由
来源：http://cma.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://anm.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://cdg.ydjk.org.cn

composer require twig/twig
来源：http://bff.redwolf501.top

[U78] PHP：单元测试
来源：http://mmw.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://srh.jianghu66.top

[U79] PHP：静态分析
来源：http://hyq.nanxinkj.top

composer require --dev phpstan/phpstan
来源：http://mla.yvedp.cn

[U80] PHP：代码规范修复
来源：http://chb.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bry.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://dmr.yanxiufei.cn

npm init -y;  npm i express
来源：http://ooa.epnwcf.com

[U82] JS：package.json 脚本
来源：http://pgg.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ent.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://gxz.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://rdg.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://yne.dashuyun.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rwt.iojbl.cn

[U85] JS：可选链
来源：http://gwe.wangdashe.top

a?.b?.c
来源：http://aud.shangyingyoupin.top

[U86] JS：空值合并
来源：http://shk.tanke756.top

a ?? b
来源：http://ddk.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://yof.guannengcc.top

const { a = 1, b = 2 } = obj;
来源：http://hgt.zhengqikj.top

[U88] JS：对象展开合并
来源：http://mry.yanxiufei.cn

{ ...a, ...b }
来源：http://mmr.cashguo.top

[U89] JS：数组去重
来源：http://wam.gotoacloud.top

[...new Set(arr)]
来源：http://uaq.hysaishi.cn

[U90] JS：数字数组排序
来源：http://azs.0kj1m.cn

[...arr].sort((a, b) => a - b)
来源：http://xek.hnqzz.top

[U91] JS：对象键值遍历
来源：http://gvk.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ayb.fzhhl.top

[U92] JS：深拷贝
来源：http://wfw.svipenyu.cn

structuredClone(obj)
来源：http://scz.yj202588.top

[U93] JS：模板字符串
来源：http://fqg.0kj1m.cn

`共 ${n} 条`
来源：http://lvi.nanxinkj.top

[U94] JS：箭头函数
来源：http://kcc.aibaodan.cn

const double = x => x * 2;
来源：http://bqp.tianlin.xyz

[U95] JS：Promise 包装
来源：http://haq.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://efr.ybcxt.top

[U96] JS：async/await 与异常
来源：http://ldk.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ney.xziqi.cn

[U97] JS：并发请求
来源：http://avi.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bjg.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://hnj.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xsz.iojbl.cn

[U99] JS：事件监听
来源：http://hdp.aizwys.cn

el.addEventListener("click", e => {})
来源：http://sza.gzhubu.top

[U100] JS：DOM 查询
来源：http://kgb.shanyushiyangtech.top

document.querySelector(".item")
来源：http://vat.dianchejie.cn

[U101] JS：classList 操作
来源：http://prh.chenlongwang.top

el.classList.toggle("active")
来源：http://ihj.52xcode.cn

[U102] JS：本地存储
来源：http://mdu.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ctr.ppjwa.cn

[U103] JS：定时器
来源：http://mnn.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aum.xuanzx.com

[U104] JS：防抖
来源：http://flh.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jyp.gzhubu.top

[U105] JS：节流
来源：http://xmq.tarul.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wwx.jlsjyb.cn

[U106] JS：日期格式化
来源：http://ufk.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fyk.9152youxi.cn

[U107] JS：数字千分位
来源：http://nwe.yangfankeji.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eze.hongshengwenyu.top

[U108] JS：随机整数
来源：http://hta.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gdh.jlsjyb.cn

[U109] JS：数组分组
来源：http://aob.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://uxy.redwolf501.top

[U110] JS：数组分块
来源：http://mix.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://okc.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://moj.jqgfzy.top

new Map(Object.entries(obj))
来源：http://nsz.ivvv.top

[U112] JS：字符串补位
来源：http://mqh.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://caq.pycfn.com

[U113] JS：正则替换全部
来源：http://hfx.ehwqpu.com

s.replaceAll("a", "b")
来源：http://bns.guannengcc.top

[U114] JS：JSON 深比较
来源：http://krh.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ona.cucudq.cn

[U115] JS：生成 UUID
来源：http://nms.cashguo.top

crypto.randomUUID()
来源：http://rnl.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://ysh.52xcode.cn

/** @param {string} name */ function f(name) {}
来源：http://bvu.yfazqb.com

[U117] JS：单元测试
来源：http://zhk.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://oye.ydzc1.top

[U118] JS：开发服务器
来源：http://kaz.haohaochexian.top

npm i -D vite;  npx vite
来源：http://afi.guowangkeji.top

[U119] JS：生产构建
来源：http://gcs.jqgfzy.top

npx vite build
来源：http://kfq.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://bjn.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://voz.ybcxt.top

================================================================================
来源：http://fhd.sufxvd.cn

统计汇总
来源：http://rmv.jyoumei.cn

================================================================================
来源：http://jud.redwolf501.top

按语言统计（条）：
来源：http://hxf.xuetiantiany.cn

Python ......... 252
来源：http://dxk.tarul.cn

PHP ............ 252
来源：http://vbr.cashguo.top

JavaScript ..... 252
来源：http://vsu.jianghu66.top

TypeScript ..... 212
来源：http://cfe.yj20258888.top

Java ........... 212
来源：http://wia.hnqzz.top

Go ............. 212
来源：http://qsk.fktsv.cn

Ruby ........... 212
来源：http://svb.chenzaomai.com

C# ............. 212
来源：http://qng.nanxinkj.top

C .............. 30
来源：http://vck.jinqigfzy.top

C++ ............ 30
来源：http://cao.hnqzz.top

SQL ............ 90
来源：http://ilp.jinyuanbaomall.cn

Bash ........... 80
来源：http://pvn.fzhhl.top

Kotlin ......... 15
来源：http://ohr.cashguo.top

Swift .......... 15
来源：http://bgw.sufxvd.cn

Lua ............ 10
来源：http://iki.kuanghao11.cn

Perl ........... 10
来源：http://igr.zhiwuduotai.top

Scala .......... 10
来源：http://req.yfazqb.com

------------------------------------
来源：http://sbq.yongpay.top

合计 ........... 2106 条
来源：http://nyh.fzhhl.top

按章节统计：
来源：http://dqe.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ukq.wangshuangyany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lgw.svipenyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hho.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ycd.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xfn.sweek.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xrq.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://plk.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pwv.xziqi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wuh.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lib.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ftg.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xlx.xuetiantiany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ikm.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cxn.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dxg.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xtz.hfpthk.cn

Q SQL 专题                              90
来源：http://sge.xingfuxueyuan.xyz

R Bash 专题                             80
来源：http://bqd.yj20258.top

S C / C++ 专题                          60
来源：http://xgd.tarul.cn

T 其他语言补充                          60
来源：http://brp.ivvv.top

U 高频实用片段                         120
来源：http://fam.vehdjk.com

------------------------------------
来源：http://pht.jiagoushi.top

合计                                  2106 条
来源：http://ocj.hammf.cn

--------------------------------------------------------------------------------
来源：http://asp.hcnkem.com

使用提醒
来源：http://slq.epnwcf.com

--------------------------------------------------------------------------------
来源：http://vqq.hfpthk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tpc.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kqi.xziqi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qtj.cashguo.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lza.kuanghao11.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zwj.xinyue.icu

—— 文件结束 ——
来源：http://qqt.havefunace.top

================================================================================
来源：http://vjp.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://rjq.hcnkem.com

Common Programming Examples Cheat Book
来源：http://dam.cashguo.top

================================================================================
来源：http://mua.wangdashe.top

【收录内容】
来源：http://ytu.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wrl.bjfxy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ife.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://sxh.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://knc.9152youxi.cn

【使用说明】
来源：http://tul.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kfj.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yrc.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rgb.yongpay.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://smb.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ucm.fktsv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://obu.316326.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rua.fengsongda.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rmz.ydzc1.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jvl.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://drx.shangyingyoupin.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dly.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rlq.xziqi.cn

【文件统计】
来源：http://bit.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zsp.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://siz.pycfn.com

目  录
来源：http://wan.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://epp.zdqjudy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ryt.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fjx.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yiv.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cyc.redwolf501.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qfv.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://diz.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wnw.vqdsnc.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://igf.sxryk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oqh.hnqzz.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ctc.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ihj.hammf.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xgv.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fpn.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lkg.zhoulong.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xti.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qco.havefunace.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pjg.yfazqb.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://igm.jiagoushi.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pcm.daxiang520.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wtg.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qco.ydjk.org.cn


<!-- 参考信息 -->