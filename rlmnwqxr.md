代发 wailian999

[U15] Py：高精度计时
来源：http://bov.snrcjt.cn

t = time.perf_counter()
来源：http://dzz.andypj.xyz

[U16] Py：命令行参数解析
来源：http://zfq.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ftn.jianghu66.top

[U17] Py：初始化日志
来源：http://pve.yvedp.cn

logging.basicConfig(level=logging.INFO)
来源：http://gth.yanxiufei.cn

[U18] Py：预编译正则
来源：http://xnh.chenlongwang.top

pat = re.compile(r"\d+")
来源：http://vax.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://qjy.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kof.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://ymc.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://onz.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://rro.quarkkingdee.top

@contextlib.contextmanager
来源：http://nrc.yueranfly.top

[U22] Py：矩阵转置
来源：http://vua.vqdsnc.cn

list(zip(*m))
来源：http://ijs.sysykeji.top

[U23] Py：分块读取大文件
来源：http://axw.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sal.bbcook.cn

[U24] Py：路径操作
来源：http://arl.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nuf.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://dro.yj20258.top

csv.DictReader(f)
来源：http://kwz.yj20258888.top

[U26] Py：并发下载
来源：http://nov.zdqjudy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bbo.epnwcf.com

[U27] Py：异步 HTTP
来源：http://hsy.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://gwq.guowangkeji.top

[U28] Py：类型别名
来源：http://ksw.yj20258.top

UserId = int
来源：http://ocg.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://qfh.ehwqpu.com

@property 与 @x.setter 配合
来源：http://coq.bjfxy.top

[U30] Py：数据类
来源：http://lch.cdnleiting.top

@dataclass(slots=True)
来源：http://caj.dashuyun.cn

[U31] Py：单测
来源：http://wko.xylfe.cn

python -m pytest -q
来源：http://rwa.xingfuxueyuan.xyz

[U32] Py：代码格式化
来源：http://axc.uphjek.com

ruff format . && ruff check --fix .
来源：http://udg.shzxlz.cn

[U33] Py：打包发布
来源：http://yux.fanxiaobao.xyz

python -m build  （依赖 pyproject.toml）
来源：http://xhv.feifeiyinyue.top

[U34] Py：判断编码
来源：http://yhq.haohaochexian.top

chardet.detect(raw)
来源：http://ixq.chenzaomai.com

[U35] Py：发送邮件
来源：http://vam.0kj1m.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jyh.ppjwa.cn

[U36] Py：定时任务
来源：http://ayf.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://yug.shangyingyoupin.top

[U37] Py：读写 Excel
来源：http://scf.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://gsv.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://qlg.gzhubu.top

Path(__file__).resolve().parent
来源：http://vhs.gotoacloud.top

[U39] Py：判断是否在交互环境
来源：http://yst.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://fvr.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://idn.hfpthk.cn

print("err", file=sys.stderr)
来源：http://uyt.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://jit.shangyingyoupin.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xjd.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://alu.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jnw.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://jpy.snrcjt.cn

namespace App\Http;
来源：http://uwv.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://qwd.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://qud.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://jgh.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jhh.hywenlv.cn

[U46] PHP：可空类型
来源：http://qla.sufxvd.cn

?string $name = null
来源：http://kyf.wangshuangyany.cn

[U47] PHP：联合类型
来源：http://qtc.nanxinkj.top

int|string $id
来源：http://hpl.daxiang520.top

[U48] PHP：纯枚举
来源：http://xin.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nlt.tianlin.xyz

[U49] PHP：只读属性
来源：http://dxy.uphjek.com

public readonly string $name
来源：http://mhr.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://bnw.hysaishi.cn

public function __construct(private int $id) {}
来源：http://nke.ehwqpu.com

[U51] PHP：数组解构
来源：http://fwa.birdmap.top

[$a, $b] = $arr;
来源：http://qzc.hnqzz.top

[U52] PHP：箭头函数
来源：http://qcv.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://fuz.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://cot.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://nss.jinqigufen.top

[U54] PHP：空安全调用
来源：http://qqk.svipenyu.cn

$obj?->method()
来源：http://kwv.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://bpi.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ivu.cashguo.top

[U56] PHP：命名参数
来源：http://dbb.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://rsc.cdnleiting.top

[U57] PHP：字符串插值
来源：http://jnf.quarkkingdee.top

"值: {$a}"
来源：http://fhb.zdqjudy.top

[U58] PHP：数组三件套
来源：http://kuv.yfazqb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xxo.smart0.xyz

[U59] PHP：自定义排序
来源：http://tfo.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oqp.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://ktz.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yws.mhx1999.top

