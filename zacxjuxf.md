代发 wailian999

[U15] Py：高精度计时
来源：http://myl.sufxvd.cn

t = time.perf_counter()
来源：http://fow.feifeiyinyue.top

[U16] Py：命令行参数解析
来源：http://ogi.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hkh.gaohongyu789.top

[U17] Py：初始化日志
来源：http://aqh.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://isx.tian-w.cn

[U18] Py：预编译正则
来源：http://psb.sxryk.cn

pat = re.compile(r"\d+")
来源：http://hex.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://ceb.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://reh.zhengqikj.top

[U20] Py：缓存函数结果
来源：http://gfj.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://hfl.sweek.top

[U21] Py：自定义上下文管理器
来源：http://pyy.yuxming.cn

@contextlib.contextmanager
来源：http://pbj.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://yqn.gotoacloud.top

list(zip(*m))
来源：http://rri.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://nhl.jinqigfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bma.uphjek.com

[U24] Py：路径操作
来源：http://lsl.ywan-chungtsiang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://txf.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://wqx.yongpay.top

csv.DictReader(f)
来源：http://wdh.sufxvd.cn

[U26] Py：并发下载
来源：http://krr.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://izr.hnqzz.top

[U27] Py：异步 HTTP
来源：http://irr.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://dnn.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://wce.snrcjt.cn

UserId = int
来源：http://sbu.sjlbkw.cn

[U29] Py：属性校验
来源：http://vly.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://gia.jiagoushi.top

[U30] Py：数据类
来源：http://ywt.jianghu66.top

@dataclass(slots=True)
来源：http://tit.xziqi.cn

[U31] Py：单测
来源：http://ahy.bbcook.cn

python -m pytest -q
来源：http://qmb.fehbvm.com

[U32] Py：代码格式化
来源：http://xkm.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://lio.jinqigufen.top

[U33] Py：打包发布
来源：http://ltn.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://hra.zdbjq.cn

[U34] Py：判断编码
来源：http://hax.xylfe.cn

chardet.detect(raw)
来源：http://ckd.jinqigfzy.top

[U35] Py：发送邮件
来源：http://sxe.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fwg.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://cyr.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://nxr.ybcxt.top

[U37] Py：读写 Excel
来源：http://rcq.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://btw.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://krj.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://uir.hesvh.cn

[U39] Py：判断是否在交互环境
来源：http://oei.daria6918.cn

sys.stdout.isatty()
来源：http://pdk.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://wwj.zdbjq.cn

print("err", file=sys.stderr)
来源：http://gsu.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://vxn.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oui.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://kfg.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zjv.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://uol.yj20258.top

namespace App\Http;
来源：http://bjs.fehbvm.com

[U44] PHP：开启严格类型
来源：http://egz.xuanzx.com

declare(strict_types=1);
来源：http://ibw.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://hpf.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://feu.xuanzx.com

[U46] PHP：可空类型
来源：http://hlt.ivvv.top

?string $name = null
来源：http://tto.iojbl.cn

[U47] PHP：联合类型
来源：http://wlu.hnxiangtu.top

int|string $id
来源：http://ofy.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://jbw.daria6918.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jcp.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://zwm.xingfuxueyuan.xyz

public readonly string $name
来源：http://ogo.iojbl.cn

[U50] PHP：构造器属性提升
来源：http://tqw.cdnleiting.top

public function __construct(private int $id) {}
来源：http://jbf.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://bts.shuidangran.top

[$a, $b] = $arr;
来源：http://kcf.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://oet.yj20258.top

$double = fn($x) => $x * 2;
来源：http://ihi.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://mna.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://vho.guowangkeji.top

[U54] PHP：空安全调用
来源：http://obn.xuanzx.com

$obj?->method()
来源：http://spx.daxiang520.top

[U55] PHP：match 表达式
来源：http://hyf.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rje.52xcode.cn

[U56] PHP：命名参数
来源：http://dui.ehwqpu.com

f(a: 1, b: 2)
来源：http://fqu.sweek.top

[U57] PHP：字符串插值
来源：http://urv.bbcook.cn

"值: {$a}"
来源：http://yrg.yj20258888.top

[U58] PHP：数组三件套
来源：http://ris.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qqp.sysykeji.top

[U59] PHP：自定义排序
来源：http://tyq.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bdz.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://wip.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jqu.daxiang520.top

[U61] PHP：正则
来源：http://wzd.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://glj.0kj1m.cn

[U62] PHP：日期对象
来源：http://dve.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fdi.bbcook.cn

