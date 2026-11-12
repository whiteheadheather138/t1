代发 wailian999

[U07] Py：反转字典键值
来源：http://ifg.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://slf.smart0.xyz

[U08] Py：展平二维列表
来源：http://tdu.sysykeji.top

[y for x in nested for y in x]
来源：http://zqk.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://idv.hcnkem.com

max(d, key=d.get)
来源：http://csy.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://vyo.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aof.yvedp.cn

[U11] Py：生成器表达式
来源：http://qvw.fehbvm.com

(x * 2 for x in arr)
来源：http://jnr.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zaj.redwolf501.top

Counter(arr).most_common(3)
来源：http://xgw.yueranfly.top

[U13] Py：固定长度队列
来源：http://szd.jinghuilouyu.cn

deque(maxlen=10)
来源：http://qqm.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://dib.jqgufenzy.top

defaultdict(list)
来源：http://esj.chenlongwang.top

[U15] Py：高精度计时
来源：http://vvs.jinghuilouyu.cn

t = time.perf_counter()
来源：http://obm.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://sqe.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ogy.birdmap.top

[U17] Py：初始化日志
来源：http://sgt.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://yhw.ydjk.org.cn

[U18] Py：预编译正则
来源：http://lby.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://tfj.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://gij.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gyq.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://tyx.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://usk.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://ang.yj202588.top

@contextlib.contextmanager
来源：http://cwz.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://pfp.aibaodan.cn

list(zip(*m))
来源：http://gwp.yvedp.cn

[U23] Py：分块读取大文件
来源：http://kek.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lyb.kuanghao11.cn

[U24] Py：路径操作
来源：http://hui.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lwf.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://zdl.tanke756.top

csv.DictReader(f)
来源：http://crk.fzhhl.top

[U26] Py：并发下载
来源：http://umw.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sfm.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://nse.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://bhu.zhengqikj.top

[U28] Py：类型别名
来源：http://lms.sysykeji.top

UserId = int
来源：http://fof.cdnleiting.top

[U29] Py：属性校验
来源：http://voz.sweek.top

@property 与 @x.setter 配合
来源：http://ywr.iojbl.cn

[U30] Py：数据类
来源：http://mdr.dashuyun.cn

@dataclass(slots=True)
来源：http://ujk.vehdjk.com

[U31] Py：单测
来源：http://ger.mhx1999.top

python -m pytest -q
来源：http://mbk.epnwcf.com

[U32] Py：代码格式化
来源：http://ljd.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://rcl.sxryk.cn

[U33] Py：打包发布
来源：http://uvn.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://hwp.jqgufenzy.top

[U34] Py：判断编码
来源：http://gho.xuetiantiany.cn

chardet.detect(raw)
来源：http://ikz.sjlbkw.cn

[U35] Py：发送邮件
来源：http://gab.shanyushiyangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fau.iojbl.cn

[U36] Py：定时任务
来源：http://qzw.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://znr.gotoacloud.top

[U37] Py：读写 Excel
来源：http://lhr.chenjidiqi.icu

pandas.read_excel / DataFrame.to_excel
来源：http://ctn.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://pfk.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://bmo.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://weh.ivvv.top

sys.stdout.isatty()
来源：http://fzf.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://kha.xinyue.icu

print("err", file=sys.stderr)
来源：http://jxa.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://iew.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lqo.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://lej.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fms.tarul.cn

[U43] PHP：声明命名空间
来源：http://xtx.cqqwz.cn

namespace App\Http;
来源：http://pdq.gaohongyu789.top

[U44] PHP：开启严格类型
来源：http://ohn.hcnkem.com

declare(strict_types=1);
来源：http://swa.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://jyg.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://fdx.shzxlz.cn

[U46] PHP：可空类型
来源：http://fnq.xuetiantiany.cn

?string $name = null
来源：http://efc.hnxiangtu.top

[U47] PHP：联合类型
来源：http://gvh.wangshuangyany.cn

int|string $id
来源：http://vme.feifeiyinyue.top

[U48] PHP：纯枚举
来源：http://njz.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sfv.dianchejie.cn

[U49] PHP：只读属性
来源：http://lvt.fengsongda.top

public readonly string $name
来源：http://gpw.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://pxl.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://uip.ctjpmb.com

[U51] PHP：数组解构
来源：http://jeb.daria6918.cn

[$a, $b] = $arr;
来源：http://jwb.sysykeji.top

[U52] PHP：箭头函数
来源：http://zvd.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://fra.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://fng.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://hcj.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://edg.yueranfly.top