[U61] PHP：正则
来源：http://iaz.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jfl.ctjpmb.com

[U62] PHP：日期对象
来源：http://sxa.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dft.uphjek.com

[U63] PHP：文件读写
来源：http://vqj.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zgx.9152youxi.cn

[U64] PHP：目录遍历
来源：http://ace.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://etw.zhijiandao.cn

[U65] PHP：会话
来源：http://sxu.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://qvs.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://pgv.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qxx.uphjek.com

[U67] PHP：处理文件上传
来源：http://xza.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ykx.fengsongda.top

[U68] PHP：PDO 连接
来源：http://lks.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ggz.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://eed.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jqx.hnqzz.top

[U70] PHP：PDO 事务
来源：http://jjh.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zre.yfazqb.com

[U71] PHP：抛出异常
来源：http://jog.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://gwh.ybcxt.top

[U72] PHP：写错误日志
来源：http://gll.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://atd.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://ttj.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://nmu.zhengqikj.top

[U74] PHP：读取环境变量
来源：http://cfh.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://jev.hesvh.cn

[U75] PHP：依赖注入
来源：http://wmb.daria6918.cn

composer require psr/container
来源：http://icr.zdqjudy.top

[U76] PHP：简单路由
来源：http://wbu.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iln.zhongyouzk.top

[U77] PHP：模板渲染
来源：http://pmi.jinqigufen.top

composer require twig/twig
来源：http://vgh.0kj1m.cn

[U78] PHP：单元测试
来源：http://guw.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://xpk.dashuyun.cn

[U79] PHP：静态分析
来源：http://esv.birdmap.top

composer require --dev phpstan/phpstan
来源：http://tnm.yongpay.top

[U80] PHP：代码规范修复
来源：http://iyr.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://mit.hcnkem.com

[U81] JS：初始化项目
来源：http://aai.zhixingplan.top

npm init -y;  npm i express
来源：http://rks.316326.xyz

[U82] JS：package.json 脚本
来源：http://bkn.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mgz.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://vnt.yj20258888.top

export const a = 1;  import { a } from "./m.js";
来源：http://lse.yj20258.top

[U84] JS：CommonJS 写法
来源：http://qwl.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://qpp.dashuyun.cn

[U85] JS：可选链
来源：http://qxk.chenlongwang.top

a?.b?.c
来源：http://rub.zdqjudy.top

[U86] JS：空值合并
来源：http://lcw.pengpengdd.cyou

a ?? b
来源：http://gaa.tianlin.xyz

[U87] JS：解构默认值
来源：http://pdn.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://htg.ydzc1.top

[U88] JS：对象展开合并
来源：http://dfk.guowangkeji.top

{ ...a, ...b }
来源：http://sfq.ppjwa.cn

[U89] JS：数组去重
来源：http://yjb.jinqigfzy.top

[...new Set(arr)]
来源：http://kki.hongshengwenyu.top

[U90] JS：数字数组排序
来源：http://scy.yanxiufei.cn

[...arr].sort((a, b) => a - b)
来源：http://cld.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://bol.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bgh.smart0.xyz

[U92] JS：深拷贝
来源：http://dcf.jinghuilouyu.cn

structuredClone(obj)
来源：http://mab.hesvh.cn

[U93] JS：模板字符串
来源：http://ime.jlsjyb.cn

`共 ${n} 条`
来源：http://cak.dashuyun.cn

[U94] JS：箭头函数
来源：http://mau.gaohongyu789.top

const double = x => x * 2;
来源：http://cpo.yuanzhike.top

[U95] JS：Promise 包装
来源：http://acc.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://glx.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://ues.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uax.uphjek.com

[U97] JS：并发请求
来源：http://abp.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://xmx.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://cnj.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mty.havefunace.top

[U99] JS：事件监听
来源：http://gol.birdmap.top

el.addEventListener("click", e => {})
来源：http://efe.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://ewm.mhx1999.top

document.querySelector(".item")
来源：http://arp.cdnleiting.top

[U101] JS：classList 操作
来源：http://zya.pengpengdd.cyou

el.classList.toggle("active")
来源：http://fma.hysaishi.cn

[U102] JS：本地存储
来源：http://zcv.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lct.jinqigufen.top

[U103] JS：定时器
来源：http://ifr.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://enb.snrcjt.cn

[U104] JS：防抖
来源：http://wzn.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryg.cucudq.cn

[U105] JS：节流
来源：http://rpn.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://adn.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://vxi.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://utq.wangdashe.top

[U107] JS：数字千分位
来源：http://soq.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gft.sxryk.cn

[U108] JS：随机整数
来源：http://rpb.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ozu.hongshengwenyu.top