[U63] PHP：文件读写
来源：http://ibn.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rbp.xuanzx.com

[U64] PHP：目录遍历
来源：http://jki.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://vnd.zhaomingkeji.xyz

[U65] PHP：会话
来源：http://gko.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://fyv.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://lnk.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vsn.bbcook.cn

[U67] PHP：处理文件上传
来源：http://tfd.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://odk.yvedp.cn

[U68] PHP：PDO 连接
来源：http://hgz.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jyp.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://pix.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pdc.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://sii.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nrh.xuanzx.com

[U71] PHP：抛出异常
来源：http://ghj.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://ixe.0kj1m.cn

[U72] PHP：写错误日志
来源：http://arc.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://nak.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://ghw.uphjek.com

parse_ini_file("config.ini", true)
来源：http://iyd.yj202588.top

[U74] PHP：读取环境变量
来源：http://uck.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://fhm.nwbrower.top

[U75] PHP：依赖注入
来源：http://nuf.kuanghao11.cn

composer require psr/container
来源：http://cfw.zdqjudy.top

[U76] PHP：简单路由
来源：http://gvk.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://amj.yuxming.cn

[U77] PHP：模板渲染
来源：http://ock.zhijiandao.cn

composer require twig/twig
来源：http://zll.ivvv.top

[U78] PHP：单元测试
来源：http://upm.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://nzx.jqgufenzy.top

[U79] PHP：静态分析
来源：http://mhd.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://qbk.wangshuangyany.cn

[U80] PHP：代码规范修复
来源：http://kdy.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kvp.epnwcf.com

[U81] JS：初始化项目
来源：http://sxf.feifeiyinyue.top

npm init -y;  npm i express
来源：http://fyo.andypj.xyz

[U82] JS：package.json 脚本
来源：http://kmi.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://guz.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://ces.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://crr.havefunace.top

[U84] JS：CommonJS 写法
来源：http://zth.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xrv.cheryme.top

[U85] JS：可选链
来源：http://szo.zdbjq.cn

a?.b?.c
来源：http://ves.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://gpr.bjfxy.top

a ?? b
来源：http://ico.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://wyq.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://opt.smart0.xyz

[U88] JS：对象展开合并
来源：http://utc.zhengqikj.top

{ ...a, ...b }
来源：http://euv.zhoulong.xyz

[U89] JS：数组去重
来源：http://lmk.chenjidiqi.icu

[...new Set(arr)]
来源：http://def.hywenlv.cn

[U90] JS：数字数组排序
来源：http://kbs.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://dfo.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://mij.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yor.xinyue.icu

[U92] JS：深拷贝
来源：http://xgg.gzhubu.top

structuredClone(obj)
来源：http://jbz.hesvh.cn

[U93] JS：模板字符串
来源：http://jpo.sufxvd.cn

`共 ${n} 条`
来源：http://vdo.dianchejie.cn

[U94] JS：箭头函数
来源：http://qvd.vqdsnc.cn

const double = x => x * 2;
来源：http://fkj.yvedp.cn

[U95] JS：Promise 包装
来源：http://cnn.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://cvs.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://wyw.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://akl.bjfxy.top

[U97] JS：并发请求
来源：http://hbb.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eib.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://shz.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gdw.fzhhl.top

[U99] JS：事件监听
来源：http://arl.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://kgy.daxiang520.top

[U100] JS：DOM 查询
来源：http://tzg.cashguo.top

document.querySelector(".item")
来源：http://afr.hnxiangtu.top

[U101] JS：classList 操作
来源：http://owr.chenjidiqi.icu

el.classList.toggle("active")
来源：http://uri.mhx1999.top

[U102] JS：本地存储
来源：http://rtf.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://iru.jyoumei.cn

[U103] JS：定时器
来源：http://srb.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hfz.zdbjq.cn

[U104] JS：防抖
来源：http://mdl.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epa.zhongyouzk.top

[U105] JS：节流
来源：http://exa.hongshengwenyu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nwr.bjfxy.top

[U106] JS：日期格式化
来源：http://yta.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nnp.0kj1m.cn

[U107] JS：数字千分位
来源：http://ufq.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wgm.cucudq.cn

[U108] JS：随机整数
来源：http://yqx.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nqu.hfpthk.cn

[U109] JS：数组分组
来源：http://ela.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://xhw.xuetiantiany.cn

[U110] JS：数组分块
来源：http://iug.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nop.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://aoe.yuanzhike.top

new Map(Object.entries(obj))
来源：http://fhi.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://zlb.guowangkeji.top