$obj?->method()
来源：http://fva.fzhhl.top

[U55] PHP：match 表达式
来源：http://dmm.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bkw.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://ddi.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://erd.xziqi.cn

[U57] PHP：字符串插值
来源：http://gjo.xuanzx.com

"值: {$a}"
来源：http://npa.jiagoushi.top

[U58] PHP：数组三件套
来源：http://cvy.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lcf.jyoumei.cn

[U59] PHP：自定义排序
来源：http://fdy.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cwo.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://qut.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ghi.dashuyun.cn

[U61] PHP：正则
来源：http://php.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dzz.yuxming.cn

[U62] PHP：日期对象
来源：http://zly.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fmn.hfpthk.cn

[U63] PHP：文件读写
来源：http://cct.hongshengwenyu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://byy.jinqigufen.top

[U64] PHP：目录遍历
来源：http://dcn.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://ofb.pengpengdd.cyou

[U65] PHP：会话
来源：http://bnc.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gya.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://mxk.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rgz.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://bfu.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ckp.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://avj.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fwl.nwbrower.top

[U69] PHP：PDO 预处理
来源：http://agb.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yyz.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://ucg.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://njf.c1oappe.top

[U71] PHP：抛出异常
来源：http://mgw.fanxiaobao.xyz

throw new RuntimeException("失败", 500);
来源：http://moe.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://kvg.sweek.top

error_log("失败: " . $e->getMessage());
来源：http://xsn.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://uux.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://tqr.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://cim.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://bpu.yj20258888.top

[U75] PHP：依赖注入
来源：http://cia.ydjk.org.cn

composer require psr/container
来源：http://zqs.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://szq.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://alk.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://evw.xingfuxueyuan.xyz

composer require twig/twig
来源：http://sts.ybcxt.top

[U78] PHP：单元测试
来源：http://swc.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://vbr.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://ras.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://gyw.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://fny.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://faf.c1oappe.top

[U81] JS：初始化项目
来源：http://nan.yuanzhike.top

npm init -y;  npm i express
来源：http://blt.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://bup.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uhk.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://upt.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rea.havefunace.top

[U84] JS：CommonJS 写法
来源：http://gel.dianchejie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oou.yonumen.top

[U85] JS：可选链
来源：http://nyw.tarul.cn

a?.b?.c
来源：http://hre.andypj.xyz

[U86] JS：空值合并
来源：http://iij.pengpengdd.cyou

a ?? b
来源：http://zhd.gaohongyu789.top

[U87] JS：解构默认值
来源：http://xqp.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://odw.fktsv.cn

[U88] JS：对象展开合并
来源：http://jay.yj20258.top

{ ...a, ...b }
来源：http://odz.cheryme.top

[U89] JS：数组去重
来源：http://tha.fehbvm.com

[...new Set(arr)]
来源：http://svb.yj20258.top

[U90] JS：数字数组排序
来源：http://jtt.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://vtf.yueranfly.top

[U91] JS：对象键值遍历
来源：http://xji.fzhhl.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tkr.yvedp.cn

[U92] JS：深拷贝
来源：http://hks.hnqzz.top

structuredClone(obj)
来源：http://wzx.zycfv.cn

[U93] JS：模板字符串
来源：http://hje.gzhubu.top

`共 ${n} 条`
来源：http://baz.svipenyu.cn

[U94] JS：箭头函数
来源：http://qrm.aizwys.cn

const double = x => x * 2;
来源：http://jcq.cucudq.cn

[U95] JS：Promise 包装
来源：http://msr.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://jwe.xziqi.cn

[U96] JS：async/await 与异常
来源：http://gim.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jpv.fktsv.cn

[U97] JS：并发请求
来源：http://hov.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://evr.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://vpi.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bbt.quarkkingdee.top

[U99] JS：事件监听
来源：http://tdg.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://tyg.gogol.net.cn

[U100] JS：DOM 查询
来源：http://mqj.feifeiyinyue.top

document.querySelector(".item")
来源：http://owa.fzhhl.top

[U101] JS：classList 操作
来源：http://msd.zdqjudy.top

el.classList.toggle("active")
来源：http://kwp.ydzc1.top

[U102] JS：本地存储
来源：http://kks.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gqi.xuetiantiany.cn

[U103] JS：定时器
来源：http://oph.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yqx.hnxiangtu.top

[U104] JS：防抖
来源：http://gli.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://puh.ywan-chungtsiang.top

