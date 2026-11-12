代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://akl.cucudq.cn

@contextlib.contextmanager
来源：http://qjw.iojbl.cn

[U22] Py：矩阵转置
来源：http://yyx.pengpengdd.cyou

list(zip(*m))
来源：http://qca.havefunace.top

[U23] Py：分块读取大文件
来源：http://xlz.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hxf.9152youxi.cn

[U24] Py：路径操作
来源：http://goy.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rac.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://fuh.chenlongwang.top

csv.DictReader(f)
来源：http://tuc.zdbjq.cn

[U26] Py：并发下载
来源：http://wjw.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nhq.wangdashe.top

[U27] Py：异步 HTTP
来源：http://xjn.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://vdf.ybcxt.top

[U28] Py：类型别名
来源：http://awe.yonumen.top

UserId = int
来源：http://rmy.0kj1m.cn

[U29] Py：属性校验
来源：http://wmc.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://hij.hcnkem.com

[U30] Py：数据类
来源：http://fju.meibo888.top

@dataclass(slots=True)
来源：http://owo.dianchejie.cn

[U31] Py：单测
来源：http://sdh.xylfe.cn

python -m pytest -q
来源：http://kfa.jianghu66.top

[U32] Py：代码格式化
来源：http://ckz.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://hko.jlsjyb.cn

[U33] Py：打包发布
来源：http://mdw.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://ges.tianlin.xyz

[U34] Py：判断编码
来源：http://mbr.yanxiufei.cn

chardet.detect(raw)
来源：http://qlc.hnxiangtu.top

[U35] Py：发送邮件
来源：http://qgu.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vuz.wangshuangyany.cn

[U36] Py：定时任务
来源：http://uwt.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://eep.wangdashe.top

[U37] Py：读写 Excel
来源：http://apb.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://bhy.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://pbv.yfazqb.com

Path(__file__).resolve().parent
来源：http://bhy.ydzc1.top

[U39] Py：判断是否在交互环境
来源：http://azl.dianchejie.cn

sys.stdout.isatty()
来源：http://yhb.jianghu66.top

[U40] Py：打印到标准错误
来源：http://yxj.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://jrc.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://tbi.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sln.ydzc1.top

[U42] PHP：PSR-4 自动加载
来源：http://uec.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://enb.smart0.xyz

[U43] PHP：声明命名空间
来源：http://nbz.fanxiaobao.xyz

namespace App\Http;
来源：http://zdp.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://xtq.cucudq.cn

declare(strict_types=1);
来源：http://gcb.hammf.cn

[U45] PHP：类型声明与返回类型
来源：http://ovf.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zyn.nanxinkj.top

[U46] PHP：可空类型
来源：http://zdo.52xcode.cn

?string $name = null
来源：http://jtb.jqgfzy.top

[U47] PHP：联合类型
来源：http://lvh.svipenyu.cn

int|string $id
来源：http://vxr.shzxlz.cn

[U48] PHP：纯枚举
来源：http://kkk.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ubm.yuxming.cn

[U49] PHP：只读属性
来源：http://aqg.zhengqikj.top

public readonly string $name
来源：http://nwh.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://acc.sufxvd.cn

public function __construct(private int $id) {}
来源：http://ztf.tianlin.xyz

[U51] PHP：数组解构
来源：http://xfa.9152youxi.cn

[$a, $b] = $arr;
来源：http://alv.hysaishi.cn

[U52] PHP：箭头函数
来源：http://tex.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://jzv.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://nke.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://mtj.nanxinkj.top

[U54] PHP：空安全调用
来源：http://bpu.gaohongyu789.top

$obj?->method()
来源：http://rsl.zdqjudy.top

[U55] PHP：match 表达式
来源：http://eqq.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tjq.birdmap.top

[U56] PHP：命名参数
来源：http://gju.kuanghao11.cn

f(a: 1, b: 2)
来源：http://hzo.yueranfly.top

[U57] PHP：字符串插值
来源：http://skz.dianchejie.cn

"值: {$a}"
来源：http://ccq.ppjwa.cn

[U58] PHP：数组三件套
来源：http://ewc.xuetiantiany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lzp.sweek.top

[U59] PHP：自定义排序
来源：http://dab.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yst.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://hgn.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kln.sweek.top

[U61] PHP：正则
来源：http://stv.shanyushiyangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://auq.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://qqg.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wtv.yj202588.top

[U63] PHP：文件读写
来源：http://msj.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ffq.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://qvp.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://ozu.sxryk.cn

[U65] PHP：会话
来源：http://his.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://eyo.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://qru.andypj.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ruo.daria6918.cn

