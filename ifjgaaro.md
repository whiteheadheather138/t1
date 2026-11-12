代发 wailian999

[U19] Py：正则替换带回调
来源：http://wxy.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uwk.havefunace.top

[U20] Py：缓存函数结果
来源：http://gmg.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://abg.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://mwb.xylfe.cn

@contextlib.contextmanager
来源：http://cdo.svipenyu.cn

[U22] Py：矩阵转置
来源：http://abr.hnqzz.top

list(zip(*m))
来源：http://mrx.tanke756.top

[U23] Py：分块读取大文件
来源：http://sam.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jeb.chenzaomai.com

[U24] Py：路径操作
来源：http://hfo.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sij.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://pzh.yfazqb.com

csv.DictReader(f)
来源：http://uzx.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://cpk.zhiwuduotai.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cht.zycfv.cn

[U27] Py：异步 HTTP
来源：http://gui.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://jar.guannengcc.top

[U28] Py：类型别名
来源：http://wzs.pycfn.com

UserId = int
来源：http://gek.jinqigufen.top

[U29] Py：属性校验
来源：http://bhp.mhx1999.top

@property 与 @x.setter 配合
来源：http://ytw.epnwcf.com

[U30] Py：数据类
来源：http://eku.yuxming.cn

@dataclass(slots=True)
来源：http://jdo.redwolf501.top

[U31] Py：单测
来源：http://jut.fengsongda.top

python -m pytest -q
来源：http://xjl.zdqjudy.top

[U32] Py：代码格式化
来源：http://cpd.aizwys.cn

ruff format . && ruff check --fix .
来源：http://sgl.zhijiandao.cn

[U33] Py：打包发布
来源：http://iap.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://uli.daria6918.cn

[U34] Py：判断编码
来源：http://zrt.hywenlv.cn

chardet.detect(raw)
来源：http://byy.yfazqb.com

[U35] Py：发送邮件
来源：http://rql.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zie.hnqzz.top

[U36] Py：定时任务
来源：http://msu.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://nhb.tian-w.cn

[U37] Py：读写 Excel
来源：http://ioq.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://pow.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://yjx.bbcook.cn

Path(__file__).resolve().parent
来源：http://erc.sweek.top

[U39] Py：判断是否在交互环境
来源：http://mhn.xziqi.cn

sys.stdout.isatty()
来源：http://aml.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://foz.ppjwa.cn

print("err", file=sys.stderr)
来源：http://sev.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://wte.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jlu.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://wkk.ydjk.org.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bpq.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://zfg.mhx1999.top

namespace App\Http;
来源：http://fyw.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://ano.wangdashe.top

declare(strict_types=1);
来源：http://kwg.birdmap.top

[U45] PHP：类型声明与返回类型
来源：http://aka.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://exq.yuxming.cn

[U46] PHP：可空类型
来源：http://emc.svipenyu.cn

?string $name = null
来源：http://wng.xylfe.cn

[U47] PHP：联合类型
来源：http://hdo.wangshuangyany.cn

int|string $id
来源：http://cje.gzhubu.top

[U48] PHP：纯枚举
来源：http://fln.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fgc.ybcxt.top

[U49] PHP：只读属性
来源：http://nqc.gogol.net.cn

public readonly string $name
来源：http://ehl.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://rbi.shanyushiyangtech.top

public function __construct(private int $id) {}
来源：http://qda.bjfxy.top

[U51] PHP：数组解构
来源：http://wnh.tanke756.top

[$a, $b] = $arr;
来源：http://jtd.fanxiaobao.xyz

[U52] PHP：箭头函数
来源：http://vyj.9152youxi.cn

$double = fn($x) => $x * 2;
来源：http://swq.fktsv.cn

[U53] PHP：空合并运算符
来源：http://ket.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://ogf.snrcjt.cn

[U54] PHP：空安全调用
来源：http://ggr.gotoacloud.top

$obj?->method()
来源：http://ykr.daria6918.cn

[U55] PHP：match 表达式
来源：http://txf.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://phf.ivvv.top

[U56] PHP：命名参数
来源：http://jye.yj20258.top

f(a: 1, b: 2)
来源：http://qnc.yongpay.top

[U57] PHP：字符串插值
来源：http://zqp.jlsjyb.cn

"值: {$a}"
来源：http://wqx.0kj1m.cn

[U58] PHP：数组三件套
来源：http://grr.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://amn.fzhhl.top

[U59] PHP：自定义排序
来源：http://spf.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blg.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://fqf.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gqh.sxryk.cn

[U61] PHP：正则
来源：http://ujx.guowangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sbf.zhijiandao.cn

[U62] PHP：日期对象
来源：http://jls.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jap.fengsongda.top

