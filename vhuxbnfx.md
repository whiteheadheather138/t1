代发 wailian999

[U19] Py：正则替换带回调
来源：http://oqh.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ong.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://ffb.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://ggf.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://cek.cheryme.top

@contextlib.contextmanager
来源：http://yrr.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://cyh.yfazqb.com

list(zip(*m))
来源：http://tre.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://ybj.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jbg.gzhubu.top

[U24] Py：路径操作
来源：http://flf.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wkp.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://cgk.pycfn.com

csv.DictReader(f)
来源：http://uuo.wangshuangyany.cn

[U26] Py：并发下载
来源：http://wbd.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://brj.fengsongda.top

[U27] Py：异步 HTTP
来源：http://pvb.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://xmo.fengsongda.top

[U28] Py：类型别名
来源：http://tje.iojbl.cn

UserId = int
来源：http://tef.fanxiaobao.xyz

[U29] Py：属性校验
来源：http://bsl.yj202588.top

@property 与 @x.setter 配合
来源：http://sjt.yonumen.top

[U30] Py：数据类
来源：http://duw.yangfankeji.com

@dataclass(slots=True)
来源：http://tom.mhx1999.top

[U31] Py：单测
来源：http://dup.jqgufenzy.top

python -m pytest -q
来源：http://daf.ydjk.org.cn

[U32] Py：代码格式化
来源：http://mkb.tarul.cn

ruff format . && ruff check --fix .
来源：http://pph.uphjek.com

[U33] Py：打包发布
来源：http://tjh.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://pkt.ivvv.top

[U34] Py：判断编码
来源：http://uvw.kuanghao11.cn

chardet.detect(raw)
来源：http://wxe.sysykeji.top

[U35] Py：发送邮件
来源：http://tjy.yanxiufei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mny.pengpengdd.cyou

[U36] Py：定时任务
来源：http://nox.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://zzp.hywenlv.cn

[U37] Py：读写 Excel
来源：http://czt.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://zid.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://lnk.zdbjq.cn

Path(__file__).resolve().parent
来源：http://wjn.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://ijl.zhongyouzk.top

sys.stdout.isatty()
来源：http://ivb.cucudq.cn

[U40] Py：打印到标准错误
来源：http://ado.redwolf501.top

print("err", file=sys.stderr)
来源：http://btt.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://trp.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lkm.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://hil.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wpq.xziqi.cn

[U43] PHP：声明命名空间
来源：http://skd.aibaodan.cn

namespace App\Http;
来源：http://ggy.ybcxt.top

[U44] PHP：开启严格类型
来源：http://xru.uphjek.com

declare(strict_types=1);
来源：http://mqu.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://bni.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eey.uphjek.com

[U46] PHP：可空类型
来源：http://jlv.gzhubu.top

?string $name = null
来源：http://pgu.svipenyu.cn

[U47] PHP：联合类型
来源：http://vmb.ivvv.top

int|string $id
来源：http://pgr.gzhubu.top

[U48] PHP：纯枚举
来源：http://kez.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ths.jinqigfzy.top

[U49] PHP：只读属性
来源：http://cmf.zhoulong.xyz

public readonly string $name
来源：http://dqw.redwolf501.top

[U50] PHP：构造器属性提升
来源：http://euo.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://hfp.gogol.net.cn

[U51] PHP：数组解构
来源：http://uiq.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://nps.zdbjq.cn

[U52] PHP：箭头函数
来源：http://rof.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://elo.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://qrq.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://kuj.jqgfzy.top

[U54] PHP：空安全调用
来源：http://xix.sjlbkw.cn

$obj?->method()
来源：http://kvo.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://ibf.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eln.cucudq.cn

[U56] PHP：命名参数
来源：http://sxx.snrcjt.cn

f(a: 1, b: 2)
来源：http://ggm.c1oappe.top

[U57] PHP：字符串插值
来源：http://tot.redwolf501.top

"值: {$a}"
来源：http://vul.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://ato.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zpx.ehwqpu.com

[U59] PHP：自定义排序
来源：http://jzs.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://phb.yongpay.top

[U60] PHP：JSON 编解码
来源：http://jsx.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wul.xziqi.cn

[U61] PHP：正则
来源：http://eso.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eug.ivvv.top

[U62] PHP：日期对象
来源：http://spk.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sno.andypj.xyz

[U63] PHP：文件读写
来源：http://iwt.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hkt.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://rqq.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://sbe.tanke756.top

[U65] PHP：会话
来源：http://ihg.sysykeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bku.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://kut.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oeb.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://frd.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ffo.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://piz.yonumen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fjv.yfazqb.com

