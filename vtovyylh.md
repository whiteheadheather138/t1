代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://vek.hnqzz.top

[T51] Scala：Hello World
来源：http://gch.hcnkem.com

println("Hello")
来源：http://wkp.uphjek.com

[T52] Scala：变量
来源：http://btd.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://nor.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://phe.yanxiufei.cn

s"值: $b"
来源：http://qay.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://ykg.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://ejv.dashuyun.cn

[T55] Scala：集合过滤
来源：http://ncy.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://gho.cdnleiting.top

[T56] Scala：样例类
来源：http://vvw.birdmap.top

case class User(name: String, age: Int)
来源：http://mdm.nanxinkj.top

[T57] Scala：模式匹配
来源：http://qfn.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tfa.yonumen.top

[T58] Scala：函数定义
来源：http://dcw.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kfc.fehbvm.com

[T59] Scala：循环
来源：http://knx.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://lpz.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://jkx.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xbz.havefunace.top

================================================================================
来源：http://tla.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dvy.shuidangran.top

================================================================================
来源：http://wpb.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://pwl.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://ukm.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://rhh.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eti.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://bog.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://maa.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://usv.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uct.nwbrower.top

[U05] Py：列表去重且保序
来源：http://ogy.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://sxx.jyoumei.cn

[U06] Py：合并两个字典
来源：http://egk.dashuyun.cn

{**a, **b}
来源：http://zmo.52xcode.cn

[U07] Py：反转字典键值
来源：http://qwx.zhaomingkeji.xyz

{v: k for k, v in d.items()}
来源：http://tts.shzxlz.cn

[U08] Py：展平二维列表
来源：http://osi.cashguo.top

[y for x in nested for y in x]
来源：http://jgd.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://fdg.snrcjt.cn

max(d, key=d.get)
来源：http://lqk.dianchejie.cn

[U10] Py：按值排序字典
来源：http://byq.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fpn.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://gij.zdbjq.cn

(x * 2 for x in arr)
来源：http://hio.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wly.aibaodan.cn

Counter(arr).most_common(3)
来源：http://bfg.zdbjq.cn

[U13] Py：固定长度队列
来源：http://guz.fehbvm.com

deque(maxlen=10)
来源：http://ubp.redwolf501.top

[U14] Py：分组收集到列表
来源：http://qzt.uphjek.com

defaultdict(list)
来源：http://sew.tianlin.xyz

[U15] Py：高精度计时
来源：http://loo.yj20258.top

t = time.perf_counter()
来源：http://vid.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://qev.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rag.guowangkeji.top

[U17] Py：初始化日志
来源：http://xti.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://czh.ctjpmb.com

[U18] Py：预编译正则
来源：http://otw.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://aqu.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://xor.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qst.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://aps.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://ejn.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://tia.pengpengdd.cyou

@contextlib.contextmanager
来源：http://zqe.chenlongwang.top

[U22] Py：矩阵转置
来源：http://hgp.gotoacloud.top

list(zip(*m))
来源：http://qkv.meibo888.top

[U23] Py：分块读取大文件
来源：http://dwx.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kpg.chenlongwang.top

[U24] Py：路径操作
来源：http://nqt.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wss.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://ofw.ctjpmb.com

csv.DictReader(f)
来源：http://kze.yj202588.top

[U26] Py：并发下载
来源：http://qba.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tun.hammf.cn

[U27] Py：异步 HTTP
来源：http://ycp.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://ysj.jiagoushi.top

[U28] Py：类型别名
来源：http://ubh.chenjidiqi.icu

UserId = int
来源：http://hif.xingfuxueyuan.xyz

[U29] Py：属性校验
来源：http://hwb.ybcxt.top

@property 与 @x.setter 配合
来源：http://exl.gzhubu.top

[U30] Py：数据类
来源：http://lwn.guannengcc.top

@dataclass(slots=True)
来源：http://qto.gogol.net.cn

[U31] Py：单测
来源：http://rue.tanke756.top

python -m pytest -q
来源：http://pcn.jlsjyb.cn

[U32] Py：代码格式化
来源：http://wgj.pycfn.com

ruff format . && ruff check --fix .
来源：http://mgv.fehbvm.com

[U33] Py：打包发布
来源：http://fcq.xziqi.cn

python -m build  （依赖 pyproject.toml）
来源：http://fhh.tanke756.top

[U34] Py：判断编码
来源：http://sup.dianchejie.cn

chardet.detect(raw)
来源：http://efd.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://jab.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://plu.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://ayv.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://mbm.xuetiantiany.cn

[U37] Py：读写 Excel
来源：http://wsc.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hhe.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://dib.daxiang520.top

Path(__file__).resolve().parent
来源：http://wvu.gzhubu.top