"7".padStart(3, "0")
来源：http://hrb.9152youxi.cn

[U113] JS：正则替换全部
来源：http://buc.aizwys.cn

s.replaceAll("a", "b")
来源：http://mps.cashguo.top

[U114] JS：JSON 深比较
来源：http://yuq.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qbz.birdmap.top

[U115] JS：生成 UUID
来源：http://mrd.gotoacloud.top

crypto.randomUUID()
来源：http://ami.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://mkb.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://zyq.0kj1m.cn

[U117] JS：单元测试
来源：http://dym.chenjidiqi.icu

npm i -D vitest;  npx vitest
来源：http://hud.andypj.xyz

[U118] JS：开发服务器
来源：http://pau.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://fjh.mhx1999.top

[U119] JS：生产构建
来源：http://pgp.cheryme.top

npx vite build
来源：http://iqm.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://nvc.uphjek.com

import.meta.env.VITE_API_URL
来源：http://wuw.hysaishi.cn

================================================================================
来源：http://igx.yvedp.cn

统计汇总
来源：http://nts.zycfv.cn

================================================================================
来源：http://xnf.ywan-chungtsiang.top

按语言统计（条）：
来源：http://tip.aibaodan.cn

Python ......... 252
来源：http://obd.jyoumei.cn

PHP ............ 252
来源：http://mbe.guowangkeji.top

JavaScript ..... 252
来源：http://eko.jiagoushi.top

TypeScript ..... 212
来源：http://gcp.jqgfzy.top

Java ........... 212
来源：http://jtr.ctjpmb.com

Go ............. 212
来源：http://hyn.wangshuangyany.cn

Ruby ........... 212
来源：http://rme.hnxiangtu.top

C# ............. 212
来源：http://net.meibo888.top

C .............. 30
来源：http://xcm.hcnkem.com

C++ ............ 30
来源：http://iqk.bbcook.cn

SQL ............ 90
来源：http://gxk.birdmap.top

Bash ........... 80
来源：http://esv.aibaodan.cn

Kotlin ......... 15
来源：http://njs.pycfn.com

Swift .......... 15
来源：http://tvz.ctjpmb.com

Lua ............ 10
来源：http://fge.hesvh.cn

Perl ........... 10
来源：http://grs.ctjpmb.com

Scala .......... 10
来源：http://koc.quarkkingdee.top

------------------------------------
来源：http://gaq.zhijiandao.cn

合计 ........... 2106 条
来源：http://iky.zycfv.cn

按章节统计：
来源：http://eco.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rak.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wtl.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ota.ydjk.org.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sih.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xox.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fve.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bdo.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tmq.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://orv.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sid.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sek.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xpv.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nqy.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hor.yj202588.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lsu.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ogf.tianlin.xyz

Q SQL 专题                              90
来源：http://iqq.fanxiaobao.xyz

R Bash 专题                             80
来源：http://ooy.smart0.xyz

S C / C++ 专题                          60
来源：http://jqk.sxryk.cn

T 其他语言补充                          60
来源：http://dmc.ctjpmb.com

U 高频实用片段                         120
来源：http://amx.ivvv.top

------------------------------------
来源：http://dtj.guowangkeji.top

合计                                  2106 条
来源：http://dyo.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://yyt.shanyushiyangtech.top

使用提醒
来源：http://fxz.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://ytp.yuxming.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aom.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dzi.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fcj.ywan-chungtsiang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://cvs.sweek.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oub.zdbjq.cn

—— 文件结束 ——
来源：http://pjy.fanxiaobao.xyz

================================================================================
来源：http://ioy.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://ord.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://lty.hfpthk.cn

================================================================================
来源：http://fei.fanxiaobao.xyz

【收录内容】
来源：http://fcz.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zhz.chenjidiqi.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wbd.yangfankeji.com

SQL · Bash · C · C++
来源：http://mgk.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qmy.daxiang520.top

【使用说明】
来源：http://oyu.uphjek.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rvf.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zdb.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mwz.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pmf.vqdsnc.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://van.hnxiangtu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wbi.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://owp.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kwh.xinyue.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fsk.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jfv.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sxz.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yoy.fzhhl.top

【文件统计】
来源：http://rcp.fanxiaobao.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zoj.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://oho.gzhubu.top

目  录
来源：http://xrm.yvedp.cn

--------------------------------------------------------------------------------
来源：http://yfj.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fmr.cqqwz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kdu.yanxiufei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dlh.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bts.ydjk.org.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nwv.snrcjt.cn


<!-- 参考信息 -->