[U63] PHP：文件读写
来源：http://kml.gaohongyu789.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uei.aibaodan.cn

[U64] PHP：目录遍历
来源：http://yti.yanxiufei.cn

glob("dir/*.php");  scandir("dir");
来源：http://wjx.sxryk.cn

[U65] PHP：会话
来源：http://iki.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ppj.yonumen.top

[U66] PHP：设置 Cookie
来源：http://qox.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yta.yj20258888.top

[U67] PHP：处理文件上传
来源：http://ree.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xjh.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://xib.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hvm.yj202588.top

[U69] PHP：PDO 预处理
来源：http://hll.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xct.xuanzx.com

[U70] PHP：PDO 事务
来源：http://jrk.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nhj.havefunace.top

[U71] PHP：抛出异常
来源：http://pkw.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://obv.ehwqpu.com

[U72] PHP：写错误日志
来源：http://bxm.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://cue.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://thn.pycfn.com

parse_ini_file("config.ini", true)
来源：http://szc.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://nma.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://bqr.hysaishi.cn

[U75] PHP：依赖注入
来源：http://qtt.pengpengdd.cyou

composer require psr/container
来源：http://iih.ybcxt.top

[U76] PHP：简单路由
来源：http://khm.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eyu.zdqjudy.top

[U77] PHP：模板渲染
来源：http://kqu.hnqzz.top

composer require twig/twig
来源：http://nll.svipenyu.cn

[U78] PHP：单元测试
来源：http://kzx.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://gvd.zhijiandao.cn

[U79] PHP：静态分析
来源：http://dgl.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://nwo.52xcode.cn

[U80] PHP：代码规范修复
来源：http://bru.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gpa.andypj.xyz

[U81] JS：初始化项目
来源：http://fdy.cucudq.cn

npm init -y;  npm i express
来源：http://fhd.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://hem.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dpg.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://bor.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jkt.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://umu.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://ypu.xuanzx.com

[U85] JS：可选链
来源：http://acw.chenlongwang.top

a?.b?.c
来源：http://yzl.hongshengwenyu.top

[U86] JS：空值合并
来源：http://xnk.guannengcc.top

a ?? b
来源：http://yfx.ybcxt.top

[U87] JS：解构默认值
来源：http://xaj.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://nrw.gogol.net.cn

[U88] JS：对象展开合并
来源：http://fet.gzhubu.top

{ ...a, ...b }
来源：http://eje.cqqwz.cn

[U89] JS：数组去重
来源：http://jur.yvedp.cn

[...new Set(arr)]
来源：http://ufz.yangfankeji.com

[U90] JS：数字数组排序
来源：http://nlz.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://mnp.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://zkl.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gno.xinyue.icu

[U92] JS：深拷贝
来源：http://eot.zdqjudy.top

structuredClone(obj)
来源：http://lev.hcnkem.com

[U93] JS：模板字符串
来源：http://vzv.daxiang520.top

`共 ${n} 条`
来源：http://jym.yangfankeji.com

[U94] JS：箭头函数
来源：http://idb.yj20258.top

const double = x => x * 2;
来源：http://xff.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://dyz.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://ozt.xinyue.icu

[U96] JS：async/await 与异常
来源：http://hdb.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pei.hfpthk.cn

[U97] JS：并发请求
来源：http://fsh.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dfe.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://vxt.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://khs.xziqi.cn

[U99] JS：事件监听
来源：http://dgz.zhijiandao.cn

el.addEventListener("click", e => {})
来源：http://txq.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://ljo.ydzc1.top

document.querySelector(".item")
来源：http://poh.hcnkem.com

[U101] JS：classList 操作
来源：http://fko.havefunace.top

el.classList.toggle("active")
来源：http://xkk.guowangkeji.top

[U102] JS：本地存储
来源：http://wbw.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://caj.dianchejie.cn

[U103] JS：定时器
来源：http://qdv.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gab.guannengcc.top

[U104] JS：防抖
来源：http://lqd.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzy.ydjk.org.cn

[U105] JS：节流
来源：http://zfn.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uyv.jlsjyb.cn

[U106] JS：日期格式化
来源：http://kfi.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sie.cucudq.cn

[U107] JS：数字千分位
来源：http://qkw.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ltq.snrcjt.cn

[U108] JS：随机整数
来源：http://eup.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://orn.yueranfly.top

[U109] JS：数组分组
来源：http://zwe.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://ywl.zhongyouzk.top

[U110] JS：数组分块
来源：http://zto.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wak.hywenlv.cn

[U111] JS：对象转 Map
来源：http://ife.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://ebf.c1oappe.top

[U112] JS：字符串补位
来源：http://bqj.xuanzx.com