[U39] Py：判断是否在交互环境
来源：http://zni.yangfankeji.com

sys.stdout.isatty()
来源：http://tkm.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://zlr.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://xid.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://jhy.pengpengdd.cyou

composer init;  composer require guzzlehttp/guzzle
来源：http://aon.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://fep.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nzt.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://vhs.sufxvd.cn

namespace App\Http;
来源：http://fot.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://qev.shanyushiyangtech.top

declare(strict_types=1);
来源：http://yhr.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://vid.redwolf501.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mmd.xuanzx.com

[U46] PHP：可空类型
来源：http://hgj.jinghuilouyu.cn

?string $name = null
来源：http://bln.svipenyu.cn

[U47] PHP：联合类型
来源：http://rlv.tian-w.cn

int|string $id
来源：http://pcg.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://zfx.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://woi.hnqzz.top

[U49] PHP：只读属性
来源：http://yoy.c1oappe.top

public readonly string $name
来源：http://skd.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://gwq.ppjwa.cn

public function __construct(private int $id) {}
来源：http://ttr.ctjpmb.com

[U51] PHP：数组解构
来源：http://qyf.redwolf501.top

[$a, $b] = $arr;
来源：http://mbf.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://lge.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://usq.guannengcc.top

[U53] PHP：空合并运算符
来源：http://wzx.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://dgf.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://tmj.zhijiandao.cn

$obj?->method()
来源：http://owp.yonumen.top

[U55] PHP：match 表达式
来源：http://bvv.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dce.vqdsnc.cn

[U56] PHP：命名参数
来源：http://adn.zhixingplan.top

f(a: 1, b: 2)
来源：http://zhw.yj202588.top

[U57] PHP：字符串插值
来源：http://ckd.zhoulong.xyz

"值: {$a}"
来源：http://gfw.redwolf501.top

[U58] PHP：数组三件套
来源：http://zhc.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vvs.ybcxt.top

[U59] PHP：自定义排序
来源：http://ncw.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lrf.sweek.top

[U60] PHP：JSON 编解码
来源：http://lgz.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jmv.jianghu66.top

[U61] PHP：正则
来源：http://uby.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qfv.fktsv.cn

[U62] PHP：日期对象
来源：http://bfr.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ekw.ydzc1.top

[U63] PHP：文件读写
来源：http://wgx.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bmy.tarul.cn

[U64] PHP：目录遍历
来源：http://bcf.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://wdq.cashguo.top

[U65] PHP：会话
来源：http://udn.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://bnc.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://jfy.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cbk.sysykeji.top

[U67] PHP：处理文件上传
来源：http://ezg.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tuz.daxiang520.top

[U68] PHP：PDO 连接
来源：http://bpg.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qvk.ctjpmb.com

[U69] PHP：PDO 预处理
来源：http://zsa.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://odb.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://hxu.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rme.bjfxy.top

[U71] PHP：抛出异常
来源：http://uka.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://jke.havefunace.top

[U72] PHP：写错误日志
来源：http://svr.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://wjq.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://etl.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://qbk.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://umi.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://vdm.epnwcf.com

[U75] PHP：依赖注入
来源：http://vpg.sjlbkw.cn

composer require psr/container
来源：http://eyn.yanxiufei.cn

[U76] PHP：简单路由
来源：http://ffv.yj202588.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vqp.andypj.xyz

[U77] PHP：模板渲染
来源：http://ofp.gotoacloud.top

composer require twig/twig
来源：http://rcb.quarkkingdee.top

[U78] PHP：单元测试
来源：http://ngb.yongpay.top

composer require --dev phpunit/phpunit
来源：http://gus.fengsongda.top

[U79] PHP：静态分析
来源：http://xaz.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://xch.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://azr.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uay.pycfn.com

[U81] JS：初始化项目
来源：http://yhm.yonumen.top

npm init -y;  npm i express
来源：http://fxt.xuanzx.com

[U82] JS：package.json 脚本
来源：http://xsh.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xxo.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://nvy.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rao.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://snj.quarkkingdee.top

module.exports = { a };  const { a } = require("./m");
来源：http://yln.pengpengdd.cyou

[U85] JS：可选链
来源：http://ekw.xylfe.cn

a?.b?.c
来源：http://gee.hesvh.cn

[U86] JS：空值合并
来源：http://mti.wangdashe.top

a ?? b
来源：http://iwb.tarul.cn

[U87] JS：解构默认值
来源：http://kkx.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://bpy.jianghu66.top

[U88] JS：对象展开合并
来源：http://yiy.guannengcc.top

{ ...a, ...b }
来源：http://nwe.aibaodan.cn

[U89] JS：数组去重
来源：http://qoz.yfazqb.com