[U69] PHP：PDO 预处理
来源：http://gri.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ikj.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://esc.yj20258.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ygu.jyoumei.cn

[U71] PHP：抛出异常
来源：http://wlg.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://ota.dianchejie.cn

[U72] PHP：写错误日志
来源：http://ibg.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://ohk.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://iwl.uphjek.com

parse_ini_file("config.ini", true)
来源：http://xng.hnqzz.top

[U74] PHP：读取环境变量
来源：http://hdi.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://qwo.svipenyu.cn

[U75] PHP：依赖注入
来源：http://jqj.fengsongda.top

composer require psr/container
来源：http://yxp.fktsv.cn

[U76] PHP：简单路由
来源：http://ydy.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bkd.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://hks.ivvv.top

composer require twig/twig
来源：http://xwz.haohaochexian.top

[U78] PHP：单元测试
来源：http://nps.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://zkr.mhx1999.top

[U79] PHP：静态分析
来源：http://qkl.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://pjf.xinyue.icu

[U80] PHP：代码规范修复
来源：http://utp.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ckt.nwbrower.top

[U81] JS：初始化项目
来源：http://dja.andypj.xyz

npm init -y;  npm i express
来源：http://ifp.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://jja.9152youxi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dhw.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://ell.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xtq.snrcjt.cn

[U84] JS：CommonJS 写法
来源：http://wcm.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://pij.mhx1999.top

[U85] JS：可选链
来源：http://xiz.zhixingplan.top

a?.b?.c
来源：http://tdx.cdnleiting.top

[U86] JS：空值合并
来源：http://jck.fktsv.cn

a ?? b
来源：http://eho.hammf.cn

[U87] JS：解构默认值
来源：http://qkt.chenjidiqi.icu

const { a = 1, b = 2 } = obj;
来源：http://puf.nwbrower.top

[U88] JS：对象展开合并
来源：http://aea.andypj.xyz

{ ...a, ...b }
来源：http://btk.fehbvm.com

[U89] JS：数组去重
来源：http://bop.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://tlm.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://qhy.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://hzr.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://app.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ewh.yj20258888.top

[U92] JS：深拷贝
来源：http://ijg.zhoulong.xyz

structuredClone(obj)
来源：http://tvp.sjlbkw.cn

[U93] JS：模板字符串
来源：http://usf.guowangkeji.top

`共 ${n} 条`
来源：http://smg.tanke756.top

[U94] JS：箭头函数
来源：http://nsb.guowangkeji.top

const double = x => x * 2;
来源：http://hou.jinqigufen.top

[U95] JS：Promise 包装
来源：http://vxg.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://jmn.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://rae.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zei.fktsv.cn

[U97] JS：并发请求
来源：http://ghb.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zcf.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://mkc.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zro.epnwcf.com

[U99] JS：事件监听
来源：http://mkb.jianghu66.top

el.addEventListener("click", e => {})
来源：http://cyg.redwolf501.top

[U100] JS：DOM 查询
来源：http://bvv.ybcxt.top

document.querySelector(".item")
来源：http://tzw.zdbjq.cn

[U101] JS：classList 操作
来源：http://ykk.pengpengdd.cyou

el.classList.toggle("active")
来源：http://gve.hnxiangtu.top

[U102] JS：本地存储
来源：http://fbu.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qap.gaohongyu789.top

[U103] JS：定时器
来源：http://zmq.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wwn.sjlbkw.cn

[U104] JS：防抖
来源：http://xsr.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xuf.zdqjudy.top

[U105] JS：节流
来源：http://por.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://umw.haohaochexian.top

[U106] JS：日期格式化
来源：http://daa.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xeg.hysaishi.cn

[U107] JS：数字千分位
来源：http://bax.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hpz.zhoulong.xyz

[U108] JS：随机整数
来源：http://tdl.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ojd.guowangkeji.top

[U109] JS：数组分组
来源：http://ugz.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://uwm.hnxiangtu.top

[U110] JS：数组分块
来源：http://fbt.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kxm.yj202588.top

[U111] JS：对象转 Map
来源：http://kgj.cdnleiting.top

new Map(Object.entries(obj))
来源：http://isz.yj20258888.top

[U112] JS：字符串补位
来源：http://lln.zhoulong.xyz

"7".padStart(3, "0")
来源：http://flc.xziqi.cn

[U113] JS：正则替换全部
来源：http://fph.hnqzz.top

s.replaceAll("a", "b")
来源：http://fjn.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://exu.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dua.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://ihr.tarul.cn

