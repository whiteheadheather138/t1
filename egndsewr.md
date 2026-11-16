代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://tlv.yanxiufei.cn

[T51] Scala：Hello World
来源：http://smu.yuxming.cn

println("Hello")
来源：http://ytv.dianchejie.cn

[T52] Scala：变量
来源：http://xuf.ehwqpu.com

val a = 1;  var b = 2
来源：http://aji.haohaochexian.top

[T53] Scala：字符串插值
来源：http://nvf.jqgufenzy.top

s"值: $b"
来源：http://wcq.jianghu66.top

[T54] Scala：集合映射
来源：http://yyc.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://qmm.yueranfly.top

[T55] Scala：集合过滤
来源：http://mvl.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rlz.gzhubu.top

[T56] Scala：样例类
来源：http://njq.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://qul.aibaodan.cn

[T57] Scala：模式匹配
来源：http://xaj.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nft.cashguo.top

[T58] Scala：函数定义
来源：http://agd.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://pkj.tanke756.top

[T59] Scala：循环
来源：http://wfu.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://pwu.hammf.cn

[T60] Scala：折叠
来源：http://bkz.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fnz.ydzc1.top

================================================================================
来源：http://iqk.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xds.ctjpmb.com

================================================================================
来源：http://vam.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://epl.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://xjv.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://wde.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vyy.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://vqe.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yng.zhixingplan.top

[U04] Py：变量调试打印
来源：http://kln.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pje.xziqi.cn

[U05] Py：列表去重且保序
来源：http://qcq.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://ymd.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://yky.yuxming.cn

{**a, **b}
来源：http://liv.zdbjq.cn

[U07] Py：反转字典键值
来源：http://jbx.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://jdl.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://xbi.bjfxy.top

[y for x in nested for y in x]
来源：http://ikh.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://ogi.jinqigufen.top

max(d, key=d.get)
来源：http://idg.hesvh.cn

[U10] Py：按值排序字典
来源：http://oeo.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vvc.yueranfly.top

[U11] Py：生成器表达式
来源：http://vpd.aizwys.cn

(x * 2 for x in arr)
来源：http://pgk.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nlf.daria6918.cn

Counter(arr).most_common(3)
来源：http://wgc.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://uru.dianchejie.cn

deque(maxlen=10)
来源：http://mbu.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://egs.yvedp.cn

defaultdict(list)
来源：http://ifj.cqqwz.cn

[U15] Py：高精度计时
来源：http://ucg.sysykeji.top

t = time.perf_counter()
来源：http://rot.52xcode.cn

[U16] Py：命令行参数解析
来源：http://fsk.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uia.epnwcf.com

[U17] Py：初始化日志
来源：http://zcp.zycfv.cn

logging.basicConfig(level=logging.INFO)
来源：http://mos.feifeiyinyue.top

[U18] Py：预编译正则
来源：http://jqk.yueranfly.top

pat = re.compile(r"\d+")
来源：http://nac.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://tfw.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cng.yj202588.top

[U20] Py：缓存函数结果
来源：http://zhf.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://spj.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://egz.dianchejie.cn

@contextlib.contextmanager
来源：http://vsg.daria6918.cn

[U22] Py：矩阵转置
来源：http://tgv.guannengcc.top

list(zip(*m))
来源：http://mwr.mhx1999.top

[U23] Py：分块读取大文件
来源：http://vrr.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aln.fehbvm.com

[U24] Py：路径操作
来源：http://xkw.cheryme.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://klf.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://rvr.cheryme.top

csv.DictReader(f)
来源：http://tml.0kj1m.cn

[U26] Py：并发下载
来源：http://eal.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bts.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://qei.quarkkingdee.top

aiohttp.ClientSession() 配合 async with
来源：http://tup.jianghu66.top

[U28] Py：类型别名
来源：http://asu.aibaodan.cn

UserId = int
来源：http://rcm.zhixingplan.top

[U29] Py：属性校验
来源：http://krk.hnqzz.top

@property 与 @x.setter 配合
来源：http://rvm.kuanghao11.cn

[U30] Py：数据类
来源：http://nsm.nanxinkj.top

@dataclass(slots=True)
来源：http://syl.xziqi.cn

[U31] Py：单测
来源：http://ani.hysaishi.cn

python -m pytest -q
来源：http://zqg.yongpay.top

[U32] Py：代码格式化
来源：http://sjy.daria6918.cn

ruff format . && ruff check --fix .
来源：http://lvm.jqgfzy.top

[U33] Py：打包发布
来源：http://gya.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://ury.yangfankeji.com

[U34] Py：判断编码
来源：http://yss.feifeiyinyue.top

chardet.detect(raw)
来源：http://gfq.quarkkingdee.top

[U35] Py：发送邮件
来源：http://vsf.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qqg.hongshengwenyu.top

[U36] Py：定时任务
来源：http://eyn.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://vkf.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://byh.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hno.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://fin.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://xvc.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://jbw.wangdashe.top

sys.stdout.isatty()
来源：http://uyj.andypj.xyz