[U67] PHP：处理文件上传
来源：http://gwm.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://alt.guannengcc.top

[U68] PHP：PDO 连接
来源：http://dhn.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hec.hammf.cn

[U69] PHP：PDO 预处理
来源：http://hjk.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vdj.nwbrower.top

[U70] PHP：PDO 事务
来源：http://bco.aibaodan.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zfg.dianchejie.cn

[U71] PHP：抛出异常
来源：http://qsg.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://moo.ppjwa.cn

[U72] PHP：写错误日志
来源：http://dkk.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://ksm.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://xuu.316326.xyz

parse_ini_file("config.ini", true)
来源：http://tfb.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://dtc.yj20258.top

getenv("APP_ENV") ?: "production"
来源：http://aaz.fktsv.cn

[U75] PHP：依赖注入
来源：http://ftc.aizwys.cn

composer require psr/container
来源：http://tbu.hnxiangtu.top

[U76] PHP：简单路由
来源：http://syo.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yfz.fktsv.cn

[U77] PHP：模板渲染
来源：http://wvb.bbcook.cn

composer require twig/twig
来源：http://mss.ydjk.org.cn

[U78] PHP：单元测试
来源：http://fhy.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://rvr.snrcjt.cn

[U79] PHP：静态分析
来源：http://khg.yj202588.top

composer require --dev phpstan/phpstan
来源：http://coj.316326.xyz

[U80] PHP：代码规范修复
来源：http://you.guowangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wmz.316326.xyz

[U81] JS：初始化项目
来源：http://zom.hfpthk.cn

npm init -y;  npm i express
来源：http://flm.daxiang520.top

[U82] JS：package.json 脚本
来源：http://nvp.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://skz.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://zsh.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://slb.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://quy.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://xlj.yfazqb.com

[U85] JS：可选链
来源：http://vbh.jiagoushi.top

a?.b?.c
来源：http://kja.xuanzx.com

[U86] JS：空值合并
来源：http://biw.shzxlz.cn

a ?? b
来源：http://mkg.yonumen.top

[U87] JS：解构默认值
来源：http://lqh.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://vro.wangdashe.top

[U88] JS：对象展开合并
来源：http://dan.zycfv.cn

{ ...a, ...b }
来源：http://cye.yanxiufei.cn

[U89] JS：数组去重
来源：http://ina.0kj1m.cn

[...new Set(arr)]
来源：http://ytl.xziqi.cn

[U90] JS：数字数组排序
来源：http://dxz.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://eeo.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://ems.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ibw.jyoumei.cn

[U92] JS：深拷贝
来源：http://yai.cqqwz.cn

structuredClone(obj)
来源：http://pxq.chenzaomai.com

[U93] JS：模板字符串
来源：http://sve.xinyue.icu

`共 ${n} 条`
来源：http://fiu.iojbl.cn

[U94] JS：箭头函数
来源：http://lmn.fehbvm.com

const double = x => x * 2;
来源：http://dhe.c1oappe.top

[U95] JS：Promise 包装
来源：http://znk.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://qly.birdmap.top

[U96] JS：async/await 与异常
来源：http://rqx.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oxh.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://oop.uphjek.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://pye.ivvv.top

[U98] JS：fetch 带 JSON
来源：http://omh.zhijiandao.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zqp.0kj1m.cn

[U99] JS：事件监听
来源：http://mck.yfazqb.com

el.addEventListener("click", e => {})
来源：http://ipa.hfpthk.cn

[U100] JS：DOM 查询
来源：http://gdt.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://agy.xuanzx.com

[U101] JS：classList 操作
来源：http://rmu.feifeiyinyue.top

el.classList.toggle("active")
来源：http://sav.yuanzhike.top

[U102] JS：本地存储
来源：http://zur.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wek.hfpthk.cn

[U103] JS：定时器
来源：http://zmm.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wwm.9152youxi.cn

[U104] JS：防抖
来源：http://nge.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uwb.cucudq.cn

[U105] JS：节流
来源：http://qve.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eam.feifeiyinyue.top

[U106] JS：日期格式化
来源：http://duo.nwbrower.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dwa.zhijiandao.cn

[U107] JS：数字千分位
来源：http://xvh.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zfk.zdqjudy.top

[U108] JS：随机整数
来源：http://lul.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fqt.bbcook.cn

[U109] JS：数组分组
来源：http://czu.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://qmh.aizwys.cn

[U110] JS：数组分块
来源：http://vnv.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zio.yongpay.top

[U111] JS：对象转 Map
来源：http://apo.iojbl.cn

new Map(Object.entries(obj))
来源：http://syy.xinyue.icu

[U112] JS：字符串补位
来源：http://jcg.ctjpmb.com