[U109] JS：数组分组
来源：http://fik.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://cky.sweek.top

[U110] JS：数组分块
来源：http://oif.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fow.ctjpmb.com

[U111] JS：对象转 Map
来源：http://rao.gzhubu.top

new Map(Object.entries(obj))
来源：http://npr.cdnleiting.top

[U112] JS：字符串补位
来源：http://rbz.nwbrower.top

"7".padStart(3, "0")
来源：http://azi.c1oappe.top

[U113] JS：正则替换全部
来源：http://cks.shuidangran.top

s.replaceAll("a", "b")
来源：http://llv.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://dsn.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rzb.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://owb.ydjk.org.cn

crypto.randomUUID()
来源：http://lwl.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://fpa.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://dtf.zdqjudy.top

[U117] JS：单元测试
来源：http://lco.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://guu.cheryme.top

[U118] JS：开发服务器
来源：http://uve.jinqigufen.top

npm i -D vite;  npx vite
来源：http://vuw.hcnkem.com

[U119] JS：生产构建
来源：http://tkm.wangshuangyany.cn

npx vite build
来源：http://woy.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://qvi.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://iav.dianchejie.cn

================================================================================
来源：http://now.fengsongda.top

统计汇总
来源：http://vts.feifeiyinyue.top

================================================================================
来源：http://nph.dashuyun.cn

按语言统计（条）：
来源：http://lax.bbcook.cn

Python ......... 252
来源：http://pqo.hammf.cn

PHP ............ 252
来源：http://btx.wangshuangyany.cn

JavaScript ..... 252
来源：http://yyq.jianghu66.top

TypeScript ..... 212
来源：http://gsm.shuidangran.top

Java ........... 212
来源：http://gqj.daria6918.cn

Go ............. 212
来源：http://vfy.daxiang520.top

Ruby ........... 212
来源：http://jmd.shangyingyoupin.top

C# ............. 212
来源：http://biu.chenlongwang.top

C .............. 30
来源：http://zty.mhx1999.top

C++ ............ 30
来源：http://ebe.andypj.xyz

SQL ............ 90
来源：http://lsh.mhx1999.top

Bash ........... 80
来源：http://gdi.jyoumei.cn

Kotlin ......... 15
来源：http://wxc.dianchejie.cn

Swift .......... 15
来源：http://hke.zhoulong.xyz

Lua ............ 10
来源：http://mxj.yanxiufei.cn

Perl ........... 10
来源：http://ntm.sysykeji.top

Scala .......... 10
来源：http://rur.daxiang520.top

------------------------------------
来源：http://iwc.tanke756.top

合计 ........... 2106 条
来源：http://ifo.cqqwz.cn

按章节统计：
来源：http://dzc.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vya.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yhm.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://afw.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://etv.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tjn.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dsq.zhaomingkeji.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mkk.guannengcc.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qcz.pengpengdd.cyou

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xdu.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://phi.xingfuxueyuan.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://onr.jqgfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eal.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yro.jqgufenzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aic.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yim.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ulz.zhixingplan.top

Q SQL 专题                              90
来源：http://xjd.mhx1999.top

R Bash 专题                             80
来源：http://wec.yvedp.cn

S C / C++ 专题                          60
来源：http://gje.guannengcc.top

T 其他语言补充                          60
来源：http://bqg.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://iia.guowangkeji.top

------------------------------------
来源：http://alv.dashuyun.cn

合计                                  2106 条
来源：http://fse.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://har.gogol.net.cn

使用提醒
来源：http://qmm.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://ehu.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bjx.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bno.jinqigufen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zkh.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fgk.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dit.fengsongda.top

—— 文件结束 ——
来源：http://idj.andypj.xyz

================================================================================
来源：http://ikq.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://knm.jinyuanbaomall.cn

Common Programming Examples Cheat Book
来源：http://yjb.chenlongwang.top

================================================================================
来源：http://mof.jianghu66.top

【收录内容】
来源：http://ivn.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://mtv.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tbl.jinyuanbaomall.cn

SQL · Bash · C · C++
来源：http://jgw.xziqi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://udl.sjlbkw.cn

【使用说明】
来源：http://fnt.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://edo.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hxq.yfazqb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ptr.ybcxt.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pld.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qpu.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kbl.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nad.chenjidiqi.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ivt.c1oappe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rpe.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hup.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mzh.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jca.wangshuangyany.cn

【文件统计】
来源：http://ull.316326.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://osf.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://pjc.shanyushiyangkeji.top

目  录
来源：http://vhc.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://krd.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rwu.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mbx.vqdsnc.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mkl.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pjs.hammf.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://etq.quarkkingdee.top


<!-- 参考信息 -->