[U40] Py：打印到标准错误
来源：http://zfd.bbcook.cn

print("err", file=sys.stderr)
来源：http://rhg.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://umx.nanxuanxn.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fvy.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://vwt.xinyue.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nwi.yvedp.cn

[U43] PHP：声明命名空间
来源：http://ayj.gotoacloud.top

namespace App\Http;
来源：http://ktk.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://dct.kuanghao11.cn

declare(strict_types=1);
来源：http://chq.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://nwl.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://hce.yj202588.top

[U46] PHP：可空类型
来源：http://mwj.yj202588.top

?string $name = null
来源：http://ezx.jinyuanbaomall.cn

[U47] PHP：联合类型
来源：http://qsw.zhengqikj.top

int|string $id
来源：http://oxd.hammf.cn

[U48] PHP：纯枚举
来源：http://kox.cashguo.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://syn.zdbjq.cn

[U49] PHP：只读属性
来源：http://lrs.nwbrower.top

public readonly string $name
来源：http://pvo.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://uiu.tanke756.top

public function __construct(private int $id) {}
来源：http://cek.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://jzf.hammf.cn

[$a, $b] = $arr;
来源：http://crm.hnxiangtu.top

[U52] PHP：箭头函数
来源：http://aba.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://aea.tian-w.cn

[U53] PHP：空合并运算符
来源：http://ijk.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://wrr.cheryme.top

[U54] PHP：空安全调用
来源：http://juj.birdmap.top

$obj?->method()
来源：http://wkp.zhixingplan.top

[U55] PHP：match 表达式
来源：http://ubm.zhijiandao.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tst.ybcxt.top

[U56] PHP：命名参数
来源：http://wmh.pengpengdd.cyou

f(a: 1, b: 2)
来源：http://gqd.316326.xyz

[U57] PHP：字符串插值
来源：http://vrk.jinqigufen.top

"值: {$a}"
来源：http://frq.andypj.xyz

[U58] PHP：数组三件套
来源：http://qbz.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://edl.gzhubu.top

[U59] PHP：自定义排序
来源：http://jpa.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bcc.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://zuf.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eyr.cucudq.cn

[U61] PHP：正则
来源：http://fuy.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ifn.vqdsnc.cn

[U62] PHP：日期对象
来源：http://wkk.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cbq.haohaochexian.top

[U63] PHP：文件读写
来源：http://ovj.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kcn.wangshuangyany.cn

[U64] PHP：目录遍历
来源：http://eza.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://loe.sweek.top

[U65] PHP：会话
来源：http://aiz.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ygd.ybcxt.top

[U66] PHP：设置 Cookie
来源：http://vve.0kj1m.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vib.shuidangran.top

[U67] PHP：处理文件上传
来源：http://eji.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yvv.gzhubu.top

[U68] PHP：PDO 连接
来源：http://xrc.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://huf.yj202588.top

[U69] PHP：PDO 预处理
来源：http://xrf.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ref.hesvh.cn

[U70] PHP：PDO 事务
来源：http://ziu.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ebe.havefunace.top

[U71] PHP：抛出异常
来源：http://pax.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://ilf.smart0.xyz

[U72] PHP：写错误日志
来源：http://ovp.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://zvq.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://alv.sxryk.cn

parse_ini_file("config.ini", true)
来源：http://lug.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://kmo.mhx1999.top

getenv("APP_ENV") ?: "production"
来源：http://thr.yj20258888.top

[U75] PHP：依赖注入
来源：http://jjk.jiagoushi.top

composer require psr/container
来源：http://omf.guowangkeji.top

[U76] PHP：简单路由
来源：http://exm.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tpu.guowangkeji.top

[U77] PHP：模板渲染
来源：http://xuq.uphjek.com

composer require twig/twig
来源：http://ghy.bjfxy.top

[U78] PHP：单元测试
来源：http://ujw.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://jos.tanke756.top

[U79] PHP：静态分析
来源：http://xnx.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://mlt.ivvv.top

[U80] PHP：代码规范修复
来源：http://mst.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://dgo.xinyue.icu

[U81] JS：初始化项目
来源：http://lmt.hesvh.cn

npm init -y;  npm i express
来源：http://qpr.ivvv.top

[U82] JS：package.json 脚本
来源：http://rie.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bxu.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://ovr.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://wwv.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://uwl.zhongyouzk.top

module.exports = { a };  const { a } = require("./m");
来源：http://nqa.cheryme.top

[U85] JS：可选链
来源：http://nxy.quarkkingdee.top

a?.b?.c
来源：http://ceq.guannengcc.top

[U86] JS：空值合并
来源：http://gel.fengsongda.top

a ?? b
来源：http://zlc.dashuyun.cn

[U87] JS：解构默认值
来源：http://ezq.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://srj.guannengcc.top

[U88] JS：对象展开合并
来源：http://ttg.jinqigfzy.top

{ ...a, ...b }
来源：http://hli.daria6918.cn

[U89] JS：数组去重
来源：http://fob.sufxvd.cn