crypto.randomUUID()
来源：http://ejt.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://sfn.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://afo.sufxvd.cn

[U117] JS：单元测试
来源：http://ldq.tanke756.top

npm i -D vitest;  npx vitest
来源：http://yiq.zhoulong.xyz

[U118] JS：开发服务器
来源：http://pdw.yonumen.top

npm i -D vite;  npx vite
来源：http://uda.ppjwa.cn

[U119] JS：生产构建
来源：http://mph.quarkkingdee.top

npx vite build
来源：http://tuk.daria6918.cn

[U120] JS：读取环境变量（Vite）
来源：http://fht.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://nuu.hywenlv.cn

================================================================================
来源：http://vre.jinqigfzy.top

统计汇总
来源：http://thk.jianghu66.top

================================================================================
来源：http://iod.bbcook.cn

按语言统计（条）：
来源：http://ble.tianlin.xyz

Python ......... 252
来源：http://ruv.epnwcf.com

PHP ............ 252
来源：http://ogd.xuetiantiany.cn

JavaScript ..... 252
来源：http://xiz.bjfxy.top

TypeScript ..... 212
来源：http://kys.ywan-chungtsiang.top

Java ........... 212
来源：http://oth.fzhhl.top

Go ............. 212
来源：http://ogz.yuxming.cn

Ruby ........... 212
来源：http://pis.zhongyouzk.top

C# ............. 212
来源：http://gzr.uphjek.com

C .............. 30
来源：http://cab.hammf.cn

C++ ............ 30
来源：http://sck.dianchejie.cn

SQL ............ 90
来源：http://nii.zhengqikj.top

Bash ........... 80
来源：http://zjp.fanxiaobao.xyz

Kotlin ......... 15
来源：http://dug.zycfv.cn

Swift .......... 15
来源：http://gcp.xuanzx.com

Lua ............ 10
来源：http://egw.yangfankeji.com

Perl ........... 10
来源：http://jio.fanxiaobao.xyz

Scala .......... 10
来源：http://wpr.smart0.xyz

------------------------------------
来源：http://cjp.xuetiantiany.cn

合计 ........... 2106 条
来源：http://guu.jqgufenzy.top

按章节统计：
来源：http://rhn.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gcm.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fny.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hfc.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gav.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lyq.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ogr.yanxiufei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fxb.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vmf.snrcjt.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fhe.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gxp.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ggu.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://big.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mfy.hnxiangtu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hhm.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dpx.pengpengdd.cyou

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://juj.yuxming.cn

Q SQL 专题                              90
来源：http://bei.shuidangran.top

R Bash 专题                             80
来源：http://cig.cqqwz.cn

S C / C++ 专题                          60
来源：http://mcl.zycfv.cn

T 其他语言补充                          60
来源：http://ewl.sufxvd.cn

U 高频实用片段                         120
来源：http://rax.xuetiantiany.cn

------------------------------------
来源：http://ikp.hysaishi.cn

合计                                  2106 条
来源：http://xbc.smart0.xyz

--------------------------------------------------------------------------------
来源：http://qky.jyoumei.cn

使用提醒
来源：http://mjl.yfazqb.com

--------------------------------------------------------------------------------
来源：http://tti.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vxl.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://avt.feifeiyinyue.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://idz.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fsz.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ejw.dashuyun.cn

—— 文件结束 ——
来源：http://dez.ybcxt.top

================================================================================
来源：http://qao.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://psj.gaohongyu789.top

Common Programming Examples Cheat Book
来源：http://vxr.yj20258.top

================================================================================
来源：http://zck.nanxuanxn.top

【收录内容】
来源：http://psd.nanxuanxn.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://slg.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rul.svipenyu.cn

SQL · Bash · C · C++
来源：http://olv.daria6918.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iss.shzxlz.cn

【使用说明】
来源：http://ubk.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://drb.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lbj.gzhubu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vjz.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://joa.shanyushiyangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pun.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bna.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lmk.daria6918.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tet.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xdr.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jyl.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://spc.gotoacloud.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bwm.sjlbkw.cn

【文件统计】
来源：http://jgn.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://isp.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://hht.svipenyu.cn

目  录
来源：http://tlq.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://hsu.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://huq.tian-w.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zkb.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rex.zhaomingkeji.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ewj.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sae.jinqigufen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://stt.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uva.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hdo.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oas.hongshengwenyu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://irl.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nih.jinqigufen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lbp.xylfe.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pje.xuanzx.com


<!-- 参考信息 -->