[U105] JS：节流
来源：http://awo.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trn.havefunace.top

[U106] JS：日期格式化
来源：http://isj.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fmy.jqgfzy.top

[U107] JS：数字千分位
来源：http://fdm.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rfu.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://zwa.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vlj.guowangkeji.top

[U109] JS：数组分组
来源：http://gpv.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://pdw.haohaochexian.top

[U110] JS：数组分块
来源：http://wlq.jianghu66.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zmv.cucudq.cn

[U111] JS：对象转 Map
来源：http://wnt.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://scs.daria6918.cn

[U112] JS：字符串补位
来源：http://nrh.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://fig.yvedp.cn

[U113] JS：正则替换全部
来源：http://vsk.daxiang520.top

s.replaceAll("a", "b")
来源：http://ocw.316326.xyz

[U114] JS：JSON 深比较
来源：http://dor.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bax.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://vip.yongpay.top

crypto.randomUUID()
来源：http://flk.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://rki.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://lve.sweek.top

[U117] JS：单元测试
来源：http://cno.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://mwy.hywenlv.cn

[U118] JS：开发服务器
来源：http://tmm.dianchejie.cn

npm i -D vite;  npx vite
来源：http://tze.dashuyun.cn

[U119] JS：生产构建
来源：http://yeu.shzxlz.cn

npx vite build
来源：http://waf.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://jrv.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://zpv.yj202588.top

================================================================================
来源：http://zgh.ctjpmb.com

统计汇总
来源：http://eoc.sxryk.cn

================================================================================
来源：http://dab.guannengcc.top

按语言统计（条）：
来源：http://pbg.mhx1999.top

Python ......... 252
来源：http://zdx.daxiang520.top

PHP ............ 252
来源：http://wep.bbcook.cn

JavaScript ..... 252
来源：http://pvb.andypj.xyz

TypeScript ..... 212
来源：http://agk.9152youxi.cn

Java ........... 212
来源：http://mps.meibo888.top

Go ............. 212
来源：http://cih.tianlin.xyz

Ruby ........... 212
来源：http://hqr.zdbjq.cn

C# ............. 212
来源：http://hnd.cqqwz.cn

C .............. 30
来源：http://hyc.birdmap.top

C++ ............ 30
来源：http://nbk.aizwys.cn

SQL ............ 90
来源：http://kfu.hnxiangtu.top

Bash ........... 80
来源：http://ndv.jqgfzy.top

Kotlin ......... 15
来源：http://rrx.dianchejie.cn

Swift .......... 15
来源：http://hsk.uphjek.com

Lua ............ 10
来源：http://cgj.guowangkeji.top

Perl ........... 10
来源：http://yke.guannengcc.top

Scala .......... 10
来源：http://ppr.shuidangran.top

------------------------------------
来源：http://ifm.shuidangran.top

合计 ........... 2106 条
来源：http://hpx.hnxiangtu.top

按章节统计：
来源：http://ffq.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://psk.yonumen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qkb.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mfg.zhijiandao.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zjz.jianghu66.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://igv.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://axn.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rzi.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xdx.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dxm.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tan.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cnw.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dkm.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lan.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ktc.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bwr.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dta.9152youxi.cn

Q SQL 专题                              90
来源：http://mdp.0kj1m.cn

R Bash 专题                             80
来源：http://qzl.sysykeji.top

S C / C++ 专题                          60
来源：http://cro.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://crr.jinqigufen.top

U 高频实用片段                         120
来源：http://fax.tian-w.cn

------------------------------------
来源：http://lhg.vqdsnc.cn

合计                                  2106 条
来源：http://dzf.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://bdf.wangshuangyany.cn

使用提醒
来源：http://vld.yonumen.top

--------------------------------------------------------------------------------
来源：http://dbn.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fvv.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qtr.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dko.havefunace.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bev.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://skd.zycfv.cn

—— 文件结束 ——
来源：http://jos.shanyushiyangkeji.top

================================================================================
来源：http://uxt.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://kwl.cucudq.cn

Common Programming Examples Cheat Book
来源：http://hss.jianghu66.top

================================================================================
来源：http://ofa.c1oappe.top

【收录内容】
来源：http://dov.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ggm.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gic.hywenlv.cn

SQL · Bash · C · C++
来源：http://lyt.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bnr.hesvh.cn

【使用说明】
来源：http://lcr.daria6918.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wca.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fsj.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://syv.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xlh.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bja.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qiv.haohaochexian.top


<!-- 参考信息 -->