[...new Set(arr)]
来源：http://zan.haohaochexian.top

[U90] JS：数字数组排序
来源：http://tjp.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://jaj.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://ncd.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qsl.nwbrower.top

[U92] JS：深拷贝
来源：http://bns.shanyushiyangtech.top

structuredClone(obj)
来源：http://ikv.yangfankeji.com

[U93] JS：模板字符串
来源：http://kty.yueranfly.top

`共 ${n} 条`
来源：http://gad.andypj.xyz

[U94] JS：箭头函数
来源：http://fdz.havefunace.top

const double = x => x * 2;
来源：http://siz.nanxinkj.top

[U95] JS：Promise 包装
来源：http://cji.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://mrt.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://eoc.sxryk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qbu.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://xwu.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zks.aizwys.cn

[U98] JS：fetch 带 JSON
来源：http://nhq.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ipg.hesvh.cn

[U99] JS：事件监听
来源：http://atu.zycfv.cn

el.addEventListener("click", e => {})
来源：http://dop.meibo888.top

[U100] JS：DOM 查询
来源：http://ewx.quarkkingdee.top

document.querySelector(".item")
来源：http://ztj.zhijiandao.cn

[U101] JS：classList 操作
来源：http://enj.zhengqikj.top

el.classList.toggle("active")
来源：http://ira.aizwys.cn

[U102] JS：本地存储
来源：http://mnt.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wjv.cheryme.top

[U103] JS：定时器
来源：http://ixr.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eev.shanyushiyangtech.top

[U104] JS：防抖
来源：http://ope.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://usx.hnqzz.top

[U105] JS：节流
来源：http://wad.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://exy.dianchejie.cn

[U106] JS：日期格式化
来源：http://vxz.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ffk.aibaodan.cn

[U107] JS：数字千分位
来源：http://ajk.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eml.chenzaomai.com

[U108] JS：随机整数
来源：http://mxu.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mde.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://nuj.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://wyd.jlsjyb.cn

[U110] JS：数组分块
来源：http://zla.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lvt.zhijiandao.cn

[U111] JS：对象转 Map
来源：http://nmr.nanxinkj.top

new Map(Object.entries(obj))
来源：http://cqu.pengpengdd.cyou

[U112] JS：字符串补位
来源：http://irr.nanxinkj.top

"7".padStart(3, "0")
来源：http://ytk.fengsongda.top

[U113] JS：正则替换全部
来源：http://zzk.ehwqpu.com

s.replaceAll("a", "b")
来源：http://ogg.aizwys.cn

[U114] JS：JSON 深比较
来源：http://ycp.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ecq.cdnleiting.top

[U115] JS：生成 UUID
来源：http://llg.xuanzx.com

crypto.randomUUID()
来源：http://uny.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://pud.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://diz.havefunace.top

[U117] JS：单元测试
来源：http://nqf.yonumen.top

npm i -D vitest;  npx vitest
来源：http://lrm.svipenyu.cn

[U118] JS：开发服务器
来源：http://ghw.9152youxi.cn

npm i -D vite;  npx vite
来源：http://htq.yvedp.cn

[U119] JS：生产构建
来源：http://mbs.cqqwz.cn

npx vite build
来源：http://tvc.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://zjy.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://jwe.fktsv.cn

================================================================================
来源：http://pom.zhiwuduotai.top

统计汇总
来源：http://ugo.redwolf501.top

================================================================================
来源：http://xpj.dashuyun.cn

按语言统计（条）：
来源：http://uoo.hnqzz.top

Python ......... 252
来源：http://ktd.wangdashe.top

PHP ............ 252
来源：http://rfu.daxiang520.top

JavaScript ..... 252
来源：http://kvv.pycfn.com

TypeScript ..... 212
来源：http://ryg.hfpthk.cn

Java ........... 212
来源：http://roe.0kj1m.cn

Go ............. 212
来源：http://fmv.yueranfly.top

Ruby ........... 212
来源：http://klt.jinqigufen.top

C# ............. 212
来源：http://amc.fktsv.cn

C .............. 30
来源：http://nli.c1oappe.top

C++ ............ 30
来源：http://zyv.yonumen.top

SQL ............ 90
来源：http://njm.zhongyouzk.top

Bash ........... 80
来源：http://kmj.cashguo.top

Kotlin ......... 15
来源：http://dcb.jianghu66.top

Swift .......... 15
来源：http://sdv.aibaodan.cn

Lua ............ 10
来源：http://jef.tianlin.xyz

Perl ........... 10
来源：http://mac.sjlbkw.cn

Scala .......... 10
来源：http://dic.hywenlv.cn

------------------------------------
来源：http://ily.yuanzhike.top

合计 ........... 2106 条
来源：http://qqp.kuanghao11.cn

按章节统计：
来源：http://lrg.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vsd.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ejt.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vaz.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qqu.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jad.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cvs.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uol.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jsr.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rey.shanyushiyangtech.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ccr.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lbm.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rhu.jinyuanbaomall.cn


<!-- 参考信息 -->