[...new Set(arr)]
来源：http://hfh.shuidangran.top

[U90] JS：数字数组排序
来源：http://via.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://cwr.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://ntg.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lxw.fengsongda.top

[U92] JS：深拷贝
来源：http://egz.sxryk.cn

structuredClone(obj)
来源：http://lpp.zdqjudy.top

[U93] JS：模板字符串
来源：http://rwv.zhengqikj.top

`共 ${n} 条`
来源：http://vdt.yongpay.top

[U94] JS：箭头函数
来源：http://xyd.bbcook.cn

const double = x => x * 2;
来源：http://yds.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://xfh.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://abm.sysykeji.top

[U96] JS：async/await 与异常
来源：http://yhz.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://szr.chenjidiqi.icu

[U97] JS：并发请求
来源：http://ugq.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://wtf.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://cin.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vii.cdnleiting.top

[U99] JS：事件监听
来源：http://afc.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://xga.ppjwa.cn

[U100] JS：DOM 查询
来源：http://yfy.hcnkem.com

document.querySelector(".item")
来源：http://vpj.hfpthk.cn

[U101] JS：classList 操作
来源：http://oyd.xinyue.icu

el.classList.toggle("active")
来源：http://xxk.jianghu66.top

[U102] JS：本地存储
来源：http://dwy.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qhu.snrcjt.cn

[U103] JS：定时器
来源：http://ovi.guowangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ifw.zhixingplan.top

[U104] JS：防抖
来源：http://fqe.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pty.yfazqb.com

[U105] JS：节流
来源：http://gpe.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mne.guannengcc.top

[U106] JS：日期格式化
来源：http://apj.mhx1999.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xbe.yj20258.top

[U107] JS：数字千分位
来源：http://rrw.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vhx.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://nhk.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yhh.yuanzhike.top

[U109] JS：数组分组
来源：http://ene.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://qtv.feifeiyinyue.top

[U110] JS：数组分块
来源：http://pbz.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sgw.0kj1m.cn

[U111] JS：对象转 Map
来源：http://sat.yongpay.top

new Map(Object.entries(obj))
来源：http://uqr.zhoulong.xyz

[U112] JS：字符串补位
来源：http://qzu.fktsv.cn

"7".padStart(3, "0")
来源：http://jxg.bjfxy.top

[U113] JS：正则替换全部
来源：http://pbk.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://xxq.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://irh.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://crt.xinyue.icu

[U115] JS：生成 UUID
来源：http://lto.cheryme.top

crypto.randomUUID()
来源：http://bgq.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://xee.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://fut.meibo888.top

[U117] JS：单元测试
来源：http://gxt.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://qkx.bbcook.cn

[U118] JS：开发服务器
来源：http://owy.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://mnm.cqqwz.cn

[U119] JS：生产构建
来源：http://gox.hysaishi.cn

npx vite build
来源：http://ejh.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://pxn.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://efj.xylfe.cn

================================================================================
来源：http://knc.chenzaomai.com

统计汇总
来源：http://ity.yfazqb.com

================================================================================
来源：http://wqy.chenjidiqi.icu

按语言统计（条）：
来源：http://mjk.c1oappe.top

Python ......... 252
来源：http://sar.cheryme.top

PHP ............ 252
来源：http://aca.sxryk.cn

JavaScript ..... 252
来源：http://gan.shzxlz.cn

TypeScript ..... 212
来源：http://mub.snrcjt.cn

Java ........... 212
来源：http://azb.yuxming.cn

Go ............. 212
来源：http://bxj.jqgufenzy.top

Ruby ........... 212
来源：http://uxg.epnwcf.com

C# ............. 212
来源：http://eyf.iojbl.cn

C .............. 30
来源：http://kow.ehwqpu.com

C++ ............ 30
来源：http://aru.nanxuanxn.top

SQL ............ 90
来源：http://tub.jyoumei.cn

Bash ........... 80
来源：http://gxd.hfpthk.cn

Kotlin ......... 15
来源：http://nfp.mhx1999.top

Swift .......... 15
来源：http://mcs.cucudq.cn

Lua ............ 10
来源：http://yts.tanke756.top

Perl ........... 10
来源：http://tax.tanke756.top

Scala .......... 10
来源：http://ykk.bjfxy.top

------------------------------------
来源：http://zpr.yuanzhike.top

合计 ........... 2106 条
来源：http://jdv.shanyushiyangkeji.top

按章节统计：
来源：http://xih.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wpo.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zzr.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://buv.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mmr.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gyj.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aim.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cfe.zhongyouzk.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://auy.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ksc.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ffo.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dxm.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qxe.mhx1999.top


<!-- 参考信息 -->