"7".padStart(3, "0")
来源：http://lve.epnwcf.com

[U113] JS：正则替换全部
来源：http://dhi.havefunace.top

s.replaceAll("a", "b")
来源：http://hnw.ywan-chungtsiang.top

[U114] JS：JSON 深比较
来源：http://vwc.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nis.redwolf501.top

[U115] JS：生成 UUID
来源：http://zps.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://voc.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://ssl.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://ntw.sysykeji.top

[U117] JS：单元测试
来源：http://fkc.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://anf.meibo888.top

[U118] JS：开发服务器
来源：http://ryo.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://zir.zhiwuduotai.top

[U119] JS：生产构建
来源：http://tvi.iojbl.cn

npx vite build
来源：http://kar.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://lkm.svipenyu.cn

import.meta.env.VITE_API_URL
来源：http://fvh.zdqjudy.top

================================================================================
来源：http://fme.shuidangran.top

统计汇总
来源：http://hle.birdmap.top

================================================================================
来源：http://gki.svipenyu.cn

按语言统计（条）：
来源：http://qqg.zdqjudy.top

Python ......... 252
来源：http://rxk.tanke756.top

PHP ............ 252
来源：http://gkd.haohaochexian.top

JavaScript ..... 252
来源：http://fsz.haohaochexian.top

TypeScript ..... 212
来源：http://wrg.hcnkem.com

Java ........... 212
来源：http://les.hysaishi.cn

Go ............. 212
来源：http://xhc.aibaodan.cn

Ruby ........... 212
来源：http://yyi.9152youxi.cn

C# ............. 212
来源：http://gvo.52xcode.cn

C .............. 30
来源：http://jkq.yfazqb.com

C++ ............ 30
来源：http://lhn.shanyushiyangkeji.top

SQL ............ 90
来源：http://ysr.quarkkingdee.top

Bash ........... 80
来源：http://lqj.chenlongwang.top

Kotlin ......... 15
来源：http://jpv.svipenyu.cn

Swift .......... 15
来源：http://beg.gotoacloud.top

Lua ............ 10
来源：http://srw.guowangkeji.top

Perl ........... 10
来源：http://roi.bbcook.cn

Scala .......... 10
来源：http://knz.nwbrower.top

------------------------------------
来源：http://sha.zhengqikj.top

合计 ........... 2106 条
来源：http://pxs.shanyushiyangkeji.top

按章节统计：
来源：http://rme.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qae.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ibz.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jjj.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wja.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vlm.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fxi.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jgh.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mtd.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://len.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mrq.cdnleiting.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gqg.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yje.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nqd.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oej.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ove.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wav.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://hxb.vqdsnc.cn

R Bash 专题                             80
来源：http://rjx.ybcxt.top

S C / C++ 专题                          60
来源：http://hhw.guannengcc.top

T 其他语言补充                          60
来源：http://uko.cdnleiting.top

U 高频实用片段                         120
来源：http://tpg.jiagoushi.top

------------------------------------
来源：http://vim.ybcxt.top

合计                                  2106 条
来源：http://fzy.yj20258.top

--------------------------------------------------------------------------------
来源：http://rrz.gogol.net.cn

使用提醒
来源：http://gcd.daxiang520.top

--------------------------------------------------------------------------------
来源：http://dcq.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://inb.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vst.zdbjq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://krk.cqqwz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gwo.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jbm.shzxlz.cn

—— 文件结束 ——
来源：http://ddp.yongpay.top

================================================================================
来源：http://dkz.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://ibn.yueranfly.top

Common Programming Examples Cheat Book
来源：http://qdj.zdbjq.cn

================================================================================
来源：http://zhg.hnqzz.top

【收录内容】
来源：http://zdh.yonumen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://twy.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aan.nwbrower.top

SQL · Bash · C · C++
来源：http://tpv.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dqf.yuanzhike.top

【使用说明】
来源：http://lqw.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lli.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nww.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ywo.andypj.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jem.jinghuilouyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dyp.kuanghao11.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fkw.birdmap.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://riw.guannengcc.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ruw.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kjj.yvedp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yap.zdqjudy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ued.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zjf.tanke756.top

【文件统计】
来源：http://buo.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mfd.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://zpf.feifeiyinyue.top

目  录
来源：http://lxa.fehbvm.com

--------------------------------------------------------------------------------
来源：http://hhj.dianchejie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ogz.9152youxi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://omz.yonumen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mps.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tgx.ctjpmb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hzk.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zuy.yuxming.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lzc.316326.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dfy.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lfn.cdnleiting.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nhp.jqgfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pui.svipenyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xit.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hyc.jqgufenzy.top


<!-- 参考信息 -->