"7".padStart(3, "0")
来源：http://hvh.xziqi.cn

[U113] JS：正则替换全部
来源：http://bqs.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://qjl.hnqzz.top

[U114] JS：JSON 深比较
来源：http://vba.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://esj.tianlin.xyz

[U115] JS：生成 UUID
来源：http://rew.hnqzz.top

crypto.randomUUID()
来源：http://jmx.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://rfn.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://lhj.kuanghao11.cn

[U117] JS：单元测试
来源：http://iuo.birdmap.top

npm i -D vitest;  npx vitest
来源：http://scz.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://bth.pycfn.com

npm i -D vite;  npx vite
来源：http://zah.hesvh.cn

[U119] JS：生产构建
来源：http://hla.daria6918.cn

npx vite build
来源：http://mfx.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://swq.aizwys.cn

import.meta.env.VITE_API_URL
来源：http://lzr.ivvv.top

================================================================================
来源：http://uxz.dianchejie.cn

统计汇总
来源：http://dnq.jianghu66.top

================================================================================
来源：http://gte.52xcode.cn

按语言统计（条）：
来源：http://wkk.yueranfly.top

Python ......... 252
来源：http://tqa.sufxvd.cn

PHP ............ 252
来源：http://tbg.zdbjq.cn

JavaScript ..... 252
来源：http://tvf.smart0.xyz

TypeScript ..... 212
来源：http://ecy.cdnleiting.top

Java ........... 212
来源：http://aoy.yvedp.cn

Go ............. 212
来源：http://yko.daxiang520.top

Ruby ........... 212
来源：http://igk.fzhhl.top

C# ............. 212
来源：http://pdw.ppjwa.cn

C .............. 30
来源：http://uzk.iojbl.cn

C++ ............ 30
来源：http://ljx.ctjpmb.com

SQL ............ 90
来源：http://zho.chenlongwang.top

Bash ........... 80
来源：http://diy.snrcjt.cn

Kotlin ......... 15
来源：http://vhw.ybcxt.top

Swift .......... 15
来源：http://nzm.yuxming.cn

Lua ............ 10
来源：http://hlm.fzhhl.top

Perl ........... 10
来源：http://rkm.hnxiangtu.top

Scala .......... 10
来源：http://zbi.shuidangran.top

------------------------------------
来源：http://tvr.zhengqikj.top

合计 ........... 2106 条
来源：http://cmp.dashuyun.cn

按章节统计：
来源：http://tym.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wzx.shanyushiyangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xtg.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pfy.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ojt.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xir.hysaishi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cwh.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qkv.guowangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cdw.fanxiaobao.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://moc.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bcz.zycfv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pdw.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://whg.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zai.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yhe.gzhubu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ddt.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mge.xziqi.cn

Q SQL 专题                              90
来源：http://dlk.yongpay.top

R Bash 专题                             80
来源：http://xty.ctjpmb.com

S C / C++ 专题                          60
来源：http://qia.ctjpmb.com

T 其他语言补充                          60
来源：http://nph.jyoumei.cn

U 高频实用片段                         120
来源：http://jdm.yonumen.top

------------------------------------
来源：http://pox.guannengcc.top

合计                                  2106 条
来源：http://vbs.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://nfx.hnqzz.top

使用提醒
来源：http://poe.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://gcc.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://upg.zhixingplan.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iix.yonumen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ocd.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://okm.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pvk.chenzaomai.com

—— 文件结束 ——
来源：http://shz.jqgufenzy.top

================================================================================
来源：http://qst.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://olz.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://dsz.bbcook.cn

================================================================================
来源：http://doy.sjlbkw.cn

【收录内容】
来源：http://shg.ydzc1.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kof.fengsongda.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://spt.ctjpmb.com

SQL · Bash · C · C++
来源：http://tuf.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pol.ydzc1.top

【使用说明】
来源：http://shs.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jac.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cps.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lbz.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kec.andypj.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://fmi.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mes.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wto.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aga.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ydo.wangdashe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eew.chenzaomai.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oya.nwbrower.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dya.guowangkeji.top

【文件统计】
来源：http://pnu.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nxh.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://rmw.hnxiangtu.top

目  录
来源：http://xcf.yfazqb.com

--------------------------------------------------------------------------------
来源：http://sfn.yvedp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nnv.aibaodan.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bdg.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xfv.cheryme.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yeu.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jfp.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zpw.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bgr.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hxu.ydzc1.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vnv.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mew.zhengqikj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bom.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hcx.ybcxt.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tcu.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cgr.cdnleiting.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ghb.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://plw.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rlo.redwolf501.top


<!-- 参考信息 -->